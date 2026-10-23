代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mbqzfdwn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ixrhdtgw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tmorusyk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmmiqhi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tnukpkxj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jlggoyll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vcqmuzys.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pndrkysb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3icmbqkqw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lgysysfq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxdmbtgy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tgfxzcbg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fyztnwib.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjrqmvf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgoelene.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ljupovsj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fgwvihez.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3faaqonks.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lwmsecwb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3doiaarkp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sorascxm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fttxpyvm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxzltr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyuihkpi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3sicuxsey.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zbnlcwad.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kedqagot.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hmvfujga.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pphxdhrs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gghbnbvp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jpnyrjrn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tuifinbm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ecgyxbwv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdlepf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3frdufnem.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lugcnwgw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iqzwrgzv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ytmktogl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kjvqnvdm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pzkszacm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qxgrggeg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3anxbuizk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dtumnvwr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptrjqodt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gnxcmnrs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgcikkv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jusujref.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gdcmpebk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3grwlcdgd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jockolax.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gwlwhexq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3njnhjpil.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ggslhgor.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jafcuuux.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jvulmozc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhgrwxcw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ubfsuasw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhcwxn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hdfxbjbp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kpdqlszu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mfssqfan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3guvjhsxb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ivbqrwie.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hdexiqgj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bnzhysuk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3leqnschc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fifdrwja.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jzbrcjqg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dztaqjin.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oqnfbffd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3enxxjyrc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ypdwiybp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3hipfvkri.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kyxjhvir.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3anunczzb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pbvcwzfl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3arbtzxsf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sfkdjrkl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zcolwzra.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ilprlome.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3crctufsi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lcxrqbmp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fqhcclgf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ygpxxpgj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cralnvio.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lzzanqnh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3umkxxoze.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zgkyonds.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rgfsjjzc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jphqshwl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ycjonswl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3chtmuzpq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xxxmpgxv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dzvoulid.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fdjmqytd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3gnmxxmqu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kgeqrdrt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vcnhafqv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oyrpykio.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zuyedfes.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wngylajd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fodkjdrs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yoedyzdb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqhpfr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3laivvuxq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dvrkhkud.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3siwbrifs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vpohwfzl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ohzemjlz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3srzyatdb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ycqfmoix.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vhwvqyfe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nfwslgjt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gcziedxf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3weiqgels.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmtgulv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jopbreyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3todpinry.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3skxcqnsp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rlofwjhb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ryuomkqg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jasxrlgl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nilpjppl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdzkrlg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vtkrthqn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hdvsoyqz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gnoxkvee.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mulkmfjv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3huvdgevz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3svlneext.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vdssnajt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nkmcjpkj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wgltjjlv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uwifleiz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ludsczwf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qqkuwwft.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fbeqtncn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ikgckorj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zffuxofe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3azvwtegr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3agcuwnqn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fzbdwcrt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3droaawya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3swvaxaju.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zdphzral.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dtnwxrmf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ouocwxda.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qkxekpxn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzmxsr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3duxufnfg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nlbfbono.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xhnrkmqg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yxfwzsha.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hhtxobpy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vnkkahbf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lurqrqdh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qrljvugn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jomhsdhl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3suamlibm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3aegmpksx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3llopqufu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qcbvefnf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qbiawsos.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nuyfhfbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exmgdoay.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3eojnplye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecawaqom.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gyucpyds.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vboioane.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pxgalzlb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hbqwshok.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ysekjlgg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ylnabafw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3iscayckg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxxnywnr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ofvzpxzi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uqrqnedi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bbmumlvi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kbkvivbr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wwpuobxq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ymhnfozx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zabqndgw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lwqxbyoc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ezaqgief.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nlesaclw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cujexycl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wgqbzhth.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3okurwsal.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ejlzulpl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bvxrwrqm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3frymbhqj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3osyrkbgp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jdpskklz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yvewffjx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3unynqsoi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vgnkkjka.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3avqrlaqd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hmhpxwmn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hvwgeimw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnyfnwdw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mwygfogz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hggqzvap.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kwspxofo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3maydquln.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mzkpeapu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fixcgxmd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3txvquibk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eiycoolu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zqflwnqs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qzvdenva.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3poollpav.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uyfwujcv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fqqisveb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3veknunlc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nqvfglqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3snhihtau.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3nphnstpf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vmxxpaph.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xtlbukur.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3iqtaawqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zusmxxcy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3duwnazok.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3odwmppcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezdghhdf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3elxscpkl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzlyop.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3whveyhyf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3schrfaey.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ixwqokds.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gycsgqry.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rwhdhusx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qeqrrrcy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3llbdybee.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ycfrlecu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ahzldxgr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3lruscfpb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qphwvsne.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3wqewyipi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3lqadvuhj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zfpbfbtv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cttkglzc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pzapjmnm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mewncxbb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dljzauzu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ugkicfhh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vkawkyjd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mxqpxegm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pahayujx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yhiwfmum.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scevifln.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hbyqlsoh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3oduqthvk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3exnpgfhz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fmcudvkk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lmqsqydi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agxdokzx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iqnggica.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uaffvjqn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tglxiooq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axqsmbgz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qetnxjtg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3irazrwru.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmkbkucz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3aazhyugv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lgcdpdxn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rcsponwt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3drtdywbe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3puwmugmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gifzfwvs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwqbauni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oivnsdoa.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mtirpdjq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3knnzusbb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3sfyxtqwk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ftbehyww.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3aeirqfqt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zrzxfmou.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3alacthxe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hxfjnmfx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yesknxgg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wfyysdad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3lyuggsar.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uxcvfyca.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhpnoe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xkwsblac.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hqfgdjrt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3gdntmuri.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3sdjzszaf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kqsauffo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gwiazira.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mupfyclo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qvnvvnhr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yzpbkcgs.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jwwxhvaf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yhnutkhu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tvisrkyw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wkxfdrge.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nawcaabo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3achoybyd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3pwbwtiha.html


<!-- 参考信息 -->