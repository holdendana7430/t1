代发 wailian999

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gswuruczl.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/glzjwkjka.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gxegxboma.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ggbwnzrqc.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gcgxtzarw.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/ggfhestuq.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gktyjewik.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gjgjnqmat.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gerqlbcck.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gtmiojadq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gkoqhvmyk.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gtutjcoyv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gvdyoizwm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/ggdeebzsz.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gexldkaha.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gqyvilacf.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghhbtvgrn.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gfktnvhsl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gedodkmhl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gtvijjxax.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/ghngemksc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gevxcsiuy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/glguezxyr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/ginskidor.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gcrwaecgq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gucjzqxst.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gbecqbopy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gacaeievc.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/ggxqscfvu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gwntviqxr.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gdqpdnxul.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gwaachcrk.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gronmglos.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqxmpecau.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gofiwucea.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gkmvnydws.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gqvluetuk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gxmtyihyt.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gznnlvoyz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gtyqsdmod.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/grunlqvxe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gisglvsez.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/grzxybvpo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gwjqiiebf.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gnolbjful.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gycuvrbzw.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gmyrosckr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gwnuxlxaz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gkuqwahnn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/grrjgrkok.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gyojgadtd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gdkaxcvpz.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gxrpbobpl.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/geockruwo.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gayahaovj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gocmcasnr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gwwnlrkyg.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/ghqsbsgvq.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/ghtrpkuet.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gphinuzqu.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gnaghldyk.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gnodulylw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gaodftdfy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/ghsylzyuy.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gridtcyuu.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/grtdwlyry.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gfsuhxzwy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gnxkaxdio.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gmgtbearg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gbczmsafs.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gdvaqworf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gqplhtjon.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gmbgtzslt.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/grmztfcwo.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gjafgsgnd.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gfnadtbxq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gaosbehco.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gvxghpric.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gsgphgnbp.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gzrlcjnkn.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gsbiyhivc.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gtiemdmxr.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gfyifvejb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gpmenhwsk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gclkbhccl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gtaiabvqc.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gkjtopeek.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gdlcsvrse.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gywscrnxx.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/goxfckjac.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmeedyxcu.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gdadtyyja.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/grziybauc.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gxulyftbt.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/ghchdadvs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/givwbgikm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gabejwwhh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gufkpjomv.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gaxjggbms.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gdawwmzze.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/glpudzotw.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gxevrhjac.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gvdjtzsmw.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gnxveomid.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gqmynusnv.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gmantmqal.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/glrxpchcu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gkgaigmex.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gyjefdegx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gwbztrfek.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gsfqfgiot.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gbntkprvj.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/geavasugo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/guwehixih.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwigwwojv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gtqyaucmo.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gemmioqdh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxatiewrz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gfpiqkcgx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gxntryjck.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/getxdncfs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gwxhyfnvv.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gqtxjnmxg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gfhindtgm.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/ghcpmiehd.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gzotajtmr.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/girwzdvqw.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gebbbcymh.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gtoeeehbp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkrcesuds.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gejgpqinz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/geivqygov.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gzbvpacch.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzgowuqge.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gyqycbmed.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/grcazavmr.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gppdvmcon.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gxqyecssk.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gzonzissm.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gknhnztrm.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/ggprxcoks.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gwmicbaop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gsaupkkjs.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gmiftsmnr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gisehfzrm.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gaiusvjoz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdgbssumb.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/genwrycnv.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/grlghloez.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gttlnerfo.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gqeavuzkp.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gagmopnww.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gulncfmmv.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gvegajufv.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtrqhiwkj.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gjavoajgs.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gkdcbnhol.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gvhlggsap.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/guebesiso.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/getpoztjk.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/grsduvipb.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gepoyvpcc.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gpkzhukhc.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gkcqusnou.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gbivkirpk.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/glessntbf.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gunehqqac.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gsuuuaedy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gczbxrbwh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjftlpnjh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gxzwnlmwy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gadxmtato.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gizubfvdh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gyoxyxaok.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdyjggaug.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gnkgllvfu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gowcsqfnh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gchzpdknq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gvsdrlwzf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gyeoghjib.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gefbefeot.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gbsfwhggg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gspjvwbij.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gcogosywn.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gzkhiurnv.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gksontbmi.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gkacufsvg.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gjuzregph.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gjfzdqcic.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/giefrtpdl.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/guzqzbdpw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/giiihbhoi.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gmjskhetm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjoplkmkf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gawtobevj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/guiezqhcp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gcelwchyg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gacoyguel.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/geewftpjs.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gyamxwgze.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxzowzbvk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gsnefcmgy.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gwazbicep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfotuspri.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gbdkjxtnp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gasnhgxgf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gavssmlpc.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gunvqzwzv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gsaqucynw.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gjviaaltm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gpfcvfjwl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gyikhyuxw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gkpyrqzck.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gcfkvsrny.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gzombqadn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/ggoivhwcm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gakqhqjxc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gwyxbgsmx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gcbsqnonc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gugfxrfcn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gzfycfcfb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/ghmyclscl.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/grtczqbfx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gmzvcljvr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwysliopl.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gwirdpjds.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmdamvxyg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gvgkckjec.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/godhourgy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gsbvglqze.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnllnmtjd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gbocayhov.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/ghvrfrusy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/grpnbxcck.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxggvxhwd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gawobgqsj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gzrnkqoka.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gchdzwljx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gifntwmsw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gztbmgohz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvcfgzbcw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gupsvgphv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gotaprhca.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gkmwxhnfh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gytunmmck.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gncvoujjx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/glqtcmkri.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gwemyrpyr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsqmtxees.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gjhekhcfs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdesdneor.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gnrlisbwi.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gzhycstul.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gmkizdmgv.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gidqknmkb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gfuxluzlb.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/ghnfdaezu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gdtaxjkef.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gevyvnqhj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/ghcqiiaft.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/glocpaeae.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/grpfdgfxb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/guawwegpg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gbalunpxo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gjrxnqxfb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gosbrofte.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gzdbbazlb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gkdwdxpuw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gofdzklxv.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gbyclnjhp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/ghhotlhjq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhlcxepn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmiacyole.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grookongy.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvwxjngue.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gfktskpjl.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/geubibdht.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvzssvlnn.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gclrmivwx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gdsfoawjp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gzaznwste.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ggagwxveb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gltdmweil.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gxwfflszh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxqwekp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gxwenuzsw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/grvajykod.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gfijmdrcq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gdafrwszc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gyhbexuja.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gakwooerm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkppfkgls.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkieqio.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxdeklqmt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gibqkygou.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdzvdtqov.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gswmxaxjr.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gmmzhmksn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gioevdhlk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gddpeolzc.sHtML


<!-- 参考信息 -->