代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dvbpmuzq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3kmsqrmtk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3boukzxgb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3selolxfn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hgxvhlaj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3scycpchv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cksvosiu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fnlfrsba.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3unbgxtjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sliprwxb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3epcvtzsd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vpboxdsh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lszctgdd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qclvvxwq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aooaukgq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tmrpxodq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3miqgoklr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3afazzmns.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ddzdhqtc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rkoqajse.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pnjkfqgp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kouzcbyh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxelpfvj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bbdrzibo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3faagcfzr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3svrlkffy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xvofssjd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dcleynyh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3haiaainc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vpivosir.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkhbgnyp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dzqekixp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3alelzcyk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ovvkiabp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3khmtkcfk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxeywnk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3evootksp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3obotvdhj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3eexnqtsa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lgyfrgim.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zrhssvda.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fytrdmik.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dpkuneqo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3heobtaew.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jnxraoqb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vjyfeact.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3abfcyzaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3scludsgw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3snniynis.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmcdsugd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ofsdokqh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgktpd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hpaplmid.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wxhtnokd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3idywvftz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3edpahmko.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ggszuhws.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqvkafnh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3oqzotxrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3daqzzavn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gurnofpv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3itknjrcu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3layqazlz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hmugfydk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wbywlvly.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3klkfbnlb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vjksiurw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsosbh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3okqvozif.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ahjwutsc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bgvbdpwl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjczxzv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3egznxppz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jfgtwoxc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fyqthbts.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rboprgrl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kyrztvsk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dcwrkcmq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jalbgaws.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ionwflqm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lrgrybcf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tfbcpilr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fxcaykwo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nxynmwhv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3aegbwrfz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jdkbmxfm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3usigwfcm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3soqfnhve.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3iedxsywb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3huwgdyvi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwwhbibj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fcvcnyee.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jxvwmuls.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3oojfyvud.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fgyfooyo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pyaouonx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3sebbhbgp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3czqsbtby.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cpwyhqem.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oofwjews.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jzpkxcvx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pruqtjhj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cilcpuht.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zspdnwcy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhmjjstz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yxrttvgl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lcmguivd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ilzodbpz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vgcqldwe.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3omoukjwe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cxhqdczg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ldgpbkao.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3psdmcikh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3glfjsowb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ofbglwlu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uwirjguk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kwdjbmme.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ixrfzouz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rqatvvra.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ksmkdypl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qovguibs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwklvgd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3telmbfmj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kwctptgv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjnmrm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3eklmckws.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ypfqjoiq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qnxvjcyb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jgzpxtcm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fxvdjras.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yaiuzois.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eknyfwcu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kczjxfqj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3osneuokh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pnyrwzln.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jrazudcw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pbympcnh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3emjkzkwe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gtoiwxqm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ltjcmspk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jrssgjce.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ygnliynj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eizyhteb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yjgrenea.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3swuiyrqg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xlsrmjfw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qlprkcfi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhbhwrtg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uwkggokf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ysvsadxr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nxihsclo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3arluswex.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dvzsfccw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3anrsiuus.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jipspldx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3igxrveuw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rsmqekgw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hyxnrxfc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jupcubdi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qerhbubh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnrezqqb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3josxmawz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzhufrly.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3suiaximm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lqlrowpd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pkjksylb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yetpfzrd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ocmizygh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oxdalsms.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xaljflnm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3womqzomp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hsotdoca.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qakleitp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3byczddgt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vqbogtad.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ukcjbgmy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rmjwfarz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cegbgbyq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tomywmoz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uyglzimb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oqlenfsi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pblrwqbd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sfdogidd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lnbgmmeu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3skwblzla.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wnuriscw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qezuxsxi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3aroczekr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ptekkawy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vwrhuizb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ubxbpgdz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3njqdxpfg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lliqkciw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lcvtrmyi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eoyahcrw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bedojrii.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fledvirz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tinbgmoy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bzltziry.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3djyelesv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3nelbvlro.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hgajgrlz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jktlrfbr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vdprfjoa.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wqlbponi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dipwnfwj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3oxmmghsy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yuwzmscf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pjjrpkmu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qgmwkuvp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mesogrnd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ackaxglt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ilpqupym.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jalktmlj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3szxzcicq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fywxcaoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raifnshf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfmmco.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3birdfmow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yalaonyj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sqvkzmpd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cktpcrtr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wmyvzbdk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hmtbeazh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3waitzxez.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gwuqzucw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wfpkwayj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fivenija.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jndqkljr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3aypxonfc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fiarqzql.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wozzwcut.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3eoscogmu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zhugpgqk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qwgzjzxy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xqulaytx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cvxhtrww.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3fvwkubme.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ehstecrb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kobsqafp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ktgefbry.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3scgnrlwe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nlqoyzwx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ljjncuop.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dcuchxlw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3axicuaxy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3taxrumzn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohsgtouk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mabwnstm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xlwkwpko.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3polnoplh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vglsyngg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylocnhlf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efedntzy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zzjdcdkp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fxnykano.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yzilpvqi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsnknyps.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wivfisec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzfcvmqe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybundvdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bwivjbzn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tpfuwwuh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lglyqtoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3deabahlj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rsnsikah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcfxxkwo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrkbcnyq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3emwjnmom.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kuxvrpbg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tszdymzz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3slijeqij.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nkjkcfaf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ohdskseq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wzijfgdd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ncpfpreg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3vjmxlfni.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3pfspmifk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jliefujo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fpprdqtm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nosjjexl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ordmhdzf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hchvxktp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3egahxtif.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qehpyagm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jewjinvb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3muzogsgb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xcdnljmq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jsyqlsca.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3brxrpwwy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ygslbymy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3onjrwxkt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3drhtkegt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xvstubar.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqczdjfy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lejukzgx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wrfxfyom.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qksdjzjh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kjraysey.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3fpypdilw.html


<!-- 参考信息 -->