# 0x03-Unittests_and_integration_tests

## Description 
Unit testing

## how to run unit test
python -m unittest path/to/test_file.py

## Files
### Required files 
* [Utils.py](utils.py "Utils.py") 
* [Fixtures.py](fixtures.py "Fixtures.py")
* [Client.py](client.py "Client.py")

### Task Files
* [0. Parameterize a unit test](test_utils.py "0. Parameterize a unit test")
        ** writing the first unit test for utils.access_nested_map
        ** creating TestAccessNestedMap class that inherits from unittest.TestCase
        ** Implementing estAccessNestedMap.test_access_nested_map method to test that the method returns what it is supposed to.

    #### How to install paramaterized
        * pip install parameterized
* [1. Parameterize a unit test](test_utils.py "1. Parameterize a unit test")
        ** Implementing TestAccessNestedMap.test_access_nested_map_exception
        ** Defining the TestGetJson(unittest.TestCase) class and implement the TestGetJson.test_get_json method to test that utils.get_json returns the expected result.
        ** Implementing the TestMemoize(unittest.TestCase) class with a test_memoize method.
* [4. Parameterize and patch as decorators](test_client.py "4. Parameterize and patch as decorators")
        ** Use @patch as a decorator to make sure get_json is called once with the expected argument but make sure it is not executed.
        ** Use @parameterized.expand as a decorator to parametrize the test with a couple of org examples to pass to GithubOrgClient, in this order: google & abc.
