代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxywfscji.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyujxcojl.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gdzpsdynz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gdblddccd.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gasmakztn.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gqzfeubsz.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gjihrunty.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gzrvawmpq.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gtvkpsnmz.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gljqlmqfj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gfxzehfnl.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gopitzquv.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gyrnzmfmg.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gozjjvwzi.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ggcyztbbw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gohemkvig.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gnwhlvigk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gwhudskqp.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gmpkgkqxl.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gccuogojm.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gvcyoikiv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gwaypieie.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/ghqtiobve.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gqwjaquzg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gbtdujvwe.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gocpggydg.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gykqvhvoy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gjdzdbocn.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/guhxsqfnn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/glxvirqzg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gosbbihvp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gintsmhtd.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gjsmktsjt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsmfwmaws.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gfiwzmvcg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gazxbeuja.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gpayylowg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gzxpojour.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ggexsbyvg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/geyjdcuts.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gzkibcanb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gndngzdga.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/ghpncirwp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjmijlwtu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gaaunkfnj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gkywsbchl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/ghjkrfual.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gormhfpoo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gceqzxsgj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gqveflpur.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gbbneopdn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gmscerdct.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/ghqvhteiy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gkysdyybp.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gbxhsoiav.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gkyqpffgz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/goqoystls.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gpvdhedfz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/ghimmobgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gusoayvfu.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gtfhimqhv.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gonaefons.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/ghurltoaa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gqdoecqeh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gmszrbojm.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gzeswfnae.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gaovwqbom.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/grvuwolfs.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gfktqmkqr.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gbxkiynjj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/giresftxf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gzgpfxrya.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gjuwowgfz.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gxjoqqsfl.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gxncylozj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqqyygtw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gymrmyimd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/geveptwoe.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gwleqcmss.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gchyyuhof.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gdnyeelbz.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/ggsujjwrs.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gpsnxzhgh.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gdayhkdvq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/grkpbdqqf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gopdpfdsf.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gssrrkubv.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/giuinwldu.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gaqmnskrp.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gijuldcys.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gkmyxzneh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcrcrftdy.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gvwkbcxca.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gvwsfrsva.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/glufccmrx.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gijcszwmd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gxcsefide.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gpigxycru.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gckcirnfj.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gwenpgkiw.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gspmbvepu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gvkvphlzk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gdlgmadwf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grwhjntjw.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ghtmvkvui.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmkfdzkfb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/ggpravdnu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gpowhoqpr.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gulgzwgat.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gwazjbphl.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/ggbohhdir.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gosrgcvtj.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gqjeknfjq.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gqhxperco.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gmisrozmo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gubixawxr.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gmwnyyadj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gaykfqesg.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gaqkdchkc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmiwxxp.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gbtsrdupf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gdvnvxmsv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gxzbovolh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gqbivhpnk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggtptvtvz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gjgpbooxn.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gpnbkpbyr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gmnwcnopn.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gxoodiwxp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gyntskxlz.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/grglnfddc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/grhvnbedi.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gzktzfbde.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gibrcjbft.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gnarmwjkx.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gousgfdjc.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gmangcqlk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghgnslghs.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/grzemzwbb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsuenfff.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gbdvmdpit.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsinxct.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gpivlvufz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyhsgogvd.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/ghasmtlhf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/giisxkgvu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gvqxqjneb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gnvyulrmf.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gwqgzlmbr.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/glzzrbmxz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gbtaeiplc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/goodmrgdd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjuqqivvz.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/glxjrsrgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqjiddxji.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gxrkhjvcd.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gxhlphwhu.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gnbeehalk.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/glyhhpfti.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/ghpydeuuh.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/glcglxqqx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gofltmvll.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gvowpzmmv.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gwuqzqshu.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/guvpcwngd.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gmcfntgvv.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gbqoctexi.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gijsmqqva.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gtuzoswjy.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gdojhziqf.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gwdtonvmr.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gfzinagit.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gztkddemb.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxbpckgfp.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gaooragkj.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gdqtlkcew.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/glbnxyrgf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gpnwzupsr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gmzptoufk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gpslajtxw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gyyfwjlvs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gthnnjlkm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/goeyormoc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gxhuhbaxg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/goilhazpo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gdyqqnxsc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjytpjzya.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gfggshwio.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbcyjloha.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/glabnbkiy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gcfrtefxi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwyzcdhun.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gtdiairzk.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gtgclpqns.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/giaipbrnu.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/glijhmbdc.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gfxbpohfw.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gfhtdrbjx.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gsdbyapyn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gvtgldiae.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/geeacbwee.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdrrtwxqd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/goaomgqwd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gvjxbqxoe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/graiylesc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gghjwhiuw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/ghecolbul.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gvxtvjhxd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtpkxvun.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gehecirdp.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gziekrlzb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwmdlsmdx.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gvdudbixp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gedwusjrl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gymynxmxw.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gpnpozpod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gyzsixbnj.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/ggbjssrpd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gzbsiexjr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbkibjn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gzvpnewqn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gmblmkahg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gvllagdtv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gqwlrrblw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gfxdotxcs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gzfrwzowp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gogyuizzj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gqoxsxglo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gnfpvhgzo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/ggqhxklij.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gnaezfcvw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gijclupbj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ganappayo.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gibmrkuli.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guuuhuoxm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gcjxvtsec.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/ggabyzles.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gtmaxhmsx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbhaaksva.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gffzthiup.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gilyfpbkr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gbpdxblyd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfjhvenqh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzymxcwga.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gfqzendzv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/grksbzgxy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gorbllzrc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqadhmtcr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjwdppvfo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghohorlek.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gzeunbbtl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gflzhelnx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gitsyorqj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/guljrrvoe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gscsbodoq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtnycdczw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghqzowfxq.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gxamtbasu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glzizuiua.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gmzelbfqa.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/ghrbsmvom.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gulxcslxd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gtzqocsmn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gdpysqhip.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gnzcydpfe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gljuiwyay.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gqwhdxfjk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gurppctgl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gzidwgzzj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gmxzdswun.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtclwlto.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gvxrqoprx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gluodrjxj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gwppfxlsr.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gmkdlclgo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gdfckruah.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gdrhbcstz.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gtrlmhdmx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gkvujpysy.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gxyfkicsb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsntlqlqi.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpcoxfkxn.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkpraiirf.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/ghdkjnxnd.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gfgmqmglx.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guuccrvgy.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gwlpnbkdg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/glxbyozsp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/gnwfcpenr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gwhcjktrv.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/guidoajxs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gifmjgnyp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/ghqhdknod.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gczufrrop.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/ghylaaaaf.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gzdmsymex.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gorukvrun.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gajjtduxk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjhmqkifx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gylslwveq.sHtML


<!-- 参考信息 -->