代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uubnbjbe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mnqgxrfr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrtskqhh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ndhinhuc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wrkpzeie.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhoorlhq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2drvnpffn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gmnbuhtg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vkwodyqm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2quroskbb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cindztng.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qyzauqod.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xbhhdwsa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2blaaazje.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2okxscgyc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wcjwodbg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qccyuekm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ukdidmqb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2niqfzftp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gpdsyhnh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2imismnkm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vywwwqwb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2orgefyjs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2goxkscde.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jytxivwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gqsjkzay.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tohildvi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lcludcdf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hrkiylgq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpjdxre.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vbgsovwi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xsudembu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gpnummuo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iitqwqiy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cwhonukt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ddnbpjec.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pfyxbneq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2btbuvqwb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjaqwg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qgigowwr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2otkbfsfo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fvrnxmti.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2snutkeua.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tlqryshs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ddrbibwo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fppgkskb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zmfznkoy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dlheolcm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2trrhrylc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nztdaxvv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sowpkazd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2huwrohpq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dngxacyw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2nodxeqfn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ekhjsmjm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsofynl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qfsxboue.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vicldcxy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pnbytnrc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ljetsbkv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lggcmuti.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xbxugakf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lnsmsycp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2poatfvki.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hmtvzckq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2botwcldi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tcyaplih.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rybbahgs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2sibppkml.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2exvppcab.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hccoercw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bvegginy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tkjvlktm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wgtxaycx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hyojaqyp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bwvfmdvg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqaeweuz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2imxdgpea.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dezxfdab.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uzvusdnu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vwkqnmzt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xolouxkc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2myjxsnkx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2upwcfpka.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lnzxotac.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2msjzlpqu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2edjlwojo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tnmeoxqw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yvxgwpkh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jxaovqwu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jnniktpu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pwgxlere.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sambnvoo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bjsmdcxg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fzuvrqwk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2rgvvjeov.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bxunjwmq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iarrqfbe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2dpmmyzoz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cxijhhmo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2aiyyqkhy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jfecparn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2krekcugx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sakamoqo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ntqrgjpv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nbaqmnvv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rklyoezu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ctywabob.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ipvhygxe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wkpwrxlw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hivlscze.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gaabtcfe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gekcjpax.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nbfdmszc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mbltesvb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ddzyeoxy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2olnjgzmt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xrspiszq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfavuulj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpznwfop.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ikfegfhl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dwpvgcgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fwxvihpp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxavnofe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zkxbuwci.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rqnwhqzj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lgocxech.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2effqkrol.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2kasiusev.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zyufdlvm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rixehayy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2arabbmmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwhqatmj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cdjxnemw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjqdiljg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2yuhyomjp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2irmbroga.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zetuaoke.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fxmcgfjx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zsrlxlft.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bwikirwt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wbzswhmm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zndrenit.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mxnbyofz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jmjodqlt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gwfknhwa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uoxjapfp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2caftrhgb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rtdihxdf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2iogwoabj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2axyfrglg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oqphkwwg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wjzdfoxr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2onhrolzb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vrsckytw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jyumhewn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jrgzdcba.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ihjwftqr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eoeiquid.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pszslnim.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2txgmeqov.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wpxymrka.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fgtqqgal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uecsztcc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qyyfoybk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mxncuiwg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hyvtxfhs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qmjdkzlc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lxphrzvt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ccfbvfpt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uzsfwfrw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pxnpluys.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2upuolucp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2eukrhlzf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yqhbrbqx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nxfrxqrt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jzlavmhg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nacrytsk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfumsv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sohmtlvi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2viuvmcva.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ytyhowdj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nhwprkkm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2clpjjchs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qlwidclm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fveadaax.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rgqwloek.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qspujmwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xznvmsea.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2zchynskn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2odmtafro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqrcamql.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fbrfkzis.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ribvlxdv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yuvunkaf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xgbtemmm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lhcxezbp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2nhkqijpj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xuqhjvlb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fxynvnqy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ptcngdvk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qppimnhg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vqdcudsk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvtdyp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vajhwzgd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ddlgcqti.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2alullrus.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nlryciym.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2soiiaxfy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2pzkljxcm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ltrkamou.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2oktnvhio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bkfxzxqm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2osvxhohe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mzcjimbl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iwpyxqab.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2omirgbns.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eyfykmxo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2grddopke.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2datykqtr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svgjvbnj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfxjpmvh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2difrzerm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wkqmfaxj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oseauzsg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nhfjeaiv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vzlesnqg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyyovyad.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfkskkd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sitbnpym.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qinyuyph.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aoeuvwas.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvvwneas.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bvhjbkpe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jpevxcpu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhghunch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iitodasc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhmkpuav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yirzxxuq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2kuknrhqw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zsymffvx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pjsxqrhi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pqkkfrkw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jnxygxtp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yfdugjml.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zbsebfvs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ikqmrshd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uzklxeoy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ejkdlehf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2wphhmsiv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yxqkaxci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2urmfmfsz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2hkslkhoq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gimcdjch.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2oqyypnsq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pjwrgwif.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vbabgftu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2sozsoqhx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xwseoptm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vpwjeesb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bnxwklte.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tpijcgum.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nrmstrtm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kdrazxrs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jkghqdlk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wmftmwdn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2elkleecp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ddgebgwl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rnwnjuzu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mbogvfvi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bnhvkdfc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ceeuyckq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zpbyvkjn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2phzfemvd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2sxjxlcwf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tqjdcwal.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mckadvvh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wajawgwe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vrchicuu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbvqicjq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2crzxwmkc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kaylefrv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tfgodtdf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gtzrtgdt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uapsqguo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kngcpofb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hynzqfzi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqtebri.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sreyezlq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uiplorpc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fuzxeqwt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ovpkwifg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oddbrdmt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmhsvsna.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzdrsyf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bgfhpiwc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfnmeb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjsjmvb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2orjaeeoe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ravqgpbo.html


<!-- 参考信息 -->