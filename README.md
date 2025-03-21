# Zoho Creator Hijri Date Widget

This repository provides a guide to setting up and running the Zoho Creator Hijri Date Widget using a React-based Hijri Date Picker.

## Prerequisites
- A [Zoho Creator](https://www.zoho.com/creator/) trial account.
- Node.js and npm installed on your local machine.
- `zet` CLI tool for Zoho Creator widgets.

## Steps to Set Up

### 1. Create a Zoho Creator Trial Account
Sign up for a [Zoho Creator](https://www.zoho.com/creator/) trial account if you do not have one.

### 2. Clone the React Project
Clone the React Hijri Date Picker project and navigate to the directory:
```sh
git clone https://github.com/mobgreat0/react-hijri-date-picker
cd react-hijri-date-picker
```

### 3. Install and Run the React Project
```sh
npm install
npm run build
```
This will generate the production build in the `dist` folder.

### 4. Create a Zoho Creator Widget
Run the following commands to initialize and validate your widget:
```sh
zet init
zet validate
zet pack
```

### 5. Replace `dist` Folder in the Widget
Move the built `dist` folder from the React project to the `app` folder inside your Zoho Creator widget:
```sh
cp -r dist/* path/to/zoho-creator-widget/app/
```

### 6. Update `index.html`
Modify `index.html` inside the widget's `app` folder to point to the correct asset paths.

### 7. Validate and Run the Widget
```sh
zet validate
zet run
```

## Screenshots

![Widget Initialization](https://github.com/user-attachments/assets/7053a590-0926-44d7-8a1c-e64c87c3a616)

![Widget Validation](https://github.com/user-attachments/assets/f6424475-fabb-4867-845c-9087fc101dd2)

![Widget in Zoho Creator](https://github.com/user-attachments/assets/9a41b719-d1ca-4685-962d-f31afe18327c)

## Conclusion
Following these steps, you should be able to successfully set up and run the Zoho Creator Hijri Date Widget using the React-based Hijri Date Picker.

