## How to handle multiple tabs in automation test in Pytest on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Pytest-multiple-tabs)

If you want to handle multiple tabs using an automation test in Pytest on LambdaTest, you can use the follwing steps. You can refer to sample test repo [here](https://github.com/LambdaTest/pytest-selenium-sample).

### Code

To open a new tab, you can use the following line of code:

```python
driver.execute_script("window.open('about:blank','secondtab');")
```

To switch to the new tab, you can use the following line of code:

```python
#by using tab name
driver.switch_to.window("secondtab")
```
or
```python
#by using tab id
driver.switch_to.window("2")
```

For full code, refer to `tests/tab_switch.py`.
### Run your test

```bash
python tabs.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

