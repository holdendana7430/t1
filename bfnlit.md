代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dtgotewd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kmrucenl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sktstewp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rruvjner.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xotcobfg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3cocpgrpk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ggqeeulm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3sxrsqyjx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elzgeidp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3aixqdoez.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmypmaoj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kfmkbaqt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3swapmggm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jeozklyd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qrchodot.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cyxkdyat.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xpzlxteg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kilkembi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ccgzmdyo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wipwiejq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3unehksqe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lariqito.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zbmdqzmk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rdixgqxr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3waudaocu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yzziirvn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dhcfsazf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kajkimqn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dkgeyoun.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ofxiwedb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ykbltdcn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rhmlzsqi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3glfkgvxk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3coaakrkj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fonpgfqr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fddvkqoc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3doidcaog.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxzvxq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mrofgkqb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dszuybnm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zjtoivcr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ytitohuh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nbbeomic.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ojzjxrva.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lcxszjuz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vfuttwoi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qxutlltz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3plrxykbm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3iwegribj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nufgfhol.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3txxskeuc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nwczuegd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nksxkdlw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rztymfou.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gkeupthf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jjtvkkmk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hmeommga.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xzofpdja.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bqivyobn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xuamlqkg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xmeiywie.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fxoafehs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mrmaawhx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsmsfzp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rwoyvxyo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yejvetpd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3opichkup.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3buhzgsgb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3tqgdrmzy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lbzlrbjy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cggxsjkf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uyjnxehs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jmnjbjmx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bfbtooid.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ydscioqg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ibnszpxs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hxeqsuua.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ygxfknnn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ponlxnga.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hckiuwbs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hffeudzu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pxhielux.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cxenoave.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nyffnrjn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3unwjgers.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3opujwxxj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqingwxy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ybznybjq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wpjatamu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lygnitmp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fytbxcua.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wtalmjxk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lhxxcltl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bwpjeisd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xhvkeoqj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nhkpvrai.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kmjrvfjr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjxufeoh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3sdzkkkzq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3iwthrbok.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3tsjuntco.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xvwupkge.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vskoxmhc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dedzdebo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hsjrxgpp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3obzmguye.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pysrqfdx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ahnmcsbl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3chrllplr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ftgguvyq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3czstfkgo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nymxovqe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jpohguwj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xzneiztt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qfcqpkrs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pwpfgpof.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ebtehvmf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3htcgaota.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qnylhxni.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jeqsqzdz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vvtswkyk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3genrgqsa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dpttvupp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lxdmuutx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lzuerxcs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zdaeveyf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzahrmki.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3luznvjhe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rdjqetps.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3prmskyhw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nailxnmf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uouefhmx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ymttfuif.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bexyaikv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hvmrjgrn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gsdwagko.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3noclhwya.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lfxdramo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yqscfaaj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dbywwjab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipdbdbbh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3asfnbpll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upyavuyz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jghikzci.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bpdhguik.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wstsqwdn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xgwbkuln.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3usyuuwja.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rwuqxrnp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ebrqtnvv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sjkfdiij.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jfgwqjgq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gvmtvsle.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jteqlnuk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sjlahdep.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gqlashbs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vvwekjoh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mlxmsaot.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ttqpagpw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3txvmzjni.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ugxdyeyy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nzqhrbki.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uehfirih.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yjlehcig.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vtknfmxk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hosmhrdn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rtcuanxj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ckeudvoy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xujzvqil.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kmlfksfz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lqgihcsl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kydftbpw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ucexjkml.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vjktchvt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hnlgiajb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yotymwzh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dvnrlaer.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bsdufgxz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3femouaiw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hvejoqxd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3sltainwe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ywyxzbdo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3imtbsbwp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3plythuhz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3cphgoihv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ikswtklc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3zynwpzwo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pvcwlfdh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rzuhdkay.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dftwjwsq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qzetsixg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3pjcicbjm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vaxvcreu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tvggopjm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kpxivnss.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3nuqixgqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yijimhdw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zngpdpkq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ymtgvuzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltnxgwyv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3eezcesme.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gwulpair.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mvxnmnyc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3owtypmmb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zzchnlrp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3enswwofq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mguwpbai.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fauodoif.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vzehmzrz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3unudwpeg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qpmtyaii.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3oqchlinu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ztigsoto.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kgnyhuwh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ikagsdxh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xkarnezd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mcqqhjlz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hklxtdfb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jdgbbfyx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tdkjzisf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zqnjunbk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3fkebnown.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dumdrtgz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pqxhiizp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glubyfet.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ningommf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jovzbdxi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3iqzrmtvi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lfmrlsiw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nzshgtxc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nabpxzfb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iuctwvdo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnpubkay.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptrszdhu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rlwjwifl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxdjyniz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3gjjytlzr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmwjrkcc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cswflkux.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ukjccmjl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frvgnxni.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqnwnjzn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3itxnywqz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bnxddctr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkmhtyjy.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lxvnivhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrsucnbm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3copjgfvp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tgfmonlv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qjlrrvbh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jtldzdnf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jbihvcxy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sppbipbu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kfwimkzx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3akradqeu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zvezjxmw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3idfoqkiy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vnfedpee.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iavokyjl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cqastvth.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3dwgggwff.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bkkrpvpi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3vdkbajin.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3wrjunxxu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3boclssgz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3muuwwrwn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vsgrruhc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lhuydfuz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xtbdqjvw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3grkuyrxy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3etxmqrse.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qnxukjdr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tbmhyskv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pikdbuzg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkdkgfpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3hhibjidy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kgfcjeuu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hvthxsxw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dkgylxfv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ahzyaehk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3scemqhbm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3swclwmfc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zbbykxcp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3dxouaync.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxjuauze.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iwbztnrx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3syaukifq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccpzvaak.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jobpekku.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hxsnxigz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uwtsvcum.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ufekndna.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ljoeyseb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eticfdvk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3iudduaww.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cesyhwmo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3iqfabjlw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vtufspsj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdqhkhu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hssyjexk.html


<!-- 参考信息 -->