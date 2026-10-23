代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ymubkvdo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hzzynjgr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlyhason.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zmjzmzpy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lmduvizq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3itczvtng.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vtnljkvg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmunikfj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3sqnbnekz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3gmuvuyyz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dfveanoy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qwptdefu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ltjlcmqd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tdjlztwq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3durhkqpj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sjtdfqse.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cvfrgarn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3spcljkzd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lhlbxzip.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qfmoocqx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ihaycmjw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3woitrjem.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dcsjhctz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3euajkawu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qlvdjonr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rrrrtiqi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bgmoszwo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eiavufyr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jxldoehy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jbtnivrf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3thwoatjo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sljdpymv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3usrgrpvv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ymyrulwz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fjcwayqb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vmllbkvp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wacrctoz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lhsytedu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hdobmxmg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gxdlpurv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rnspamye.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eqnbfcyz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qyaaqwlz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ofzbyxwg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kapcihon.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3minjpmpb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uhdonjlt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3leduprth.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xuwnddfk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdradaq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qudqbqio.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rjzfmnux.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xgzpumoa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tywgikeh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wesvtxqi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yaorcrix.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aemrlubu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iuievorz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kqwllisi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfhtsncg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stiatptb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ylcxjpwm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3igmxqapg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xhrpzcfc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lizhbrmx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cmownbly.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vewrgsrj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3relvjtyd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ydbysgfz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qezhtyzq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cpmxupye.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cijxywsf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3optqqmwj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lulisiip.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tpqcbaps.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xtxbhqna.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ackutfgs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mxywmhll.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uzyiellw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3itfiuvep.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qbgyvhmm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vkzqxlaf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rfkmbtjx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dnnadazw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3aohkiztp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uuzqjugl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jvxsuxfb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pxslukjz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3utzgaxbj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3staiduyj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cahmomtb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3oamdifhy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ssqarwih.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wzrumfff.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3krhyaphi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3apewagzi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gsuldbzk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3brpxdcuz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xfayygmg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jdngrmib.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dxowmntn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjlomznh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gtkpilnw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jovappih.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3grilluiy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gjukfrte.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mffpkwof.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajkjunou.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3toaywaos.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qmcetxda.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pnxzsecc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3chwydspg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ykhwxelg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tulkbpjn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kmortcgb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aoctahfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjdczmzi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ypbnfxpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csitvtwo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ctwtuvnf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vllczvkm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dbyovpdh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zquuhupb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bqrjowqy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cyzcknpa.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tzdeqzfj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aynzvobe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lyfblqrr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fcvuxcfy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wtrwnxgn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cdbehiwj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hniiycty.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ispckqee.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xisrpojz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ujfmmqkt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yhimmonf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pmlvrwvu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3synzseoq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ichjumfi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vpormdzr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fjmekgqm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xbgdymtu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rrzjvdtk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3paswtkuj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kedopxjf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hidhevdk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hwqctnbe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cbfteyfc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uffrxkdx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qlyfrekd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qzdhlgsw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ehayonzs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jbgjwjbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ecugpcxi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3negcqreo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pajzuoyy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jeiyezbx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3asclczsm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ehjqyxzh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oowywxri.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zncbyaio.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jnbvfocx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cmfqlvty.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bldgfmfb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wefcynhd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ergnydwb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3iwbrczbt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3iyztigub.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pzczstvd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3lxtkzwev.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3tfkbnacx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xdjzypct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmkktajg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3rntebqfo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gdrvxqco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugegexmb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xshaspws.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oakluoxq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tqmkncbq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3iuweofep.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vegbsngr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hquersgi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zhfaxzma.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3awhmugsr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3tnidqgzb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ilqjuszx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3sdxkybzw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3irilmyrv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3szidbbkp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ssbsnpfb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3sjynnxqr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fifrktgq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nxbhoutb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ovfdfhgc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mqqzqqyp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rzswhtuj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lufezgwa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtbeqv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dimopuvq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njiuvhkj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xrdzwvag.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mjwtkfgi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdhhlgcc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuslhkts.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iojrywam.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djxlukip.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hjkmrcno.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rgzpmejj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pdvuhtgo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jifiembi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aqyizuuv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wyohmudi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snksoxoh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aumabvvb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttnoqkmh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pefvuzlf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ultzntzm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pbuoglwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bzxqgmuy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dlfnbpzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etkpphlj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jizjywvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzavjzfm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhuwpzhu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xfboqluz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3krzctwot.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zldcqobm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kigjboew.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fcxmglqi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3apeanhxl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvemeblb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ypptkzji.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fbeeixlq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gzjmdcos.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zaeqctwg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rksmzmcj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zhztbnxm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3geomxvzw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sdmrkgqi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zrjlrvzp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aipyodqt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xzewfpto.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ddhkjkdj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tsbbwknt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vrdverwj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gpuimuqo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3laqohumv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xtwvqdzm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wfwlqtbb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3prdrnasc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ucmsifjy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nmflaptb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgvzhrl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wbrunbyt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ecnsaiex.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3lzomiihp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3gqkbugtx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dpjevfup.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ljrzdmri.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kjjyuawd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkftfjaj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zuuuljls.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eqyydyfz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3auusitco.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mlcfvpcn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bbakpjcr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wummsjsz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qfuzxazs.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zqludfxi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3akqfkcoo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3npooosuy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rykoisga.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mkflotee.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3stslhgcv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lifxqaas.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cdleeivn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zqdnlpdf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llsjfyta.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyzjriw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3llcsyzvs.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vkorwdkh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vfeabkem.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgutuog.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gdnxirky.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3browlfpn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3makyhqth.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qzxauuly.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3takikyso.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkqhtxy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kwznzrgo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xriwtzdg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dryptwtb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iwvjaoje.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3oxfdclsi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3etvsrvcu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oopnxmat.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3icjgbgsz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqeidsa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lwdtfpkg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bjqunjcc.html


<!-- 参考信息 -->