# Streamlit Law Practice Dashboard with Firebase

This repository contains a demo dashboard built with **Streamlit** for small law firms. It stores data in **Firebase** using both the Realtime Database and Firestore. The app can be deployed to **Streamlit Cloud**.

## Setup

1. Create a project in [Firebase](https://console.firebase.google.com/).
2. Enable **Firestore** and the **Realtime Database** in that project.
3. Create a service account and download its JSON credentials file.
4. Note the database URL shown in the Realtime Database settings (ends with `firebaseio.com`).
5. Place the service account file somewhere safe and set two environment variables:
   - `GOOGLE_APPLICATION_CREDENTIALS` – path to the JSON credentials file
   - `FIREBASE_DATABASE_URL` – the Realtime Database URL
6. Install the dependencies and run the app:
   ```bash
   pip install -r requirements.txt
   streamlit run app.py
   ```
7. On **Streamlit Cloud**, add the same variables in the app secrets so the dashboard can access Firebase.

## Files

- `app.py` – Streamlit application with Firebase integration.
- `requirements.txt` – dependencies needed to run the app.

