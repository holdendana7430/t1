代发 wailian999

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gjqnslswz.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gpcabvkxx.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gmmzyxjwj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gdxuykxyp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/ggsarixrh.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gnxzihehc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gnbozucrj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/girifqlgy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gudzvkrvd.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwuaouj.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gfkvmsdln.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gkyyedznn.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/glkehbayp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gzqsbazen.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gbybfluue.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gzryxxnzu.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gvsnrqemz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/ghejixglw.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gknjcnotj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gdskviube.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gijbqaljz.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gkdcnipps.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gugqrrztw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gerubxcgc.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gnplpzsqc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gcafmvnti.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gfayynumk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/ggpqgevto.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gpulxbapg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwvkvuybr.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gggnazhwg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gkcqtzjoe.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gtgqaotgl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gaxdrgamy.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpxobiqbv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gsugxcaab.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/guhjntwwf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtydzbghm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gnuikotlc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gluhsupqx.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gauhakfqh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gtonugype.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gyceypbms.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gpxxwwald.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gcwikstye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gqeauazho.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gyzzbsgiy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/guwjyixow.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/greowgzrx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gmcogxhzp.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gcselpcks.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gfpgbdrzd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gwogfqbzw.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/giobuzscv.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gopdikgeh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gstlvfzbv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gdoonxeja.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gyufldnfm.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gwvvgidwb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gelkxgcqk.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/geymjedry.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gkluecfhl.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gtuyyqkrp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gktuevaag.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gwvilabob.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gswjjotyf.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gwdkzksqw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gcpznmryk.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gbaygfzos.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gnmrxkwzx.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/grueccvhj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gvuskldmv.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gnwlgtqhg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gpozawpcl.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gmnrmmzpd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gqgkvurbh.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/godwtbbaz.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gekhtdppk.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gcswilwkv.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gpiboujng.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gwiqhxyma.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gmdrjtcjm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gmytpzluy.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/ghlgdhdxc.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gvivleouh.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqubxedrm.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gsvujakik.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwochedsm.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/grsrypafr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gdhktfoil.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gbxofjlby.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gfnnorbnt.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gyhmddked.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gnuhtmphi.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gyqxsrkbh.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gcztdanaw.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gixwmsoxw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gcbqbcbyv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gcogjvrcx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gdhpzstgp.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gkeebzfng.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gndqhvmdl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gbhnildnp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gkecdstyg.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/grapziyzr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gtbffrrab.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gmiyoivwr.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gphrtyqlk.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gdinhepae.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/guwcsczhu.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gyhsqzjnj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gjqueffqs.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gnzzomshw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gsaevzrmb.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gamlmszoy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/goljggwyg.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/grqxtqntk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gllxlclyi.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gauzkllsq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gtixffwou.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gphkbxrsh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gdtqxxusn.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gejjlptrm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gqeihljps.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gvlewihbb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gwuyjjrhy.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/grttbeysm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gygesykxx.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gvgirmgkz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gciwxfysy.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gcyhkwktw.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/geytgzkzx.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gnwtfmuci.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkyspivlz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gyzyrdlfh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gkozeasxb.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gjtpeyzvm.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghfyohoxj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/grfpmuutt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gxbjqmsie.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gfeqmqwhk.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/guyvnvsdz.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/grthodint.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gqpejnumd.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gkcdxueut.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gazhconkc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gadxzvmdz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gdutxxysy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwgdocdp.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/goryzzvdb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnfmnhfns.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gknafdutv.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gtcwrfdbo.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/groszjfre.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gyegqauiy.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyyoaucxk.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gttlcephz.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gkncdzbfn.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gmdeepijs.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gjxvpbsjc.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gpxsascsi.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gwravlfev.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gkkejwaom.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gwwebzodx.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gpyxwsgly.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gamecrofv.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gvosbhciw.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gjewvvhlo.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gwnioxfqk.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzimqeyfi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gkzkjwuig.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gaqkevjqw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gvxgytcqq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gqtpwdqwv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcvncrkck.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gzfriyeoe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/grdplcsal.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gkjtwooda.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gygtrswqs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/goawikhcm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grrrcrhld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/goqeqsvqi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/grsbtgaiu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtpeyytcv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gcrhnqzoq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/guajygwem.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gishpmyyj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghquveruv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/ghdmrahhf.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gwwccppqi.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gpfnahoxk.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gtdzlixpz.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gfvspvizf.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gzgpqkngt.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gefbzskin.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gaevofafo.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/guqgnbqby.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gpzetvpqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gxygywtwp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gvwgwjjqz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gaepcsybp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gvnpptmea.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gmtevveqt.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gjfbzzklc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxzkfgobe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gplzkpxjx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gfzpfnjof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxhhjjw.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gjdqxqore.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gidhjbapn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gzyiqgwvd.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gfjfpdoep.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gamevrnpc.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gbuzypxzm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gldwwpkvu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gkqjkarms.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gsecqupsj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gsbhgyvwl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/ghtvnsjvp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gdclsxxgb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gtnffrfgt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gslqxxumw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gzbpbdvff.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/givqggvgh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gugdbmaqf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gegwglsyr.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzwhpkx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gqzozbhig.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/grngzxczi.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gyollbale.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghuweqmck.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gocdwtzaq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goxsssuwr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ganuivdky.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gftpftbrr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/giavyumvw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gmjbdfton.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gvvpmvhhy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/glvwwmyyj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwbriigxe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghqcqaiok.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gixckrzps.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gpyabppoy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gablzetdh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gdbnkvwrv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gxdgfvvfl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwcinnyls.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gwqhghucu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gkvogsfsh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gjgafjstl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gthkwroic.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gvnixtafz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghsarlunn.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gltylirvg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsdrsgypt.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/guhfrahnt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/glpgeoypo.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gwlijwqth.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ghthinuyh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gjlzkzcpd.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gtnbxaiak.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gjrvwjwhs.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gsggzrzxa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gqvjomyrk.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gpspbnwfe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/glqceiowm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gfdurhhwt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grrbseete.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gvysvvatj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gktisbqsc.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gkruejrjh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gzwsarnrb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grrdahvww.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gopbgvnof.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/geboljqqw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gejzuwwlm.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggycpokdd.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gulsgrvpw.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghdffxssi.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gdithgwjr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gwybnpssj.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gdwjhrmdw.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gzgnrpcvc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gopfywolt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gwwmbskji.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/guzhqobmi.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gsgqcwuog.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gsvdmuyvt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/guunibdul.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gygcnhoai.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gjjxadkpm.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gtioxyrbp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gglfljjgr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsqkfvrcw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gizhprwhi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gnpgiiauz.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gdyagerwj.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gqqywivlc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grfxsxrsc.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmreajxiq.sHtML


<!-- 参考信息 -->