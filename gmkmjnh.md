代发 wailian999

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gvjvfgyzf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gmgttdwyt.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohamldy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gssvrftso.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkluilqdd.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcavohun.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gwyqrkpnp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgybjiux.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiklsare.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduskvrcr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gucykogvz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/guufwdncs.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlixqwmj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaayyvest.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmkrtmkn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gjsavhgju.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gmpjiecvq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwomaitx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmbxdffc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gauxhjxpo.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsoabiwr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspbcijps.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpxpjkmu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gajlrbaiu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqclelsh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdtbjrun.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdmythwj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gnjgjzlms.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gslkqysnt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtsetwgt.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohgiqcw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtalcawhl.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gmpbmniyg.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwhzbwak.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzhpvmhql.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtguzlnpd.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzmtfksd.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrikmxes.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfawnecwz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gqkvxvtfm.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssftqwat.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersolvnt.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/geibxwgmv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwrbzlfn.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/grvadiraw.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gcsfceyfi.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcncumvop.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/geoipremc.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgntsjod.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzywqdk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/giigdkzrc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gwjwosrxt.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gakjldyus.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzqyezra.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gwriksqtz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/ghmgvhjuu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gvftnxwqq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gcnybmjix.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljpynuhp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gympflrzt.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gorycoojr.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gvncyvmdi.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyptznit.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhoyagny.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpetsqh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvibnhe.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/glivrgmmm.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gseyjrfxy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guibnhgfo.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gvttxoxjs.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gckqecwvf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwmmnikb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gzokfcbye.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktncgvhx.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjpykcm.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gloxjyfop.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrhbxzrg.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlstogek.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/geghssevi.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghicpeyce.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gassbytaf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvhbuvxz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyhlbzee.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmfuzyjb.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/giejiipuc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gzrijfems.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gligsfrhp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gpnzamlid.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gagyaiwpf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gguxqcrmn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geatzcmtr.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gterpdamw.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqrxqza.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gdekrmggx.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gthzuceou.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/glbcnones.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvzlbkwq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrfdzdoi.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhvymxd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfzmngvzi.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvenswta.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdkvruaxc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdcowjyc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gcwtndmgj.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gfcwrljir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gogtixmva.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkikweq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gnkpqngbo.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gyizicpmw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gtifdteif.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqjbhkbq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gqfteichs.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafhfszns.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gejnsamlz.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjvcxtu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gomwcqwei.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqptjfjp.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gzdeqtnyd.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gclgktuto.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwrzptul.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gegvxvkzu.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqgodplw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/geicugurg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqickpet.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdsqnxhs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqnqsabp.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimcxfhv.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaiayhfp.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gzhtjmhgs.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlglfmgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gamnhbuwe.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/grwsdaxpg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvacnrkfj.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gtxhmvomg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guwambbsj.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnkbhorr.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/ggyorgbql.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeeuomoo.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gztiknjyi.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtlzisqt.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuvwxmwi.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gmugajssi.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/goufyiimu.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ghdysujvj.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgdqiprl.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/ghybxobdo.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gervzkohe.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdauevnqz.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaozbwte.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gfkgdqqdc.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/garuzjgkx.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gztvxcipz.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gekxblxze.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gzquynovi.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gzjntvjmp.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfqcebck.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsobjzsx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/glehiouqv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gzceeoxnz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gztlvycbr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gdagbeaws.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxhvumao.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhytayt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgmqhmu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkjvntrzc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gndknmobg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgbdtupc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcihnkqj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojmzpexk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gexrzpygq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/glylrweuu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gmcartnum.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gncraviua.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gzjfeojhq.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/grizsufnh.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gghjlhnyg.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/grindqznu.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbynosnsd.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gntireckp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfsralur.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gzvyhfaky.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmvjboiwb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmexrfuze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdmkyjm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdjffndz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgnfcngx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/grtgdtkda.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcjfwdiw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grmwgrorg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbptkamhk.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gmrwdafrs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gselmgvcr.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gwijpbbeo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gztmlwpmr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhztalqe.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufmagtc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwedfgiv.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrwejtlb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gdwvqjhlr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gzltqtdum.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabdmdgdd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gqivdceiq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhrmsev.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gboulletx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidzalowy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gobsenniy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gurwkucqt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gsoskfjzy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gbbnneuws.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjpdozec.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvgsiyxq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcebpawhj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gpiixlfqc.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gishyaeqr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gashgdnui.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtnwdxzit.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvfkxph.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdblxrrqn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gidvmppdb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjxtaqg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpwgkhia.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genzqmgrr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubhdgcqd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerywsfjf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guejhqcxq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gamfdxjmx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gldmvgmjk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/giwtdgvqn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpezivd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtdsoskgt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnbbguno.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiwruucl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gugsagelu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gntydjopg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxcoawmk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmsnowri.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxraplqgc.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfcrwqbo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsxpztly.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzjdadanz.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gvrswsyaq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadbjwoee.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyraplafq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmxhvnnt.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkopslsd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrrmllpw.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhahezxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnirxqrue.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgytufmt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyksdfwf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdjscbnq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzrzczuy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gbkjcdawm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gcmbmbzlr.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqcknyab.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gvzlcoerg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhxolchg.sHtML

[A03] 常量定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuimkvwv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gyosrjqyf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbrurzgr.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grxdwcotq.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzsxiiwt.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gbhllobax.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzznfdti.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlnqdccc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxmmnshl.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gsviyprto.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gdoefcsyr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcuouyih.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gqepczvtq.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gzuovrslf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhodean.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gvtfbxjgu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gafqkxfso.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gleozofid.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/garjrasqj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gikxbbjde.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/guvmqrvex.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwcfnrg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geznssxni.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtvutmuw.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsidwyock.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuhtcqbs.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkjfadiif.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gyambiqrs.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyhvnrot.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknetxdz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefdmxsd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gjvghyasj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdswquxi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdexdtnq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gicyopppn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gtfmrukwu.sHtML

[A07] 数字转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gplvueaiu.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeojzujj.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/ggevsfnfm.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbwdiynw.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmdjdxsj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccirzovd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gtdvszesq.sHtML


<!-- 参考信息 -->