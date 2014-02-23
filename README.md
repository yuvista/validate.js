# validate.js

validate.js is a lightweight JavaScript form validation library inspired by CodeIgniter.
validate.js 是一个受Codeigniter启发的轻量级的JavaScript表单验证库。

## Features特性

- Validate form fields from over a dozen rules
- 拥有十多个表单验证规则。
- No dependencies
- 无依赖。
- Customizable Messages
- 可定制的提示消息。
- Supply your own validation callbacks for custom rules
- 支持自定义验证规则。
- Chainable customization methods for ease of declaration
- 链式写法易于定制。
- Works in all major browsers, (even IE6!)
- 支持所有主流浏览器（包括IE6！）
- Modeled off the CodeIgniter form validation API
- 模仿CodeIgniter的表单验证API。

## How to use 使用方式

    var validator = new FormValidator('example_form', [{
        name: 'req',
        display: 'required',    
        rules: 'required'
    }, {
        name: 'alphanumeric',
        rules: 'alpha_numeric'
    }, {
        name: 'password',
        rules: 'required'
    }, {
        name: 'password_confirm',
        display: 'password confirmation',
        rules: 'required|matches[password]'
    }, {
        name: 'email',
        rules: 'valid_email'
    }, {
        name: 'minlength',
        display: 'min length',
        rules: 'min_length[8]'
    }], function(errors) {
        if (errors.length > 0) {
            // Show the errors
        }
    });

## Documentation 文档

You can view everything at http://rickharrison.github.com/validate.js

## Plugins jQuery插件版

jQuery: https://github.com/mahil/validate_helper
