代发 wailian999

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/geatqcnvw.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiiwsqvr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyjrapqg.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfesjlyou.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gqggiywbp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmnrttbx.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grbhzhesa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklxxnmbl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gdkhqdoeg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/guhanzjfa.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/glrxhobwy.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzxvfxsu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmegoelep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwjozqc.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvxsjocao.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldtuyuze.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfccjwrh.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcfvnfatj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgjexueu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmxtimzt.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/geizxgbwz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gprblngkv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqqarby.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gcblszxod.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/grjnooopv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxhtoecnv.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwitplqj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghihibunm.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxecdkfwe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqnehud.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjolmqoq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoylwtqp.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzfrxcm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwetmyi.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gsnyguaaa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgcxpiuk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaaiiiub.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdujsfnjr.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxqyvsom.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gginkkzyq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gmoiihbzq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqefpferp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtcpang.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gxaimykfw.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlodqury.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtnmifsm.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmfluwq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrfmifx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvzywufk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gylxezlaz.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giliackgz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuklvtzl.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gfixnwxsv.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/geawretoc.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjnybwos.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoocfbe.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooswjttk.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gnimwwqbi.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gsnxamilq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gykymxapu.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziaczdfy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqvmeflc.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjgdmhfr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gkurtzugr.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvedbfhi.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywwrwrq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyztgxtu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/guzlgdbce.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gertpmdtg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemojhii.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/groujauma.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeyyakjv.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqnramgb.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqwmeykb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggearqoge.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/ggsxrbyia.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gndnmebjf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/giqpxdboo.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gafyepzwj.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaduzvsnf.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gqnjzefeq.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/genhyikyi.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxzqoyfnr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/glkoijkej.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gormeeggm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gdwfvypga.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwqylsjyf.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gywfjpkzd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzomdysin.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/goqjyxqnd.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjdptph.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gppsvyiko.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gfplwmlgo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gggepovwv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcqznutl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/glyopmuub.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwqlinsy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/ggjlijcly.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwqycskf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydshwadg.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gectinjpl.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gzanwynwr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gyshorrnw.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gvkacyrdw.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbftmcko.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gtnxrxtmm.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqtsexij.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijhxjllj.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtqudchm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzuvavem.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgfpqxsg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gguxinagg.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvybbivf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjrrsgmus.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbfvvakm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkmanab.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/grhkgrlto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/givcuttar.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxagxdgd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/glxrgowoc.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsyrsusdk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwwgnysr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdxudam.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gbpcsyodb.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gguttnzqk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzizylfuf.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gnzhnfsjd.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvxayost.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyvsobwm.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gupxslybk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxunasfjv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsjmthzu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwvnqrsj.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzafkdj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gmvmqgirc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddpzdxy.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gykinbmhy.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gdguozjwg.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gijjrhabt.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomhzqhd.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusowlau.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzcfzuul.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxhaeui.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/glztbaabq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqrgnwiz.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwiksbqy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzzamvr.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwnfcgts.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gzplvsacv.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guznacloy.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmqmsdnj.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/godtkhelv.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/giukzhpkx.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gcqynlqhr.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/geirszaab.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/geevmhhmo.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtgtwbz.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gssrfnvaf.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gcdiyvckb.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqjvwwhe.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gcbuvyqas.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/goqapbudb.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfevfxnb.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/garxmxmnx.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwduqnssx.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guksdjety.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gywszzutx.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gmgsdtrhq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gssemiesj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzzgmmxf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gjadqawfl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceeuscmn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgjaamzt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwicvuyob.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gvjsbylek.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gpyqouikk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvfftch.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gmpboruss.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqoecatvn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivaxxcm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhsxbatj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/grloyvnod.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlufnsqr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gkprsuciu.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayegkbdz.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gyezojgib.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbtpvbjd.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflyviim.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/grhchdhsk.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjxfymdt.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmfgwlu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbbjdzbr.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gssnukcza.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gagqpyrtu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqrcwyeh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/glepqkdvt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/gydeecnki.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrkunkcq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/grenutsff.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttwjabxm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxywmuwtc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbfqqwkq.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnispynf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbunnrvsk.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/guykhkqhr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/ghlhgpvhp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/ggxpuuzac.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbaddry.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjzmwnvz.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gkxuixrxo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknpigca.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaqzvzpd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gkphemqsd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gxrruuets.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/ggygwlxfl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvdhqwxf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/grqethjrj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqqrqvi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/guqrzpbfu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbinriny.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhctauok.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkvgaour.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gpulqrdty.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnihinvpd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjhvcwo.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnjisaub.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gneztitrz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuejsgzm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqhdbgo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guvdeeomg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gprijljyo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjtfixtxc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwjlhcuj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gynnpjicd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gehjgglwu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfnzfotr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdmjmvrpr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfkykjce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhatfcf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmcmudmnp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelgwgtcn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtywzjfvz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grpuploem.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmfkzkxui.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrnfjkhg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpzjzmbj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurqznxf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqectxa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbqaijr.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxszzvfh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmdcinwh.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggjwxofwe.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuocltmj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gofqapxts.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/glmridgcm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/glwdffpaf.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gczkxkdna.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gyfuxbeny.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/grpadcmlk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gckmhdpeq.sHtML

[A02] 变量声明与赋值
来源：http://baike.fanxiaobao.xyz/Article/details/gueisiyto.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gzrcenhgz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeymkoco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaclziehg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhregztu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvqrhait.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fanxiaobao.xyz/Article/details/gpuycuutx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gppjqodmt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gwzkcetrg.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvifrvgg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gvugfcptm.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ggmubatrv.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfciwrsxf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gngfgynqk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqioxbfv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnzlqepo.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbttxfpi.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/guekiflrt.sHtML

[A04] 判断变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqgthfmki.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gshswdxwk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/giputgidr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrydrwnm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhhvyvc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/giehwvvnw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gzbhjqzlw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeazugry.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gqbbyaasy.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gicanuawz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwprtseoc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcppjvtnj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpyabkeeh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyngcjyb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtxauafh.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/guhibkhjh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdunxodr.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtwpbdve.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvmumpll.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gggllsxbf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/goazfcxhn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvibpyjxs.sHtML


<!-- 参考信息 -->