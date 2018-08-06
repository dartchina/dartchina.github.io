    {% comment %}
    This file is generated from the other files in this directory.
    To re-generate it, please run the following command from root of
    the project:

      $ dart deploy/effective-dart-rules/bin/main.dart

    {% endcomment %}
    
<div class='effective_dart--summary_column' markdown='1'>

### Style


**标识符**

* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E4%BD%BF%E7%94%A8-uppercamelcase-%E9%A3%8E%E6%A0%BC%E5%91%BD%E5%90%8D%E7%B1%BB%E5%9E%8B'><strong>要</strong> 使用 <code>UpperCamelCase</code> 风格命名类型。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E7%94%A8-lowercase_with_underscores-%E9%A3%8E%E6%A0%BC%E5%91%BD%E5%90%8D%E5%BA%93%E5%92%8C%E6%BA%90%E6%96%87%E4%BB%B6%E5%90%8D'><strong>要</strong> 用 <code>lowercase_with_underscores</code> 风格命名库和源文件名。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E4%BD%BF%E7%94%A8-lowercase_with_underscores-%E9%A3%8E%E6%A0%BC%E5%91%BD%E5%90%8D%E5%AF%BC%E5%85%A5%E7%9A%84%E5%89%8D%E7%BC%80'><strong>要</strong> 使用 <code>lowercase_with_underscores</code> 风格命名导入的前缀。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E4%BD%BF%E7%94%A8-lowercamelcase-%E9%A3%8E%E6%A0%BC%E6%9D%A5%E5%91%BD%E5%90%8D%E5%85%B6%E4%BB%96%E7%9A%84%E6%A0%87%E8%AF%86%E7%AC%A6'><strong>要</strong> 使用 <code>lowerCamelCase</code> 风格来命名其他的标识符。</a>
* <a href='/guides/language/effective-dart/style#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8-lowercamelcase-%E6%9D%A5%E5%91%BD%E5%90%8D%E5%B8%B8%E9%87%8F'><strong>推荐</strong> 使用 <code>lowerCamelCase</code> 来命名常量。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E6%8A%8A%E8%B6%85%E8%BF%87%E4%B8%A4%E4%B8%AA%E5%AD%97%E6%AF%8D%E7%9A%84%E9%A6%96%E5%AD%97%E6%AF%8D%E5%A4%A7%E5%86%99%E7%BC%A9%E7%95%A5%E8%AF%8D%E5%92%8C%E7%BC%A9%E5%86%99%E8%AF%8D%E5%BD%93%E5%81%9A%E4%B8%80%E8%88%AC%E5%8D%95%E8%AF%8D%E6%9D%A5%E5%AF%B9%E5%BE%85'><strong>要</strong> 把超过两个字母的首字母大写缩略词和缩写词当做一般单词来对待。</a>
* <a href='/guides/language/effective-dart/style#%E4%B8%8D%E8%A6%81-%E4%BD%BF%E7%94%A8%E5%89%8D%E7%BC%80%E5%AD%97%E6%AF%8D'><strong>不要</strong> 使用前缀字母</a>

**顺序**

* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E6%8A%8A-dart-%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E6%94%BE%E5%88%B0%E5%85%B6%E4%BB%96%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E4%B9%8B%E5%89%8D'><strong>要</strong> 把 "dart:" 导入语句放到其他导入语句之前。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E6%8A%8A-package-%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E6%94%BE%E5%88%B0%E9%A1%B9%E7%9B%AE%E7%9B%B8%E5%85%B3%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E4%B9%8B%E5%89%8D'><strong>要</strong> 把 "package:" 导入语句放到项目相关导入语句之前。</a>
* <a href='/guides/language/effective-dart/style#%E6%8E%A8%E8%8D%90-%E6%8A%8A%E7%AC%AC%E4%B8%89%E6%96%B9-package-%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E6%94%BE%E5%88%B0%E5%85%B6%E4%BB%96%E8%AF%AD%E5%8F%A5%E4%B9%8B%E5%89%8D'><strong>推荐</strong> 把"第三方" "package:" 导入语句放到其他语句之前。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E6%8A%8A%E5%AF%BC%E5%87%BAexport%E8%AF%AD%E5%8F%A5%E4%BD%9C%E4%B8%BA%E4%B8%80%E4%B8%AA%E5%8D%95%E7%8B%AC%E7%9A%84%E9%83%A8%E5%88%86%E6%94%BE%E5%88%B0%E6%89%80%E6%9C%89%E5%AF%BC%E5%85%A5%E8%AF%AD%E5%8F%A5%E4%B9%8B%E5%90%8E'><strong>要</strong> 把导出（export）语句作为一个单独的部分放到所有导入语句之后。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E6%8C%89%E7%85%A7%E5%AD%97%E6%AF%8D%E9%A1%BA%E5%BA%8F%E6%9D%A5%E6%8E%92%E5%BA%8F%E6%AF%8F%E4%B8%AA%E9%83%A8%E5%88%86%E4%B8%AD%E7%9A%84%E8%AF%AD%E5%8F%A5'><strong>要</strong> 按照字母顺序来排序每个部分中的语句。</a>

**格式化**

* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E4%BD%BF%E7%94%A8-dartfmt-%E6%A0%BC%E5%BC%8F%E5%8C%96%E4%BD%A0%E7%9A%84%E4%BB%A3%E7%A0%81'><strong>要</strong> 使用 <code>dartfmt</code> 格式化你的代码。</a>
* <a href='/guides/language/effective-dart/style#%E8%80%83%E8%99%91-changing-your-code-to-make-it-more-formatter-friendly'><strong>考虑</strong> changing your code to make it more formatter-friendly.</a>
* <a href='/guides/language/effective-dart/style#%E9%81%BF%E5%85%8D-%E5%8D%95%E8%A1%8C%E8%B6%85%E8%BF%87-80-%E4%B8%AA%E5%AD%97%E7%AC%A6'><strong>避免</strong> 单行超过 80 个字符。</a>
* <a href='/guides/language/effective-dart/style#%E8%A6%81-%E5%AF%B9%E6%89%80%E6%9C%89%E6%B5%81%E6%8E%A7%E5%88%B6%E7%BB%93%E6%9E%84%E4%BD%BF%E7%94%A8%E8%8A%B1%E6%8B%AC%E5%8F%B7'><strong>要</strong> 对所有流控制结构使用花括号。</a>

</div>
<div class='effective_dart--summary_column' markdown='1'>


### Documentation


**注释**

* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E5%83%8F%E5%8F%A5%E5%AD%90%E4%B8%80%E6%A0%B7%E6%9D%A5%E6%A0%BC%E5%BC%8F%E5%8C%96%E6%B3%A8%E9%87%8A'><strong>要</strong> 像句子一样来格式化注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E4%B8%8D%E8%A6%81-%E4%BD%BF%E7%94%A8%E5%9D%97%E6%B3%A8%E9%87%8A%E4%BD%9C%E7%94%A8%E4%BD%9C%E8%A7%A3%E9%87%8A%E8%AF%B4%E6%98%8E'><strong>不要</strong> 使用块注释作用作解释说明。</a>

**文档注释**

* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E4%BD%BF%E7%94%A8--%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A%E6%9D%A5%E6%B3%A8%E9%87%8A%E6%88%90%E5%91%98%E5%92%8C%E7%B1%BB%E5%9E%8B'><strong>要</strong> 使用 <code>///</code> 文档注释来注释成员和类型。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%B8%BA%E5%85%AC%E5%BC%80%E5%8F%91%E5%B8%83%E7%9A%84-api-%E7%BC%96%E5%86%99%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A'><strong>推荐</strong> 为公开发布的 API 编写文档注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%80%83%E8%99%91-%E7%BC%96%E5%86%99%E5%BA%93%E7%BA%A7%E5%88%ABlibrary-level%E7%9A%84%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A'><strong>考虑</strong> 编写库级别（library-level）的文档注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%B8%BA%E7%A7%81%E6%9C%89api-%E7%BC%96%E5%86%99%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A'><strong>推荐</strong> 为私有API 编写文档注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E8%A6%81%E5%9C%A8%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A%E5%BC%80%E5%A4%B4%E6%9C%89%E4%B8%80%E4%B8%AA%E5%8D%95%E5%8F%A5%E6%80%BB%E7%BB%93'><strong>要</strong> 要在文档注释开头有一个单句总结。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E8%AE%A9%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A%E7%9A%84%E7%AC%AC%E4%B8%80%E5%8F%A5%E4%BB%8E%E6%AE%B5%E8%90%BD%E4%B8%AD%E5%88%86%E5%BC%80'><strong>要</strong> 让文档注释的第一句从段落中分开。</a>
* <a href='/guides/language/effective-dart/documentation#%E9%81%BF%E5%85%8D-%E4%B8%8E%E5%91%A8%E5%9B%B4%E4%B8%8A%E4%B8%8B%E6%96%87%E5%86%97%E4%BD%99'><strong>避免</strong> 与周围上下文冗余。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E7%94%A8%E7%AC%AC%E4%B8%89%E4%BA%BA%E7%A7%B0%E6%9D%A5%E5%BC%80%E5%A7%8B%E5%87%BD%E6%95%B0%E6%88%96%E8%80%85%E6%96%B9%E6%B3%95%E7%9A%84%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A'><strong>推荐</strong> 用第三人称来开始函数或者方法的文档注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8%E5%90%8D%E8%AF%8D%E7%9F%AD%E8%AF%AD%E6%9D%A5%E5%BC%80%E5%A7%8B%E5%8F%98%E9%87%8Fgettersetter-%E7%9A%84%E6%B3%A8%E9%87%8A'><strong>推荐</strong> 使用名词短语来开始变量、getter、setter 的注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8%E5%90%8D%E8%AF%8D%E7%9F%AD%E8%AF%AD%E6%9D%A5%E5%BC%80%E5%A7%8B%E5%BA%93%E5%92%8C%E7%B1%BB%E5%9E%8B%E6%B3%A8%E9%87%8A'><strong>推荐</strong> 使用名词短语来开始库和类型注释。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%80%83%E8%99%91-%E5%9C%A8%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A%E4%B8%AD%E6%B7%BB%E5%8A%A0%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81'><strong>考虑</strong> 在文档注释中添加示例代码。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E4%BD%BF%E7%94%A8%E6%96%B9%E6%8B%AC%E5%8F%B7%E5%9C%A8%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A%E4%B8%AD%E5%BC%95%E7%94%A8%E4%BD%9C%E7%94%A8%E5%9F%9F%E5%86%85%E7%9A%84%E6%A0%87%E8%AF%86%E7%AC%A6'><strong>要</strong> 使用方括号在文档注释中引用作用域内的标识符。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E4%BD%BF%E7%94%A8%E6%95%A3%E6%96%87%E7%9A%84%E6%96%B9%E5%BC%8F%E6%9D%A5%E6%8F%8F%E8%BF%B0%E5%8F%82%E6%95%B0%E8%BF%94%E5%9B%9E%E5%80%BC%E4%BB%A5%E5%8F%8A%E5%BC%82%E5%B8%B8%E4%BF%A1%E6%81%AF'><strong>要</strong> 使用散文的方式来描述参数、返回值以及异常信息。</a>
* <a href='/guides/language/effective-dart/documentation#%E8%A6%81-%E6%8A%8A%E6%B3%A8%E9%87%8A%E6%96%87%E6%A1%A3%E6%94%BE%E5%88%B0%E6%B3%A8%E8%A7%A3%E4%B9%8B%E5%89%8D'><strong>要</strong> 把注释文档放到注解之前。</a>

**Markdown**

* <a href='/guides/language/effective-dart/documentation#%E9%81%BF%E5%85%8D-%E8%BF%87%E5%BA%A6%E4%BD%BF%E7%94%A8-markdown'><strong>避免</strong> 过度使用 markdown。</a>
* <a href='/guides/language/effective-dart/documentation#%E9%81%BF%E5%85%8D-%E4%BD%BF%E7%94%A8-html-%E6%9D%A5%E6%A0%BC%E5%BC%8F%E5%8C%96%E6%96%87%E5%AD%97'><strong>避免</strong> 使用 HTML 来格式化文字。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8%E5%8F%8D%E5%BC%95%E5%8F%B7%E6%A0%87%E6%B3%A8%E4%BB%A3%E7%A0%81'><strong>推荐</strong> 使用反引号标注代码。</a>

**如何写注释**

* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E7%AE%80%E6%B4%81'><strong>推荐</strong> 简洁.</a>
* <a href='/guides/language/effective-dart/documentation#%E9%81%BF%E5%85%8D-%E7%BC%A9%E5%86%99%E5%92%8C%E9%A6%96%E5%AD%97%E6%AF%8D%E7%BC%A9%E5%86%99%E8%AF%8D%E9%99%A4%E9%9D%9E%E5%BE%88%E5%B8%B8%E8%A7%81'><strong>避免</strong> 缩写和首字母缩写词，除非很常见。</a>
* <a href='/guides/language/effective-dart/documentation#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8-this-%E8%80%8C%E4%B8%8D%E6%98%AF-the-%E6%9D%A5%E5%BC%95%E7%94%A8%E5%AE%9E%E4%BE%8B%E6%88%90%E5%91%98'><strong>推荐</strong> 使用 "this" 而不是 "the" 来引用实例成员。</a>

</div>
<div style='clear:both'></div>
<div class='effective_dart--summary_column' markdown='1'>


### Usage


**Libraries**


**库**

* <a href='/guides/language/effective-dart/usage#do-use-strings-in-part-of-directives'>DO use strings in <code>part of</code> directives.</a>
* <a href='/guides/language/effective-dart/usage#%E8%A6%81-%E5%9C%A8-part-of-%E4%B8%AD%E4%BD%BF%E7%94%A8%E5%AD%97%E7%AC%A6%E4%B8%B2'><strong>要</strong> 在 <code>part of</code> 中使用字符串。</a>
* <a href='/guides/language/effective-dart/usage#dont-import-libraries-that-are-inside-the-src-directory-of-another-package'>DON'T import libraries that are inside the <code>src</code> directory of another package.</a>
* <a href='/guides/language/effective-dart/usage#%E4%B8%8D%E8%A6%81-%E5%AF%BC%E5%85%A5-package-%E4%B8%AD-src-%E7%9B%AE%E5%BD%95%E4%B8%8B%E7%9A%84%E5%BA%93'><strong>不要</strong> 导入 package 中 <code>src</code> 目录下的库。</a>
* <a href='/guides/language/effective-dart/usage#prefer-relative-paths-when-importing-libraries-within-your-own-packages-lib-directory'>PREFER relative paths when importing libraries within your own package's <code>lib</code> directory.</a>
* <a href='/guides/language/effective-dart/usage#%E5%BB%BA%E8%AE%AE-%E4%BD%BF%E7%94%A8%E7%9B%B8%E5%AF%B9%E8%B7%AF%E5%BE%84%E5%9C%A8%E5%AF%BC%E5%85%A5%E4%BD%A0%E8%87%AA%E5%B7%B1-package-%E4%B8%AD%E7%9A%84-lib-%E7%9B%AE%E5%BD%95'><strong>建议</strong> 使用相对路径在导入你自己 package 中的 <code>lib</code> 目录。</a>

**Strings**


**字符串**

* <a href='/guides/language/effective-dart/usage#do-use-adjacent-strings-to-concatenate-string-literals'>DO use adjacent strings to concatenate string literals.</a>
* <a href='/guides/language/effective-dart/usage#%E8%A6%81-%E4%BD%BF%E7%94%A8%E4%B8%B4%E8%BF%91%E5%AD%97%E7%AC%A6%E5%AD%97%E7%9A%84%E6%96%B9%E5%BC%8F%E8%BF%9E%E6%8E%A5%E5%AD%97%E9%9D%A2%E9%87%8F%E5%AD%97%E7%AC%A6%E4%B8%B2'><strong>要</strong> 使用临近字符字的方式连接字面量字符串。</a>
* <a href='/guides/language/effective-dart/usage#prefer-using-interpolation-to-compose-strings-and-values'>PREFER using interpolation to compose strings and values.</a>
* <a href='/guides/language/effective-dart/usage#%E6%8E%A8%E8%8D%90-%E4%BD%BF%E7%94%A8%E6%8F%92%E5%80%BC%E7%9A%84%E5%BD%A2%E5%BC%8F%E6%9D%A5%E7%BB%84%E5%90%88%E5%AD%97%E7%AC%A6%E4%B8%B2%E5%92%8C%E5%80%BC'><strong>推荐</strong> 使用插值的形式来组合字符串和值。</a>
* <a href='/guides/language/effective-dart/usage#avoid-using-curly-braces-in-interpolation-when-not-needed'>AVOID using curly braces in interpolation when not needed.</a>
* <a href='/guides/language/effective-dart/usage#%E9%81%BF%E5%85%8D-%E5%9C%A8%E5%AD%97%E7%AC%A6%E4%B8%B2%E6%8F%92%E5%80%BC%E4%B8%AD%E4%BD%BF%E7%94%A8%E4%B8%8D%E5%BF%85%E8%A6%81%E7%9A%84%E5%A4%A7%E6%8B%AC%E5%8F%B7'><strong>避免</strong> 在字符串插值中使用不必要的大括号。</a>

**Collections**


**集合**

* <a href='/guides/language/effective-dart/usage#do-use-collection-literals-when-possible'>DO use collection literals when possible.</a>
* <a href='/guides/language/effective-dart/usage#%E8%A6%81-%E5%B0%BD%E5%8F%AF%E8%83%BD%E7%9A%84%E4%BD%BF%E7%94%A8%E9%9B%86%E5%90%88%E5%AD%97%E9%9D%A2%E9%87%8F'><strong>要</strong> 尽可能的使用集合字面量。</a>
* <a href='/guides/language/effective-dart/usage#dont-use-length-to-see-if-a-collection-is-empty'>DON'T use <code>.length</code> to see if a collection is empty.</a>
* <a href='/guides/language/effective-dart/usage#%E4%B8%8D%E8%A6%81-%E4%BD%BF%E7%94%A8-length-%E6%9D%A5%E5%88%A4%E6%96%AD%E4%B8%80%E4%B8%AA%E9%9B%86%E5%90%88%E6%98%AF%E5%90%A6%E4%B8%BA%E7%A9%BA'><strong>不要</strong> 使用 <code>.length</code> 来判断一个集合是否为空。</a>
* <a href='/guides/language/effective-dart/usage#consider-using-higher-order-methods-to-transform-a-sequence'>CONSIDER using higher-order methods to transform a sequence.</a>
* <a href='/guides/language/effective-dart/usage#%E8%80%83%E8%99%91-%E4%BD%BF%E7%94%A8%E9%AB%98%E9%98%B6higher-order%E5%87%BD%E6%95%B0%E6%9D%A5%E8%BD%AC%E6%8D%A2%E9%9B%86%E5%90%88%E6%95%B0%E6%8D%AE'><strong>考虑</strong> 使用高阶（higher-order）函数来转换集合数据。</a>
* <a href='/guides/language/effective-dart/usage#avoid-using-iterableforeach-with-a-function-literal'>AVOID using <code>Iterable.forEach()</code> with a function literal.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-listfrom-unless-you-intend-to-change-the-type-of-the-result'>DON'T use <code>List.from()</code> unless you intend to change the type of the result.</a>
* <a href='/guides/language/effective-dart/usage#do-use-wheretype-to-filter-a-collection-by-type'>DO use <code>whereType()</code> to filter a collection by type.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-cast-when-a-nearby-operation-will-do'>DON'T use <code>cast()</code> when a nearby operation will do.</a>
* <a href='/guides/language/effective-dart/usage#avoid-using-cast'>AVOID using <code>cast()</code>.</a>

**Functions**

* <a href='/guides/language/effective-dart/usage#do-use-a-function-declaration-to-bind-a-function-to-a-name'>DO use a function declaration to bind a function to a name.</a>
* <a href='/guides/language/effective-dart/usage#dont-create-a-lambda-when-a-tear-off-will-do'>DON'T create a lambda when a tear-off will do.</a>

**Parameters**

* <a href='/guides/language/effective-dart/usage#do-use--to-separate-a-named-parameter-from-its-default-value'>DO use <code>=</code> to separate a named parameter from its default value.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-an-explicit-default-value-of-null'>DON'T use an explicit default value of <code>null</code>.</a>

**Variables**

* <a href='/guides/language/effective-dart/usage#dont-explicitly-initialize-variables-to-null'>DON'T explicitly initialize variables to <code>null</code>.</a>
* <a href='/guides/language/effective-dart/usage#avoid-storing-what-you-can-calculate'>AVOID storing what you can calculate.</a>

**Members**

* <a href='/guides/language/effective-dart/usage#dont-wrap-a-field-in-a-getter-and-setter-unnecessarily'>DON'T wrap a field in a getter and setter unnecessarily.</a>
* <a href='/guides/language/effective-dart/usage#prefer-using-a-final-field-to-make-a-read-only-property'>PREFER using a <code>final</code> field to make a read-only property.</a>
* <a href='/guides/language/effective-dart/usage#consider-using--for-simple-members'>CONSIDER using <code>=&gt;</code> for simple members.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-this-when-not-needed-to-avoid-shadowing'>DON'T use <code>this.</code> when not needed to avoid shadowing.</a>
* <a href='/guides/language/effective-dart/usage#do-initialize-fields-at-their-declaration-when-possible'>DO initialize fields at their declaration when possible.</a>

**Constructors**

* <a href='/guides/language/effective-dart/usage#do-use-initializing-formals-when-possible'>DO use initializing formals when possible.</a>
* <a href='/guides/language/effective-dart/usage#dont-type-annotate-initializing-formals'>DON'T type annotate initializing formals.</a>
* <a href='/guides/language/effective-dart/usage#do-use--instead-of--for-empty-constructor-bodies'>DO use <code>;</code> instead of <code>{}</code> for empty constructor bodies.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-new'>DON'T use <code>new</code>.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-const-redundantly'>DON'T use <code>const</code> redundantly.</a>

**Error handling**

* <a href='/guides/language/effective-dart/usage#avoid-catches-without-on-clauses'>AVOID catches without <code>on</code> clauses.</a>
* <a href='/guides/language/effective-dart/usage#dont-discard-errors-from-catches-without-on-clauses'>DON'T discard errors from catches without <code>on</code> clauses.</a>
* <a href='/guides/language/effective-dart/usage#do-throw-objects-that-implement-error-only-for-programmatic-errors'>DO throw objects that implement <code>Error</code> only for programmatic errors.</a>
* <a href='/guides/language/effective-dart/usage#dont-explicitly-catch-error-or-types-that-implement-it'>DON'T explicitly catch <code>Error</code> or types that implement it.</a>
* <a href='/guides/language/effective-dart/usage#do-use-rethrow-to-rethrow-a-caught-exception'>DO use <code>rethrow</code> to rethrow a caught exception.</a>

**Asynchrony**

* <a href='/guides/language/effective-dart/usage#prefer-asyncawait-over-using-raw-futures'>PREFER async/await over using raw futures.</a>
* <a href='/guides/language/effective-dart/usage#dont-use-async-when-it-has-no-useful-effect'>DON'T use <code>async</code> when it has no useful effect.</a>
* <a href='/guides/language/effective-dart/usage#consider-using-higher-order-methods-to-transform-a-stream'>CONSIDER using higher-order methods to transform a stream.</a>
* <a href='/guides/language/effective-dart/usage#avoid-using-completer-directly'>AVOID using Completer directly.</a>
* <a href='/guides/language/effective-dart/usage#do-test-for-futuret-when-disambiguating-a-futureort-whose-type-argument-could-be-object'>DO test for <code>Future&lt;T&gt;</code> when disambiguating a <code>FutureOr&lt;T&gt;</code> whose type argument could be <code>Object</code>.</a>

</div>
<div class='effective_dart--summary_column' markdown='1'>


### Design


**Names**

* <a href='/guides/language/effective-dart/design#do-use-terms-consistently'>DO use terms consistently.</a>
* <a href='/guides/language/effective-dart/design#avoid-abbreviations'>AVOID abbreviations.</a>
* <a href='/guides/language/effective-dart/design#prefer-putting-the-most-descriptive-noun-last'>PREFER putting the most descriptive noun last.</a>
* <a href='/guides/language/effective-dart/design#consider-making-the-code-read-like-a-sentence'>CONSIDER making the code read like a sentence.</a>
* <a href='/guides/language/effective-dart/design#prefer-a-noun-phrase-for-a-non-boolean-property-or-variable'>PREFER a noun phrase for a non-boolean property or variable.</a>
* <a href='/guides/language/effective-dart/design#prefer-a-non-imperative-verb-phrase-for-a-boolean-property-or-variable'>PREFER a non-imperative verb phrase for a boolean property or variable.</a>
* <a href='/guides/language/effective-dart/design#consider-omitting-the-verb-for-a-named-boolean-parameter'>CONSIDER omitting the verb for a named boolean <em>parameter</em>.</a>
* <a href='/guides/language/effective-dart/design#prefer-the-positive-name-for-a-boolean-property-or-variable'>PREFER the "positive" name for a boolean property or variable.</a>
* <a href='/guides/language/effective-dart/design#prefer-an-imperative-verb-phrase-for-a-function-or-method-whose-main-purpose-is-a-side-effect'>PREFER an imperative verb phrase for a function or method whose main purpose is a side effect.</a>
* <a href='/guides/language/effective-dart/design#prefer-a-noun-phrase-or-non-imperative-verb-phrase-for-a-function-or-method-if-returning-a-value-is-its-primary-purpose'>PREFER a noun phrase or non-imperative verb phrase for a function or method if returning a value is its primary purpose.</a>
* <a href='/guides/language/effective-dart/design#consider-an-imperative-verb-phrase-for-a-function-or-method-if-you-want-to-draw-attention-to-the-work-it-performs'>CONSIDER an imperative verb phrase for a function or method if you want to draw attention to the work it performs.</a>
* <a href='/guides/language/effective-dart/design#avoid-starting-a-method-name-with-get'>AVOID starting a method name with <code>get</code>.</a>
* <a href='/guides/language/effective-dart/design#prefer-naming-a-method-to___-if-it-copies-the-objects-state-to-a-new-object'>PREFER naming a method <code>to___()</code> if it copies the object's state to a new object.</a>
* <a href='/guides/language/effective-dart/design#prefer-naming-a-method-as___-if-it-returns-a-different-representation-backed-by-the-original-object'>PREFER naming a method <code>as___()</code> if it returns a different representation backed by the original object.</a>
* <a href='/guides/language/effective-dart/design#avoid-describing-the-parameters-in-the-functions-or-methods-name'>AVOID describing the parameters in the function's or method's name.</a>
* <a href='/guides/language/effective-dart/design#do-follow-existing-mnemonic-conventions-when-naming-type-parameters'>DO follow existing mnemonic conventions when naming type parameters.</a>

**Libraries**

* <a href='/guides/language/effective-dart/design#prefer-making-declarations-private'>PREFER making declarations private.</a>
* <a href='/guides/language/effective-dart/design#consider-declaring-multiple-classes-in-the-same-library'>CONSIDER declaring multiple classes in the same library.</a>

**Classes**

* <a href='/guides/language/effective-dart/design#avoid-defining-a-one-member-abstract-class-when-a-simple-function-will-do'>AVOID defining a one-member abstract class when a simple function will do.</a>
* <a href='/guides/language/effective-dart/design#avoid-defining-a-class-that-contains-only-static-members'>AVOID defining a class that contains only static members.</a>
* <a href='/guides/language/effective-dart/design#avoid-extending-a-class-that-isnt-intended-to-be-subclassed'>AVOID extending a class that isn't intended to be subclassed.</a>
* <a href='/guides/language/effective-dart/design#do-document-if-your-class-supports-being-extended'>DO document if your class supports being extended.</a>
* <a href='/guides/language/effective-dart/design#avoid-implementing-a-class-that-isnt-intended-to-be-an-interface'>AVOID implementing a class that isn't intended to be an interface.</a>
* <a href='/guides/language/effective-dart/design#do-document-if-your-class-supports-being-used-as-an-interface'>DO document if your class supports being used as an interface.</a>
* <a href='/guides/language/effective-dart/design#avoid-mixing-in-a-class-that-isnt-intended-to-be-a-mixin'>AVOID mixing in a class that isn't intended to be a mixin.</a>
* <a href='/guides/language/effective-dart/design#do-document-if-your-class-supports-being-used-as-a-mixin'>DO document if your class supports being used as a mixin.</a>

**Constructors**

* <a href='/guides/language/effective-dart/design#prefer-defining-constructors-instead-of-static-methods-to-create-instances'>PREFER defining constructors instead of static methods to create instances.</a>
* <a href='/guides/language/effective-dart/design#consider-making-your-constructor-const-if-the-class-supports-it'>CONSIDER making your constructor <code>const</code> if the class supports it.</a>

**Members**

* <a href='/guides/language/effective-dart/design#prefer-making-fields-and-top-level-variables-final'>PREFER making fields and top-level variables <code>final</code>.</a>
* <a href='/guides/language/effective-dart/design#do-use-getters-for-operations-that-conceptually-access-properties'>DO use getters for operations that conceptually access properties.</a>
* <a href='/guides/language/effective-dart/design#do-use-setters-for-operations-that-conceptually-change-properties'>DO use setters for operations that conceptually change properties.</a>
* <a href='/guides/language/effective-dart/design#dont-define-a-setter-without-a-corresponding-getter'>DON'T define a setter without a corresponding getter.</a>
* <a href='/guides/language/effective-dart/design#avoid-returning-null-from-members-whose-return-type-is-bool-double-int-or-num'>AVOID returning <code>null</code> from members whose return type is <code>bool</code>, <code>double</code>, <code>int</code>, or <code>num</code>.</a>
* <a href='/guides/language/effective-dart/design#avoid-returning-this-from-methods-just-to-enable-a-fluent-interface'>AVOID returning <code>this</code> from methods just to enable a fluent interface.</a>

**Types**

* <a href='/guides/language/effective-dart/design#prefer-type-annotating-public-fields-and-top-level-variables-if-the-type-isnt-obvious'>PREFER type annotating public fields and top-level variables if the type isn't obvious.</a>
* <a href='/guides/language/effective-dart/design#consider-type-annotating-private-fields-and-top-level-variables-if-the-type-isnt-obvious'>CONSIDER type annotating private fields and top-level variables if the type isn't obvious.</a>
* <a href='/guides/language/effective-dart/design#avoid-type-annotating-initialized-local-variables'>AVOID type annotating initialized local variables.</a>
* <a href='/guides/language/effective-dart/design#avoid-annotating-inferred-parameter-types-on-function-expressions'>AVOID annotating inferred parameter types on function expressions.</a>
* <a href='/guides/language/effective-dart/design#avoid-redundant-type-arguments-on-generic-invocations'>AVOID redundant type arguments on generic invocations.</a>
* <a href='/guides/language/effective-dart/design#do-annotate-when-dart-infers-the-wrong-type'>DO annotate when Dart infers the wrong type.</a>
* <a href='/guides/language/effective-dart/design#prefer-annotating-with-dynamic-instead-of-letting-inference-fail'>PREFER annotating with <code>dynamic</code> instead of letting inference fail.</a>
* <a href='/guides/language/effective-dart/design#prefer-signatures-in-function-type-annotations'>PREFER signatures in function type annotations.</a>
* <a href='/guides/language/effective-dart/design#dont-specify-a-return-type-for-a-setter'>DON'T specify a return type for a setter.</a>
* <a href='/guides/language/effective-dart/design#dont-use-the-legacy-typedef-syntax'>DON'T use the legacy typedef syntax.</a>
* <a href='/guides/language/effective-dart/design#prefer-inline-function-types-over-typedefs'>PREFER inline function types over typedefs.</a>
* <a href='/guides/language/effective-dart/design#consider-using-function-type-syntax-for-parameters'>CONSIDER using function type syntax for parameters.</a>
* <a href='/guides/language/effective-dart/design#do-annotate-with-object-instead-of-dynamic-to-indicate-any-object-is-allowed'>DO annotate with <code>Object</code> instead of <code>dynamic</code> to indicate any object is allowed.</a>
* <a href='/guides/language/effective-dart/design#do-use-futurevoid-as-the-return-type-of-asynchronous-members-that-do-not-produce-values'>DO use <code>Future&lt;void&gt;</code> as the return type of asynchronous members that do not produce values.</a>
* <a href='/guides/language/effective-dart/design#avoid-using-futureort-as-a-return-type'>AVOID using <code>FutureOr&lt;T&gt;</code> as a return type.</a>

**Parameters**

* <a href='/guides/language/effective-dart/design#avoid-positional-boolean-parameters'>AVOID positional boolean parameters.</a>
* <a href='/guides/language/effective-dart/design#avoid-optional-positional-parameters-if-the-user-may-want-to-omit-earlier-parameters'>AVOID optional positional parameters if the user may want to omit earlier parameters.</a>
* <a href='/guides/language/effective-dart/design#avoid-mandatory-parameters-that-accept-a-special-no-argument-value'>AVOID mandatory parameters that accept a special "no argument" value.</a>
* <a href='/guides/language/effective-dart/design#do-use-inclusive-start-and-exclusive-end-parameters-to-accept-a-range'>DO use inclusive start and exclusive end parameters to accept a range.</a>

**Equality**

* <a href='/guides/language/effective-dart/design#do-override-hashcode-if-you-override-'>DO override <code>hashCode</code> if you override <code>==</code>.</a>
* <a href='/guides/language/effective-dart/design#do-make-your--operator-obey-the-mathematical-rules-of-equality'>DO make your <code>==</code> operator obey the mathematical rules of equality.</a>
* <a href='/guides/language/effective-dart/design#avoid-defining-custom-equality-for-mutable-classes'>AVOID defining custom equality for mutable classes.</a>
* <a href='/guides/language/effective-dart/design#dont-check-for-null-in-custom--operators'>DON'T check for <code>null</code> in custom <code>==</code> operators.</a>

</div>
<div style='clear:both'></div>
