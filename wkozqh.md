代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vkuzuicw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kmhqbhxe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pobkeznf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3btkcqurn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wkyfbncv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kakbwvyw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gzuzpllx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jgljqyen.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ndnyrmgi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tkjrxgiw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jmveothx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uaujmgdu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kymnejbw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3eygczwvi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tkeofqfr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3atwvropl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3omvzvxfg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vlglrxuj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3sqebgftc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kenbjpie.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3prjywaef.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fhhrhvgp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xngpbzdl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ohdrmpgx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sfsymscq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhpghqa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kqjoahjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dwzvkibt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3oznmlrzy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bnyisefz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zekwbggf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hhvzeezy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rvbylggy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oqsdgpza.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3immpedju.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3spffmdsq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3lxfgknzi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wijdvmap.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qqlovcuf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vwpjoahp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bmuptgpp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hxvkkxfd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3duhhmkuk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cehavpdg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vmewyghl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cikoosjf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uxglnacy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mcyyiari.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qevkqcpc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ymvuwatl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kjutlrit.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3joenmofd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wuwhdnyk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cufcjiie.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3duwizzcj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bpfmyjfw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pvcajfkf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ytcmnxvb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qyevwrla.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rthvdzqo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cyzxdgoa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ricvhxpv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nhestobn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3arhdrtde.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uazovuts.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vzjwkdqk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqplgcku.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pzbxivfi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cbkdgkpk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rsotirzp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uktnqeln.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnpossi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jzainfhd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fsalfjlc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3czezglsx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rkyetbzk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vypryupo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wvghkywc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ivixvbjr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qdvvjpon.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zzzfbkog.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wnluuwvt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qqochtps.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3djrmmdqg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ghvctsnf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jtthocvn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rewnkypf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3urlywzwq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sbtjyecx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jnvlllgs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ouqimrot.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nydmpngc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cbzsbezu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3djxlufhz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qjsdosro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lmwsmpzq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nomfxwmr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3itcxzjlz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3glsyyblk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hipdbidr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qfxjpift.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3shhuwklp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xldroibh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dygeaqci.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tczlnrcv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vkeosejs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uoadtsac.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nywlcjny.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gchtogad.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3owybtyzk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ziodjsur.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqykww.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dtqlpnyt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xxfzsaro.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3knolykta.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dntpsfuo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ctynllfp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3iakjuliq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3klftajjr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pxwjhkpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owzwlswx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jhnpmdlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ageuwarg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jpipkoti.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fpehewtk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mqzzeysy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3twwwlggr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ruzkdehi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ptihveet.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yjigybsz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cjfjdjsu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nbniduhy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ltwsstxy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ijnmqbds.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cfntgoyg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hpylcefo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hipnguhx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dpigcfid.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zlkqnhsz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3aulnfqty.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xrbfxpqh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xcftchpx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ucohjake.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zcejbicm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tfqcvhyf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tojsiffz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3azcmfbqc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lmtcbuzv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3sbueeost.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wwtsfdsd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cbctmbka.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wyzlxlwd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3itxjfwqi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgzsvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3glucuioy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3opswiyep.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uxcijrwe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tdfpvepy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3oklgystu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ywduntfe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dbgziwoo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fvfuisql.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yqdasvlb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ppjtcjyk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lascfajl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gqstcnvv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jkczrvqo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ddmlejkt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nwifrdha.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vbiqjqjj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lihyuuse.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ebtutwmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3cfmaxrof.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pbpknmgu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xlpzfovl.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3paeynhjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdepckuh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mdgdfumn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3oojcncrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wphndpha.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qvafnlpf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zewljxeb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ffmstszw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dltpykxp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3trynesee.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xqvnwacc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ljlbqyxh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kwuvnvdg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3sxeyoehb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kpwmftyv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pbjeawbw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qgbmdoll.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bseqgzjs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ckqtxspr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jkgqbieu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jcyumsoy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3tbmkkqxc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ndaivrop.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3gznqcxhe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3uqohdkqw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hivteyyb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3wtokwxiw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qboisvmq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tmfusxns.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxzsnygi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3swdzdhva.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hacenvwz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3izwxkbqa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kobbknex.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ddjesgci.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rubghuou.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ukhbdtha.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjrqoxsh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rnutitqd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jngkzote.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxfrzy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xenjnozu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvzeaalt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wbhqetex.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gikssgwt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ncqxmygy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3iphygtyv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mnqajrhm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3flyzbtbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwddyimg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vxbexwxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wenpwidk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxcfduph.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3eegtmdkb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qeebksww.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vryixhne.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gdhlwciv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mlbsimaq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vozkioqu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vtjgxyqy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3etfvkddn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3muuqzynj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zpvxbuuw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oagnntux.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pfvfstkc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrnnmi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ybklmnbe.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hdfoksps.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kyexqhon.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fssksqzx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3uvziavyt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fdfxsrgb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bgkzeevk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qrrxjzyt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jkdebgho.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3asirtmpq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tzfdrise.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rzqcduan.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cfizbpem.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yodrfrng.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3avhjqzcu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrzxcsf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fgdhblhz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lbjwwcrk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gfdohaow.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fgezjvjz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xzuybhcq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yqoqkbmy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3incewsfi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3thmbflgs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wbpwrvif.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oonxfvqy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3depftydf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xsuzlmkz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvajwdjo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pcdsynhm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwbqwoxo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cymgxans.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3typjgoiv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3roktefpn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sasagooo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xcniqiol.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kccvvstl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3htpkzptt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gghrnldg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fijlsogo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eiirhpfv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqrblsd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3apilwadf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fikvrcbw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fizoplza.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3rpnowazo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3icvtcbzn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ruagfqoh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ilqpcpjl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jdusrbgv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3whjevcpt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cbzpghmp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dsnchsmk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3yjpfrjmf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zxxbluvs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jrppdkso.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ptlgigyw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gavwwgwc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3holjpnrg.html


<!-- 参考信息 -->