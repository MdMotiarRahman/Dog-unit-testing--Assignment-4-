# Dog API Testing – Quick Guide

## 1. Install Dependencies

Run this first:

cd server
npm install

## 2. Run API Tests

Execute the backend tests:

npm run test:run

## 3. Run End-to-End Tests

Run Playwright tests for the frontend:

npm run test:e2e

## 4. View Test Report

npx playwright show-report

## 5. Start the Server

npm start

Server runs at:
http://localhost:5050

## API Endpoints

GET /api/dogs/random – Returns a random dog image (HTTPS URL)
GET /api/health – Health check endpoint

## Test Evidence
REST Client (Test 1 & 2)
Open test.rest in VS Code and click "Send Request" buttons:

TEST 1: Click to see HTTP 200 response with success=true and imageUrl
TEST 2: Click to see HTTP 404 error response
## Playwright Report (Test 3, 4, 5)
Run npx playwright show-report to view detailed E2E test results across Chromium, Firefox, and WebKit browsers

## Browser Testing
Visit http://localhost:5050 to manually test the frontend:

Images load on page initialization
Images load when clicking the "Load Random Dog" button
Error message displays when API is unavailable
## Dependencies
Express.js - Web framework
TypeScript - Type safety
Vitest - Unit testing framework
Supertest - HTTP assertion library
Playwright - E2E testing framework
TSX - TypeScript execution