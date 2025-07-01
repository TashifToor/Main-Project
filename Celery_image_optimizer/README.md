 2. Celery Image Optimizer

```markdown
# 🖼️ Django Celery Image Optimizer

This project uses **Celery** and **Redis** to optimize uploaded images in the background without blocking the main thread.

---

## 🚀 Features

- Upload images via Django admin or UI
- Automatically resize/compress images
- Asynchronous task processing with Celery
- Background worker using Redis

---

## 🛠️ Tech Stack

- Django
- Celery
- Redis
- Pillow (for image processing)

---

## 🔧 Run Instructions

```bash
git clone https://github.com/TashifToor/Celery_image_optimizer.git
cd Celery_image_optimizer
pip install -r requirements.txt
python manage.py migrate
celery -A project_name worker -l info
python manage.py runserver
