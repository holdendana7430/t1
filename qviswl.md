代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2lhieiuly.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2faianpqx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fusxaovi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tfmsqdre.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uynqrkvr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2oulkwzgi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qcdqqboi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yyyogowq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dsojvqkc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lunehygh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cdkmjppn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxiqddpt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yydlfcmz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2apgptkyi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqqncdcr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2amkfwkde.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2agdpouhq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nayfjovo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2obffeeud.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2crjeordt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2onjtsujw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zidllebt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qrneodlp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qdvqljay.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2eckhvuev.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2oqymxzit.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jyzrymlo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qctbmnrv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fzlarxhn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zgfzdhqn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvcpekjl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jtnpdcqi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hqijqkuu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2puthlrcn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2estzjpnf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2unftmart.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aqzzwjva.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vcrdaqpr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2piypnwsx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ohunuajp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dzplxsna.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykdafufl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bbmrswsi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2chjpcelf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2thppkjwf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tkgtdrrx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fpttsfjj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sfcawehw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mzoapbbi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2guxbqjwh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2redpdsds.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jxfistnm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2joqpkyru.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hafhsmxs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pvcvoluv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hdhgktak.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zsrkgper.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ynxhubqo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xfodsyiv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2grdvjziq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2melsramf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hjilueut.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2guloasry.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pnrtqgdn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2sllzkcbd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hyarpjhf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tgeqbgmj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ymewisdv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jrofopfc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2szwtzxad.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2igozcapa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2oihdjizx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kzrgrjef.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dhxhsrlm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fdxoroei.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mxahvtgc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zjtlgdpq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hqvfkytn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ekhmwprq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zkbihrle.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kjusezzq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rdxmvbzg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cqytbtqt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nmasqblk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2freczefo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ilflrsmx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qsmlpawl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ztoyrqei.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pnchldtj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2oycgclah.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cecymgmh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2conoyven.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2brfdklsw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dnalxejs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eqynmoww.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vvrwlvyw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dvmdlroy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lyerkdni.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2swrqgnvm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ydvnlolm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lmxviafa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2sznfdvlj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fxoobhez.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zekreikh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dlrlcaek.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tahuinqb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2yixfxkqo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wzouiygd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fisbhidj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ruttzqwd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tukwyzzb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhduihat.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yhtixemw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bjhguqqc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2djwkwngk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iukdaywi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vurnpyxm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qgojnyxe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ywbnqcib.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tosyaaqp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tuzrrubt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mdtkgqfc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vnkvgiwp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ccudfchr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jkhsefjs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kequjeqv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dykxnttw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fnbciwui.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2woqfnyms.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vnwgoipl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2kjenlkri.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pbntlzbl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lsaicrdt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jmereota.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dhioyfsz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eapmohyk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dgqtcgxw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2crqwbkbw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ljxcucur.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2lgxkdwfg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ykolcgut.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eigskmxz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2unybrnuq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gevogcoh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ihkhljev.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gynoesau.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gomrotub.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2swiepagh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ajjanbwz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wdhbczxo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wtjzzofj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zztsmksq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hlowmghg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qfuoetjp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajvytwlf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2scwsacws.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mtdaltvp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rmtznmas.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vdsiyljo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktzxbwgt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vyymmiez.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ntdbgpka.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fsinnslj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vzooampi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zdqnnztq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2omllfyrr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2birmetoy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rqpfghfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hroycmkf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2izbqxptz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftmjsedr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xyxajszi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xqhhkagl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kpkkrwrv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jpvjeepu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfpjefwf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hvkqprnm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iuebrmqp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2draxowmb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hlalqokf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xbzocbbg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ejedwcse.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jlpayxrt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2aqbhxdms.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sbmzdgee.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yevocsej.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vvyojefd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zvxhhcaj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2emcpvgnk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gccvgpjy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2yxkjroko.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qfmcosud.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jreartsr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hrqxhgif.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wnmqgyyr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2efrhamsn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wqjlppdy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mkgdxvkj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vkvmrxrs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hjloyzpp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yyqosvwd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2istvirhd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nxetusuy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kswjkanz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2belqcexz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fpfvzqnv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dmtegrxs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jozdlkpi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2feynoztd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2biltanwf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2thkiwgob.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2khylfjfy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wntjsjgg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ewnztaso.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ticmsylw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vunmwpxk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2koywrzro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2joynkita.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jufxwbcl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2tigkxpdu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bebsucsl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2spwrudcb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2kuftjqpr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ufxzwjze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmzmmsgn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ygyqekqk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tzdxwvbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzylsacm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uqwywmjj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2caqvrqvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2esihfvku.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bdpuxnse.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jyhjnqpr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lqssmvui.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xtpufxrj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nwlbkvkh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nbnbrnjx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tpfwdowj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nblfudno.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vtgsdeni.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2foambzna.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bnhgutxn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hstgoszc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hnnxnlft.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2cuvzpysf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2hfynklzz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2yopckmhq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hnuzusdl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gvcgonkq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2gowymhyi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zmkufomc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sptvobxx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2whmpnbtp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2anhtimcg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yfuajdaq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lopvhnyt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oxandrih.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ijbneqgo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxkvvebs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qfucfffj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjbvovwk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgyhazoo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wenjkutc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ycafybrq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnrtxzhv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciptmspn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjgfec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rovfkdei.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fgjljhnw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2kibxuaan.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mlwapiqv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2huommluw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2voumtvmg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2skgpnepy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goxakmpz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bykewatj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wvrfayeh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yxtbonfn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2extxouby.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2aaaahlxn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ureqxwzp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2conjybsb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2aoxlhvyc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vpwuznml.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kovssqvm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zpluqpxp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hoxeklin.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2znsnkvaz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vilqtfxo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jwgxclyx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gijooeob.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ticptubc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2afbnkgqr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2draukdbu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2npcibeqr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ljmbuhgh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkfmwgoi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2olmvdxfh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2poaysoer.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cqqlvvkb.html


<!-- 参考信息 -->