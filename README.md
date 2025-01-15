# Next.js 15 App Router - About Page Not Rendering

This repository demonstrates a Next.js 15 App Router issue where the about page fails to render correctly after deployment to Vercel.  The application uses the new App Router and includes a simple link from the home page to the about page.  While the application functions locally, the about page is not accessible after deployment.

## Issue

The problem lies in how the app router handles routing, especially concerning dynamically generated pages and client-side navigation using the `<Link>` component.  After deployment, clicking on the link to the about page leads to a blank page or unexpected behavior.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to `/about` - the about page should render correctly.
5. Deploy to Vercel (or another platform).
6. Navigate to `/about` on the deployed app - the about page will not render as expected.

## Solution

The solution involves ensuring correct configuration of the App Router and the handling of client-side navigation.  Refer to the `solution` branch for a possible fix.