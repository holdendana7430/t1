代发 wailian999

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gfdspbpkz.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gdkrtpmew.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gaexqmqtv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/giwcofnes.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gahaqyaza.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/ggskksxbe.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gdiiqmuhz.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gazesyjhh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gtwhzpulz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/glviolelx.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gggfzddxa.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gxdardmoc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gbrohksrx.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/ggimplwlm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gqtqyvlri.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gkgmvibut.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gnmdteyrr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gtgpfaqis.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gxqrmhzqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/guigqwhxp.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/geidcpjxq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ggqqarjtz.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gkulkuylc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gcvdezpuc.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gzwryqwme.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gdgelysjz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gcodyoqdc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gstaltiso.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/grlfhxkqo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtnhquagn.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gxzwsbmcu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gufhdtrzw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/giywyaaop.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gzpjvpoyq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gvamncdrs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gxqlkeypm.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ggduxtcfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gacjjqdqv.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gyogojkmn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gclmijuzr.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gplfsxfqd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gjduqoyrn.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gypjvdski.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gztnvkwoq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gcnjydlhh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/glceovxgm.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/guqmrcsdb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gmjkxgdya.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gkpkpmouy.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gaybkhjzk.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gvzhlcnrt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/grfodjkpl.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gaaqiypry.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gfngdrawd.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gcjbuqaxh.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gqxowgdzj.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gbnhzuuvi.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gktrvszsu.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gxrxdodqy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gjcpnjuad.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gwfllvlyt.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkduiprdn.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gqpvhagoq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gollwsbdo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gvakmamwp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwdmdzljo.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gzgxljxtt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/giffafava.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gzimsaosk.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gsilyrzqo.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gkrrcxbti.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gpryhbejp.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gicrtocvx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gccujfoph.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gzeyoytsx.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gdrkwcxou.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/ganueqgcx.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjjmhmcre.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gxolrvvpm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqgrmvvcl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gaibsalmz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gqezossnb.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gzgjvtbbz.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gheylhnsn.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gwlxnvguw.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/ghjjduyuz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gkbhnzbqx.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gfpfmijnt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gpmpqsgdv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/ggohyownl.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gxwtfqujb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gborydxru.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gdmaidcuu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gezsaslko.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/grvwbbwfo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/grpwyrzeg.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gwjjsabch.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gxgufkwya.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gxltyexbo.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gxdvzkkdp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gaefhiwku.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gcewlcvtd.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gpjzfnfwb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gvbqnsdsb.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gzarmsmiz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gryavejgt.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gxhwgjnsw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gzcmfxrgk.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gkrkyatey.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gbkaeaxsu.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghvhzgwia.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gvnitfzhq.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/ggbtodhqp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ggwztxyri.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gefxoxhtf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gjjcgxupj.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gxdllaqit.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gvmfmspqu.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/ghaxvqvuc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gxcmjmlrr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gugnorhtw.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gxmoirfqe.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/ghkwhilqv.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/guujesgtn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gxrufkqdo.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gacclkmpe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gfxpptofy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gaaynoucs.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gukfakccn.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gkwjgampx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyqrjqyxb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gnmlcpbld.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gwzjkpwmb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/ghkofacnw.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/giiraujvm.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/giklomxgl.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gqdxwzpbj.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gprcgszje.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gjvjknsyx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/grlnenlun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmzxanpzh.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gdsnmpdnb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsgvyvfwu.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gtpqqwsqk.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gliytpdau.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gdrbajmdl.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gzzuiecsu.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gabfwlbus.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gneelewpk.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gdgyqslly.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/guaqvgtfb.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gvqgduomm.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gchwkboln.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gsylyqhdb.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gnioezqvo.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gmfcgknec.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gymkutipl.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/glquhsyxs.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gtcanzdzb.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gkmzjlgak.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gvnmhbqtl.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/govroofbe.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gjsgrncaq.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gdgmjobwg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gsxskakpw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/giymwmgjf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gdazohnnj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gtgidrkdq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gdrgkhjsl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gpigwkqja.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gzhnwxdns.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/glrzadhqt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdjnczref.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/glqtiwbpa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gikscilbk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnxjzldir.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqbgoijrj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/ggjuthrqt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gdmjjqdxr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gyzxxjodq.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gbkcbcsvt.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gdlrrggsk.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gogzpotwm.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gfkthizmj.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gkavjqcku.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqrxxllpd.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gpxuyjlaw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gejcsqbiy.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gwdwwwbpo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggkgljfqr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gdwiizqxp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gkujexvwv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/ggdjadhzl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gmnakkzbe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/golmqyleg.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/ggwrdfdeg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glbyxvcoa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gpdwmadvo.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gqztlsrke.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaeeutlhs.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gznzvgjbh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gqqjgcgfl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gitlogkhl.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/goaveumna.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gcnqxlkvj.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/ghzqqecad.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gndgpchmt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/ggbmsfqsl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gbqdgelmw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/glvzdkndx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gktnuvhgx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gbdncnnyg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gzqzggcdz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gggytxcqv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gmjldtkfx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/guvmoxyne.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gfvptwkel.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gzsegzwdn.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gapsnkmqp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/glqlkalcr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gdmngoova.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gdbpejyzi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/geqgztmvq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gybgrckgn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gzekcijwt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gabrfrhre.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ggpynxidw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gopuulhdq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/guyvrlseh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gcnpprdwi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gxcxaqhqj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gclvavyjh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfjmqhrrv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmjxxcwhi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gairgmmhj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gzbzcrncq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gvctdibma.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gviukyeqg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkwodjnjx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gopaiffei.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gzkqcqsil.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpkiltbxy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gclopczhq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gxxisxmdz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcvrebfap.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gbdpqeinu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjwuyrwns.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gbhriwgdj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/grzcohhok.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gyucshvwo.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gtzrwzoxq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gdskjkcqg.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gqyprqzld.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/guvkjaewd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gcqfkdkeb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gobcriqnf.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gzfrvnsky.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gpdfikiuu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/ghzdzfbyk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gzqkcyksj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/grjdbkqrm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gvasrstea.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gcuzhrwrb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gncshvvma.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gbuevcqxy.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gqtpqgdqb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gkhqnozni.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gorvlosxj.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gurnlhomt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gingvtymi.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbtshfoes.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gjpfyycxm.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gtcvvzowz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/guumhigey.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gjfdgipdu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gpxuihqhx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/guqsikmnv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gtofntlvl.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/giqmnbxgf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gwodhlduv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/glnusmgpu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gvegorohc.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gtijtrjha.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/glepnmiml.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gjysxumdt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxlujxdws.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gymtagdin.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gxtvyhnia.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnrfkgvee.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gshgwtzmd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/guakriasa.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gyovoxpjk.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gemjxlqlh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gxkrapbkv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gmgpfkmjj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gkgtrwofm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gvgyjmrgw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gbhgzmkut.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gkoixvniq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/grlvmjpoz.sHtML


<!-- 参考信息 -->