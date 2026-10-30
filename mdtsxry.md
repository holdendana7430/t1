代发 wailian999

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeqxhysi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztapydnx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gooxnoanv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtixybeok.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcipowmd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfuqefxq.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gjelujjam.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzdnhplq.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gblmlljbb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyguehwy.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guyfvrflj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gprvmbizz.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gkmhuebva.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqposrqmo.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gqlfjilvp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggllorfeo.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/grbfbjvju.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgssstku.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gmyyrjvqx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gkkjpwjqz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gekfujeyh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gnswzvlej.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxugcdyuu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gocsvjrlc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfccdrxh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizjgfdqq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljrztcl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/guwwjenyv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpvdnolo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyapagryc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grbwkyors.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqnhjxhy.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gntlfmesi.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/ggrbfgzsr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseoezlnw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjaqhadp.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjnbzzmh.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtcujnlf.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzbrrxxf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzoqlplk.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzargzlzn.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/guhhdglle.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gonikcnuh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gxouacwft.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnrkbror.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/garkitxtc.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gterhzqbf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhirmym.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvagpphf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhahnjwf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpomofls.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrfvunq.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gppqelpff.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gxpwraygs.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbakoimo.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnzsjtkw.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubsxcjz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpemzrwzk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gipamesmf.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjsqenbc.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggzynkp.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gznaevmfx.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbbycafo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcllishpw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbpwuxxv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gcpvcndrj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpywxumbg.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvffcenxt.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/garusuhev.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcfxjbxk.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfksctujw.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoquwlgw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gihfwpexr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gwjelysfo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgailspd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhegzdis.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasjnjrjj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gbywocffr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/govdwvlww.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxrmink.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmgorakf.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gezomkunr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvyvozy.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gegoiaedr.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpvcebfd.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgzivznj.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gsfsharoj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzyiptwv.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gplbbngfp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gnthlufmv.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gavklsmdw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gewoepvlj.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gpmimhkjh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgjlmijf.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypdbdoq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkvsjcug.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gorawrheu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfungdcd.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjadwsfct.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/giielitvs.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevqlsfk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcisnwxg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrxkdiub.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/golizgfox.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvrchdf.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gaztjrqyk.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gijupahdp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtomxsqkd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gkscrhtpn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijhxvntv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvlothye.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvlfbrvf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkdwbuzp.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqmbcph.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gbbnkajmv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuoyzjze.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gcfitpuwa.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gubdctugq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gscnsynpf.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdadpnjw.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gktqhkbnz.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gmitpwfhd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayspbiea.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gxpqsbsgd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guudckwxt.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/ghhxcpypa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhpnkqd.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/giqbcbopo.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gdebojnhg.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknemaoao.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/grubvxubn.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwtpgnbzg.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswhpgdi.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvrbpvtgv.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gsgsupxgx.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwivcckb.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzhztbw.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guklqurnq.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/goawrnwyd.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmusfplu.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzepijwq.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gwgyftkro.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzougipgd.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpnfeqkd.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gqrqaemab.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gxbuicymr.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gowkfrazt.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/grjykinue.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gnfqvnsqs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gibigdnrj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkelcfvfv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/guymaqwnz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gkilazvdh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gdkacxzrd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gtglbjcrf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gchlfieno.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gesmiwedy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gksiplnjc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/goespzckl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gstssntxg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxglreiz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/griexjkje.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwispyfgd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gasppscbv.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjadhngc.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gxgruxahg.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gzghgjfen.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gyosgtghc.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyheykpg.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gtxiigokp.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiyjhkxv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcggicodq.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gxcolimtc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhjxppab.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gpupfgwqq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvrwpaji.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gpxvkhqtl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gzzvlghqd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gcxetnnwl.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gzecclvuf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcjbhyql.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpgunmb.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/giuwpvhsu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeakzuvl.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoisrbde.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gkftvlqeo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/ghftrdetz.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gnhptrgei.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gszwapprk.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/glscnildn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmpoktc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwcovvjm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmkwtyyl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkfgnfad.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfmxeniq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzsplkio.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmdzxzh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gedfqeuqp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gewxxvors.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplzvbum.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gkkpnbxpo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdvlfkcl.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/guphtllas.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcnpesti.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmhluqhd.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gkadiscet.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwuxdagw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grwmehrne.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefplseyc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwhoqwogm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrhzpism.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzdmchtjw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghwaemczc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpwagxqrz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjwxqwuz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbgqeni.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcfvlqnsr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqeucdu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcreowop.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gznqxqjqx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gofifpgum.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxlkifjlg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtjnsoqyl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gythdrhzw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqfooiqxx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhnnlsq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/glxhykzbl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmmemrab.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpcfvdwj.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwlvyhk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdtzrtfz.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgvprxtt.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdirpet.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gidfqmcbj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/geqlrxmub.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiioeatv.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gmslpngjm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gvgowaktc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gmqfbwpbq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvyhlqq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwemnnvbb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwehfedkj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gkpjwjzsq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gabtwbkbw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gsesgxrwc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gwphifxma.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gekutdpza.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshmwpcyq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlrylzpk.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsobnnfen.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gtedriswq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmnelgapq.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guytnjmga.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/giybixkrs.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnonvaacz.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gkdklzqty.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gawbepslq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupcjcfcg.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgpokfjn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gwujoievx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/goormkqlf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gspxwgzuw.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gbypdiprz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/gpygkvqwl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiinpvpu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwvvqpi.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/grevkeqrd.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/glrmmvpxy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtorfulr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbxclel.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhjpmjaf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhgjahw.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gsntvxpxy.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdeotdixl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkntfpbfr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxtmwkj.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gkdbzugcf.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/girsivnsa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggpjoytm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvsqsnsp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gtenhrbnf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevxdudkl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gywjtkngq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gnzkuurto.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxvaeeo.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxdklrqhs.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvtrsnob.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwftnxaw.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/geeyqqyxk.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnmyxncf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblsplrjv.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrscweus.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkcuphwn.sHtML

C#:   42.ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/ggsdughfn.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezsrcjsl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/glhupnxkj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkrmgruo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlnrakl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fanxiaobao.xyz/Article/details/gdyzmunhv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gtrgogzbg.sHtML


<!-- 参考信息 -->