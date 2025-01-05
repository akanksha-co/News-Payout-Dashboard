# Responsive News & Payout Dashboard

A modern, responsive dashboard that integrates news articles and payout management features. This dashboard displays top news headlines fetched from the **NewsAPI** and allows users to input payout rates for each article. The dashboard also includes a **pie chart** for total payouts, **dark mode** support, and **pagination** for articles, providing an intuitive and user-friendly experience.

---

## Features

- **Responsive Design:** Fully responsive and mobile-friendly layout.
- **News API Integration:** Displays top news articles using the [NewsAPI](https://newsapi.org/).
- **Payout Management:** Allows users to enter payout rates for each article and automatically calculates the total payouts.
- **Pie Chart:** A pie chart visualizes the distribution of payouts for each article.
- **Pagination:** Navigate through multiple pages of news articles seamlessly.
- **Dark Mode:** Toggle between dark and light themes for improved user experience.
- **User Authentication:** Displays the logged-in user’s email from localStorage.
- **State Management:** Uses React’s `useState` and `useEffect` hooks to manage local component state.

---

## Tech Stack

- **Frontend:** React.js, Bootstrap
- **Charting:** Chart.js (for pie chart visualization)
- **API:** [NewsAPI](https://newsapi.org/) to fetch the latest news headlines
- **Styling:** Bootstrap CSS
- **State Management:** Local state using React hooks (`useState`, `useEffect`)

---

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/responsive-news-payout-dashboard.git
    cd responsive-news-payout-dashboard
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Run the development server:**

    ```bash
    npm start
    ```

4. **Open your browser** and navigate to:

    ```bash
    http://localhost:3000
    ```

---

## Environment Variables

You will need to create a **NewsAPI key** for the app to fetch news articles. Follow these steps:

1. Go to [NewsAPI](https://newsapi.org/) and sign up.
2. Create an API key.
3. Replace the placeholder API key in the `AdminPanel` component:

    ```javascript
    const apiKey = 'your-api-key';
    ```

---

## Folder Structure

```plaintext
/src
  /components
    AdminPanel.js       // Main dashboard component that manages news articles, payout inputs, and pie chart.
    PayoutChart.js      // Pie chart component for visualizing total payouts.
    Pagination.js       // Pagination component for navigating through news articles.
    Header.js           // Header with dark mode toggle button and user info.
  App.js                // Main app component that integrates all components.
  index.js              // Entry point for React app.
  /assets
    /images             // Any images used in the app.
  /styles
    styles.css          // Custom styles (if any).
```

---

## Customization

### Design and Styling
- Replace the default Bootstrap styling with your own custom design by editing the `styles.css` file.
- Update color palettes, font sizes, and spacing to better match your branding.
- Ensure responsiveness by testing the app on different devices and screen sizes.

### Chart Configuration
- Modify the `PayoutChart.js` component to customize pie chart colors, labels, and animations.
- Use additional Chart.js plugins to enhance functionality, such as tooltips or legends.

### Dark Mode
- Adjust the `Header.js` and `styles.css` to provide distinct styles for dark and light modes.
- Persist dark mode preference using localStorage to retain the user's choice across sessions.

### Pagination
- Update the `Pagination.js` component to support custom page sizes or styling.
- Implement a loading spinner while fetching paginated data for a smoother experience.

### API Integration
- Extend the `AdminPanel.js` component to support additional filters (e.g., categories, regions) when fetching articles from NewsAPI.

---

## Future Enhancements

- **User Roles:** Introduce different levels of access for admin and regular users.
- **Analytics:** Add more advanced visualizations like bar charts or trend lines for payouts over time.
- **Offline Support:** Use a service worker to cache articles and payouts for offline viewing.
- **Multi-language Support:** Add support for multiple languages to enhance usability for a global audience.

---

## Conclusion

This responsive news and payout dashboard combines modern design with essential features, making it an excellent tool for managing and visualizing payouts alongside the latest news updates. With its intuitive interface and robust functionality, it can be customized to suit a wide range of applications.
