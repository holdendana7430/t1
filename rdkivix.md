代发 wailian999

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gqhecqljf.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gukoadnmi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gcpbjdkfi.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gcvhubhaz.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gwvjpgjra.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gxvhmzsfs.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gplwwphfd.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gicldynid.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gbapijjxx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gdenfvisj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gesdvhlzs.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gqmehoozi.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gsxfyylmj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gzydgagne.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghfskopro.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gauercusq.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gppzweofk.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gsxxafexo.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/guuxwbwfl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtjbzziia.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gvbruypjf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/goxrdnyqg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gbmhbyzol.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gsgxqtbwq.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gxklfoofm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gavpqflax.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gagsebedc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gyaxuajpu.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gmwitsfig.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gtitktvbl.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gonmshgfu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gpmjjeyyb.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gbmbolhqd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpgtnrkxm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gscygwiay.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gwjuqmhlt.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gfqvsnibn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gaxsonmsg.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gzxetgpdn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/ghxqaynxk.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gjbktuhpv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gtlhmpqne.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gmhaxzfca.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gnyedpftj.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gsfynjlgv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gcryoooug.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gjmngwdxn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gzomixbqv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gezvoejbo.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gqiwsvyzs.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gywmodzbk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gapkeiidd.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/ggbvxesra.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/goigymkti.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gkybykdle.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gzznondqt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gpduqevjs.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gjlwbbhgx.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmawhjrtx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gfrgjnecs.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gkoktgnvy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/ghabvrgcq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gjbiocazp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gjsrjqbnk.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gnmldaebv.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gvgbhnrwq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gynianwqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gzfjjfbal.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gppgbnpgn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gyxwvegpg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/ghjnetamf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/glvyzbhoc.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gbruttuak.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gsexzmccn.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gthjmtgwe.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ghwaxhzjb.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/ggkmgjqjv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gtcjlevji.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gklcrkrfi.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gzjhrzmoh.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gcqilbiel.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gclaogatp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/goiaimqye.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdnqtjpmj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gjzmyipap.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gonjpxmfp.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/goprvknys.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/grvupkgou.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gpbyjddkh.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/guyxldoyw.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gzumsywtw.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ggkychhvw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gagtfkvyk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gpqwfgvrz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gjfzrxryc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gahdnlkxm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gnhtvxusc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtfmbnqrg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gjzgymrog.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gazqcsqzo.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gjfiboyhb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/grdeykeih.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/ggemisjks.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gphuwgdkk.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gzmboefxd.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gmtyuhnji.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/ghdupulzz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gsyyxgnxo.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gjebkqroo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gxqzogbvq.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gefuahoya.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gcnzyutsl.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/ghgtaagpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gkyprxfgs.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnmqajuqd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/grjilgywo.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gcjuvfsqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gaswujzbu.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gmjioitgo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gajdcqwsj.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gtrtzixto.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gtptbcjlh.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gehestimr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gywyqrznq.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gwnadhius.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gatlqqwum.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/ggghvlziz.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gnbcnzyhz.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gtasjzzda.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggwtjubtb.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gdfwakkpm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gfrxvpkpg.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gqgaifvnx.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqloyzj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gcvgnfdik.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gwgicsngf.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gniqhevzo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gbiihqjie.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gscqjlqvx.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gubugecqh.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gvmjuebqw.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/glekmydwn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gnpotonjg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gbycionds.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmesheeb.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gssfpxuro.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggikgzzky.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/guqunzewn.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gxeysnmae.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gzardplyl.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gcvmipkmx.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gvzuksvwf.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/ghswlqqtb.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/grmaktniz.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gwapdvauq.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gcjwzawxu.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gxqssigjl.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gkbnycvnj.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gdwsxsavv.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gnwktlzhb.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gwquwrnjo.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gvjaazkwr.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gpiwxeocw.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gcswynnnv.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/glijbrqgv.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpzavefru.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gbhvygegz.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gcnfbkwlw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gbgazeuuo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfrwkiimp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/grwknzyfk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gptdiomhw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gmmdummsd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/goggnqhub.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqhddod.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/glehsipnj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbxzeeuud.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gcjofxypb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ggtaqrlpa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gdrxvhpij.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glbbqmiig.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ggyoaawlt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gjevcpuou.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gaqspbpvn.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gwiaasfsj.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gefhdhlzp.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gamdrghcz.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gygneewwc.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/guyykkoir.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ggmofyesm.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gugglzmrn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmbrjigay.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gzajjxuqv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvqclem.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gayzrrcda.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gcywnulyh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/ghpwmkhin.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gqqykagyr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/ggovywxds.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gujsntsmi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glnpvufnj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/geguxjxly.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gpzpvuqfr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gobuuhono.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gbsnnapxm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gzonrcejv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/givynuina.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gsjnflsrq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gxfpmycjj.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gcqpypwhf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gmtyvqzix.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gwcliaxny.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/giuaxbajp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/ghbmrmzmb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gnirwmzio.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gdzsepzca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gnmwueqey.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gyroufxnn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gdcvbybcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gstmdzpep.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gogdkxhwj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gihcpamqn.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gswrkbleo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gmsjdypol.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gveolckhh.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gduxvuuyp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcyodgntf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gjzfqebsw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gvexplvaz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gdienvxjx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gfcpsdiju.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxewsfrzf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gjpymurjd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gtmrtfliw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gevmmhduz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gmqestokn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gxojwtcfc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gavydurqa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjaitjyfs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/grknfqwys.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ghuvkogdl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/geoddgxjo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/guthvllfx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gsodbbdgj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gmwyyzjoy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gefxsjizl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gwhcvzscg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gpmpnumvt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfodbgmzs.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/giclcbezx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmgwqqehx.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gaglyxlyc.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gozzsweaw.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gbybfqkxz.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gfcyivyjj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gsfdvgvuu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gpwmspvfv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/geuhonwmw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/ghjxmlmxd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gecdnsaor.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gvxngmugg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gpipnkplu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqnbhxcli.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gpiflvvyh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gwwucvcum.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gwblvojwo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/ghnxpopuu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gvztiiwwe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/guhtpnrsw.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gtqhfjdec.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gstangflc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gymxyehmu.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gyphpazmi.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsflxfcuv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gudlbryng.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gururjwtv.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gnqwtuyua.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqmmeojgk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfrunjl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gkkiwxyoy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gmccgkpns.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gydxcjylr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/guevzgryb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gbcljlatr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/ggdzsvpaf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gzseoqvoc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/givkwqtwg.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/ggtouzjpj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gehtwicvb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gxntnvrwh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvyryti.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gxumoffcc.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gdvrrjpmp.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gupyexslu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gafsvidrj.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbvinhgzn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gfmtugaka.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gvxaasmpk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gakyfellk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gitwxarbt.sHtML


<!-- 参考信息 -->