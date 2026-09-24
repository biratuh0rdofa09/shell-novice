version: 2.1

jobs:
  build:
    docker:
      - image: cimg/base:stable
    steps:
      - checkout
      - run:
          name: Say Hello
          command: echo "CircleCI setup complete!"

workflows:
  sample-workflow:
    jobs:
      - build
