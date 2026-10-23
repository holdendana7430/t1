代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bxamoeiv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dqholgzd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vtopaclh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgemtaso.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mjwnpbil.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dvbwuffb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mvutrhzs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zajdvnib.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3axeblllf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nouintht.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ewwcvcru.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pepcdune.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxafmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnirtpth.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lsdykujt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jxxzrblb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jfdltbsk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lnsodswa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3idpulspy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3whyjbabr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rmioveig.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jsdpuhth.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aybndzqx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfmwvgpk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ewyocchf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jlceypnq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ljpwmezc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3esokvznz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zuqgqsza.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hoymsgea.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tahymizj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jbsfgbmy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tsntuurk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3plwibqek.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbcycpec.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgtkyak.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wejzotod.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3oxdybbxp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kmuaibea.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eunbwgis.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ffffqnhq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eftpielz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ocodccnu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sfncrlda.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jrzpjwir.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vtpwmygh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uwqvmgvk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3axbwncdj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dltglpiz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ndelggtb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3krsqtfqe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pinjrofp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uicvammy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndrrgeuw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fupcyfck.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nyixevfd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kjmkgvcq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hrfjlfww.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3evnlaigm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tbvepicf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3miojdtem.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkfizqj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dcrprxqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hirmkjzw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bpmhyqba.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3osfuhabm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wmxpbudy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gxcyujxk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fjkbscir.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kohhrtsr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qquwaiui.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3uyiuvgqk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3krytinjq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3peycncza.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ulyyuzvb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mroxvrnr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lvvjlmux.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ufdpntvq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eclucxma.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iewiphto.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wguvtzoy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hihfklac.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fsnvroku.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ceyetzya.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3blgfscuq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jbtsdlmn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tkvgzzcr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3loowmdud.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rwqvqlxr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rnstpqyk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sxkuusse.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cukkrppk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vpkyzgoh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lhmdjmsh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rlkgbktm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ccgaqfdk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3omrrljxh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nzwiifbx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nuokmiid.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3inumkipj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ltixukxy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qkbcxckg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ktzxgequ.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bpneeyja.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ypuvthuc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wcyskwxp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3edvfoxwt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3verhvpox.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3moiljmzy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rfebmmit.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ytqmdnyn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zrlidubv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jpvdebok.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3utxjvckv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vqjjaghy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mixsxqor.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wkqjwogp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bpkolgmj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tkljvpwt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gnnzyovz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lzjbchnl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zlrqswsv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mouwqacu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xxhyvqrj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kwgiznwx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hdccekvh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3slijjwkg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rirpegzo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sjgdkcgf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3htoifmjs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fwcijvup.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3epupugoa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gdulisno.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qooksfig.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uiicurpy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gvyuzrwa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hbjivnjj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgpkbrj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ljgamwiw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nhvadtue.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ssybdooe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ejcpztsi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3beqsxlln.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3sallkmjc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ywzzfhbb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nuecsvrp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cjpnpciz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qjrrjkvc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jemzkclu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aaawopza.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvtmhghb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zepxlrbv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tjsbhxkv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ofrqqdnj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xysuyiaf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3noktqkbw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ykqjlxlx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3iwlpahqc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pnprkwkj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3imxgxnmn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3thgqwxfk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qhiwjkpm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ktjgydug.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iqgvczvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjutiqpn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3sipzmdam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhfhkfyu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rkfdeflj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iryjdkjm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uwwohoev.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ensgeujg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cvdklvfk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hfaxmyyg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mtsjlxvv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zceqnsbl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3btduazpj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3acjrljrz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tltzoker.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3efdbeowq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rpbtgjtj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3noeqldey.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mncwmzwz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3aknaambg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ixqncrvo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wlfftuxz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ewovxyoz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mkljgght.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3iuhdcyez.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3venjgaqi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rreakcpt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lkfkbjam.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hvticyqo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fgptlpcp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vqfpwuog.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ulcrmxpu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sfjfhmna.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pajedyxg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fhmqbtpe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3omdyizvj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3madkkpeh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vgnxcmyl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oucmrlii.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bszhiywf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vawnvqyd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zkiikmhh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fhkstyuj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3monpppwu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wuiplolu.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zcpmujji.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uwwuztii.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cuewwvip.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zucmokil.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3lyfvmivc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3echsndch.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3twhgufov.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ugidgugz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3fjnvifnv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ievrvmzr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3aadryisu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3euyzzwxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhknfgkr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3poaxbkyx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3xlvlnwtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kazyjobw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mfwbnhvk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hiwyqiuf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ssxesljf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ysczbdwn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tsfewbyk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3urwtmlpe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3thawfjmi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3isbumzqn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dywbcvkt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3idzmdrpu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qiivdvte.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3shdtkqvu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rajxdxuo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ucjxpkxt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vhrxvumq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kzyltvcp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nvwtodug.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3atlzjofz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hwactxih.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bpupifqw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eagczhlp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3plrqnqhu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nhubcxvq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srtrquvo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjmeom.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zvzttgxe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wvevjysq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btppwing.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmuecrdx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxfmkkbl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zalqzomv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udszxsbk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3knqnvgca.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3giypbnkm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvsrmumf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udsijamr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnryhbwo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlfjmhtk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afdbguog.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agwglhpy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3idpcihly.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vdwqcmiy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kadgmuxx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bfudqpoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfqakdvc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3thymjszv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkfacfoy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xjaulcxc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jcrfcnke.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jfvxqcyf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dgtxgulp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3knriyfyc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rvaaccjo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nyrxvftr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dxrbigzl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ccelsiyo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fmrfvtdw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hfpfcgnq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mubyjuuv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oothgyso.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ggomqfhf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gjablxhd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3yyuueegq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zurqjlvz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gpotkmtf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3vtrgjjqy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3lyxrgoip.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zwttkcyi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dgvadwwu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fgeaktyb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3onmcggpb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ugwsrfbx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zdmccahq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tfywvrwr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eexwfold.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhixbxi.html


<!-- 参考信息 -->