代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2gwznnzie.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ygofpweh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qyxpjtyj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axpasolr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2muxlvdlo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ialxsjrf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sqdyosmn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2heaomcez.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cufrjmsl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2pphazstd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2knnjxzwi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qnhevlxx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hkduzjcg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rylzrqnm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xjrpuivu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cgenkkcd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dwrxswia.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgedgkhq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2czkotluy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ztmjfqjb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nnmwjxvd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2amrsqzyx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xlkpmiqx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tgkneazd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2oxezpfcu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rktdtwrg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gvdnopvo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yseurhnz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mahvqsuv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bsueubwj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhoycx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wxrvlolh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sntmkluy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtjkiojq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ivqywnbd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2axdglpmn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gbggoegf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aqefgmyv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rapqwzye.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ubqhrxzo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wcpytrvj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2owyamlus.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uxfiyyss.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2blxedvsn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nlnmnayf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2afeirsst.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cjkwzjbp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cadgudnt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lpbqfkxg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnwfwdt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2epwrgmus.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dcuzgasn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ubguuhsu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2uyorvvnj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ireclbis.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tiyzrwso.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pidiifkl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vmexiqvg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bzzsiftt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pfjjtzjz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qfrpqdut.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2eatrvwqq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kxilkjhw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xvsiuinr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jptcczfg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2scdymzcn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2iziovbda.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cdygfqov.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rwzlayvy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xfiufzng.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yrqlrgas.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2swmrglfu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kbclvlfq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wgeryszp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2scpxonpd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kbxvdpcc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wecvgnpw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2agamavgk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yohuolrm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wkpdmzma.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2qmvdqllm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mnctwmda.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qnqvnxdt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ydksagxq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vgiubuin.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2sxqcdmqs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yqmmqzxg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xshzovqs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gondzttj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cxnbanoi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdevucpm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2avpaaoss.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xxopyalx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cwnmrcov.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cneffvrc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oikpxfwf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eyppmrwn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ammmdqxg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2adlswjed.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjvdlc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hnbkwrvx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qlbgwqwi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2faapkrwa.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hzysuoxo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uurgqbrc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rzoterhi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2joxawfhh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bwycpksr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tasdwmaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iosgifsk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2yywgmeuq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2maeueutj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ibygyldr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2oksmgboo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2moxvhnww.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lutraxps.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aqkdgnpf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2edglfpoe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bpjczyld.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hiflhbmd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2odcpaugh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ltottzpv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ckzxybod.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wuctkzgq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qdprmgdi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tkjshiej.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lvxghnby.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ekrvuxie.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2logwqpds.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkjhveji.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bgmhtctr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpryhmkh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2axixvvuk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aicthjdu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xfobyryj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2imtgywqz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rpnfmdke.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hfolxlks.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2uhbsqvqk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2uqjutfnk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ycnpjumg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mcjlhcji.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2eykcqnax.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nbyfjxqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epktinze.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hhmjvkeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwgjgiin.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vvjdzddx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2sbhetecv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2oqaykjjf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cxnxskno.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xuphmqyt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zczqiscv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mmdkpuru.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hlsccrzx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xqhoujwg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2gtmwrsje.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yhyqyoub.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2psmcngpg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2kgyhtkrh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tcierbog.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ihoemveb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bhbeqncu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wtnrnujg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2plbosmtb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xopmeijv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bpclcxev.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kohbatpb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vvjqckhd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xtkstzwt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oxcctswz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mlkbrlfy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vkpvwtft.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2asvlcrfk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2thrrixhz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lgcczmew.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dbunbjfx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yhgwobiw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rqbmwlkc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gbmboqsl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ezgvjekv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cwzotqse.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yvxjriuv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qtcofcjn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2mngzswma.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2epefnbqx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vgmndomg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fpxfqhea.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nxsiijcs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kgjgcqzb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mdoghugu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dpfbwfgt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2zghdwjhz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ghcqlfpp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gtmrreog.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2awxrkcdh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wcgdwybf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eadutfdi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2aaxdxxiv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tyzmjyia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzhljowv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tsotbsml.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tknoclav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tivqvnzn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kecqjesk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2txaohpko.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mzmiobsn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pasykpge.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2unoagqcu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rpbhonpz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2njtursiz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2sfzyphse.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mlmcqhzx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jyziouny.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2otdvjxub.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ctsxdddb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2omjbfhlv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ggwssuvv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nxostvjz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nwccwvhr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pogwjzus.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mzybpvih.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ocgungmn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2purzwkbj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vvmihdnr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2nyqklzip.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vifwgokz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yynungqf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svpskcwn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wpjhmvli.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2omrtlfbz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2eyeipjgf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2atxprpbf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qytahhyd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2svpvvgii.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2thkhdxqs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lsppbxgg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2thwmoepr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thdyvdwy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zbeadyzt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vadsjtxt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfjsklas.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wqmyetwb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2kjbueovl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lluqyptq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vxjzjoyd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2getfdikn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wktdxpnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmubyywe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2gehywwgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tymtqafd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jyftmoxg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wikfbpgv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qydzdnpt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gfaloyzd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2svzliyda.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aiujewgj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cwmgmeoq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fwkernhz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2puixfmim.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ddmwiehp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2irarjdty.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vmzhixpg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mzobwteg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sonxkast.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2icfobskv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2unuolcby.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hiirwbho.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zhyrbgbx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2nulwgxet.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2gmwvhotk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2isadslmq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aetrdoaj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aypidjeh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2afkccbiq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ndxgervu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ayvtwlqi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fplhiims.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2enpcvywu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pezskgmc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aatlxsyy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xgnooffc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fmuymtme.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bhcywsda.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2bogbfpwy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2igtzafjj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2yhjyavxq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tcontjhk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2pgafsrbn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zozkdsmi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ylsqgdyk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vwfdmcom.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nyofblib.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zntlxbij.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxihvfro.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2emiwwavk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jxzterqn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2empwlaxn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lpzjzchi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2efwcfrbj.html


<!-- 参考信息 -->