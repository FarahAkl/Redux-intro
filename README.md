# Bank Account App 🏦  

A simple banking application built with **React** and **Redux Toolkit** that allows users to:  
- Deposit money (with currency conversion support)  
- Withdraw money  
- Request and pay back loans  
- Track account balance and loan purpose  

This project is designed for practicing Redux Toolkit slices, async thunks, and state management in React.

---

## 🚀 Features
- **Deposit funds** in USD, EUR, or GBP (auto-converts to USD).  
- **Withdraw funds** directly from your balance.  
- **Request a loan** with amount & purpose (only one active loan at a time).  
- **Repay loans** and update account balance.  
- **Loading state** while converting currencies via [Frankfurter API](https://www.frankfurter.app/).  

---

## 🛠️ Tech Stack

- **React** (functional components + hooks)  
- **Redux Toolkit** (`createSlice`)  
- **React-Redux** (`useDispatch`, `useSelector`)  
- **Frankfurter API** (currency conversion)  

---

## 📦 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/FarahAkl/Redux-intro.git
cd Redux-intro
npm install
```
## ▶️ Usage

Start the development server:

```bash
npm run dev
```
Open in your browser:  
👉 [http://localhost:5173](http://localhost:5173)  

---

## 🧩 State Structure

The Redux store for `account` looks like this:

```js
{
  balance: 0,
  loan: 0,
  loanPurpose: "",
  isLoading: false
}
```
## ⚡ Available Actions

- `deposit(amount,currency)` → Deposit money.  
- `withdraw(amount)` → Withdraw money.  
- `requestLoan(amount, purpose)` → Take a loan if none is active.  
- `payLoan()` → Repay current loan.  

---

## 📸 Demo
To see the live demo click [here](https://redux-intro-olive.vercel.app/)
