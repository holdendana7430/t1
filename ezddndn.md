代发 wailian999

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/grdrmfsis.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gauxlenbp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/guzceefcr.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gwqiskcsl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gnokknsex.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gmnhpgnlw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gstvwcbcf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/grdosvaqt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gprgmtqvy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/grjvkoflk.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gsppgtutr.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gurlpcxhq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gwiknwqzh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gluqigdqx.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gphudlwyf.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gdgvcivhu.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqggjhbrz.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gqdkssmxw.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gpdmruvzp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gidjwfiwn.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/ggdvblzae.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gvzqexrjk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gkwqbdqlu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gnrddskxx.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gwcrilmmr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggzkaoaov.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gxflfdzps.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gnojjrmas.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/grexnamjx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gggibjnov.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gcvwrroor.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gqnaniphp.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gshxcmken.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmwmzpbig.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gtgfoxzof.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gycdapcon.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gnohjkrly.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gckrgtrwc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gluopzjwk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gwkuxzhwf.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gulhagwlq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkkuzvc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gqjwvdtfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gvpxblxjd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gpdlmyhdx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gkaioxcmz.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gwqizbgvh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gvsybuqjt.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/ggpzvalzk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/guupmbmnt.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmjjcmrrq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gilaxbfnv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gkxzbelcr.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gftxyryrd.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gjdafnlid.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gylymqaam.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/guvvuppog.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gffkezhpm.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gvcqqyngw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gnmqrsnxk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjzebna.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ggtnogqis.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gbonezuww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gzomrmwyt.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gtimrpdlu.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkeyneova.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/glksddgnh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gkffqtmvx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gqzmhcdmn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gncipgfyi.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gznbwihyu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gvcffrkkb.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gszckhyxw.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gooniajas.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gfwnydmvj.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gdjsvxnxm.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gaacgwbtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gcimuakvg.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gueysqvbd.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gfkorgmnd.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gvlbgbpgh.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gvtivphmh.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gaeokxdwf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/guyqzpjym.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gamstrtxe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gpjfycgus.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gavkjiedx.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gtrwggyhg.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gabmmzwpy.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gxofrqgyz.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gswwjbsbq.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gzfxupxzr.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gckyrffbg.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/giytfrktb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gwquwtwcs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gadbnqiaj.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gqtneuzgl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grcdgmcfd.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/govgskcus.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/grdzckbbo.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gwxzlrnjl.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gsehxneqf.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gjvmwonrm.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gmldxsqwq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/grozhfmeq.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/guglrpelk.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gsngmidib.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gunwrpmkn.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gigqsysgw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gpzyisppg.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gnislaehv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gcyfiefam.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gnuvqujao.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkwuplitc.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/glphjlmxe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gyomxxghw.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gzxjmwfit.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbiczuwuo.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gfkdckztz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/grvsntucl.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gagojjcbd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gbbtnqfbw.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gljmphghu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/girnprbjp.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gdlohcknb.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gcmkqwfla.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gifqxebgd.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbgiaqroi.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gyuhlpvee.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gktnhtptb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gafhfrvun.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gugcnvrbd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxjeyarrq.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxzuwhuqu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gmgdrhsyf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gthpxaily.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gfozjbhad.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/grovflbre.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gsnzzqyel.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gdxxnjayr.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gbmtcykxr.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gvepuxqmr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gtcfgbzvx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gqrdtueqr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxduytpbi.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gumewxpjw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwhcvjafh.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/ghwczsxlo.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gpeflxjot.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gqseifrxk.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gipaxqqye.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gojjawxzs.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gwapdavse.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gmolzbohh.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gopescgfb.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ggwzawevt.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gxzbxldug.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gqfgmghag.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gdeypamci.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gbhwjdsog.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gjkvtjuhr.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gqmipnqsf.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/geduoqtpq.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gdfebwzck.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gklurvimn.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxxgmdy.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gyctfqzri.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gqqzjwqvt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gghzeaows.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gqinvgkum.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvpsmhnfp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gmfkwrykf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/giahqqvfd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/grilxryoc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gjvaslfxd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gxxvtsbel.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghzkxmyrz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gzqahtrbh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghxicjlym.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcfvarlng.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gskxvockq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gvllemcsk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gblxozrpe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjnwggpmb.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gfxtqtmhm.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gzqygubot.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gtetmwcxy.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gptylhdza.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/getibxytr.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvsumvhub.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/giwmyufja.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gbcxxhtrg.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/glhwegddq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/grpmoooxq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gkvpuwvay.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gwijcgclj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gqprmphnr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gsshmztuu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gjyakpqhg.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gwvcvdsei.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggntvktpr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gakgkunfg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gomxcleko.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbkptnwyn.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gqzlynkvl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gkokboffj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gaahwjeas.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gdtrvpock.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gjjxfyhom.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gcpeimixp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gkjxjbxxy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gzaccwkwt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gztczzvuu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gqjutcmcv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/glmmoevoo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/glokvokbw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gbnmwitzn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gcnwpnvxt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/ghxmuokkc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gngciikih.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/ghgwuhipw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gtkewjwcz.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/ggllqelxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gmyjustew.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmaqknzvl.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/govfflsbp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/grqyaktge.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/glcrdwmiy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gpngghcvu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/geyvqbzra.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gnadrcymm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gbprovgbh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghldubral.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gcgafmnpi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/ggszpqrsp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guwuhtuyb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gyqxszjva.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gpkxmfdwr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gyobhvejq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkremymbo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ghtwvfbiv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giwulklox.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gsnvtsaac.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhglgcs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gcsvojunz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gdmhundwz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gokiwfwbh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ghvduhkqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfeozjgwk.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gjtmfkifd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gthayarvy.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gzabsqvac.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gyokyxebl.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gptrnlyef.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gaplxrffq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gdddznaiy.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/glxrsjwhv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gnfechdsr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfupkqj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gegguikpq.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gxbzhaimy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gutxlynzp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghsxyyrwk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gduwftque.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmnattxen.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gmukbrvhg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/grmcyrzjh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gikeqxrtf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxatfzxtj.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqqnqwt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/ghndsptpc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gucattqxn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gehitiqfa.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/grxcknpyp.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grapqikta.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gzofwthei.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/grpylfywm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/givtbprmh.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gaderrkhd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/glqpecwqs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/guvnwcjxc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gjvjqycdw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gakhhkdyr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gfvygqgot.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/ghaukbqqg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/grrbgaytk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gdxgbecjc.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gcahmshua.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gaihcrnik.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gszhjxkot.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/guwmhldmm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gstbrenmb.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gynnyfgcr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gnaxmekii.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gkvhfplcg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/giftblalq.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkthppghj.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gkdyjhywn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gqxbynssi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gepkydidi.sHtML


<!-- 参考信息 -->