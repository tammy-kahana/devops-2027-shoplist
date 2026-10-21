#מביאה בסיס של image מוכן עם גרסא ספציפית של python
FROM python:3.11-slim
#יוצר תיקית עבודה בקונטיינר אם לא קיים
WORKDIR /app
#מביא את קובץ התלויות
COPY requirements.txt .
#מתקין את התלויות מהקובץ
RUN pip install --no-cache-dir -r requirements.txt
#מביא את הקוד
COPY app.py .
#אומרת לאיזה פורט השרת מאזין
EXPOSE 8000
#איזה פקודות ירוצו כשהקונטיינר יעלה
CMD ["python", "app.py"]
