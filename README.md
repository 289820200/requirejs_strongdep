# requirejs_strongdep
requirejs support strong depend version, Test for typescript



这是requirejs的一个变种，这个版本在requirejs的基础上加上了强依赖加载的逻辑。

使用方式：在 require.config中加入strong_deps项，代表强依赖表，requirejs_strongdep根据这个强依赖表对脚本进行依赖加载。

格式为：

require.config({ strong_deps: { "Test/TestA" : {"TestB": true} } });

示例中代表Test/TestA强依赖于TestB, 支持多个强依赖。
