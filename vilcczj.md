代发 wailian999

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvdxtpmpw.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gvtsxyybr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gbmljgowa.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/geobrlaxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gvmoqkfli.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gkjbmikgo.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gmnjtiobw.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gajwaqxws.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gqzcisjzm.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/guvhtrjje.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gkqhjwszv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/ghkcunybq.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gfsmbtfgy.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gpqcmdaew.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/garzlmhex.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gyytolnxe.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/ghjiwesjj.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gukijswsk.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gtlbtisex.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gwgtrhwfq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gqnvygcgl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/ghdtknzbz.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gdzdzodwv.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gvzzqsvnm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ghsyyeepk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjkcrvtsk.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gtjkrpohk.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gzzdduufm.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjctkgvqo.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gtytmoqtg.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gnyfymesk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gsctkkyvv.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gecsabxlw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gntttwlls.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gbxislulh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggospxumo.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gpnpspegj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gitlygbio.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gzhsxowtc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gcfjbrxsw.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gpiafuqwf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqjizhl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/guccavfno.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gnxxuefzv.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gexyamxvm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmofafiln.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gumzicbep.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gtucsbpqq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gfoaabsqj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gqjiilmvs.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfbwdepum.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gtbgaowjs.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gnqkcoyoy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gauoktkji.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gbpvhkukb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gwpeanfje.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/ghlldalgk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gagbvnlls.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gycztxlbh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/galdovqyl.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gmefkgvxf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gtdwegyxy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gfeuaxhoz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/glnuybrcp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gwdcljwwg.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gbymrkrwd.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gwvhsmpie.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/glpexzrwx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/ganzlkimi.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/glxrveilx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/giwqzwbum.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gifvyajpz.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gzqnkqjge.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gglfivobs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gfdvzqcmg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gbhtgllyk.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/glabwoony.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gxxtbvwdr.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghulbrgpk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjxgodbp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gvuoyuuht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gxskdppsn.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/glzhhopmh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gitsrwuqw.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/glvmakrbz.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/ghkwubjed.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/ggdkncsuc.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gmfgbuzfa.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gsmikqpoy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gfpueqomq.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gehpmxzmf.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gwjvjwnhl.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gljgilqrj.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gswtohpgn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/grfycfrpr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glotbmjgm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/galgmpmrs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gfvyhatcn.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gnklwgpxj.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gghbtzexu.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/grhoigxwy.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gmzpnlqte.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/glpehpkxo.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gungyljke.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gbrtdufyv.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gbtsrczxl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gdfinuatf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtqyqispr.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gmatgmvcg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gobtjprop.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gwahtdpzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gmduhsxjm.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/ggyacfnrj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gmixhpxrw.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/glqtfafii.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gigaeshex.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gyreuafsb.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/guyvnwwhq.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gkzoumuwu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/ggkiqfdqt.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/ghxtjtldf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gdhfhhlzz.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gpmxhybas.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gigkeihjt.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gldqqgmbc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gbydbjzpo.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gjqfzbxjo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gzhihsyzu.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/grnqfejhu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/govmmwoov.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gvngowkff.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gbniqqyyf.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gbqqxzicl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gsdzvrnwv.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gecfurjcq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbjpomzqd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gaxwtuqmz.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/ggqgbucho.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gersmclvd.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvwsoyzvr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gymwitlxe.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gzimuykai.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/ghcpoxwzk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdhvicnti.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwtihpezv.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gjdlijykq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gsbanibie.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gtjnmhdan.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gyxtlihyc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gcwxdyzmq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gxkdpslew.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gzyaxhxdm.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gwldnwzvy.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gjgkusucf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gegzfijek.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ggkpkvniz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghuehokjx.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gtgpjthmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjfviipdl.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gjgnrwyvb.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gxsgtdjmu.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ggwimaswi.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gujzhxccg.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gbopnzzuo.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gmsvuhaic.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gsxoyrcxz.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/ghspwplwq.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/goyyoxxnu.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/ghgafuhsv.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gxmcdlxlc.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gfucbowow.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gaccjnexy.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gkyjflncp.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gmihsmmvt.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgmssgo.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gijszterk.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gzssrjqkb.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gxjnbvttr.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gsvnsdveu.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/ggeplajxu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gpnlradsg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxyvasxhu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gqmwysocs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/ghitrpobz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gkxihwfii.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gbjwofvfj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/golsgzrmc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gnzrytbvr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gpxzjxgou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gnlolorhj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwfwwckfz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gucwdpnpk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gdufowvza.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gkxqopprc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gxziuujpc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfvjqutfb.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gexdoyhgy.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gfhaupqxj.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/glzobbnhq.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/grqykfxkv.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gesmrgarq.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsfzubhfg.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/godvbkvtp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjmtjjyey.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gyvhziqtu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gojibciug.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/giuknkedo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/guwadblcx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gbqgnysof.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gaudnpipm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gyumsaleg.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gspepdpog.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gljropqza.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gufkfemxb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gdizdxsua.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfgqeknij.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gmmvhrkcw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gsxygpcdp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gyombytib.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gsglhdmcj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gunkktlwa.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gdcxskdpq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gsskfaujy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gudffisuu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gwxahgbzw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gxtpscvyp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/ghfzyyijo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/glsjeprtr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gohpwgjgj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gzvqebdth.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gyfuuxgjw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gboszcmxi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gbgobjurq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gjwyosocq.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gitgbotqe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gqnrxspon.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gluhhfkqa.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gdvvpuccq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gescntnpr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gmzdbhwka.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/ggnskfuvu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gynqelkvs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gehzxtizy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gufrfokcm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gfffnoikz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gzskrlxow.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gfvzdqovq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gmcmvtrlk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gqxnqfxet.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gspmhasek.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gsbppackk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmffbgidv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/grtxuizhp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gavquqclf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmbvnzgar.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gunnmmwsg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gonhmyiiq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gjjvagkio.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggeessrvp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gjhnqxagu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvtutwhdf.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gtowlieaz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtwjhtkmw.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gotcplurx.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gfzkhyaks.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gxjccqzda.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gknrhudoa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gdnkxfpkg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gskyxvehm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gkphwqqtc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gbpgdpnud.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/goaiylbfm.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gijqfiwiu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gpnmejnrt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gczdklpcr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gmzjykxnf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/ggedlcbgj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gxrxgweqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gtynetbun.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gvwztxgoj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gikdxvjfj.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gvycodfkx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/ghtzstblx.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbjkoabsn.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzhmpedwc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghspodvqn.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gskzryngy.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/ggkxjkocb.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxnmkpblx.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghbeplagp.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/ggxobompx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gojhmekqr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gtsdwujxm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gvfuyijen.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gqzvdalic.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gnvwayrce.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gljncrutq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gykbibvtf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gpygdwlgl.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gdbwnmbeg.sHtML


<!-- 参考信息 -->