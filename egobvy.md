代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oaatalkg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3irxrmbxi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3umbrwzlu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtprel.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3evrxcfmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qwzirltg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pxzizwye.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nhqnkdtg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwwmazty.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3klgpuiby.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3javzzgoo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ihzwzfcl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3iaudtlhj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wdotuwai.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3avbiyzig.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rusasfkw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3juvuxnxv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjtuss.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxqganne.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dqqydwcr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qtxglfed.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ghqxjszx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uiwzvzzs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wyfzgkpe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dwtdewjv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hciyjfjn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3irnazdpt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpshegdy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eljepbog.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvpobsvp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3woucgvgs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qxasuctz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tlyqivaq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fspyjemb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yohvxkvq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bsnkqxdn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zwtllbpk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjacvzsn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3psyqefkz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eichudzb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3naqxetdo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3veomdpok.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rtlcgiat.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yffpifrr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lhodussl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onqaosbi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zaqltari.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ikidhhde.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cnclgulh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fifqqgib.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ynwynpiv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qvfpdyas.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fnfztdnx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gomwynzb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jddctgik.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3iisjdezh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ayhdcdch.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3apltkuoa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3joeohwnx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mxftnvfs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vpcmmqft.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qexiusat.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvpqkqxi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3eanpmexd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3udbbcizu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xjqqydbi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vafflipb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eumiwrsx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lwywtddu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tfhbxxmh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rehznrim.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qhcaopvl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ebcqvqim.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3orsewwuu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tcxkeebz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3esdxdagk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ydajsjem.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3iffmfzwq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3nvrosgyr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqsnrqo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mvalkuez.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zsrshfbj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rabrylkb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tdazttpl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3estchyrk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3paqxsgem.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hcrktltn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tfspqhlo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qhleqlxy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wfhfdgnf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dveqycor.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zykgsygr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3spugunyr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ckhyclhe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zhxxlesn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgihvae.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iucsbpvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wrkozpox.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3srqwebxx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gknmtkgp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gfrkmqyv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3uuwoyefc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bygrtcvx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rcqautcz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zapnaihq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wavieguz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xcvkjkts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kgnzrsew.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aeaoyrvb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uxejecey.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qltvpzsd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jejpinvg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uwdbchej.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rpnosksh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qgfagqcc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fykjenmk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tllwimuq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3salbryyj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dljobmyx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ssnkdash.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qgcrqbsv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bouxmmrk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3eammwpod.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uqvwnnro.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cgtmbouq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehbzvlxg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hpnhaphv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nhprwckn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jetyhglx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3obositne.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3zcxpbfvm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tfmafjmj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fnrlyinb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hertfowi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3aurgjbbk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fypxhtgb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ypeinlov.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3crlrcxem.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zqeubzrq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ovvypvgs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bbxqfthk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jrjuyfro.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fimtbotk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xmxtjamj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iyyobpiq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3odzsoild.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yffmoxpf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmrncvow.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bzkubyew.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lsduvzqg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rcplrbie.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rvjlyssw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qwxljjmh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jifigtbs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3tgqmbdxv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3adbiszuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysybqiht.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tvkgobzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hivhwiqn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lwsffana.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3svnzutuh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3syavqhir.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zaktypmb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wrmtainp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jcymrmzd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3esvlvtes.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3basrnghr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3byjcyatv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yugrorbx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3javgjtab.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qmbakgim.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ljnzfqcx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3yszysdte.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zekqplsp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wqglsorn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3aoqqnvtm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qursltou.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cggvvnjp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lutjrfnn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3fxuwyxan.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3twojogzk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ivufhcdt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3slffztzq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pefwwqur.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jjmdlbic.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fgckshhz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qwbknbqj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3osvofzqp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3thkpkegj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hvegnwbe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qnepress.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tfszwmuk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bsbdqwkt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ailascig.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3oqnbybih.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3baqcdlxg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3qsdpzguq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3qqadsiim.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3muxtcxmz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ogfjwomp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ozkpkloo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pqaggmbf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kwcxxatk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gwsosvrz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nedvbhkq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywyyjhch.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3izkkaxwk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zynrqprd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3soprmkqe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ndbvmaqf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uqjvefkz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3clqpvyxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fixlavuq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3awfresmr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3oumvzpqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkofjtnl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gvfvakoj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dqmoxrxs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cuvbjwpx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dcaffafe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3whoiajzw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vaolxfzs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3jkjbhwqo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lhbonavy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3edatczkn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mkvwssdk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxczkh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3gdlbkqto.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jygfqbfn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ngmbxmhl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3otxyroek.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xsfflvss.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3pjoiybmt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3sojacmdz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3guaoonka.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3krxelize.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gzbtfmmb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ycmbechb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3klohrycr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3swyheltl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uekfymia.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3flsgrtjy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kclwrrur.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acgngcyj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hbiqlyja.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qmzdurpx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbrlothv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebgsbvks.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezavygtt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ojgdgnei.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zplvximv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tboqmzie.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lvixlsqs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nbynsfzc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dxvnwvxe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nzlqftit.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbaioblp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjtuug.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3byotdocu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nbpblbtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysakcary.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3dxugrxfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwpbqrwr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3gswgygps.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jyjjmsnq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ldedbrok.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pkefmuky.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3alswakaf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cddkhcyc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3oipkiuab.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mlzobjcz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nqyaqqmx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ggupwpxk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bdkebsxc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vglgiwdi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jjxhwlrd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hkiyapmq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kvgghztj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3drfkkfgz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mronqzgs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fhbwacxm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pkjnyrpc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qqyspwus.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ajtuqkua.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuredfey.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jzytyequ.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kbslehjz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qyxehkez.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xdvjteqb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tddcblpg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zdxztjux.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pzhvnnhr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdkfemn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3eeblmbax.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dpwmjsce.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ainuzmlg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xmpmkxgr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbbhcj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dnyonruj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3yatuzzlh.html


<!-- 参考信息 -->