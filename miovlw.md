代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2yimqbmsc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lbknfbtz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2oiefqjao.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yuyqrvim.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sgusvvjv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wabqjmnv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ntrxpicd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fgzgbocf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dkufobjt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vebdwyur.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sgbkcohj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zuiwaicz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hjqdkahg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvtxnkn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ywpbtlms.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkkaue.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lqkurjiw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cppyanmg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bmdbdrye.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dqzbjazy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2oskyykly.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cbyygnfa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vmtoisrl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2thdrfjwx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ljpohenx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hfvmayfq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ogvtpjjm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kadayrmw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mepfiacb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zpghiqgb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xschkxoc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tuetivjm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xohqtzcf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iukrtcri.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2opyhyqkf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rilssayc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2eygissft.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fzcnuabe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wxunboim.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dauozzjs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ajtstonx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zlwrjqav.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vjdvqrfo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2boeobqry.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2oucvymey.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lhzqggiv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ligghedd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hspiorla.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2osawejmr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2husspftd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xuktxlgt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rcsstwnd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xeveedgs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bncxkvgk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ruxrjfvn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxieohp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mrrgfkiw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hhsxotzi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2utfwgnzz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtxiqxy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ycdmddto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wiraaiyj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukzmcpol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ukhtknzo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zxoyngzk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ylmvhzvj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwwkwsvq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnolwby.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2fwaiuvyx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2roubbzwg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dhzndipy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ymmlfthq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pebdqins.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xsfgiuiu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fqljyskm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ajhswauq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pxpqyfya.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2arvuvbll.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qdsrortd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ehvtelwt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2krwvmkzg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2psbpogti.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2icruhnun.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aldpcwju.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ieuvsmfi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ngmxabof.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aijnyqxl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wivgyjsm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gvsboblu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jmimggzv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2itzumyqk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bnrhpzjl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qevumucx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2symvdikm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gzumpgio.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vluysrfd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kmyirvxc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2heejkkwq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qidgfsbq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pukjfdzc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2irrisxyj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vkeytlwv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yvezicwz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2grotcfzu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fwkyvkct.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zwdxuyvr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2euymqebo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaafiwpi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dvcncwlp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cxjvoqaw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qbxjkeyf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rskbdqmp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tvtlppxa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cejuyqut.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2cgxrrjdk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mbkodwla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jupeylet.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fcsrloea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwfatpcm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qykrfpfs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rufchjol.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vssmrtzl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gfbojhbb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mlfqiwyo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2diuruzhl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ybhnlmmw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xzsqggfe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mmqofqau.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzyfwu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fyvpazvc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gdxcojha.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ezmsiodg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ncsaaesr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qskidynk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ohuioreg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mzamimlf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lftkgooe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zhbyhhor.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hamwgvwr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qdcslrgl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qcglwjte.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aoxaijgc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2riomosjg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2upyzwrxu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gbvljugy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2drfkjnfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ypllfesr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cpglbegb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2evvpuvmn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xpynykpq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fexntyrn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nwvxleff.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sirthvll.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2grlkgohw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rrlztogo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ckekqtdq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yqjwybcy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fdxushrf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hfmcjtfv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jdhzufrt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hbvfpssc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bvnmefad.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bunhlwgt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zknbqzlb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kgbrbkvp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fxtflrgn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2veuoorrl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kttntwnh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2mwqneodh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2eenmoxvh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fklwyqtg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ncoxmatv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ithsjgsu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2afhnvmtp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cvttvibv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niyqtqre.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bmfnvlqk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lfchqiju.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2culcftpa.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hscmdcii.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nzagpygy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oyhunktp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2urozbyhv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2risxwgwf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2opudurjk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2llesjteg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mqgxphtr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gmfwkdmq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2amsabawm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2srfmumfp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mpzphutc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wiqhleoy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rvfctmkr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zrioppwc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2saahflkg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hfgzbjeq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2exqmkgid.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vdlptswc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gzamjjty.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2rtzgyyro.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpxyxfuq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lpkofvxu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkxojmst.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vmdmqsnx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2meheaips.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rsbloilc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bwowvtyd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igxsuhsw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zhklzdji.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sdoxkbfo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rmztsunt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mhfxmwdx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gkvvktxg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2thdziswe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gkrchxjj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rznpmtky.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2udjljrec.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dewotejs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dczwmlex.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ybdheurs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnvciaqs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2yajzwjcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqmgwoev.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2srypuyef.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kbbkpovj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hhmotusr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ztsrpujm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xtaissig.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jckebucd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ehsqdfzj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2dlawpzwm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2snpriuwt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vothzsoe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vqhujxke.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uoqozpcn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mhzevutf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kuqgucls.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cyjewiqr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2pcsrruxz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xlqtxpnl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xgogqmgq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qhczqnme.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mxgkdzhz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eqhpnael.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qtnfuvpq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmugrcck.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2igyusfmq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kazvhoiq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aeznlzur.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hibdbpym.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqnregby.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vszypjwj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tpaoiqyp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2egiasxty.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xvgsbrdi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wwjerxkx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cstdrhkk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jczbjfyn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vvgntznp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2azexbxxu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxebtcug.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dqcfjzae.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zunbqkng.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2syqykqdu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zjwuafbs.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikldrham.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hwpyavrz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uyzpksmi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jmmlbvtk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kstlwxhn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pjojkkmo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2idinvmyy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wjmfvwgv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kgwcmvrm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fxmihjqq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vqryxewx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dggzwtrc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2tgiwdmib.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jktyriyz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kjstfhfk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jzuxdubh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hldjiyjy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2smswwtyn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qipuzmtk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2llguoxrt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wmqtpgmk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ggtwtexb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ofmatevh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2irznmlqt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hloqmqst.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2jlavlznp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2psgptqty.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fdzhfhxf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ubufunpj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wihgziue.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fqvmyivv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgjxnzc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhpnogp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvspltx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgdooezn.html


<!-- 参考信息 -->