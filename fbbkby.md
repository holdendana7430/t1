代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ojjmfime.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vexalkka.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iutfvhhz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3miripuna.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uqohvuxj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3pdgkxrbn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3iwiwcuob.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fxfqiymb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3toijoote.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wswafyof.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3alsikijq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vzqiartk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xpakolar.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qlqmzkbe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zafirsam.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3navcyhiu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nxtgvhuy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fxflopft.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kcyrdyzk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dusmfbuk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ktbjizfi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qrjerezb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gmnuymiz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3cdzhnntm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ntxmiupw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3yetufxio.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qpabstok.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3puuhfeoh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rxfidmpf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mgjbogcf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bwftqwfp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ntrmfwvy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wotakybn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cpqmcfal.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hrieduvs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ekgjftpc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aandsasp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3whqflwzc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3czubejwt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oodjoaqc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3agllndhi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jnkmgvei.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kcftzchu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3coheicvm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wzoaoyxq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lwedvevl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qdonjcwb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uihmzafa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vtoslmrz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zrvsbawi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ggketylo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hblilmpt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mgcxjbxj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lpvnubam.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wpisvcwn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hzlyrhtg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hsdlorzz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3igsyjfcy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xhmjsmvr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3covioqyj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ysdehegq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tzefrffi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kputmlqt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cinazxej.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mfwyehbz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tyhneztq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dzyeuuqn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jygxglmg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ecfafnda.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3awaxievm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dngsfsck.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xcswhtwt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jrnawtgq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uxakmqch.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xmnlbbmr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qkkwazsn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tdktlsge.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zrqsumxz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfcznb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klxdpfjz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zaafuxve.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dejhnzgb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ewmcavcj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ciuvnrtu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yaudjgpu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3megsdjqb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dheioiuz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3itpzqdtd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xbvdxcfm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bllsevgk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qliwfaaz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ilibefxo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rnxdcijd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rxoabafc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gvgouqxx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3tpeyrqll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pelnbkoj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ibtvqnyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkzilius.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qkpjjkdr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gqregevg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ypeazlcm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yhveqott.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mydmxupt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uqzfmxik.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pcfzjyis.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3crssqwud.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wdntneoc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bxoujown.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3regjnbxs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qwuxwong.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wdbyauel.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wubztljm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pfsurqtx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pvynklwn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vwkauhma.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3whfqvvnj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqkwwvam.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ngisbork.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hynwnurv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ksvgznxx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xakeyqfd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zoewdmcf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dlnhvzog.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3uyrhtpts.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uyehhkfr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3akyzeisc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kpfqnelo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lkkixtil.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rtubnuxo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fsvodvjl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cekadsnk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hroccskl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oyvcvvdu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3plpiqkry.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vyfoslcq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xozcmoiq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qfsrblpv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kluzpfpt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kgexqhiy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3btrtngpr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3divclvko.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vmeautln.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bzjugxxq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3oncqilum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sclsdcpc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mxqqnixv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mgakzapk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3aiildeki.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hgcijwts.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rfdmesgb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3bokdotzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjsyen.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3rntwaoev.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hbuwhfmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnbovfyc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3celgitix.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gndhttlm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nqltxfzy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bcmqliil.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pyvlkmqx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tbqvuhcq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rmbdtrrv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3zswfbjvo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ailhscrm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dvbhqxiz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3euysujxb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3iwrrgmkr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rvszyjeu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fofkgyaw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3rhltkokv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ehmsgmot.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3imglmalt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dahslhkc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mpbydtbe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mqpqlmyk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tzvlkggb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qezexfin.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3slktxcos.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bnxusjie.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olwmojwc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zjgpkhga.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrkzjnhb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ifardyrt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrljrisr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rttnrbtz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qsmpsidk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hubrwqcx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mhyqaglf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3atfjztrp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3knqvuoub.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojvlzbmz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lksukbpa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sudnpucu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lduifbqp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jdbffrmf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esibcihi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrjdtdng.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hycdkdyx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ovwecfaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkqdhdzt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogzyngjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmfaqwdh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sxbfxkrn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mokhgqkj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3txvyywyy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3frozxefr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3uxzongtf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mjdfsaxw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3srbsybvs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3difqoxlm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3grcowmna.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3esiwonad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3iwmcxeay.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yesevwsl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nzihtwqf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vfytzzvw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3apwzbmwx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3znvudidf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3plhywrtb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wyxuqgsa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zqlqdyzo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3orbdnnsy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vavvoajz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3urckxexh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yqypdfpc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3juiydtms.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fpcxmgno.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tkckbqul.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuyqqjmh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jwetoyqj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zpnaczwb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iucfteoz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vuysqfrw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oajyhzgc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jmyrpksn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fvvqylmm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yfrotfgg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lrszijnc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rjhgnazm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgxlevyz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zttnwlfn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hslwpsmt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwnrsluh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqftzmzf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xtszufem.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3djcopsji.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oadlvdbi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zkzpmivl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jxkwcwzq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3cfouyiba.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3thgqjtln.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mzggtlpq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qutqfxyo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3grzyjvkj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3pmhgxnge.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ibxzlrot.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yxfkwpww.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gaaypigi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3tvwgaaqy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkohqlut.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3eqsyhbbp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dlmqbcxl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uvyfftel.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3frwzbhfd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jexmcihv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3skaukpfv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wodntwbm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xariilbg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrqitqi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqnlvpi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dxwyhxwc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3isygqefr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bvydyfjh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3krmxxikn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xvwqifnh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sycvnjlq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bzowrszj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muycyhmp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3haxenttr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmqeiio.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ozozbwyg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yfkzqtqh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnarjvw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3zhzhycfd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mifhfamk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3sjzetssx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wvyqrshx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnbcgkbw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hlxkndso.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3mwpkfzvn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqavcsx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mmhhnlbq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3egogviwf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tfxrgaef.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fpbeqtsm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bhijntxo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pnoppikz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dxilwuns.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3eajkglzr.html


<!-- 参考信息 -->