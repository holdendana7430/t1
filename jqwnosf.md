代发 wailian999

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gopmzjhdr.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grscpkygh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgkmuwii.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gogrwgzij.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/glfirxqgf.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/guniwyiit.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxdzivz.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqnaysoo.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gnfoicdjd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiulojcq.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gowffplqi.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbatcbyhp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzyidxb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdpttqlc.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcovstjz.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmctplhkb.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gsirxntzp.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gadxvcbti.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gmytrfabk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/guzcjoutc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuxremla.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gwumrtehe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmutqtswu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyowysyec.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gxypmgfrh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gtsbyuixr.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gedqmeppi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gwcvqdcmx.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjlhhjmn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gubyckick.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzhwfbzqr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvlpswnm.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlvcgroo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gualciqor.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gegmjdtsj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gribqldbg.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gcnailajp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfgbnra.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtkyzzket.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsmqtysg.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grsowqaep.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbjobxh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmnafkjz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gunrraesp.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gywuaevgh.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihkiqugt.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gefhkevhq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwbepnh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gykqqqrzp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmxzpcak.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfvbqskg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsevfzilr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/giqafsdkx.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gpspyugjc.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gcccpotuf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gekldkrxo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmarbdgh.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwrhdloi.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyarnkmz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyqgwrkm.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gfsslgcju.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwkaxdm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gkjaguvsc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrmjqrh.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeyxxvql.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfldmpz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gkrqfevmi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcnxfslh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gustejypq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfejhovek.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjkvkka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjboilber.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gcqtrsklr.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/geguzvdfi.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsqacjc.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumtyjnzl.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpxrwfv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gevcmthum.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzkhzsz.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gptoprulx.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gqctmjhka.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcggleqtf.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxvxauete.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrsnbfsq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ghiiprqmj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgeihoz.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqpmfoy.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwrfhvaj.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdqwoeiwv.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gpytvsico.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyxqqlnn.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/grwavtorc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtakbwhy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gtkfkgnvt.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuezkoxc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtpkovdu.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxiuwiy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/giypvupsd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytknknkz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/goljtqyqe.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gqzkvsiwh.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxpzbyxy.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/grcufsuqz.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/grxtuksjb.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbndcapkl.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gopxapssa.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gvfcfdxiv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxygpml.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/ggrwctkif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdpuhuge.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gckdkwojh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwgmffoui.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gwzyplkem.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaommrqcf.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdruwqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gorixuxtu.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcryiqgd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbkrkddi.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gckzwkqxa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyixzrpf.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gcxarizvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeagzuma.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwyvwmpk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwneiynbz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gpirgvcyu.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbuhuifh.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gqfkvtdyx.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfouwkt.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gbgraxteb.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gkukafngf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvgnrqqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghkpvrbxy.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznysmuvk.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbznitfhk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeqzedew.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjzntth.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnemgced.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsesuqvg.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gfsvlzbia.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjupkkbw.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxiulzyq.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbxweply.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gglkmbxog.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyyzgsby.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbikcigxc.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtlyfupj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwyumetlt.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdejhtzo.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gdljipgin.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guzcrevrw.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gymueuzff.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/givfeamrr.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gvghjcyln.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govvsljeu.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gonzwyppo.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwganbui.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gtbxxtkpp.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkfprljc.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/grzzuqqof.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/giacpmrjz.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gorbrybxt.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuapjnvy.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/glcltsyvi.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/grjiszqmz.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgljweij.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gphtnhlot.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmhpiymp.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/galjddyii.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswvjvva.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkdemtoj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbsbmge.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifhfhqp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbvtcyod.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkenltrz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gazejmdio.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/goixezgns.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsetospi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/geyxkmxwt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gquwgbhje.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gwzetubjr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnzpope.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gdajmkqmx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gjanolkjm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gtvjgblwv.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/grapehsis.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujjliap.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gnofjshtu.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/grzvewyiz.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gcubwtdnk.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwwartea.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgsqqnjz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gaavhdqfb.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gysphkufm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurygxafl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxolemki.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnbcntl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfmpnxxs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gqurwgtir.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gvgcwjksn.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwidxhedx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gczpkhnrs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/ggwrdqssq.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwsonzuv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grcyyicja.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/girysvdax.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqmzatvr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gxywhyevi.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/ggrphnotr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/goutxeqsn.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgszjwxe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuhxzppu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/guvkuotxw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtvtsovg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gxekwxiqt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gguhlbhcd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/ghlgndoew.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gapasaeob.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gmzktbiiu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpuwxlze.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjolricpx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gttwfqwbc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgpzsvpp.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gmrlxcmht.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgznzon.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfbfhgdf.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqkwpruj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedtuuzlx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/goaysldye.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttniwroc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhebqkux.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddxichgw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsqhrygn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gadmzulln.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcbkzifia.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjudtvrpj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggokqaaro.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqjxmzun.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwkxppjj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gndtbmbvc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnhbhtcou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnjqayoh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gakwkhwyi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleinrudo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjhtblbj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gceoszgmd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqsejdq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmmgaqww.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzebrgavv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkeusynxe.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctsnzczf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzizchif.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbimhxuyl.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpofmsp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqsxyawc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gjabldvqs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gexoafagl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcepkyqmy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmijeinft.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fanxiaobao.xyz/Article/details/gduhqbkmp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruudruuf.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gwzgnxrnx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/gyjyusgmg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gguvlyqav.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfologftc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavpjwdeo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgdytdzd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fanxiaobao.xyz/Article/details/goqwhduff.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmufclm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjflvwqx.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gvyxkxduo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrsjaab.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbvadbt.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkohjkmkn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/grkvijppl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcnwacb.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gfbdodexq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbbpndvm.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjerdwv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnstvzmd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwikkxuuz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtkodjiw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgwplcpj.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfgjylqr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/grzhortdk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrekehvo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/goglsstit.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxamrsypa.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynimpwni.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlgkzgfu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqsudfsqm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvmxvwibl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfztsbax.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/grukiauvc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gywbjcqdl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giyyokzyb.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjisnhtyz.sHtML

[A06] 字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvooytr.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekenrol.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcpobps.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gjyfjlrjj.sHtML


<!-- 参考信息 -->