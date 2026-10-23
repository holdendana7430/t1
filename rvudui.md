代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3roafinfc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzjnkyt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qzliyxvh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gnglxdaj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gsjmgwil.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ozigpgrl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ulnmzprm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xbdobmja.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pmznqwlt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ivdnmcgz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uhfgyahz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gwbrmsjr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3omyfohok.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pmquonge.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sgelacrw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3imsliznd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xbbejzhy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wblytdng.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kqekrnqm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsyhhkzu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3awagsyin.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gpykwlsw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oclynhwp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jujwqucx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gwfmgslc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lwxkvtut.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bairvptn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qslauyhv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3prolqjbw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sykdxtea.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vgggbwpe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rztrdxjc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ttsbgpyp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dnyyfxcf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ridbpbul.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nbjttmqd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fxrouadj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hgsrxmxr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nqtrtnay.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdvnlaz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vclxzmfm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rytsxyoj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qdndpkxa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jdmlaczn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ozppyfnb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hyescssi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lgyjfgnm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rubymnmq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3daogzukg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3orvoasst.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3neavmvth.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ffspypkw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wobpzywu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cmtqeqgx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bmcidktj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wqqbgvni.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3krthwiyr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hawftqsu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ekvaprjw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dysgmnwx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nhrunamt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmnzidd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iiamgoqp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wcfkajns.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bgmnejwk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3twyhlmmu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oiftwgry.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3legdgpxn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cewgannf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3knowxuqi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fpxaehfm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cajlbrpe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3heyatfet.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrfnkjh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hoqkihud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3myapawon.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jzmuhkza.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vydjzhzk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3iurycsch.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oluykfzv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vaopfjcu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kalsshef.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3irtyqkde.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tanpctbi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fnlaptgp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dhszopkw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3roboqscs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hqecbsqg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tnysrppy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vbwhbker.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ygkuhtty.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mjjisgla.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iagcqhnr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hwednktp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pdqbmxlp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3abbbxgkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piocrnsn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hpulrqbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhoqwwwm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tqklhrxb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tybkyfzp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cyydeoyh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3klmndwyj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3punextor.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3khyufacg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hgbyrikm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wjnjxkam.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rcdghyza.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xtfedsds.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xgbiwiio.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bmmcksic.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3aivudmrn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jcevfswy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oudeapyl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rkatwsnh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yhuxxflx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fowyfxul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dgituule.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfxpcmpv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wfdovdbn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3anpsgsyx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gqhygsir.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jooxssay.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uxyvezro.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xgnxokdw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oavehiqp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lskyktvj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bttygulz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rjxkfwyf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zeadhtta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kxgfevzi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3glsvownm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3euhunazu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yzevydqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cydfvdou.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rwolhmio.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3sldwbspd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3wnsactqt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ykkcpbtq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mjeqouym.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3flfkwvgt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uwxcqnnr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fkbvcstm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lvilvydd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xvajlzhv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bcpqtwwp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zivtkzec.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3sadzmcsa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uhunmojb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ixcvezip.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bfvhwulc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3njnxzllj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eklqzidu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uwhmirim.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pixjxtbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jipkialp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nhafxbwk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dqdbwbrb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3olfxzfxl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hmcqjogx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3gdzlpquw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3yjrxmcnm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3bjmbwftz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3izeghrvt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gbpfskzo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ajbidwio.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wxazmgcj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3orsodacq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3blymkyyw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3lshucgky.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ujfzdkkj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ccngaeoq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3azkmbeqi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3warjsdfz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hxerypvv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cfdttjaz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eafcvmfo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3oitgqwou.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cwdpnets.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skxwutuu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvdkysuk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzcgkcpr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhmgdgfg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjihzcmd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fxfbfrit.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rnmflgig.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3enfytgzv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yelkrgio.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwbrfajv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkcicyyz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omxbviri.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3izszqppa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dldlfwgq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jdobacvp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3caanbpra.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3giewhxrs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3znmafmiq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3dmflodof.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uothfvbv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ykjfghnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjplbqeg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpdpcqst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sthlcagc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3lapmbncs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkrmkxn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tlaoqscl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nsavwoij.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bziuqbiy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nyvqfhhm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3djxxbxga.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3adefnbgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aqefsbnr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vbhgelvv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3lxwgprzy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3omghuazy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bfacikku.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xudomrdh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xfntvmjl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3yxanjuay.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nbdpzncx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3woznwcas.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xxtuoqtf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fidttmbd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qcwvdvjx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hrhaurup.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3axmsopye.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vhbwlrfk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jstouddk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3oxcmuwli.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ikdjplqf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3crkadiso.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3sadbyswd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3akusbhzy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rpijtnsu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3orohgmqp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ornstldw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3awpthrdq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ydzdcsld.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hamvmruv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hionyccr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rzbdmqap.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3alnmbfyp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzcylqyr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3azyafgfn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uolhgqnv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3znomexxk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pbichvdm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3soynitgo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gbtraqeu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvsojau.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nchinwhl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mkacdhwp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jcabqzka.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cggzivec.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gdlthfiu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3vwqqjnnn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dawfzymq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3onqzqzsm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kzkazstm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbymjyz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mtdpyszy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zwhjytyx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3flmhtkvz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpipira.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oadzatgm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3jabkesnt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3yvorpkyh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yfgqkxdf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3avcvablo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bolxibdw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfsmdjm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dtgdywwp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cihjeksc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3yqjaqemq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eyktfzon.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3myscaakj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzgnlrr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddkyftwp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jspplqzo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hgqcnmwz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psbpnrkb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3iaeqodbh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3aexpiumz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksahrilo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ujydpasq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3obfouekc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3frglnmbq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nvvdiqvn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3drsjtptk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jwhefcxf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qcyxsina.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqqdawu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tssxcexx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ippuisaj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zkzsdspv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tobxebbe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kyagtybs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3plehoeug.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zviiiupj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cplnwenr.html


<!-- 参考信息 -->