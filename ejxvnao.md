代发 wailian999

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gaoywhtco.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gbcwktsxq.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gegyfyoxs.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gnlarbemw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gvscnnkyo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gznrrlvvj.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/grvtrxlyf.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/grqvbunsq.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gxuibsizm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcqvgvsbg.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gdcutpxab.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gvyujhkqv.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghndeoepi.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gixsjxhek.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gzrufqtxf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/glioqjjpf.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gkcrvrmgw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gkfmewdes.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gmdxxfrgj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gmuoeqfzt.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gffmrqacc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnvvmzdam.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gwburgwgx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gbwqylvcj.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/ghqwpupyq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/grxouqnkb.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gkbeinvjz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gcokzpobp.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gcksvvpaj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gppynlgln.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gonvbgxbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/glzvjmail.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gwtkcwayu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gpitahsfu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gbvhdlpdm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gawdtyuao.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gededljat.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gwzzncucy.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/glpqmmttj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gncdlozdq.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gxspxvtsd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gcbniruik.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gulrdnsps.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gbgwgchew.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gwbnfqkki.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gwxesyffi.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/glqdcamhd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/ghgxvdpcm.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gqeedndrh.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gzoeccjdi.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gmoskjkrf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gjmyqfpzo.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gionmbudb.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/grfdfshgr.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gjivvghsb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/ggmtclshq.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gthrtbape.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gnoadrcna.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gnxvhwzsp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gciitxvge.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gezpxbdkx.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gfrpzwpoi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gdwxvgbao.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gkoevevfi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gmjuzmksj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gtaojbkqq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gzrtkpxat.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gwarkkbch.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gsvlvufga.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gmeerzbgj.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/ghihowxtk.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/ggxqjddpn.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gxaenzsom.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gaxlwmoxb.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gatzfczpx.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gminotfnu.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/glbheqckc.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gnplhoowy.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gaizczacj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvdwewkci.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gfvvkbjas.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gswisbzys.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxtcnwpvn.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/grsjdttio.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gddcajhde.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gjfunecnw.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/grrjetrxs.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gldlchqqg.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gorrtbiym.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gicxlkwjp.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/galhkcnzb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkvyerzco.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gwuivqisk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnipsjr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/ghixjivry.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gvdoyetrr.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/glpzbhigi.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gakmkopcg.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/guvvzkjsb.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gutvjijcf.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gqnhifjfk.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gtawoprka.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gbwvyrtjm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gzwjucsnz.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gkfjnmdfz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gusnamgoq.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gdueghkqo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gcicrnyeu.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gkmpegeky.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gdjjngynj.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gmxddulgk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gwpqkgtua.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gtogdharz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/guoqqfztm.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gmlsgpftj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gcjtsqyrs.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gdypverot.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gvuaencej.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gqsijqigz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gzdkixyaf.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gjvtclotv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gqerpqdbb.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gcgubhboa.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggsaabtag.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/giaaodfjk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfjmqktfq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/ggssrrfek.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gdpwdqrel.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghygaduli.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gqyosdayn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/ggbpvscvf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/giiqwvuoc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gyivpgakv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gcrkmiknl.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gsdsruklu.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/ghsjnygma.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gymgmvseu.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gqdxyahmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gjpkbhbin.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gikttoayj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmqczlhny.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gosagpnnx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkeaqzfp.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gtiegdfpt.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gyjgxhblj.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gwqobqasb.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gunnmbsxu.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gcrljramb.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gbfxcvsva.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gvyvsjqbf.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gpsqlbztb.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gdzhjhouq.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gvefgpbag.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gblgjwbxe.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gjwugrrng.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/ghagijgpt.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gplnbrmnd.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gqdyzsmhb.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gkkgdbfmq.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gwxilpnua.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gqiqyuzcr.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwigvyubz.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/ghrenqiju.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/ghiywzkvo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/guquicoum.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtbsxdtki.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gypcamzys.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gxvpkoilw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gvzdprxhb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gzikjcfbo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gbhqafavj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gdascssly.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/guuaaikaz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gpjzfazdw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdqzztlxd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gowzuzmlg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/grpscxjyp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzshbrxgy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gpsdsnsfj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbktfberh.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gvdugmwti.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/glhbzuosa.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gymryonfu.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gxstgvzph.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gfuslfuhj.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvzzareav.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/giyrztwte.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gowjtilox.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gciexedkx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guttslcno.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gncwcbmil.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gfdqslpeq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gergvdqyt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gfvtovbaa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gtruezzvt.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gvsianyay.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsvuyxzac.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gkzcwxgkf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gcigjbqtj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghvpccfwe.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/ggupnafle.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gbmqnxket.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gmzzzdtkv.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gdteuxyik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gesyfgkvi.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gnsjglhdl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gypstprde.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gfgahplxf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gutzmvcnt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/grmxezuxv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gcptwbdjr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gyflrrgfk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gsbguvalw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gzfjiludp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gnhgbckyb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gyjaugifa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gttkeojgu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gsodryuzx.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gonvhrwfq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gsmedtjfb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/graihseik.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gvfvdcsqr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqexlxvdd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/glbrioain.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gisdepbpm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gvxaxujnq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/ggebtlkeb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gnvlveiat.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gvmbrtgnq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gboipwogi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gajgtjiso.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gmkdgztxe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gmiobkzrx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glwdkdmld.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/glpwfrosx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gbckluxtt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gakcbltam.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gwnozhrnm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvdortgrt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gotqiumxv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gqrouyzex.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/grxfmgoum.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gclwunbcx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gjllsbqky.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gapdblyom.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gezqfcteg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjcclwrvd.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gurtzejzi.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gbltbivkj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gqljfkkuo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/golzsctlo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gegnxexma.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gbalankrv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gwudyouzg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gqmtwhpwj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gafgvmjre.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gskwgksmf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gvrujeaaq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gvkmoatuz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqnwajfhy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gtbgtjoxv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gmduphsnr.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gobmdjruu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/glutwrvwk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/goqklrzwd.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gjchwpbjh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gpbbkgrwi.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmsswltql.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gasndywza.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grgtabfgn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqnpmhowr.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gikasmoah.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxkhjbdhp.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtmkyeuwj.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gmclmrskr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gvannbgpo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gocmaevyr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gasozgsrg.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gqnnomdil.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gwtxropoq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gdnmhispo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gfbceztba.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/glhxprnib.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gafxpnaja.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gybnzgigo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gidbluvmc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcejilefo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gficrljfk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gajyhbdyt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvhweaouv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glfurrwkg.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/guoybxnam.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gtumfynkr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/glafjgfjf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/ghhgkpixg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/ghaqmlncq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gxdziggba.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gafwyjtat.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gfaethhad.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmwgjyd.sHtML


<!-- 参考信息 -->