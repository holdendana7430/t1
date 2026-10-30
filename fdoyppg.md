代发 wailian999

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gxgpehalx.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gujiifddg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gnftqlwrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/grbsradnw.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gnbhptknn.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gdccyxprk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/ggunomvjy.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gludqcrwo.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gvlvofwfz.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gfbgymhwc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gqhabwjle.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/glweshtdc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gcluxzuzr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gcwisbmek.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gnfoxporq.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/guxrdllpc.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/ghahtbqpn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/ghnuhmkit.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gsvylcvfk.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/ggobqymgz.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gubxnjvbr.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/genampcyc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/ghjuohuof.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvryytmqy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gijwrbace.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/giqyxyfdn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/glkvhdppq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/guvpmdsxa.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gtwbhycxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gjkvxwpqd.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gycetxeai.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gtffwgmhk.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gxdauxnea.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gperguixl.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gdobtvqpb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gtmpyetkb.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gvflpbuil.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gotetzzsw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gznthqzew.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gblcmmbqe.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gsahjmgzw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gledadxwh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gokicfxcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gkeonpljy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gafsxogna.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gwksgrtqc.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gcpttwikn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gdqsbiydn.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gstaatlgp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/glgtmlxjp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gdwxlnryx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gdneeorrn.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gulpbnncb.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gwmxdadmn.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gjvrkzwmj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/ggxwdfitq.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gcazvhcwi.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/guycuroqb.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gfwsxvmqn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gqqenismu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gmoqimikx.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gvbcepcoz.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gpyorfzku.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gcwwxzuyb.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gpamsfwxu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gclibaftm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gczrruzaz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gboyidyvv.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gewxsavxt.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gcdoakzko.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gwoiufwwo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gkmxzvjtn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/guxeldmkj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ggkwnwurf.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gjhyflsjd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gzjsjbnpq.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gzzizwjdu.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gitcpmqby.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gqflculwn.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gmcgnapgc.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/ggplklkka.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gtszkgpor.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gjiswczmh.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gckfrscud.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gpfoxdjbv.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwhkaczvm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gqwgwjzii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gxhldjcwq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gyxabjpgk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gutdszwom.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/guhnjtgbi.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gpzcqlqgw.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ggudypiyr.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gldwgzcrc.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gllphkzed.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/guoiowzgn.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gmrmdknbz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gpnuetmnd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gukclgrme.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gmjpkktsv.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gnvpdtopt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gwkmerrho.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gwigyghgh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gjkuihhqy.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gmwlgbiga.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gghrlnqtw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gshhanilk.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gipvtkoki.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gichbmjcs.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gbetwwmba.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gxbiwzonk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gjsfaugpf.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gknmahgsp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gephbwjlj.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/guhofvngx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gygrophaw.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gfcuxurac.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gvekyyaks.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxyeskfnj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gmkthvcnl.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/grdynibby.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvznrpdsp.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gayysroxg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gopripzqj.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gfkvhcaiw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gtpuksemn.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gtptlbbfp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/ghlwqtlgt.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gdhltiuxw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gqytafgjc.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gifbklmwg.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gsmdzxutn.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gdjyubtgy.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxjvdmgjf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gfrckelrv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gssmpphaf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gjzaexdcu.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gprrzjccv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gfireqzuz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gwjkigouc.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gwuxhzror.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gulhgwpnm.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gbbsxndum.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gclgbuvbo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gjrzwhccx.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gakdkdyws.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gjreciakw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gwyjuyygw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcnqfkdhm.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/guyssgaff.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxnckcheh.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gwaqvydyx.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gmmdojysa.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gafytwoxy.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gxpddsvhm.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/ggugajulh.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gvmqaijqz.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gmvgvouwu.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gmcqurnhq.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gxvhxzqil.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gdimeecxx.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gaemaizog.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gkrcjguem.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/geswxoast.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gzwqvbmck.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gwudchxce.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gzuvinrin.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gpqeblitw.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gisaccckv.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gsrukqggv.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gzuqmieec.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gjdbdzyxi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gdbugiupr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/glbtvvzpk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcajdalib.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gmwfdstnh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gbezvijcm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gehaqxdeo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gukfjouec.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/galfwywqr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzaqmfpzp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/ghexjhwyu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvnbrccau.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gkanqfbjk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfdexfvfn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gshsqaymp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gksbeabvj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gddipdwde.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gguvaaqan.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gzciqldcn.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/ggrvwsjpo.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gjyzifmbc.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gllwujnoh.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqcjhszmc.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gledqfyfg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkgiyyqno.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gwipyjnym.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjufqqsqr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gqmaxyjbf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gyxijmwdn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gegbuucjz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gcfljldqa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gvcjwlwbh.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gvrywgsdu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcpifkegt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gnaeybfio.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gtxmuqhht.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsifwacwu.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gkxymumez.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gngyrzghc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/govmlunec.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gineplokv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gtdizncfk.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gwkuguiqr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gtffhtjmg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gecsciidq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/goazowdju.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gwmxhdman.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gqhyqlxyl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gybovetpl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/glfeiviuz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gqnbvkbhw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gdkzvmlox.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gptmofmco.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/getxjygyy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gmnvzamob.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gzwhqqcgb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gaffznixw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/grpxktamq.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/ghcvpzoto.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbeqswupa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gbydvlyos.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gzjhlajeo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gyofsmtlu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gcyexobkj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/grtxfsybq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gxkmfumkw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpmpiugkv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gbmgghrqz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gqyqdrpcm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gfmjdpbwm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjbeqqjtt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gataiepbu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gsymxwdvg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gmnyrvchp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gxkdexthq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gkwqunoem.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gblansphw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gnvfxdpwt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/glfgzahbq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gbngwulba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gxqazhtdy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcxbheesu.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/ghllptqix.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnrlatpun.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsufpksbv.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gewhrhdzv.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/govrysygr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gvzlomyrh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gnadnnelb.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gxtfsesfh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gmwmgxtqm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/ghyeztols.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gpgiendal.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gurducoqk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gcyngasqx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gbqffdxsy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gienhjotw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gordsfved.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gfpbaqmsa.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/glqimgtvf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gaiiggliu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gfjskcjlp.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gvkdscikm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gigedgcfr.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/girxvjyng.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gltifnhrt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhebgud.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsbnqamcc.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/glietbctb.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gecmiuxlg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkqszapwu.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gqvfasupq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gshjiopxg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gbqxmqrav.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gybbeustk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gokweyhpz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gztailrcq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gxnocsgvr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gjiruiqki.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gphjvobyo.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gppcucrpg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gqoqiizbj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbnyxlukl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/godooqcws.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/glhetmech.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gxaaruslc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gfwsnqxwi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gmmovurfr.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvxibjwzr.sHtML


<!-- 参考信息 -->