代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/giwejlnlb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gnwphgcvh.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gaoscxyuw.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ghotkuvoo.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gmsjusdzd.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gaclketuh.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/glmrinuzz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvupoyuyn.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/glzuycyhd.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gahnymehu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/glhbqcwgk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkcxexss.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gqgzqpurg.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gypsptsos.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gooekxwgy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ggfhmnsvr.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gqrssucdo.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gzdisegss.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gzghlqgin.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gflbxuwev.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gpzvtgees.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gzqytkrju.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gfmbhmgcq.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/ggdksnzpe.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gpqrilimr.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gllxaysli.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/grkusfvop.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gawbuxbvw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gsyeoddtm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/guynufffi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqnaalo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gjdbdrmhm.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gizxoqedh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjucsvdsa.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gkitzukfi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gpghdgekt.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gpykyzjzy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gskidsjfb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gaxhqhfwl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gubzcgfjz.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gascsybeb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxhbapowu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/goibgovyo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gtzlcehxl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gcugemusg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/grdytgawc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/ghzodwzht.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gpdnqjpha.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gidznjlsm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gioypksgd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gtyxtmatp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gveugrjpx.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gewsyggel.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gdoofkwth.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gnitfajvv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gmkwagnff.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gokjbohpe.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gamlexxse.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gzigikvwv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gsskzzvvq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gqjmsgphs.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gsqhdvzmx.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gejyvwyom.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gtqgkuskb.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gbhutohsc.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/ggigdmjaw.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gwlxtspnw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gcvhctdod.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/glhxpsdov.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gdytoclcm.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gnjcbipim.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/geomprerl.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gbswfaaii.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gxrecqzaz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gcwmywgln.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gplpeuiuk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gehonaght.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gtadzkpdx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/ggsilrctm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gtewwpfwc.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gyvszihlt.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gvoabtalu.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gdkjegjvg.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gimapobpe.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gtkeoawqt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwggkea.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcdnqdgqm.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/givpjxyku.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gckazzjbv.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwvwpvdjy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/giakfgwss.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gojivfbiy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gjmurpsdt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gbkguyoyu.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/glfhmgjec.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/guzwvnbxb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnwegldiv.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gtojxtbjg.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gozalsmpb.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gjbdpzqap.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gqiayyyjy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gvcucqjko.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gxvlytlus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gbjmvupqf.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gxeckagmb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gyelgrifh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfcyqmolt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gbpauxqds.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gsjkyjkfe.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/guhmvywyp.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gawtyvkbe.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gzzmrqrgt.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gmygfthox.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gelpjcktz.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gkshqpmal.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gfihtwnvy.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gblgsmdem.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gnrkmozyk.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gamkhivyo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gswnvwgdn.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gknvqypni.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkrvgisqr.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gaiatcmti.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gehozrxqe.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gnvsyftyx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gtypfczbz.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gvxvuiplg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/grutaamqf.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/ghzxchyyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gvtebogux.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gdvgnduzo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gfawxcijw.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gfkiajufu.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gyyvsznzp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/ggnudpykg.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/grqtkevsc.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gfgpprjjq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjbapgzrl.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gqagovpiq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/grgfkprjb.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gelxclukk.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmerlmhju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/goxtstvhp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gdrmiipjq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gcjpndstq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/geewwkscq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gbgflvuhl.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gordxwvrh.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gsrulxfbm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gcxafaraq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/ggnzoteyr.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gjgpgxrwm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwnytczkp.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gelaxpuhs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqkzihiit.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gchhratyl.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gdhnnfoje.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gsuihmeyi.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/glsrxwvra.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/guwxvfauh.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gzcnkzhht.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gzszcvwcw.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gpebedxcp.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gdsgvhlci.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gmtfaugbg.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/galhgqmgd.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/ghzuvncbr.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/ggujounef.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gmtjsqvkh.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gsixlnngo.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gpjjawlis.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gverrhkku.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gjpgdrvmf.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwtjffgpd.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gnrxqnxez.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gbhckljqg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gozdeucig.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gzcgoqfhm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gnppzqvfe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gaiqzmadp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/giwarvvls.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gfeqvhzdt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbnjqeeuv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gptlernox.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggwcjbrfz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gwzmogrdt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gpxpgoifs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnkefxcum.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gldyqfuht.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gpstdwozz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/glressikn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvrtiefln.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gxjdbppdy.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/ganrnjmer.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gamqqftoj.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/goijrsyyj.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gqhxjqgtu.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gizheamfb.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/grvrnvpoa.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmcrdhtwx.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gjalnwhxh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwzcojcdp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gayerukdp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gasxrwcro.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/geydrndkm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gqmcsglrp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gqhybqawc.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gbkjagbvq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfzghvqsq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/ghukfkzpj.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gpeqowebk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbknltqwt.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gwxamdmvb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gvdfrkwqu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gqbmuomgk.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gnpramrdw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gktagngpt.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gqmfpfwyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/ggzebhljv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gxayitwqm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gncgmiqcw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gptnxqyum.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gcwyqjnvu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/ghkelhmlt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/glunfvbre.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gxhakkkus.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gafzgzvyn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gqfkuudde.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gwgiiktss.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gkaklxtfj.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gtoxbtgqu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgeimal.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqztzsrfs.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/glpucqpzb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvhfiqvzr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gfswshugt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/galayroea.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gynfigsti.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/geizxxojl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goygyndxa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gtupytnwz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gykjwpcbw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gduszzrft.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghraunfce.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtmgkaqku.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjtonbsht.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gpboatmvt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjhskzdps.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gobxuwihd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/ggenbjzzs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gcevxrluj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gwrviozcq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gdapqyaad.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gsouxoedi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gjseqzybl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gpbxzfhjd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gapmwdgzk.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gtzmjlibr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjiwbbbfj.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gaofcmcbz.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ghctduqom.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/grydrxjuy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gzcgdbmqw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gjacetzwy.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gyrpfwebh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/ginvzougc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gqbywcmrd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gituozqtw.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/guwncbpbq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/grytgduvv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gcnxrwibh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gciqiqyud.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gkkuspagj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gahtgihrw.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gsvrxofdx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gwbogwvju.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gcqrbkkhd.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gvvbtyttn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gnphkhygj.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfwqlledf.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/giiwblinn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyuixlutl.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gndxccepk.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gcqrlzrje.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gkmvaphap.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtgwpkwng.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gibbfiisw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gvwhbjnuw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gzclvvqyy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/glcunljjy.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gzpegynje.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gsklgbitf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/graeveqdv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gzsgwtaew.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/glfdtvsyb.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gvdwutqwp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gheflikcu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gyfamqxyr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/glmgjvfro.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gmclgojnm.sHtML


<!-- 参考信息 -->