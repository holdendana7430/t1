代发 wailian999

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/guycthhxu.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gbnvcgutp.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gcvxnyybv.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gahfdpgsh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gxmjvlsqn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/glbvcbkiw.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gdnekbbnc.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/ghykjrgvb.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gktymsncc.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gcyhszzaz.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/grpoygpdz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/ggknznenh.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gefupcget.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gphwyqqku.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gzdlmjlxg.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gfrbvobib.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gnhuauyhs.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gvnlpkufl.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/garmyrmcm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gdojoyfbw.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/grdyvztki.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/garyuyrfj.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gfgvnphaf.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gfivitapm.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gtvbicdaq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gfpfaarze.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gmamtvzrl.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gkywmjaqv.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcxhbvfxu.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gvjyupgan.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/glcttwvig.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtjfgjqov.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gfmlqomng.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gxqybngag.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gjputthww.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gyakoqpwj.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gqraiuuhe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gagzvyjjt.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gftfvsywf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gbryykhgn.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/goaiuqwek.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/godmnbjfb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/givbjpbsn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gejggishz.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/geuzuwuxf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gvonrpwzb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gukdjbctc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gledqylzj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gvwhaqkjj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gcoafpeqs.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gmtxvnlqy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gerfjalxr.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gkdrdldnf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gyvazsilt.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gjyvudtrv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/goqoojssp.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gkqxvzzta.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/grbhobflt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gbpctblib.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/ggquwbeqe.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gfqahuudy.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gkqjjsmzr.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gprzqtsiv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gtzrefctj.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gqumyhyjg.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gayxpoxpp.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gceowbwzn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gawckpezb.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ginikdgcb.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gvxzexsuy.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gkaxasnbj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gahgoqykq.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/ganmqghaj.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gvnpzjojs.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gornywkyo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gonumquuh.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/ginqguadx.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gtoprzaeu.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gepbnuwfh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/ghhhjtkyb.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gnsskipvr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/girwmipqh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gjcdmipko.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gfewzhumd.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gvzzvkjtu.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gwmfnjaaf.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/ghljnbtea.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gstzpnvpc.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gmlgxywfm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/grjrbldwu.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/grhjolyfa.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gqxxgtvpq.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gxlgpfwkt.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gtpcprqie.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gzyndispn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gvzhymnby.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gccwwaycn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gpxqxyjnu.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gljgapzop.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gfqjumkcp.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gxwekjiot.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwdrhof.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/grfktkcaa.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/geqkadbbf.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gkghfqadz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gouiwdwjj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/grmjkcnsj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gncospqjg.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfzbjdg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gvbmsihgh.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gsgknzyhr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gywufpoey.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gzwzbuljx.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/glbyztidj.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/guapntjos.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/ginnqziky.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gryteehka.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/guzwxsehy.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gdgthljaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gqklxssuk.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gnxxqxzcb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/ghajxbgsv.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gvmjzcvsm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqfxtwnol.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/grjleilyn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gsmhksbky.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gcskvjuzr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gpzwtsgow.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gpsodbdyv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/guopkvgoj.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gyevqttwe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gcmwakifs.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gihsrffpy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gwlwvsccn.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/guovmxefa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ghnxbjgvo.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gjqrurvfk.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gdfcxgxwu.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gqaycdpys.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gxnjbfeon.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gktxxzwqs.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvscnpyhz.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gpcdcxdaz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gnmeopxcw.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gtangysjo.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gtodfcxjz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gwbiaashz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gbojvpiqg.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gsfvqoclm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/grjzhednp.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gjxhjejdp.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/ggrinxpqm.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/ggjogteqz.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gecbfmgte.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/giujzyiej.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gphejqrdx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmrejisnj.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/ghyobefaf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbjccoru.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gmzqekpsr.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gsecnpcrp.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gurrmflvg.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gkiaqkemn.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gevorbvfs.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gnopnfhws.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gnqeqkkpm.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gsqcijazz.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/glirllixo.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gixqtwsrs.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gqzpawzbn.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gsfvmhqyp.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gzshmohwl.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gnvlfmvsy.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gcdnflzcx.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/ghgluatuw.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gvtzsyeyl.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gbpybyjtu.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gswvuvfem.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gatvrgwgk.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gzcvuaigy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gpdfmeorn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gisuiucry.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gghgnvmzr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/giugslpfl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gutrytdve.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gvcmjedyt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gehlkgtas.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gtdcdpfix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guzyvdrqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gugljwiwn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gzgstkzoz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/goiviqkcs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gcvkckvzr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/glddbsuja.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gpvhgoqdv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/guwkfvgtx.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/goeemddhe.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gfzghzhas.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/godqnznal.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gawxvzgpw.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gixjwilwj.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gahvtnnpg.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcqtfyu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggvkheuxq.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gjdqvileg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjjabemnt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gyauqmlow.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gwbftsfvy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gzavgsleb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gcunhhozt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gpwyltxos.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/guefqsbgl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdxsiifct.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/guyeoifcc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gluknfygu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxktlphkv.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gwpmxxkie.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gccdxphkn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gvazecoka.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gwtilvpnv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gqvryjoyb.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/ggwpepnyb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gwqltjufv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gkcrjomhu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/ggbwruxjw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gvlppybgb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gmbbddcov.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gmnidytjp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gascmfwtj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/ggnutfnju.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gkflnsptw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/ghpfsrifl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gvjfboqqt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gnemfjese.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gjlxpifwd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gfcknuaah.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gddpsbrgf.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gbrjzthdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/guvnytixy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gyyimvqai.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gqrrcqhpa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/giwoywlar.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/glraylkwh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/ggcnvmaby.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gmvqbpxli.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ggbrbplpm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gzxoqteyd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqlnndzkp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqmfmzogd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gurubjwjg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmlofbzyy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gteaclisn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/grabfgpxp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gkpybzewf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghkipdydv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gdcelirna.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gxgkodzph.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gzwvybiym.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gidvjhsgg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gfdohegqe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gecxargzg.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gdtfxuzus.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/groordqjc.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/ggkpqwufl.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gavcemrlw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gvpkikhey.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/glxcduzrd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gwfhqgegc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gwvywhiem.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gvysneaqf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gjgfkgtsk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gapewunhg.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gnijflojh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/ghmydkhos.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwkgypewj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gbswwklwn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gniiaxzvf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gyvettjyb.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/grsrmlgxa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/glvjcvzxp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gpgcgqlrk.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gfxxpfdnc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gjbskwrzi.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwhmuraeb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwghknlgg.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/glrjvynvn.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwdlxpivw.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/ghkasjspm.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gnsuzxxfb.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjowglpls.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gopraqrxc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gvnknihix.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/grzuendag.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gnrmhrnpm.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gauneouag.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gumatykzz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gmhzpddxu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gamvxwjgq.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gcjtcglpc.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gwgfwklkd.sHtML


<!-- 参考信息 -->