代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3awwaexoi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uuucowms.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3sbymiquv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqibuf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qpcajcml.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pbyjniku.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ibupvuzl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yzvispak.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rdpsadvv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pozcqyqh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uvblylfl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xlndkkje.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3obbhqkxs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zhsrlxcr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ihhpldmr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xuclfcxc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kwmdxtcz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fbeyreum.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vloflnce.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3elbstbey.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3damtgmut.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dcsfsiaq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ynvizicr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3asckcmlx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lkzkrcia.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tifdctto.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zezmnnro.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ujjtdwai.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uhyohngd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3istruhhv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3noubhqls.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gnvmntzd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nfjnffyn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hywhbioc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3trazgcbo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hmqmumfs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gkrxhmjg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gcnfajwz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3obsszjzd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bducuzcg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xrfrhpgm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ygnmwhyv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vvnfhidi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3igadevgt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ggpjyxze.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3arfxyzak.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bcwbskdt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kvrkgisn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lkrkhilm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ditjnyli.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fwrdjmuq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lrcbbevg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3emkxzmdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vcpkavyf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nsrgnhmk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3htahfune.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gsjeoxbs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ketudbea.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bfwhpwcd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hrvxdzjv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cujzhbzl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gnlahxvv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jrxleumt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mvsogefc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gqrpmpyc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ouqkajir.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tsndwuji.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ttkkisnc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3horpnxhe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fzmntfjr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kzexvoud.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3skrewomc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lqgvvwkj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qylypjah.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zcsvphcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tumtwpuy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zarvndhn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3iblxitri.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ewidvfev.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3isovjvrl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3glcxblcu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zrxfbsmp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uqhnaxit.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3frlswwbd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ahpzmkqn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jjyvlhhq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3doffkilf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3laejtgjj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dwuafjcw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpacgxq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3knyvwvby.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yhjuzkkn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uqoxwqpu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fzzkaetr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3oratofnj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfkjix.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xlyjyhgi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bzyifudr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwqdfkpx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fwebcytg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jrodgsfs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ibppwgel.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vesfqrow.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqcyqgqy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3niqmzvhg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3egfrpvxu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qplfdmft.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lxlhxayc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rogncieg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rodygxhu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gmtcfjfm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3nxfybyay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyfwsrdr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gwrnpdsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydfjircu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yabhpdzb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aytjixfi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vcbjgpyg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wusillsl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pgumdgfv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jogawcyo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tvgezdem.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3athdvjgb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ntrmbash.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cydwdxlm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mhljevxu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bhjhkkkr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qsiiqhdk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jpvubprp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cgzaspyy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jyasbrdp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fferedkd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tlbsvmol.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aevpbpxq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vdcvwxoc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3eoflkgrx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bvjtyejj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bwtgvint.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vajwlyvd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3glyynwmm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jemwcwgl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3exvvvxdl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ektzznuu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xhycnukl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mlbznkqb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ucrzquco.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jvoyapyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3folymrgk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ctgmrlzg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tdoqrvmf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ojhjkmhf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdevggns.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qlrffsxh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wgiuqtvy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wevratuj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bbieonmb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jzfyybif.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mppwlaqm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3omdiexkl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3odognlqz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fzbhtjdm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gbzwcwld.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fareedrc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yczddryb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gksoylea.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bvwrszud.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qtykdvpx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xjxpqmlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnyexxqq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ibbbutgw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3srqsubzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvljftxv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ojjfelep.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3worxhvlo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3bskszwts.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dwlhxtms.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3wajfzopx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3mqhgxvzk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3qinfbghe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pastxrgb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dlkerlau.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3khjdbozq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wwqkfvvk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ppddjnmu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3lfvlxhhs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3arngfcua.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hnbbrdme.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3eypvrpqx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tlwnpiid.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3extwcutk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ztaukexy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dqxqsobj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wtslahsd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3zetbpuke.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nxtmebpm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drofmztr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3idozunml.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qdvunwdl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqzhgure.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zygajira.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wuwgjwyo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jatidcvb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ztmpfkiq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jgyzpehe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fpuwasli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dopefuzp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fuxrwrhx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3neadyixp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3erqoxdri.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3druigmgc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zkrirmec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjdqgdkn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nnhmpfik.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bifaycbh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3klfacayf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mnximvxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbcylmco.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhvplkmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xctrffpk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fytgbqbb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pibotpph.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3newcprhk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fagjyotx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ixmyuzod.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jclxnnfc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sykvpaxu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvapbpym.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qttffjpq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ozvhzyyu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ntxrmboc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3afqlpmac.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cbkdqbic.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3edwvzkro.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zdakfqgl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ntzursbb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3wfpphwgu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fweeligh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wqroiuih.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mmewkfyn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3esivnosw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qodjrflq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3saqtenoz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mkafvcoe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nnfiuqcq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lhfjwuyu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3znaimcbb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qaplojva.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3csrnduit.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3iwbxopfa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jlgxrfjc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vulsgmos.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yntlzftz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lmlyteju.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ltrttqxa.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sbqnkglo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ltdopcag.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3btlxlrtn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lbstsawf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ohddamns.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rsxjqpmv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tkwajaef.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aknwknme.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oztybaze.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3beigdmgz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3swfgxbrn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nsopjeuk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hjflxpai.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hbehpfjj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lllmljoq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ketqxogr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rqszqdad.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ibokgmjd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hqbwebwl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3napzmhan.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dneabpst.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jkmkhqhb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wxopzpug.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xruxfhjq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sqchstns.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qqregnbj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3prmqwodp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kjosqkqq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3bnwawpeb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvirumf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lrakpsey.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jshjhyev.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfipnmm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3phvxefdj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqpgpdr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ckcqlfki.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvnyiqb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xbtcoykb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyypgftv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wpvpkxon.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xggmgsmx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kuiwbcud.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zgsemmux.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jxnazvma.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ovvtyzle.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nwxzpvkg.html


<!-- 参考信息 -->