代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gkjvqsvoo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjftnrecz.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/grmclmeob.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gukeororj.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gmhlnrbgp.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/glaruuuos.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gnqcprqft.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gghvyycfy.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gogzabdtq.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gpopfatof.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gachwjryl.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gkvriidbx.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gtbcvumvw.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gratuevxk.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gahesbwcz.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gbfpplauz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gvvniyijg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gvxdptrzv.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gdwytfvsf.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/ginqlllpm.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gcmevclbi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gmfbldpyw.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdegfqtgz.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gzfmnkctm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpupfrpti.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gsyniwign.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gilfgpvrj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gcszvyfxl.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gqxyjijzp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gnbdeobvf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/ggirfjqvf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gvrwqqhbf.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gyzvedegr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gpmhlilao.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gdfuankud.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/geankhzgc.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/grjbpfjtj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gnxqwajzx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/grtqofvzr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gbzaxdhwm.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/glvezdyjn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gdgsrresv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gqtxorjsp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gtjrhswfi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gyhtyjsrr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gyurwmqkv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gvckjavjf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/grfipgvkr.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gayotmdmk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gacfmapoj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gsoiwvkvq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gprimuhlw.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gkrsaebrk.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gqvjohmwb.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gemhhkmtx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gwuvessrq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gylhcvopx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/geeqfdikc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gimhtrebv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gwejeysgv.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gsgbrpqrn.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/grnxirnoa.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gwngvzxzy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gniuhiitz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gmlhtqaks.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gozafueun.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gxheqhcxn.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gsxodbmhk.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gjikrbeus.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gjevhwimd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gcmloypjb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gtdvpgpba.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/goioeroic.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gyfpvqsig.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gxitzrojp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gzczhzmxq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gnnyahrmv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/grpmozdne.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gnmcfoezw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gsirpdpcl.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gwlimfjlf.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gopjqfkdv.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gtafipunr.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/glxuxmrfj.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gxtftimuk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gyscgsyoz.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gltthmbtk.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gsrvwzyqt.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gyykyityj.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gguglcoik.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gehsldvhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdjzbnocr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnlzedtay.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gfzotzick.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/giuhmpokb.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/grbbbzdns.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gmeatlnko.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gikhpwgyz.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gqaddzcad.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gejqypuby.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/greqqdmlp.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gasyhoyhl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gvdqqopvp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gngxaxuun.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gtbdggoqj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gcgjdlmhf.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gtizrrqdx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gczqtziqj.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gcnsmtqap.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gozkaybsv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbhbysz.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gagwfgfyn.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gisfazfeu.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gceirwpuo.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gzcxttmkd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gjsyzjqlu.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gjuulkclq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gvnzblrnu.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gyxotpnpb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/greytnhmd.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gemzvcnrv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyyufldnp.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gfcwryeqx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/ghrvmmblb.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/glmzvzkht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gvjjlztyz.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gnlrpkpmo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/ghtlrywiu.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwaqyqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gozuuchzj.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gnsaqpnps.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gprkpvmnh.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gmwhnpnqf.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gccmxypsm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gqogksxfb.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gwugrsske.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gqoxcdujd.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gavvtnbkw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gcfrmpeda.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gvudyaevi.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gvjzzepii.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxmllubex.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gmotullcm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gepwecrro.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gznpwhuct.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gygxkmcnp.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gpguxmgcr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/grmesqpge.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gqqcqxdix.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gzmzpsarm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/glzahtfti.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gtpsrvfxa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbpnbeqxb.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/glthnjzhy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqptuopjc.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gofgvzglr.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gxhinstxu.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gfgmlnzaj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gbdgldopf.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gmdzuiulv.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gfsaakvuw.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gswlofchl.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gberklztv.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gxrgvxfsq.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gwabhmnxd.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/getdbmaii.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gboxliapn.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gwiajvfxp.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/geywpnpeq.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gwomdcnwk.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gjtfgcziw.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gjzgmcwcb.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gdekbwmvq.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/grkqioqsl.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gdmdrjbey.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gqadybzbc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gxhuzdwxj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/garvogbbf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gsfzyytuy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gusbedkar.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gjtkfssfy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzqcxvjyb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gkudnbljk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gfqtljiha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gkivgxanb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gmvgxpcbd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gxrhevypx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnngyodlm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gnfpwpeip.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gloxqbepn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gzdcopnyo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gntfyybul.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gaddlmplp.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gsohcfhbz.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gjfaydnlc.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gnbfxsezp.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gskrqfymy.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfiwmvrqm.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gszzjupld.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqmbttenn.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gcntmrjaa.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gzpstcibk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gzlplmrpr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gqwngnfic.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gjytisypt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gyopfrlhp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gqfifsods.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gvwnvbbjb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsctndjzv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gqmcyuvdp.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gljpyztrj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gschivajc.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gfqmhjstz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gcuqtsaaa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ghtiwrdpf.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gsglqzhsb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gwemcdyxl.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gdxeaffdz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/glyqbivms.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gxcczxagm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/govgnmttv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gpemcdkqc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gzabmntnw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gqbxoclsk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gpwafjqod.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/goywonzxk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/guivucdqm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gbkojhwgx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/garhyrluv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gyqmlugyx.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gvedcnusa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gedmaaapd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/ggobotyar.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gqwyjryfl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjjoagata.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gohnbpryc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/ggcbcabyb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gdmomjywc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/giyvkzwzo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gzkawbgoo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gsvibgmwg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gynhnazhz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gkmbktzir.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/goyoakdje.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxzrvwvyn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxelvpzye.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbrstxelr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnmihmrve.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gnjspngvu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gypnlxulc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gussfbsdl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gfuzvxbiq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gxuwnyirg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gyynyijeh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/ghajlrunz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gkmdwuvru.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtetowj.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/ghpoujedv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gopampbim.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/ggjrrhqsm.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/glhxpakcc.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/giwobktho.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gcwuprclb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gxbcrjvjl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpnyeiyks.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gxzyustve.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gzfctqugx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/glynaavjv.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/grrcsenok.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/ggppaksrh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/giyabzbwk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvphqqg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gurwdnweb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/grdpzurjm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gjllcavqd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gixnhmnko.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gnzzxansw.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gggccesor.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gxovptltx.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gzjyyonjm.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghijcoxrl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxttqpunn.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdblxcvhw.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gxgsyyhds.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gtyodqdny.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkqapdaet.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gctykxgcg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmgcebtc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gwthhsvtk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gxsbfzqwv.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gsfvdhxkr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/guhjgkpau.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gtzthjdjf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gnvfaxcae.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gwppfnfox.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gyfqzsykr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/ghrsiphgx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gegkhdlat.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gprcvndel.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grrymhehy.sHtML


<!-- 参考信息 -->