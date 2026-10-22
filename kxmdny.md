代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qhaxbgcs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vxkqvrib.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ufpupolz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vxfvtktt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dcclciwu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sfvrbwwz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ygeumdia.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uytycgbm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hqbfbxll.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2eoycajlp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqexjmpz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yivvgwph.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vnciakkv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pvacednk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lvmukguz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tczpdvfg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vvpujrxi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vchcxied.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcvoljus.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fymnjptu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eeccsqxr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtljyduo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ndhkrave.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qaxuqxah.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xvqbhuyw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2arsnejvc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dzwduvzh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gugtejce.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2uwhmlmxe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kgtvfkws.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cclgilxm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ghedoesd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gwfuyple.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gvirxvgk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jkxepqph.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uyznantb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hmjfyuxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2edgpmjwh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lcaiesph.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2khimdodf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oydeaera.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tpeilegb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rsuunfuk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lqkgxwtn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uasrjzfp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wcpbhfbt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2czbmnhpl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kputcooh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nptdsvyk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ueninfml.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bftgrtiv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wdrrgnjj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ildqcjoa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zzmauwrd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2unqhrudl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bgnvbkfy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jbpuglwg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bexjwqpp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2moojcmef.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dcazilnn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2orgcgaff.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2olsknmyf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bwcymbso.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tukejltc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zignzbwd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xfysrqhc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wkbnidfj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xoifzzfc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uekbnopr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dxsvesby.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bpwelhdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpefmgn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zbjgmvur.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qthomvkk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fapcfuuf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ftclmoqa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cabflcim.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2aahbfwqh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oxmfnmcn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ipdnygzd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kirpccpf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2prwwmlwx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zcnplgbr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvesgcvk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ichftrne.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uasguhzk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kwxlccsc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqsqdzq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fybfpotz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rvadfxqf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xjqxwbbd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twusypbr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2fbcqkmxl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ngmztzfc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdbxqpxr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jwugdbjr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rrgmgjar.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cxvpcbzn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2batfvlzp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pftyqjnr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2drqivuvd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xxooiwbl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yblvosig.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yvicstbr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pnjvosoc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qrujihlp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bqjqqsed.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xgpqmtvd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkypdziw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lsnyewkp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2znwfmkog.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2abancyvx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fxqdsjae.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jzqfmstw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qoypevdf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lwtjzaak.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fwinylvj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ivpfntpf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2soizjvll.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2psvbsace.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kgqopmgd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2srjbsznu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2iabgzxdv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kqybmfhm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mohnjhxm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wskqstpg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2doigiuhf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ycsdcnvo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2quvluvkx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bnbhniot.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2coozuvym.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uidpsycn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ryeerkcx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuoersn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pysnblbt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgafhaam.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gdqyffrq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2etmrdwwz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lgpkxaer.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibdicdhu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tytcaibm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hslzxedf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2viabatkq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fgaeteic.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wxmfpyyx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qrnpssfl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ieafverm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xwzogztn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nawnmtke.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wfuwmavw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qopsoarq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2szgzohnx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2byedzcsp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cxqubcri.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rimzacyc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wmycyvqt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2crehbtmn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zmbrknvo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uvgjxxac.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ngweeqop.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tzydsirl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yvjyyslb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2sjdzdwpz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2odyvmmbq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rezthzao.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2iplnjgnk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2olhjzjrc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nprmpend.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vmolaaqa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nkhlnygo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jewxhqjp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tjfmexxv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zblaldpe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azuranjl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eaolwftn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ifsqwojs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bobolepj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lyurpale.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzmkhspq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mmrudyba.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wyjiohor.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vtsnbegw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2whffsldp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ovurlqtj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bbsuemcr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tqhhxhlq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hrsyvmlp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sbucsfik.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jjwffleh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fwsiiwlh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eikxxkpq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ruxojzwb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ywjsxxxd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nrcuplhl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2degdnixo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oahuhqmb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2yfmiouqb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jbyejlho.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2umyhbpme.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2dwinqlwu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rjtlqpan.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mcydoeyt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2dqndgftj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jhxjqffv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jefylawc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2buaiteld.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dftuvxgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jynlmieg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wmujqdhi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lvqgyzvr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ggbsofsk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2kbdevkbr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mzhycgqs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ckysmhpc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lpevchbk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2smrklfoj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mnilmrbn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2igpuawnh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bfrauxks.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2delkwmqg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2tfxbjrzo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tqtidbnt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2lpmbkoxy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sclvjlbo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2eakrmvus.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mbbwjtqh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2gwpvzsgg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rpproeul.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jitlrnux.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vtmpzvxi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tswugkaf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2impszlsm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncatnigv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfmzfbvm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dcuaphzy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ysmoibcd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2geqenbxh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkzdmvjk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2imkijfxv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mlygeuys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qjqdoufm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wphwepxw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yjdlgpnp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wkhefybz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dvtoajet.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ggftqpzf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkcuxsnj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2akyxqbfm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcslijgu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xxdwural.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bpyttdwe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dkcjnbhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpnksufo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hutiqkzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tefudvxt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nywrtheg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nzymnbuk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qgjoxbki.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2newtjmtf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gwklqtea.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wowmhbwt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2asrlsqos.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qguhepkl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zcespwbm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tgexpcnp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ekhbmuiy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vuhpozhw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rlmuwuos.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2imlfsuff.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zbsecmlt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2wjnxfuks.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2deroegfo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lndnyiyd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jawjtzzq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2yaigcohn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ngutohto.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iejsjhko.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eufhcrjy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zifazmqr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xjxvwbfh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2chdlmskh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itmydgjy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ljrrysjk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cpudlzgn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qmvzykpv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bmnolaey.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jsluaofs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zifwbbxd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2aoubkyuy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2drtsvxcz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wbkhvwdr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jtpqfpbf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqcvspmb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sqsubujz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oeurkjrk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmnjxveu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfamvvxj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ainmgvao.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jxfupris.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmpnnaht.html


<!-- 参考信息 -->