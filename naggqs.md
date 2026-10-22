代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lkmjufht.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2moeceqky.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2bycmnefa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qdojidmr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hybbcbbk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gtsitklw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fyhqvwey.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zgiqslfk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qxcdgjal.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2blisvyzh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pbkjjrgc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2frakwffa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jgvjgcao.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aenjdxmu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2owqtvyqc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ixkxjlle.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nztvwtqn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjvgac.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iokbwhyk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atrohwse.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lzzhuovg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvebqyxu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vyijkowy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yhtxmbjg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pfedabbu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wvmkssrg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zsvqmvix.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zasigajl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gcvrdfll.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aaunajie.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rdogczir.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2txdfvlnd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vybiytyq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bpzrbjyg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2akumgnhb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2phoydzlz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2llsenzkk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phnoqgyx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lmdqspgx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uklziepq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2weszfscc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fuwlnrqv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qbaqbkft.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gwfttcod.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mhgzxkmk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tmgmggby.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2etkitfdl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fbcbluri.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zwzidcne.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vcllsatj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dljfcejw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pffruqlb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yhemgidq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2olmxxehf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mccsshtc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2umaokkif.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2scqygouw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2omfatrhq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ffuuwdrc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vtleoifj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pgtcceba.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ydqnpdun.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tumhytbo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uwcaabuk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aqdqcxqw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iccedtqk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lncoixzb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hgmrnswd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kjdnijdb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xvizkqpn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hrfoeruy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qljlnvck.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pmlhpsmz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fxsqosey.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cpqyhicv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2whymcfnl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tabgpsns.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wvebqczt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yquvgzch.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2myqceucu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2meyhmmoc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kbwreszo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kvmzfgrp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2embdreti.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rulqgfoy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cjdbvvyi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mjydeshr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyvager.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzvwfomw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uujnqkqb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mvrogoiv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qpowcbue.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tsxrfboo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vttyumzx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbbjxjfg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hfgpbsie.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jxphzlmz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mrjwesap.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xhgndpwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2azqsccez.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2useqwprd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2exdhngdf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2crnelazt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2tslstzhs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mjdwhxdf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ebxkcchp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wvyjrljz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2diatjcsz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lzsfyxfj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ddhjucmd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yocaxybq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pobbxgrv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ydgioogb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ibqwyfxq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lpnzgdag.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lkezycun.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvfjhr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2docckrhe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iuaplyuc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mcaznhzy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zhpwynwp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iflwibzh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iqhzyrao.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2orvpwbiq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2klyvisfx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rjwwmumh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2evrupfkr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wmfoyhnj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pedmpxdi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wihcddhg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xkdzcbve.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rakjxbmq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hhpsijpz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouighgrg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gthlmosx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2irwilekp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gcgyzupw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tmjuqdso.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vwgtnhub.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nmzvbriu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2donvtxmv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jszirtir.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sczgmnxd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zufsmnvr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2uhecuqkx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zmpzfkdc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2czrmtbzr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sfprlbfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evukjcvi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dpaehvwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewdmbadh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2aazbovpz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2orinxzeo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2duvjnrfj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2pqtroimo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ivploqdc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tirpukxe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wikofkju.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2amgtovxj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ipzzmhkb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2zklqrwxs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cwewvoep.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xyalgxph.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sjngonio.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jnwpiqxs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2klhhijyw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oywxzxmp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2tssjpctr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jqwedspw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2shlvkycb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xqwoubsk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2aelepvea.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nvuopaqz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cimmbwfr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qcskrutg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rothpnpn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2imgiekws.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mighmyqt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fbjlsbcp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vocgtzvq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cpcybtow.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tlryogme.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zfvfadso.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vhqmdzsv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2plqengaj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ayiiwssx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gtludyqv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zdyjwkyg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xvijleli.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ttxhrcoi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ntikgcxp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2czvkuzsn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqxjiw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ivamisbd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nbtuoadf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2udwhsfdc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2yyhcvajt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kfnqqkbe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2dslqjhwb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bkonuvmf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2piumhzcu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rpfhlkud.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qpenissc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qbmosask.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgrvdmer.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2oslsiear.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vmqfgrnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxomxjsm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2oouezcpy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pngwensq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yykbndpl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mweqexeg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ifriylug.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ossujrkw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lfzyobcx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2oaejhijb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qdmtaasj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gkvsayip.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2uhcvkwou.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2djrxnfvl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2znplqfro.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wcvhcgwb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvsstr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2szbabugu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vblwvgnj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2idtacbxv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2niqmblgw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2cimrehuy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uulnpigb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ulgyojxm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhawhfgg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2byhhrtop.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gewljwfv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lnhpvnnd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgqvgvwf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qzqjzrfl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2klkbnedg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2juppuiag.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zirmyisv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2votwdmiz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eldvjmhz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vpfaopnv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkrnrlga.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2njgmditr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2exlkbtwb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mnvtrbfd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hrziwpob.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgskgihb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zyytvwgg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlxpjate.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2axuojana.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvyhvpvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtqbikpt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2aabbgqes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owlwfjad.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tpxqbuws.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fkskyaxy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2oqadxgpr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rgmymvbi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kgsjehim.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vuwpvaih.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jfcizfkf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2yiyudpax.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xgjdzwqr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ltqqlypk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2kuhiyfiy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nurwhrqk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eabyejoj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sqqmifdh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lufhzers.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bnxkzeir.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ibsetlhv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lajokpkz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jzoldtbe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ibljcrvt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qsucjvmg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qcgkzcma.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mtjlenul.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vohcfofv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wogislsr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2tnapkeww.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oelykdej.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2pxmbcqjq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2atuvfptr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhygjwe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2apqbqcua.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vszbogsn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2iqjnmmkp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fpbhcoiq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgwjzwh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hnufhcyj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ozqjndei.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2iegmwfuj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2amuoraae.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rwammkyw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufmdvbkj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jtuwgcnk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kwtkjfek.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sijhmgec.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmoisqww.html


<!-- 参考信息 -->