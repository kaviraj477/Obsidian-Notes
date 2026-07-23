
| LOCATOR         | XPATH METHOD<br>                                                              | CSS METHOD                                                   |
| --------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------ |
| ID / attribute  | //tagName[@ID='attributeValue']<br>//tagName[@attributeName='attributeValue'] | tagName#IdValue,<br>tagname[attributeName = 'attriuteValue'] |
| Text            | //tagName[text()='Value']                                                     | ---------------------------------                            |
| Text space      | //tagName[noramalize-space()='value']                                         | ---------------------------------                            |
| Contains        | //tagName[contains(@attributeName,'attributeValue')]                          | (\*) tagname[att.Name\*='att.Value']                         |
| " "Text         | //tagName[contains(text(),'value')]                                           | -------------------------------                              |
| starts-with     | //tagName[starts-with(@attributeName,'attributeValue')]                       | (^) tagname[att.Name^='att.Value']                           |
| " "Text         | //tagName[starts-with(text(),'value')]                                        |                                                              |
| ends-with       | //tagName[ends-with(@attributeName,'attributeValue')]                         | tagname[attName$='attValue']                                 |
| ClassName       |                                                                               | tagName.classValue                                           |
| immediate child | Xpath we use (/)                                                              | immediate child (>)                                          |
| Subchild        |                                                                               | space (   )                                                  |
| LinkText        | driver.findElement(By.linkText("exact link text"));                           |                                                              |
| Tag             | driver.findElement(By.xpath("//tag[@attribute='value']"));                    |                                                              |
| TagName         | driver.findElement(By.tagName("value"));                                      |                                                              |
| Partial         | driver.findElement(By.partialLinkText("partial text"));                       |                                                              |
| Name            | driver.findElement(By.name("value"));                                         |                                                              |
