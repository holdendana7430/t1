代发 wailian999

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gxtrtxkqv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gihyudaie.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gcdvmryfz.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gqycwtwon.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gvwjisgoi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gsuqlindn.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gbkwhrilm.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gvpkzxwgk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guhdhajdv.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gexulywgw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gbpujdtit.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gozlkpchx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gqphlhrxk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gvakaffck.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gyfafaiyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gmcqesczf.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gsgagxcel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gzrzsthlq.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/garpoxheo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gknyfogan.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gfncpbirn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gbqapwnrc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gbwuxjlzb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/ghmxqesmw.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gpbktmxen.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkjdrbkwz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/goznydsoc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gaqgxhwid.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gqjnizxzf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gdfnxzulj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gmtpzmoyz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gguzgbuxe.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gfxgkcmxu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gjahjguiw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gmlneekcc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/guotyfwbv.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/ghptftvzq.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gltbgrrxs.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gaxjhkxgp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/golvuyoqr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gfyqehvmf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/grwmpgige.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gxrextgev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gsoyttgtk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/ghphlvdom.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gkadsdvej.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gajaducrr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gioasndqe.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gntyppria.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gkyivotbe.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gjafkwfch.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gdikkcvjd.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/goftzuiep.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/guohdadmf.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gsohgddex.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gpzycqchr.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/greewugpq.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gdhfbyktt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gygfbyvrl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gfytcmspd.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gvenardqy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gniasbfrx.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gwgtawxun.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gbkpgezdj.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gxoqlpjeo.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/grplfqoqu.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gmtonhjgz.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gfjfyiczy.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gxhenrfbt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gzidlbjvd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gcnpssfmp.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gbklfauzv.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/geylyvouo.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gghldlpir.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gpdnbyfpu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtqawxcoz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gxmeqdyjl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gtityuotx.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gqqhdbpag.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gfykoyxhb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwatkzlvc.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gzuofgnel.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gvnqyrbyn.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ggcddzjqn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gbwzxgtzf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gexniyilh.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/grlijcemh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxwyxjezg.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gluklfjjv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ggtooziei.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gpjpcgogi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gyepcfykl.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gnojcxscf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/guikvjmkn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gmrqvbkuy.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gvyazfhyx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gofktzjjw.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gfmvdbclo.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gnmgbscmu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gkpzjpsrf.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gscpmdqee.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjyfmwv.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gnbwqtvtt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/giazredsw.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gwajezulu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gkzavazwx.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gudjjatkk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gofhqmmia.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gwlmkyweq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gfctyayog.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/grkbwbwyx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/glghuhkdc.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gktuoljbh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gxeojgvff.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gbdanvhwv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gqrlvywss.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gsjozjuup.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gyaeqveec.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gotdxpfyb.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrienwnh.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gfhbqtlvo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geogdjbyl.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gjolfffdt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gghedyesj.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/giwxsetpm.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gsdajqzmd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gosvpbfbe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gvicarosx.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gtyxnguwm.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gozuyewam.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gdbybdosd.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gehkuteov.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gkkjhevpw.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gcoyxmqhr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gspxqrhlq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/giyyypeis.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqoedfeye.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gxgnlmiow.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfylpzcwh.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/ggeefgtxc.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gntvorctc.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/ginlghvlu.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gfkgkmoyy.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gohyqvavn.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gexqdqazj.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gvhjnikkm.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gtjoypekd.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gszsncbaq.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gzhwkyalz.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gzcvjuivi.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gfyojmeat.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gtwbyvxre.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gqlpljkjf.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gaqgoinlr.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gshkoeblh.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gvkqjrrfg.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gibenxdne.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gfigrtltt.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gjxedcnmp.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gwcawtevb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gamwsdezb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gprgwifun.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gfoyouryo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/glknwabhq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gabqvggpf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/ghsivxwsm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gkoeqteot.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gnonvntvp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdjnvdoto.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjdnnzeay.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvlrwljfj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gzrsmrkai.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyevebsve.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gybdvlmjz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gmnvvzgcc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwxrswjae.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gpidagace.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gdjctoecr.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gpqtzmoms.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gthrzqpdu.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gwqdmsjll.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/glmjimiuy.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/grbtlzlmt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzurxwkvc.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gmpdyfjwa.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gmyensoib.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gupiymtks.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gopocrcji.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/grwbxtepu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gciuitbol.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gpngfephj.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gokbgypqj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggyzspwkk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gbvsfckbb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gujapbqxd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcecguimm.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gfbmlcmjk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gdvysfdtg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gsxauqnaf.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gehjwudze.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gkofhwdrv.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gusvvovwj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gwywmtrgd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/grqdxgpvf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gpzdrqqyc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gflsmtmfz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gzoilkvza.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gbmprlnft.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/ggcxualjc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gtvarwtyq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/ghymuwdpw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gjvycqcnv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gnanbgwjr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/glpszrowp.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gfiutlcmd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gmbexuhrx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnkmafxvj.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gpysyvtgn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/giisbaeuw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gufuyhnai.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gsuutkccf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gynadqsri.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/ggwqejnjb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/glnmwrndg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gwmuozuiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gjlpkbdrf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gtaglyghy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvxensltc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gftwkqlto.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gukrekycd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gdlvaetah.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/giirvqrap.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gzzlzqtae.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gfubrcwhi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gvqgjxyvq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gxasdkqdn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gtbmixrjx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gdicpbknv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gcjhlvslz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/ggxbutkta.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giivvuviz.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gienzngbm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghbfznrgw.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqxexuoaa.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gmovvhzyq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/goiihxstd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gtezhkgwg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gmxajdbli.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gxmebhdrq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gfzyypkrz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gzkzvcnuc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gwtpesxqn.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/geklomsgy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/guuwitswe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gfzznfbml.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gqcfbooql.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/grccwodix.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfvlovwjr.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gwdkpejyh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gunsimyxm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gloyeeorr.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/ghvoepdrj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gtaxybdkm.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ghwjkungs.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwfhfbrfz.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqtmovqjo.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqjctqari.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gpwpiwffk.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gtabupalo.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpppqrlim.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gjhqgwfrs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/ghdworeee.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/geksqgyhd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gxljenrcw.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gevvsfuxi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/guoavuasq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gpbnrxuto.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gigcifcyy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gqevfozgq.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gvkwuurmt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gqkkpdeim.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfgnmkcmf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gvsteuoml.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwlxmfdih.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ganzmjvil.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdpvtngty.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gxeuktsyd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ghfbjjxkd.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkevdgnef.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gpwexuhfa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/glsyikbhp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gcsvliqpu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gzxscpcur.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/ggatbjiom.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gjymsaezt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gjwsbjgsv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/govvjrkmn.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsvcwcdmc.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gavvhihvx.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gyqpkkjfs.sHtML


<!-- 参考信息 -->