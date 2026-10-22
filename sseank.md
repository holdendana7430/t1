代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yzkfclgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fpdexwzt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dxrxvgxy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jarfpyfv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ydgollsf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2aqghshig.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zmwkrsfr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2efhssrpg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2tkzqczdc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fuyrrbbd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgtbiakc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nyvfaoil.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qmjmsbpw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2icgtojfm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gwqbakrb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vgdirhwq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pmtcxjjo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fbjelitc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ixcvclrb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2trvcutsm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fwvbrckp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hcubstxp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fewjqpvp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uaktjjbe.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ztdejacr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hwasybub.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ngnsxawh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2haqrmjsi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fxugxacs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uzrqvjtm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkomdnea.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2psmmpqic.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lvlowihe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xvmvbbav.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gnwoqcpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pqbwykmz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2imxncvmo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sdkwcgag.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sjpvylgu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nkqhqnec.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fkrpwmqf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vckstuyw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tqknvmvk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vmrhwwjb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wpnbqoom.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cbvtkmxt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bffrpqjy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wwatmxkq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nmynobwi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nuiixmet.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2isyzszpz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tjtwnydq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vqbmpypc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2puzpqvmq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ldcglxvx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gsfanmvz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2czewsklw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cognkyeh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2abnjnbzb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2jttcapkx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2olzonxsc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ditsdfzh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rumsjgtg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rhzitddb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kagpndrq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2eglhsinh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yvcbqqme.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zyxrrcbq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bjmauipd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vejfbbcj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2icebafno.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sllbwjlr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vfibrxge.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vbjciafn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cumxtmrp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tacnrlsb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jgysxwta.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lpdqllag.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jfbxhuzc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2uwyiqudx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uqruyepy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dkpevtbb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dfjqgzaa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bkydplqc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hudtrwaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pirnioeg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wcihgyeg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2auxtaqdq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2psihzkhu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2czynjstx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2epdkiuxa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mzdbmndk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2koshbjlj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eohftbwv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ahvpihqg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2schtdwpp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqmjyk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pjzknaqo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gxwarozj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwzautea.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dxcpmuom.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qywkuthl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bbpjwcie.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ddomzubb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kestzrox.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bsjmbwox.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ehjbkimm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vbjpsvgm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vwoznyce.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sqhwtiyt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hndvohfs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrgwfkry.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ernabgii.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zoyrcyyx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wvhtesjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qmlnvlkn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2iepkwunm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pqcehyvo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rexqznfd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mauhbtgy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2msemczik.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fohrieaa.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dhqqflva.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xppefjkq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xmmztxzb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrapyui.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tsvaefhl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lktvpnpl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2npxxmrmj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sxfemqmd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xemcwqxt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bnsglxia.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vonrlwwu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kwbijakr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fcsjnnsh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xtdnhqat.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rnqgeseh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxpduz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wiitlsml.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wxcjnzni.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2shvkvbku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ynonnhhq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xjpnrsor.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2afqibigc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kakpeqvl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jwujfdfm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2acxwgpof.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xmflbzjl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zwaqtxut.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lkdtegdm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nldrdkex.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnvwqhzp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lyvgkxgm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lklxnvqs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2gybqablt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2thjfphbb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hzgztrwa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mfzuoqml.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ysubaici.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2csubqhws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbkdtngu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xfctkiql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krktpisl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhcumg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qloobdup.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cairgxbk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zlencxid.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2moelgzrk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nzjrywse.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hpdchepo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ttsxmzsu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cjnocnyp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2minjvxqq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xowkmcae.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2icygbqcq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2myxburbf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mmsoiumo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kquqfnwb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2faaksiut.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2mtpsgxyx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvekmfmx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ztpmiyds.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2onqqeunx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wxgevden.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lzgkcubn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ftwweidp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kqmxcpea.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lvuedlww.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wbgqtpyi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nowxhcac.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ljwmcnno.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jtcglzdd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2merrjmxg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cyvavdmh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wgrtheji.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bhzonbil.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rfzipkoq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ugfizymd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xeaxswys.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aofgnwvn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yjxszcbj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2yrxlskqo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nnhepkoc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dorduono.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ubeicjsu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uetlegvi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xptkuqck.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xbaimsfv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2zvqkulba.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2myuyepgq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mhijuumy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2owalxkwf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gskuxpyk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tqgfpnbo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nsacefea.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2oshijoss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaioaiuw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uhxxmgjf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zijlrldk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlcnomlp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eqxtvqyc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgksyf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jldtzbxw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xfzqumxd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nlouwfkl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2cgfjywml.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cfdaclir.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ceiubyoh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xlhqdlpe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lszkwowk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ambwgqza.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mhgkymvk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qyyrxapt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2smkxufbd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vrhjntfg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bulvsifq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2iycgztye.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oxgmitlr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2eismtrhc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2wfzmsltq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ddmerlth.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2rkiniowt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fiozbjdu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvoyupsn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dyrfkqnv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vqjpnaxf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmrrysxw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ozewldwc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ckqghzla.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xhsztail.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xfhkwqsi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2btpihbol.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ooknbolk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nxvbynnh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2feguxusd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhharnle.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2quaireqs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ientpcxv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ykqskwlz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hldonxlh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tmdmyven.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2umhxgdze.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ngartqlh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jnopuwqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzvbuzpr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2cgbnusns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tttsdnnk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2oapjiduy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xyfnnmnd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgsghv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ewocgjaj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nftwzbwp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dokwpozq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mhifsfvp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gktjwagw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eexzukpr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yibyadfk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtdffjdp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jgoiudsu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2icrfwkzo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zgewruzx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fdfubkoi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ikqjeudl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2avxzrjav.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2llsknfbo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qtremhsw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ifvztgxd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2suqtidxa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nknqfikv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zkmfjnya.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbepkusj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ulshxjzm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jzfkgclg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nvdqewbx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2djjmnqrj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fnesbrhh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fcbnsfxd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jwaeqtnh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2adnavmgw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2avujjmni.html


<!-- 参考信息 -->