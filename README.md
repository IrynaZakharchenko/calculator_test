# calculator_test

#configure GoogleTest Framework for use in project
cmake -D CMAKE_INSTALL_PREFIX=/home/iraskolnikov/googletest -H/home/iraskolnikov/calculatorTest/googletest -B/home/iraskolnikov/googletest/build

#install GTest
cmake --build /home/iraskolnikov/googletest --target install

#configure project
cmake -D GTEST_ROOT=/home/iraskolnikov/googletest
#build
cmake --build /home/iraskolnikov/calculatorTest/build --target All
