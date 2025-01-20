# Next.js 404 Error on Navigation

This repository demonstrates a common issue in Next.js applications where navigation between pages using the Link component results in a 404 error, even when the target page exists.

## Bug Description

A Next.js application is built with two pages: `Home` and `About`. A Link component is used to navigate from the Home page to the About page.  Despite the About page being correctly implemented, navigating to it results in a 404 error.

## Reproduction Steps

1. Clone the repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about` from the home page.  A 404 error will be encountered.

## Solution

The solution involves verifying the file paths and ensuring there are no typos in the `href` prop of the Link component. Additionally, restarting the development server or rebuilding the app might resolve some issues. In some cases, the problem may lie within the routing configuration or conflicting imports.