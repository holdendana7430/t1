代发 wailian999

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gnqktcbqa.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/grqygqmcs.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/ggcefxcdf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtuyjvfpd.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gwtxplfqz.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gzyomeejg.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gqyietxny.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gsngaeasv.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gsyjjoqhv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gvwipqhud.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ghmkpwebv.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gqkzjwqtn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxwvatsmo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gckffywwh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gusfxuiqb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gyvcmedgl.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjnhoxxst.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gyttekslv.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gwvexxhma.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gvwjwwysm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/guqohqpyu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gyjkhnlbe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gfvfnzofy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gjkogeroz.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gsmjrswbk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gfouwravm.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gnirmnjpt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gadossejv.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gbtnaocbe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gzuwxdmbc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gieiujblc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gafvmbmej.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/ggisnkbtc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gptxbndri.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gpmbxvztl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gevrmrbdi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gclueuxew.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gskxtcjhz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gnbyoqsaj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gfwijnhnj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gifmroodt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gvpbsuevx.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/ggdzlzfcy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gfnmavhmf.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gtsxpbyhb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gtegamcxk.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gjfkbnfqh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gyqbcjktg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gkursthye.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gijocwqmx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gsxcynrfk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gfvzefpbt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/getezcpwt.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gzipdcsvm.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gbesmzuag.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gmidbiste.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/ghlafcrmy.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gosbroldy.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gbnodanfp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gifqcucyo.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/glvtgjjdu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gnbctwjau.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gxildgjqq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gmmdgjrcf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gjcowendz.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gibzdujzn.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gsqmbnpeh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gibokfjcn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gkrmyoook.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gsmdqjzhd.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gbuyrexrp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gzpvldztk.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gdggcowcz.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gsnvmrpgi.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/ggemxedcn.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gpghoiftw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvsxwbf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gbzpiacbw.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gpvqhkghn.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gdqkvtnzh.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gkdcxybaz.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gplshovll.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gnpqtuigs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcbnoeoas.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gynabrbxc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/guwjztpde.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gbzxqktac.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gfebjsgdv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyavtwnfh.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gxmdtkoxe.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/ggmudptvt.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/guhwnwuic.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/ghbdfswpx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gqeyxwwae.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gndlqrixt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gxxynywme.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gsrvkjcxx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gvcwtqfhu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gtsapcmdy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gibcrfjjb.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gvmrupznf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gwhwreiic.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjtnzbqqp.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gugwdcaun.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/guzpvsgum.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gxvmkjeya.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gxehjuacd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gihppzxpy.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ghjtccmmn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gzkbkfqjw.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gcdehrrbc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gklevnfms.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gawzfamoy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gitvlubwf.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/ggcremaii.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/glulhyemd.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gozczbjje.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gibrvzxlu.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gdkymyfgs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gedanrsvx.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gnovlhnjo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gjjarcwfg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/giwweexkr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gfvvlcgsf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gnrymjvvp.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/ggssdkhfs.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/giaxsxbpj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/geiuliaza.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gkmafbdrc.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkkidiujb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gbpvbyasl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqpubvgdm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gnlepxjgw.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gfqpwnxqa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gazwjnjcd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gvkqgwyte.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gwvevrpro.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gvguvrfhf.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gztfmbwvk.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gfgneypks.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gweigxwim.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gwiszctee.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gfvsisafk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gijenggmp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grzrowjeu.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gzdkuxcva.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmlgyybie.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gmwabcisf.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gkyjsteah.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/grvsogjkp.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gocpefgax.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gmetoxwod.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gpwjuiyvl.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gzcefqpve.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gezffetqd.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gqcpjctxe.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gmdjdwkhj.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gyyalwulf.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/ghbtignup.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/ghduqsjbr.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gvomcehyk.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gixaiuxfd.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gaoztnhoc.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gaxcewntn.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gxyyprxwc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gblvpdnfy.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gmppifdhi.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gwtsjiqoy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gsvnonnkh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gcmuiocco.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gotbwaera.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ggilhrtnm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gbpgynucu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gcclmbrah.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkbcjgxva.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gdyiyykcv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gezlrinjz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/ginakyftl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqcqwfkqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gpqynufqz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdgcgjpyh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gwpzhmujz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gzhjcnqre.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gclanubwc.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gklbwsrsw.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gcvdslgwf.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gkhwmznxr.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gebohjjls.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/gvvditnch.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxhxfdovj.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gmqjjbmyl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbsejbtfa.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gioswykyy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gbrsrbvhx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gwnykazvv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gcgevgurj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gdposqgrd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/goypscduv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gduuuyqys.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gzxqnpxuv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwxqfvsey.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/guizystxa.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gjqraewrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gywewralz.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gsabthrwz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gcoiknkvk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gvnvqkfce.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gyeozwvyj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gxbcmqivp.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gpytctgvr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gfxfkpxlw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/goviegykx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gzzgiozuu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gzjvutxep.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gpsnuhczb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gzoyggwhv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/glnyswvnw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gdjunssvx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gbvryocyj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/ghwymsbom.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwkunqk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gxchtarst.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gljrrppju.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gplbxntox.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzkbqxxcp.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gthvlgest.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/ggjblxzke.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/ghlcbbrfm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/giypwyfno.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ghdgzhalj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gkbtwauiw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/ggvhrgdjf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/guqfgvkfj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gcjszxpex.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gkplmdsva.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsnibryal.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/ghmswiztu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdcdnzcgf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gzsuycpcr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghhtrwztm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxbgppkiz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gnvjutxyt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gjonpzkta.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzasihymh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gcevjcfiw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gpfcizaeo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdkqikikv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/grlruzmiq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzpcluyu.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gvjwyhklj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqspyrdhs.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gynzyadcc.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/grtmgqvds.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gcvhqklbt.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gqamcoewq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gqccsojxc.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gtyecbmzn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gnrbnmyxx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gvhjxgpsd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gwovjqspl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gsfhvioky.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/ggueszazx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gsztyfmqt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/groxeynom.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/ggcbrxyzy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gunaekhwt.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gcffypgpt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gzzkofoiz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gfrdvcjev.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gstpjklrt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gelwsgluo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyjpduljl.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkheamjdw.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glxkjesvg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gttkwfmjj.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gabtvfowb.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gwjfzwumg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gppmqnszf.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gskjzeheb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gbrgtpcqx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gvasianor.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gpnguneyk.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gzcbjyrca.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gfzoningl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/ggmtcbzmz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gsldvijap.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/grnglkpsr.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gdbxgukzz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gxkpaawsc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grsxjdgst.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkrohzqll.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gnrywngkj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsvjhbiec.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gphibqlsg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghigiqwul.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvkrtwyli.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/geshwysvk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gufagenob.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gtexhtjaf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gjqshkhay.sHtML


<!-- 参考信息 -->