# IronMaidensBnb: React codealong


Codealong to practice React (React Router, useEffect, APIs, etc)

- Goal (wireframes): [https://whimsical.com/react-ironbnb-MVw1gkTJrekF2QTaEKCMJU](https://whimsical.com/react-ironbnb-MVw1gkTJrekF2QTaEKCMJU)

- Backend API (IronBnB API): [https://ironbnb-m3.herokuapp.com](https://ironbnb-m3.herokuapp.com)

- Demo: [https://react-ironbnb-client.netlify.app/](https://react-ironbnb-client.netlify.app/)



## To-Do List

- [x] General structure and routing
- [x] Functionality to display list of apartments from the API
- [ ] Functionality to display details for each apartment
- [x] Functionality to create new apartments
- [ ] Further improvements (see below)


## Step 1: structure, NavBar, HomePage

Components:
- `<NavBar />`
- `<HomePage />`


## Step 2: ApartmentsList

List all apartments:
- path: `/apartments`
- component: `<ApartmentsList />`



## Step 3: ApartmentDetails

Apartment details:
- path: `/apartments/42`
- component: `<ApartmentDetails />`


## Step 4: Create new Apartment

Create new apartment:
- path: `/apartments/create`
- component: `<CreateApartment />`


## Improvements

- [x] Store API baseUrl in .env
- [ ] Single API call to get the info (instead of calling the API in `<ApartmentsList>` and `<ApartmentDetails>`)
  - Make one single call to the API in `<App>`
  - Pass the info as props to `<ApartmentsList>` and `<ApartmentDetails>`
- [ ] Conditional rendering: if an apartment has no image, display a default image
- [ ] Conditional rendering: if data from the API is not ready, display a message "loading"
- [ ] Display spinner/loader while data is loading
- [ ] Apply different ways to style React components (inline css, plain css with one file per component, scss...)
- [ ] (advanced) create a service (a function or class in charge of all requests to the api; we did that in m2 at some point)
- [ ] (advanced) Convert all function components to class components (note: the syntax to use props, state and api requests is a bit different in class components; do some research)
