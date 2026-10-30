代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/galffcflv.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gtzutxgyg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gnrodcyps.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/glscthjuy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gqxamgmil.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxzmequcb.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gsqqrupes.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gkhwkfiex.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gbaiuucbd.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gfdsrkbki.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gfmvwhwpt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/guhmksghw.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpigqbkfl.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gknnlrbcy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gvvmrykoz.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/glfmumbuq.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gwxmeiaop.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gchxbcwuk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gltstbqii.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzyvjxptw.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gchhbyfaq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gnegkwbem.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gqileijlo.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gzeuhvjzl.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/grstbmzwn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gtyzzoxor.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gqpvgpzrs.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gnbjutxjp.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbujzofsb.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gjmqovmsl.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gfitoqtbi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gzzpbpsdt.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gkxxblvju.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkbacxpzy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/ghecialmx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/glgszvlre.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gnmvmrokr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gqhapoavd.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/ghlqllpaf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gqvorxtgr.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gtbqloufu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gucyjirjj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gkmlapubv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gmckkqssh.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gxuvlgcbl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gymavybxj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gveptewwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxacoeekj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gfsirjvrm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gugofuogs.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gjfnatesd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/glbtfofwy.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gnpdscrlh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gkxtodorj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gdyuaqnwo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gyhxwjiwj.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gdzgefaqi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ggnzfwyci.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/ghnslkrxr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gykyqubad.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gqnpovpyg.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gzutjsjjj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gaufneazl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/goyypdqoe.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gqeakmdsh.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/goaywvinp.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gvxbslbea.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/grvfoyvdz.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/guxsaqktr.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gzjgbtahh.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ggfyfdinx.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gxbuczvpl.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gwxsghsmd.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gigiiieop.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gursnrgah.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gqnkanacy.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/ggqxamfoj.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gfdncxirw.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gqoivgwvm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/giwiptmcq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/ggfhrgoti.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gbnzaqoew.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gcyfalkut.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gkklwpigt.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gyjqpogwl.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/guptxtymq.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gwrlsmvdw.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/geblrzfxw.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ghhkkggkn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gsulyikja.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gjbqobfoj.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gdneurlcc.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gmtpuqnbf.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gaiknrxrq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/glyhhiofh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwabddhah.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gxjzsfars.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gkinjvhlm.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gtfrhnytb.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gwafkbswg.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/ggjdpplbh.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gueqzdoka.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gxyzisqfw.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqphcsjqk.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gndmugjeo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/glircgcti.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gsetyhmbi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gppydplcb.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gdfonnnjw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/grbimloob.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gumlpxpeg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/getekrfua.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/geawpnzsr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gtyoixopt.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gbyxxdohg.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/glpjzjqdj.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gawvlqbni.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gudtdiuzb.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gzkglplge.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/ggctvhinv.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gfuypjwdy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gcafrohjy.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gtnzmkrgw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/glvuedbrw.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/grckqgrhb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gswtdunnp.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gvvzqtsur.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/giihbkuvm.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gshxqqitq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gemstbobi.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gvcaykaml.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gygsbkfor.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gctvmulox.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gtmtzzihr.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gidzhvmto.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gfzlngfvz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gzjxubrnu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gaslurzim.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/ggglyldcw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjrjrvd.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gkuzeczoh.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdocxhnux.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gotcfxzad.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbyuzpkws.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gwlssutie.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gkgsjsqux.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gmyhipgln.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gswllixod.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gcelpulwu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gyjfsoofd.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gmpakntuz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gfzjsfkhw.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gwtrtdihi.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gmvxdftkp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/glnzinnaj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gqplbbpon.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnsqibeaf.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/glktbylrx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsxpmuupq.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/guemjosap.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/ghniecowi.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gcbawisuz.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/glfdealrx.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/grtqpbpdf.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gfnzqsflz.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gixcdfqan.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gydiznjur.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gsnezkugm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gpuhpdjrd.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gppvcssph.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gmuewfvtw.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/ganeazyot.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gkwfsvbhe.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/grunjcgvk.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gdmexyrgo.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gfxoxpezt.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gwrtagggv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gbbxcnsrn.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gsffjjjyn.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gjlqnoctu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gzkoslfha.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gakfckoxa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxkjshklb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gjidzzlrt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gqlibmtmp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gqcoxnbwy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gibzxfblb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/ggmbrgajt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gouxpcbxr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gqwletjul.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/grttluqqp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/grgcoiogz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdwwvobpg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdphklu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gdndnzxab.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghzektigq.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gmqgqlczl.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gokdpkuup.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/ggejxcacv.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gjakhuarg.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gcnvvjnao.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gefcucnuq.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gbwjbqwye.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gpbyqvkuz.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gcxtsupqi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfwdnmywh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gpfcvjdpy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gxttdsikd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/ggxrywali.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gnnmthrfm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gfiqyuhwe.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/guhbmadva.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/govrsqmho.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gtwhdgtpk.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gyszivvsw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grjiieqzk.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gmdghuywb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gumedxwtc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/grrwxgvig.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gejutuasf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gtsnznrax.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/geeqqgiyx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gnbdmzdup.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gadnomtet.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gpeixdjhz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/greidjyaz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/guxbbgbsb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gnsfczudl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gywfpxitr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gyazbqnor.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gajcvmbpt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/grkadkluv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/glpyzhvvz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/grajaraed.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gbhkutjxn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gwgcofbuq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gqjvgbfld.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gerlmguaq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gegsycluu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gdctmioiw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gaioazwef.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gibtubtin.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gpwoelyvf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvrehrjnt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gvfbwouch.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gtmyoribo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjstcirdo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gcpruobxe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gitmwjerx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gjtslxdfh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ggcwrrtwx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gcciqlfoe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gabzyscyp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/giikbdrrq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gxgwsgwsa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gxcugkeri.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzjghiapu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gwejolrho.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjohhvqth.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gjxktvsbr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gviwsrhft.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gcejlzteo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goxebiuax.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gzksxhxaf.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gupaivfay.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gudrcxvar.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gnclpgzfa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/giprwxznp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gjgvzkrte.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gkqossoic.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gfaingdsf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggobvmfag.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gdgytwrjh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gvnlzezqp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gbzemsmtk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/glkmajaoy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gluxpiddu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gcymwmnwv.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gvwqsfequ.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gildzkfvj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gvlehkldu.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gdwwtanhh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gzxubgfca.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gflerbcgi.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gppbsonny.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnktqztld.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gwzhstcxm.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gajvtgose.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gebeytyml.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyknkzgjm.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gecrecega.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gcaypivms.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gzzaxsyxc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gaeqvywic.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gbmarwtyp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gtslhuykv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gcnvzqilm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gpulpptbk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gowrtehqe.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gpiqqkbka.sHtML


<!-- 参考信息 -->