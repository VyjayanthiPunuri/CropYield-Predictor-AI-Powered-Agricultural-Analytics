import streamlit as st
import pandas as pd
import plotly.express as px

st.set_page_config(page_title="CropYield Predictor", layout="wide")

st.title("🌾 CropYield Predictor")
st.subheader("AI-Powered Agricultural Intelligence & Analytics Platform")

df = pd.read_csv("feature_engineered_crop_data.csv")

c1, c2, c3, c4 = st.columns(4)

c1.metric("Records", len(df))
c2.metric("Countries", df["Area"].nunique())
c3.metric("Crops", df["Item"].nunique())
c4.metric("Average Yield", round(df["Crop_Yield"].mean(), 2))

st.markdown("---")

st.header("Crop Yield Distribution")

fig = px.histogram(
    df,
    x="Crop_Yield",
    nbins=30,
    title="Crop Yield Distribution"
)

st.plotly_chart(fig, use_container_width=True)

st.header("Top Countries")

country = (
    df.groupby("Area")["Crop_Yield"]
    .mean()
    .sort_values(ascending=False)
    .head(10)
    .reset_index()
)

fig = px.bar(
    country,
    x="Area",
    y="Crop_Yield",
    color="Crop_Yield"
)

st.plotly_chart(fig, use_container_width=True)

st.header("Top Crops")

crop = (
    df.groupby("Item")["Crop_Yield"]
    .mean()
    .sort_values(ascending=False)
    .head(10)
    .reset_index()
)

fig = px.bar(
    crop,
    x="Item",
    y="Crop_Yield",
    color="Crop_Yield"
)

st.plotly_chart(fig, use_container_width=True)

st.success("Project Completed Successfully")