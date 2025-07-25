# 💼💰 Payment-Tracker

<div align="center">
  <img height="300" src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExODNyZnZwbzM4M3Y2ODN4OWRqOGRrN3pzN2J1bXlidHlmNHlsNjFweiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/13ln9K5TWkNTLa/giphy.gif"  />
</div>

An AI-powered web page built with **Streamlit** created to track Payments and update them for ease of the finance personnel. So with this app you can update the payment status, values in other currencies and you can download the final output as an excel sheet at the end of the month and submit it to the finance team.

## 🚀 Features

- 💵 Can convert the currency when the currecy rate and the payment value is added
- 📊 The webpage will display a dashboard at the beginning as a brief introduction on the past data
- ✍️ When you are adding a new payment record the following are the key features of the payment data you should insert

  - The payment type (ususal payment/ advance payment)
  - Vendor Name
  - Payment description (the use of the expense)
  - Currency code (USD,IND)
  - Exchange rate to LKR
  - Total amount in USD
  - Paid amount in USD
  - Payment due date
  - Invoiced date
  - Payment terms (the time duration for the payment to be done)
  - Payment date
  - Payment status (Pneding/ completed)
    
- 📥 Download your payment sheet as an CSV file at the end
- 🔐 Uses **Ngork Authtoken** to run the app in the local environment
- 🔗 Integrated with **streamlit and pyngork** for creating web interfaces

## 🛠️ Technologies Used

- `Streamlit` for the interactive web interface  
- `Ngork authtoken` for the access for the local environment

##💡 How to Run Locally

1. Clone the repository  
2. Set your Ngrok Authtoken key as environment variables:

```bash
# 🔑 Set your Ngrok auth token directly (Replace this with your actual token)
NGROK_AUTH_TOKEN = "Enter Your Authtoken Here"
ngrok.set_auth_token(NGROK_AUTH_TOKEN)
````

3. Install dependencies:

```bash
pip install streamlit pyngrok
```

4. Run the app:

```bash
# 🚀 Launch the Streamlit app in the background
os.system("streamlit run app.py &")
time.sleep(5)  # Allow Streamlit to start

# 🌐 Connect ngrok to the running Streamlit app
public_url = ngrok.connect(8501)
```

## 📌 Notes

* The app is currently in the process of developing and currently in the process of adding the following features,
  - Adding the edit, remove already updated data.(To edit when the pending payment are already done)
  - To generate the converted currecy rate when the country code is added. (using local APIs)
  - Making it more attarctive and user friendly
  - Adding the feature where the payment will auto record when the invoice slip is uploaded to the system (using NLP)

## 📽 UI
<div align="center">
  <img height="1000" src="Visual UI.jpg"  />
</div>

---

Built by **Githmi Punchihewa**
BSc in Applied Data Science and Communication | KDU | Ceylon Tobacco Company
