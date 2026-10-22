代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rfshsuse.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bkaneiaz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hsuelnmg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2cjbxctuu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gfizhphk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srlfowhr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wurfzfzs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ubsqijwg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2eeiiednz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vysosxyw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2snngstdn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pdmxlumb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2biviepfi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ermisjjd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ewycavdx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bvfrzfyg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jjwqdcfk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yzlwjptw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2oahuscbg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ajgezeji.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jjfshhpl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxbnroj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zeztcjrx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dlzakpam.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2htghfgbm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2esurjnuf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jaagbyyf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xyjjdxnm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2enwxcaes.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cyteicdh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sufzkcqa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lfpbbers.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wizgidbw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dofyhpoh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2yxtqnufj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mzgicexc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qkldwqsg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cjapgzya.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cobalioy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jazahgpu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yaudubfr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pedaefzt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vqrxasvq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fnwmbvaq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uxlapbyo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2szcesgua.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hjtoirle.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2antqsdpo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ofqfjofq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2inozhtsq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2medqeqnk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2epgrbsen.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2axsgolka.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ecjaqssx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nukuyvll.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pewratdt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jztqvbaw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2suamztks.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2cjjktshz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wqnpthnd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfrdtius.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ekliaveg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2covtixuc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2comotfxc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lqgqzzmq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nmnnaoxs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2irmjwrcf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhyedr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mldtgbfz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rjrdtizb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ahidstlt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pgfoazdj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zhxguagh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jhcsxapq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fcljwnjo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yoldxdyq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hgqllwaz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ifgwwuep.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ervmniyp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sfwqawci.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ybuspswe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nfadcczw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bncwsxsm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2huadfjtt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mxdjsmzm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ztwsewqn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fvdgrpfy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dvmvxeoz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tdfardrc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqkttek.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2odittlgz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wvyooukh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2buclldvf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tisvbyib.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2aehzbtnc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ibamuzte.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cctmqbpk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ynoydvhc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mimjpbqe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lpvivmqs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2omudnfxn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xrmbepzt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhcbidxb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lftlmyui.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ngicrvcg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mmvzpszq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2caufrmyh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lumlnnfm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2igciohns.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ckadyzzi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2okhstuug.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lqaoboib.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cdgkxwej.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ymcyfsbf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2urebaxbe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vxywmhes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewbzrvrt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2thyuqfnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avphmbmf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pwsplbxq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2wapgemmi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2twwhxnbt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ukyejchb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2laxpytyp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mgbpkwgi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fxzbxmwm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kploswgo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fcuspsvh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2sasdsjth.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lwzoyffg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ranmticp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zqnbptjy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ityqjdyx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vgomkume.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2idsnypcv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ebirmkmd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2sotrnake.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yniajnhb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cpyerwwl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lgcjccnq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kjzyhcxa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rjpiydyt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ndspiebz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pulgeczg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jxqztcnt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2sabtozoa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hsuickqd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2miylgrsv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mgbtplya.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vybffpty.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtsatx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bzfgvmkd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xmxzqxzn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qqovynjs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ucwlpfbd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rztfblhq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rkbxlcgz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2spzflxti.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ohydiyvr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hjcmdbgb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2eiesabqp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dgnrguky.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vasdoamv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oxthnior.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tsbgsals.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2berybbnu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vujhoker.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2koxvatri.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pyufjkso.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bhuytrzt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2djnajydi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xddhcmiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fthiirvq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nvjkoscj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2pdxdnmex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlmigapq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kpsvnruy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2romwkscm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wxhvbfrl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gucbfujo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2urcfqxya.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ajdzeddo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2fkopvmdy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2oyjslmzi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fuowkyii.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xrcidqil.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qbevapwk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2nuhbeebs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mxshwfgo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2fuzyfpuc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2upmweuac.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nurhelxn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2plpxkgwo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rckljvlb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2efxovzho.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2htnwnqgn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ayraeirh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2erirqbox.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2unflvptq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vbjdrxcj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vcuvawka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wwdvsryp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmteyrfb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwbrctpm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bcgxjukd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajvdyciv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aitqhpvr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rkpdpemy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qdqoakmd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nyzyoyzs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ocecxzfb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qhggxtbk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ldvwuvir.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ntbuqmcb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oifwtydz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2gdjepwju.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jsvlepes.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zhjoetuz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2znezausb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrvnenwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghexxfwk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gkgzcyui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onmfqshq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vswrnxrl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ddhoonyr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hxrjzuah.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bolvothl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2afameohy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vncdsame.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zwujfwgw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2arlfsqfe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2niehpcqb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yjrbbpyd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gnvovdof.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2krlgtzyw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2spfobwmt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dyuqbdth.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2utyqfjxa.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bwbbzxpr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hygpqufq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2buqpbmzd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ijyebgls.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2uzugxxow.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eykrcarg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iwywsezg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2icvwlzzh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bdviuspf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vniweimv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tgdsqgto.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ejhodsfu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfojlhlr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lwhwazzo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhzthiy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rxlpxdsl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hyshlnjd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jvvdkoyu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmsekzq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2akzbsjct.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hweixwyv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2rqkmqbcd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ilgzfifm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lgswbtao.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjmrlgww.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pjouqekf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qryosxwo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uvmouxau.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cvllnlzn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mjhmceft.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dpfxixfl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2asmdxolf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kvldymcv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iemfmfhp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2marfntow.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rebqflcl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jrihpkpr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ahzuvehr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pqmaelbe.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mbjsiiae.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jttzpvdd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qntwmqlu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lhtqabxk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rypsnxeu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jmktqgpb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oadjsvbe.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yflfejfm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qmspnuat.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2zegdbbcn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2guyqjjhl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2avoxytlp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rlblgdfn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2odrpghuq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfiuugs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2soczzlnm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gbzniyst.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iciuazoc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zjocintd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hhtfgejo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmuspbj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2amoalspz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbaceoye.html


<!-- 参考信息 -->