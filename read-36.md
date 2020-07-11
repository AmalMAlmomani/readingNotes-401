# Application State with Redux

  - **Redux Store**
    - Ultimately, the “store” is where your application state is, well, stored. The store’s job is to identify the various reducers and middleware that need to be made available and used globally.

    - React uses “reducers” to hold and manage state. Reducers typically manage just one part of the larger application state. For example, in a storefront application, you would likely have a separate reducer for Products, Categories, and Carts

## Testing a React-Redux app using Jest and Enzyme
   - **Why did I choose Jest as the testing framework?**
      - Jest was never considered and I was thinking of using either Mocha or Jasmine, as these were the two frameworks I was comfortable with as I have used them on projects related to AngularJS earlier.

   - **These were the points I loved about Jest:**
      - 1. I wanted some framework which could be easily setup and start testing. i.e spend minimum time to setup the framework for my project.
      - 2. Ability to run tests in parallel. This is where Mocha loses the battle for me. Well for this example running the tests in parallel is trivial. But for a huge app with lot of tests, it will be quick if the tests could run in parallel.
      - 3. Snapshot testing. This is a really cool feature I like. This helps me in reducing the number of tests I have to write as I just create a snapshot and if anything changes in my component, I will get an error when the snapshot is generated the next time.
      - 4. Jest uses Jasmine for assertion and since I have used Jasmine earlier, it was easy to write tests for me.
      - 5. Code coverage is available right out of the box.
      - 6. In-built Manual mocking (Haven’t tried yet)

## enzyme-redux Build Status
   - Test utils to simplify testing of containers in redux with enzyme.



   - `jest` — Unit Testing framework for ReactJs developed by Facebook. Read about it here.
   - `babel-jest` — To support ES6 and ES7 for our tests.
   - `enzyme` — JS testing utility developed by Airbnb to make it easier to assert React Components.
   - `react-addons-test-utils` — Provides the React TestUtils which we won’t use directly but it is required as a dependency to enzyme.
   - `react-test-renderer` — Used to grab snapshot of DOM tree rendered by React DOM/ React Native components
   - `redux-mock-store` — Used to mock our Redux store.