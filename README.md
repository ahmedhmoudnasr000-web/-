import streamlit as st

st.title("🛡️ Smart Life Hub")
st.subheader("مساعدك الشخصي للإنتاجية")

option = st.sidebar.selectbox("اختر الخدمة:", ["تنظيم المهام", "تحسين الصوت", "تعديل إبداعي"])

if option == "تنظيم المهام":
    task = st.text_input("أضف مهمة جديدة:")
    if st.button("حفظ"):
        st.success(f"تمت إضافة: {task}")
elif option == "تحسين الصوت":
    st.file_uploader("ارفع الملف الصوتي:")
    st.info("جاري المعالجة...")
# -
smart-life-hub 
