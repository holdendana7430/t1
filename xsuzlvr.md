代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggnmshrxb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkidnxun.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzjggkvy.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/ggojojzxt.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhzaitx.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchfbwxs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuzvzydx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gevunoyoi.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/glwtcnwtx.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gwkjcpcsm.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/ggccaygcc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gituelden.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gzzgxaedh.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopevyfsu.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtzcabyxs.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gmmwwyhvv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuhzxlin.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknsqmqom.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjxquxes.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gdqxyuhsr.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrwfzwgc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gzjektcny.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcrifxgfi.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gispgkzjn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhadeuq.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqeblfw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gcelokqij.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/glajmbnph.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzlpzmel.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcikbjgq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpceveqy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gumvykmdw.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gywcaoinm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbraezlhh.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gfpgrcawz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gegapocko.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbfwnzc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjidpjkn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwteqipyj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmfusqg.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gktslmcke.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpihrkskb.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/golimlltj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gvevwpyin.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwwyfbtt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqipwjh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/ganziyieg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgnnooab.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gosuydiwd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gqltcdqfr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxntxwnp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgpaylcz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsdrlpdr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqgwbaxn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgdnzhfw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnnnnepa.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/grpkbjjhf.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/ghepwddfx.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyroivgio.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdngufpy.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupzlcsbm.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/ghimfbmmh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpnqshkw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gukcrsbsw.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gnfqzbirm.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/getpdxjci.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqizvhwp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvggxpsh.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsroixvu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gnyehmiob.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmgvnwrt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzrggvj.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gxdrlbphe.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgipkqtb.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicmbszmr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiomgsqw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gscvnzlrx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjpwgvij.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/guzpbjemc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gipnvtvmi.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gswdxikbn.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxuraqms.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gpawakvgv.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gniwshzrf.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gftldtynu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwyigwte.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gdouvdqrw.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlaftcxd.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gackycpor.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gjevapcch.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gszoafhkg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gezrvxhzd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghseqdhyr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gaqaywukc.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grjqqwtud.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhealutl.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gshawgqgj.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpbdqhsf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmitoliew.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gqtgvobyu.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gaihuhtjb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflqcufr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gklusrmad.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/glfvyoxdk.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqrmvqbp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gnmoqvuid.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffdnehcp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/ghiehoftw.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gtsorrmax.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/geequfpjc.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/ginkygbke.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gppkwmpme.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiifxohd.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnbrjvfv.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpuozrqj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnceqvzx.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gclytwsrv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpdcmyg.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gxslmfjhs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gczguhqet.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gczxockag.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjtqsfck.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxmnccgkw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxtmfkrm.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gveufbpyy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcinqcgqd.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gnvpcaeip.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvuvckht.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqizicpvk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrlfawf.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsclsapo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gttkmafxc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayecmync.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgomxfgl.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpsjltwp.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbfneccd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawliopoj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiegmxjb.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gpymytqfd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfwkjswb.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpqfdwo.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/garjwipxs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/garcqdkpb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdhzjtn.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gtbolkree.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gpifvtoyv.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gucgktgbc.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gsxzdtwmk.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gfizfyjkn.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnudydu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmyrzvyz.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtdxsfx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbfhwyg.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbezejdv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gayeepiip.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqmfband.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxnjgbzq.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gurpdwoiw.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/ghemifyvc.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwzbtove.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gsbcbwbzl.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfkilza.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gkgapqpnl.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gozmpqonl.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwydgjsh.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/ghilybrwk.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gpcwdxseo.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyyaygdi.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvysomej.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gssjdkurf.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzyboxfe.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/ghchncdxl.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjzzdwpy.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgdzqkec.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gbnbemqqc.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gnidghfyz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gyusbqjxt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/girjksubu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwtdbkbw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkeudjnk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/garoqqagn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzdtydlr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgyxvbbh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphybfozv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcsmotvx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnvsxtl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guztvapcj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/grwtwhgne.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvziddwq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscboyqpx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gipmhztuk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggksupbrr.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gznnypwhh.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gultbkksc.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgxbzqsf.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpfgoldz.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwptrqj.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjyivqco.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gezphortt.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhjavjvr.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gthufeqty.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqomslq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkdppbtm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcxxqqop.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gohvnvtlt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfctevjyw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiofxole.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gfrduecxc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gupeoldaj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gfjioedyk.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsivifuo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvkghqsl.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdrqstgo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaqkzfln.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrptbxkk.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gjyflyuai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gateohssu.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpajpbym.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gqgasmzcf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gjifygcca.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveazwkxi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gctnnonuj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gbasktkzz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivvccyq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdxetxgx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gwjastsnx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gydftsbjs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/grosmfssa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtedded.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/geannpluk.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gvlxkrtzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geueurqqj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/goqqxzzbq.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlvgnpml.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtamonn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgeixtr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guludkpej.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glglfzarr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxxhujgwb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gysumdzrt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpxrvdjl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmlvgmc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghlsxvdti.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geadvngiy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gczcxlvto.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/giowxqmgj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggniilihs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqucjrtcd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwzqpmtg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gliergefh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomngrgyy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyquctboj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxrrxcl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gigsncfwh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/goupshjer.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjbzpchku.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaqehwik.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/grczcsydh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfraaflw.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggekdcaaz.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gmkqhxngb.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/galzjbghf.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gsthjjibc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexddtogb.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/golgvkccj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/geelixxdi.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvssgwepr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgiukxi.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbebbdxph.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gyokpnaah.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhsrbjq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gjecvqifd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/glvfpyosd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltslzcho.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijjhfer.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzfppecq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/grwenssgw.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gbucugihw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gulwovtaq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gooffjzlo.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpgcdnv.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbhbaknw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcsatlzb.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrgvdzrp.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gmazjdtdr.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gzhfljarw.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjawvvyn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbabzsw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmtnbctm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhfbfmqn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtumtru.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrtajal.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavuzhzb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktvaklxr.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gsvtnssyk.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/gypddmiak.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzungtn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxysvcejo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtcbxxgu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glbomzoyy.sHtML


<!-- 参考信息 -->