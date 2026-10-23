代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tszsykli.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3fazkcrfj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mnvjiowr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emavuzxo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uufyponx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xpuklnst.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ekqijwgs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fpvyorlt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3czjzxnho.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjgeylnn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yltdrqba.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zanccrxm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vrcbdrdp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3bahhmuui.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohfsiiuz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3afcrjows.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3urpcypbt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxeosewk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3oalbhqaz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsbtlzls.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3skswtwvb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vnordcss.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pjtbwgcg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vbdpituc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3azyxjurm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dxbbounw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3beqcmcba.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3pdejgsvn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zygcqmlf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hgejttmy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yahyucjc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vmqrwlkt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ntvohmck.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qoysfdur.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjkczcgl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3undbxnda.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3szntpzay.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3udgppnac.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3atjrrtjk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mwcrlskz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bdutyojz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ndyubnpi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nmtfpcpo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hkmxkmfv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rtvicjha.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ligzfjqx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ktaivuvr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cmvjdulu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zwwjxrga.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3aehijlkp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pmmpgmtv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3swjnbzen.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bwedcmif.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hhdewhsp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dissejol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3oucdjheq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ilmrtlii.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hsheuquo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xadvjxtc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dxvisjkt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3axjpqemy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fwkxrslv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zpeomdwp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnzrvwg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3llfabqsc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mfdisonp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3trbhgoqw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3obnpvdpu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3undrdpkv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bfhhqxyg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bpdwwmqw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogoejrsg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ctfivkti.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3veralvtz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqcnegtf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gyoidphx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3oznikrjq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mahkswie.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwgovzos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3goslpuzu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hadvenqr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dzlpiyqj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3adjfnpsr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lnsipuys.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3invcbqop.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iomhrtoo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3omwimfna.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3airgdbpy.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mtqxxnem.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vpzcjxis.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hzfuaryv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pcyzduwi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lvrdvtbk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nmvnazhc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kksvbzwh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rubboncf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3irycbufb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hhglomud.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3txupwdwu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3agqenufc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iontudmw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yrverbyn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3prvosxag.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cdqbvtqb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3oettvoqu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqykhhy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tvvpgapc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ctwmmzqn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kviprjda.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3elcjmbbj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rqeyxmpu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bssgnvht.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xscvnpkt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lidiitpi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tfgdhyuf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkzbanp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3whfnohbo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mssnnbho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vmvbijmy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhtleapw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tjjvoxfd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hbvldwut.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qmugxyvs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zbwwtlkh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zfolkpzs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ahpdyaqd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zucweuny.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xtmcsfsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkmbkoz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3avheetfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peqzfrgy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bifgpnrw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3murhnobe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3izylgyma.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3djazrqxl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hsubqpig.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aqqqujbn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cmfgzggt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cjpodqrg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hismsajj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gkpnehig.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ofkgestg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3paypobpb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mrrcuhle.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pasaqgnn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pnjneqkt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mfdllwie.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oihpsrha.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jpebextr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gzwhirex.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3azdpncuf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3udsphvyc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wphhbpbw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mikpjdci.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xksvbzoj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qvewzjaa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qhxakohb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fnfsfsvb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mtkczsij.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gzjnhgjl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ilhdswif.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zsatxnyk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mqjzzzry.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mfnkvuxq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eiljjmqg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gjwczbov.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fidedcbh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wvekpfmk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3amlcsydw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3crirmayf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3opvqdsmz.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vtdxqayn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lmsawxde.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bftleiux.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tlotjulu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pdcvohry.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kgwtgxds.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bavvyqpf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rjgkxjkk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rrauefrh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ybsaqwgg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hvcrezaa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3haazlaae.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3lscpypyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbfrsdfu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3fajocdzg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3kbnsuoai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kucssujs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3edqmtrcc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gvhxhbhy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3iowprzlq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3uxykorev.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3grmlfrzx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nufblpkz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ovvfcrvn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yoexhhmo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3awrbtgqg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kmxjvmkl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3egonnnud.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ncgwqgqp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3skqbacac.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3udpgjtyo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3gmejukfy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gianythl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3valpctlg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vcjnslyr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wnhxirhy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xlqsxopm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ggcespoz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zndfqkzd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hrnyerjo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oyzqrcbm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3molluxrq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qmpzucfs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rzdccafd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjcuqyxh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbjofnmm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rayrndix.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bwoaruho.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zkfufexk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qldphzzr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcnndgrp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgsuyq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wurgilhx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zeiwrwbd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nojnpjcb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hjhzdhbf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lrztdlio.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zgcxxcvf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhhvnloc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3svaiyvek.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwtzvxeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhyubwkf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qoeibbho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfhvzwhw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ucbdsbkd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zwyvmzrp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ggibzddh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3urltiher.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3cflszowe.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hgowzxxx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mpwdmzcs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ktvnyncf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fichrpwd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mofizjta.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gbhwamma.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3katipluv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zqvybquf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bytglqwd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3osqthpfo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3xbhtgotg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3eeryhowk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nuwtjmym.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yjjvuoer.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3yimywdqq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjccttqm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svmgdanr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yvbtidak.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gjszxjmx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nnfxfsld.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mupvtdbf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3quepbvii.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohuxvsom.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3badsutqb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gogmdfbu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qdiqolzp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sahepkir.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dtqbuyhi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tkuagiqw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxfeawc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uhenbkpj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vivzlsan.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hqchbqcu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jemxyzcb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3plfyxmvx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmrtmffn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfqqvcom.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gkgmfdeo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbiesosb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3upsuskeh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vyxnyiky.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pvdpvnva.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dnnzgwte.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cytwxnte.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rlnrrdri.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pzenggpb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3evvgxqrr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uvkjksdt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kmcrgccv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwfwuafj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ranfacxl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3gjrwbrpc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3tzwvtofp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pfuqwgjh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pznyzudg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nvyhzpvf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nsidecpi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lypgvkdn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uilztgyx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iivgunku.html


<!-- 参考信息 -->