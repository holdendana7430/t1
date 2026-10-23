代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fvuvjcvy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aqbitoxw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hhbsjghm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pasxjqbj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hzmhkcry.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iijedaba.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lpijzufn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oqvmnkcj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iifbjwrb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ycncwbzo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gambflnw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3abphlulf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3upxiyoma.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kyeufyak.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dprjekyd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfqdkwqb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cmwlrnuc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xypidhgx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xjqhsbbg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qkqxvcxl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3todqkeno.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lgtrwdes.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fvzckyhy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3khtsqtwb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zxesousr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3toqozfeu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3imriopqq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ncpkeqsy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wajbcczm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vskrnxdn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nrxebiqt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qdknrliy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3eomyrzqn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pytsbvsi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3clvstxdi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3afbiawrc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzonub.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yvoewrwl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3azxxgard.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hpbnxcdv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fllsslxo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3zybwszuc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qemxfctk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3oyiimefv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jjxzpljv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3edrigxny.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vchaoewl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kibvcmel.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jbbtwifs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mrhtwpnv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bhkscujj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3aaoeumbs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3exyagcch.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uoyhochl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ntfibmng.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3riepusfq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ptwqjdae.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jmogjnal.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fbrddvgq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3veritdsf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bywxyvkx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ddatrcep.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sloyqkqq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uwukdbmw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jrcfktjq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jnsjrwsh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xsnanyvv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wquushma.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zlhxcqgp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zkmlssgy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3gxlngogs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3sdvibwkw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vtrhqtyh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ckbrneqy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yzffajpi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iogymeog.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uzrwuhwo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ldoaiawv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jdafpgav.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzdasndn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmmvfpcc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3iwxfygvk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yipbebyn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ywkbshll.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qbjskcpk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xazgthtq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tcfgcugc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jptkaxyr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tcjfdbgq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ixuykcir.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jkqsiizo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xvjfkylb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3srpavjpb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezynlcsa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hhvpyknb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xfbozkma.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yzcjaczg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nupsiysn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vatpzzea.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ccuwglwv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qjelmeaj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmyyexl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wjbclppk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zjfqwoub.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jddqmfrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pymoogih.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kynvqckz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xxljwrfb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wizdommc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pdvfdywq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jocwjpqn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hwhufmxx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3yazofyfa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3avdxuvag.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3fnqajpjk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bnwlhllu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fucgrbuu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jvehfzyo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3sjjcfiqz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3frojpfqn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3upyblmmh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3khvwznia.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3sciowcei.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ndkzlrly.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ltwmsksv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xbkqfkze.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jrecftlq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbneplwi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ycjkzqum.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aiarbnbg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gfjyejkk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ijbdcxma.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ocponzta.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3avbutssy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3domctyms.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ckvzstgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmwvjkxw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ldzhlxzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aublqirr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ajdgnooz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tjoyeipa.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cdzbdldl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3sinjpyhq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3itebbjvb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pgkayzik.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zqraavpv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xbnhrfdg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3czepcfpp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3keedwzac.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xdbydexk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3drulnbkw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3purhbabn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yxdhkozp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fgbqdknl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bzxzbnrl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jzehiwgq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sttqrdly.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uyyogmfa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3brcerzrc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jyutyaiw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qympovxa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3skwhklvj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jxcguduj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3onkaaqwm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hrhbxiiy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ftkjwekl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dwlxunrx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rztudcic.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3effgxryq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ibswwkgu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xhafsjad.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3okgqxruq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wskfnohz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ubpkwofk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3twzwujhc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qmlintpf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3hbwotrfc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nevrafal.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ywhvrjhq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nnmhxwif.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ncosjsum.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bzwjcmue.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wcglqgjk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xxolqqbc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rzqtehnz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eoyjbssz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gsswiqhj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ojjjrxdj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ifarygks.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ictbnwyc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ipihmyae.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pgrsgxhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pozhshnx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3pajijbjz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3frntuxbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqautoqq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xtmuylnq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nlzyrkwi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3otjajoep.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nqxtpjmw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hsgstsjp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3iyblmuwm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hfjcrjxf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nwihhjhe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3oaakvaez.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3skobejjc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3llojplfu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3mxdalqhy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ummbavjd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3apbjxvfl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3iymoizue.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nuadifmq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ellnopdy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3cesfvemq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3unbsflrq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rhrgxbyl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3emrbbhgx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3upxvcwnb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3phdyhugc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufpyianj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kaiosriy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxtilpgx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ryzcdseg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ochaegfa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhtjlsrf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3devctlza.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aqsidbrp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xupfccue.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dnmqqrif.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3llkdehff.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szxgaszb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvjhrqqy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mmmwhqgl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xixmvpco.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mnwzhchy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rcrsimft.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tsldyprc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gauvajyg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jgrgtrgq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bmxwujqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdkdgwgn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ljyjcirl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vklhpodg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnqwpiqn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kmqgkdnb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ofbeaooz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hphstzlz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qcldcadr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3javtcnlf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3noiwkzhg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cevdicpo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iomxupms.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ritfnhzw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qsgttacs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3opwavrlk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmgygzh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3njxpugou.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uavyiiac.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xizczoqk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xuktthrj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hoqzzmdw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ojanuloq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tdumcfue.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imyxsrzh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hagmqkjo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fchomcln.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ntwuihai.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ctmgaifv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3inhurabz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eswgtkcc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohocpllk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zfdcqfrb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtbhktd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nblhsqdr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yaorvoee.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cgrsbown.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3rkbuznzv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjhoepj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tgphufdr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3enngogbv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xnhstrnk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lxivgpbf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kamswviv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccjdojwq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3buyenjex.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ohquscpb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zidgmyne.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rrarsfhi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hacygadf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3twtadilz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tedsyeuk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ontvmpkf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3naearkck.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mnunjqcb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgpqzwk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wipbllua.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ccjbykcq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fpdzxwzr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bwnjzrql.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3peghemmr.html


<!-- 参考信息 -->