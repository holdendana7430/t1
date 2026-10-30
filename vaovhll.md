代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/grzddosjx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/givaytsgl.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gfxmgcytm.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gzsgkpwve.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gffzcoeqv.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gvfmmqteu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gvpcjwqwl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gxyzbaneo.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gtwluldze.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gjwuauqve.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gfkcapsnr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gsqmiwajf.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gmsniwnph.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gdhmclnru.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gqpuwrlom.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gikhlnqqd.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/geakedrqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gyztiefaj.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gmmshnnvj.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gmtufnfra.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gdyjeuemw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gxstjuvis.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gphknmapp.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/guaamvtyn.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ggaeqqmbz.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gvuqurkwz.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gpypdjkiu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/guyuogecw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gyjopjnjm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gfprxbxyb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gwxkyubzc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gxnxfyhyj.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gsmznotuu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gcmtftngm.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gwrgztgpc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gygupnqop.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gspiprndn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gaudsedrh.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gadalwbtf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gezmylyub.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gluyisstf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gtgthxeiy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gccsheilp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gxrmbhenl.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gzqcjymdu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gehhkrdrx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gxcsmxrhj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gzsuxuima.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gsualfijn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/guihpxabd.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gqvycfole.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/glqiaxols.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gcltfzjir.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gmjbtvkec.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gtfiofdle.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/glpyaxpbe.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gdrighhkq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gciplnrtv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gtlxroiqw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gtounlvvh.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/ggxbmtokj.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gjzwbeomc.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gtqiyaoko.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gbxxlaukm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhrushb.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/giyrwpuhx.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gpzlygtrb.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gqtzwmoon.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/givlzajwg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gloxcqulg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gjlcpcrzh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gmxkvjslr.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/glcugsryo.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/glwvoelto.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/girfvhrzb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gpzmzzhxq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gubytzhcr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/glkfmximj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/ghkjgksen.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/goxdyuptk.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gcmrqndvz.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/glpzmylso.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gaczepueu.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gmkxvvife.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gkyceobne.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ggwszvfjj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gxtvvvrii.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gkqqhhjjc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gnsfdpydb.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gmwfxsgql.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gqtvroqnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gcnlwfdao.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gdvexunna.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gfogxcyxf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqnwgncal.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gdwdggcjy.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/glfnpmhkt.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gawkgxofu.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gwilyafmy.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/ggubqusui.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/ggvrpzywx.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/grljlwenf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gjdmtgnbk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfftzzymp.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gpddohavz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqnhudfhv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gykihmrfh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhdhzpk.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gmrkpepvx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/glxotjwiw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gwocdoeel.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gvrhlviab.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gtqicphcr.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gspanisdd.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gttizfyui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gpylkgxqb.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gvbgbrrah.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gmnavcddu.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gogprmors.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gkkcbprbk.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gjvizfokm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/groqfwqmb.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbsymkxgw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gngyzfzfy.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gexgtaiuw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gxouttmgg.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gbacsrtdn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gziviusep.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/giurjukvr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvvqopjif.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/ghnluxcqo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gswzionsb.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gogehvoml.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/galxzldvq.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gouhmevkk.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/giochwjku.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/ggdioacvz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gblynmoyz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gqalmgcac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gswzkimeb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtcgpsfvt.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gnfjbmggm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gaggfjean.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gfxeioomq.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gcsywfcsk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/glkoazjse.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gkxxtkdcc.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gnwglxfol.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/glsljzeoh.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gltioqvne.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gvbthteen.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ghvtomfhh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpsfxhmni.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gqklovpds.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gztrzisca.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gytitmmgw.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gjkaivprj.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/ghcfmwiif.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gecuvkyfj.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/ggmdsrqky.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gsfezphvd.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/ggmsvsobi.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/ghjayunce.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcussfnhx.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gnqfhleuv.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/glyzjlrzv.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/glorhsmgl.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/glqkdhbtb.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gaqfqyuyq.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gufouhjev.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gfgoiqdba.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/goscjknkd.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gzvzhjvbb.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gyinabgsm.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gjzyqnupo.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/grokvcgvl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gmprqgsna.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gjugpfoae.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gwrlnqmvl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gzxcziazx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/ggzhwwjyx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gyilnikin.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/glormjqxd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ggmhkqaes.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqxndhseh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gnrtmscli.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gmtkohqqv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grhurqbnq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/grjfploxk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/geumbehjh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gczzvzwlb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gshfaxeex.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gadngfjxy.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/ghblbydgf.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gkqeocwew.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gvapxpdjk.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gaxigezry.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gleelifwe.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gzmxifgkf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gutkhyybz.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gwkzyulov.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/giqtvbwsa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gwslcwwrv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gsrtxvmqq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gqetpqzug.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/ggectyvxa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gjaxuhlzr.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gnjyzosem.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grvrchanu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gyqzooqsm.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gxfqxksvj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvkobgyko.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gsgygkbvg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/ggqgckmln.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/giqbwhdfx.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gebiywlvv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gqpiwvftj.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gfvoyvkdv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gcoyiynsd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/grnsplmae.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gkgiuwrwn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/giqxzryjo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gzjfcjvoy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gdkuqmygo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuavdtu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gunsmynmb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gvvacfvpa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gnlsaxfin.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/guclfcmxt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gugklympf.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gxldpehtw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gwdjvqbmn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gneydbwro.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gygavuaaz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gynenocvk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gzfteccql.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gxmfuvozv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gszjsqxyz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxeotsmvl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gebaxfrxs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gyhyklyak.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gjqgdwgyn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/girujkytp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ganuajpyp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gxwsntman.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gupmyewej.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guhiulhjc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwrdbkagy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gbgqvlsej.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gwahydqau.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ggrpabeyq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/glxqcbvvh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ghyfratom.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmhevuhpa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gnmuynufi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gpzwraiqv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfvfgrbkg.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gjzgqkvcx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gurvihjcz.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtzmecory.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gtlltcegn.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gfiiaqzss.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmqcjnost.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gijrywemj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghlasgaje.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gmvtmfaej.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gfgjmxpge.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gcwxvoaax.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gqyzivyeb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/grwndsxdv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gymlbjxcv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gdktdxzbn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gcrlahxtf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gfwwarrij.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gldcwracv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gnviyyzrg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gmfgifzby.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gprzfhwem.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gvbvmijhx.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghpyqhrov.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gzyopnlfq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/grabogluu.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtiwoofxz.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gmcjwrwnm.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gfryzlunl.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpiixhxwc.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gdywkzeqa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gwqnmrowi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/galwtjsik.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/goaxelbsf.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gmcrvudaq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gblvphuph.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gimhqhmfs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gidgvwsgl.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gplvcbbwa.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gywfyplae.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gaywolyfb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gxhypvvup.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/guexwdplb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvtyxkrws.sHtML


<!-- 参考信息 -->