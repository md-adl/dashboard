# Project Code Refactoring Process

This document outlines the steps taken to refactor the project code to its final version.

Assignment Link: https://dashboardyum.vercel.app/
## Step 1: Project Setup

1. Created a new React project.
2. Installed basic dependencies.

## Step 2: Reverse Engineering Approach

1 Utilized a bottom-up reverse engineering technique to import only necessary components, functions, data, images, helpers, styles, and dependencies.

2 I removed all unnecessary images from helpers and image.js 

3 Removed restaurantsData ,sellersData and orderProgressData from asset/data.js which is unnecesary for Dashboard  and all related Icon

4 Removed getFilteredProducts , getAllRestaurants, getRestaurantById, getSellerById, getOrderHistoryById function  and all unnessary import from helpers/data.js which in unnessary function for dasboard

5 Removed specialMenuData and all unnessary icon for dashboard from assets/dishes.js

6 Removed consumerReviews cardsData , restaurantsData ,sellersData, transactionHistoryData, adminDishListData from assets/other.js which is Unnessary for Dashboard and Removed all unnessary Icons

7 I increased the Performance and checked using Chrome developer tool LightHouse : Performance = 91% , Accessibility = 84% , Best Practices = 96% SEO = 82%

Link for LightHouse Result : https://drive.google.com/file/d/1ucQc-JxhcYZ6mC2eY5VJncnwv3w5I7Z_/view?usp=sharing

## Step 3: Refactoring Process

1. Started with `App.js`.
   - Identified the main page structure in `App.js`.
   - Example: Found main page structure in `App.js` under `AllRoutes -> allAdminFlattedRoutes -> adminRoutes -> Dashboard`.
2. Imported only necessary components from `App.js`.
   - Imported subsequent nested components within `App.js`.
3. Utilized browser debugger.
   - Identified missing files in components/data files.
4. Eliminated unnecessary dependencies.
   - Removed `react-router-dom` as the project is a standalone page.
5. Imported only necessary functions, data, images, helpers, styles, and dependencies in the same manner.

## Conclusion

By following the reverse engineering approach and selectively importing required components and dependencies, the project code was refactored efficiently to its final version.
