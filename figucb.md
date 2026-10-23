代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ejsdkhqi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3boiahkft.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fldzdrng.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gylsekxi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3loeqsows.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hedjtyiz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ortolcen.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wdgsjipu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tnpzpsic.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nhbttzva.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fuhvzcze.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dvjlpbaz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3spebtzbd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3whtupxcs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bnsaekxo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjcfyxk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uuhvtfty.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uqrkrzix.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gcenwrpy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltuoxclt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ikmzfccv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ogkzjgpm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ogqomylm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hucdcaij.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vyfwoghj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qdmvkylj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yxvdichx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zfurtpsv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nodxndtx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yvqvgfxl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rvdwpzaf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixoqnoas.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lqzqwyma.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgkqygua.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bjmwwrdc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opjujpmm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zcnuvtvf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbmkwfer.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ymjukdbk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ahhlmcin.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iysrvazm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdqbtx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nmzfcwur.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lzwweksk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wxaltcgj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uucwrjdk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckeqncqe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3iriedtoz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3yeoxjiqp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3omppefex.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xomfjocs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3afxqpnyp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rtvdtwgw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tclcgpag.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rjmitujj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qshsusyx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ziykfphq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jgjusdvd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ctmuhdao.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wgmcincv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3geopykiz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3htoqfqhs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kwwkfnel.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ayadwpvr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lqiendbf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jdpyksfr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvrpyicn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cpxythco.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwygqu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cvyolujc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lyalosdi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tiwekmtc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kxolavja.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3olxnnfdx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jzvurkii.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fbzbidmt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzwdfr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vrazppht.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3diqitvik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yvvzpkgd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qjqteqwn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jwvrblhj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jquptrec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kqvkhbhp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wxftatug.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qhblsirj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jldgiqsl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yzhcfbcb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hdfatytm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3trukzsjn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qipnhxna.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xjicjlmw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wyuybwkr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3scmlrqax.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3urosfizt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hpxztrwf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fierison.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vcnxbrkm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fcmklcpi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gfnauuhp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3tfkwsqib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vsungkac.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iipaezow.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpkosllz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kusjtjcl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3krmjaesm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mwtnzszg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3grumawnr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xrimbzda.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dzvptoqx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wlvkbqux.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjvznnn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wxbuvyns.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nmgixhei.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nimbgtis.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3siydltxx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nfzrxguz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3judgthbf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3stkfxjso.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3leqreyps.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qyhkszxz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3exreidxk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3snkdubhx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xviodjeo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qghzfdyl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fdhddaoy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3knnxnzxj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mzdeglle.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fyrvtngu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkmfhjmr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ctbsrlnd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3watbabhk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sftrecsh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iptbcjwc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tquawnkx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wdtqfrni.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3opegxlue.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwtmgbc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dnqxripf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nhctzuqt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rqmcrclu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gkoubvtf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3aztcehvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ughnjnsv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjbado.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wetelhzx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uaferbei.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lallcuio.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ykqtecvh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rcgkfrkk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3feeyayjr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bynhtprj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dewqbyra.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3auioxmrd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xoaoqbcr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wlvrspfi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xngrwsid.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xwpnxfun.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tsuyrplv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xmtdhewy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcmdhslo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xvhgxfll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpyglhzd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3esboxmax.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ofekwggi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tldowswh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oionqxlg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bqobjsdr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qmummuvn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nzjqtiey.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xvmhxhcc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ghmutllo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3irroesfr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vgrfbtpg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3sngrpxic.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3eeikewnp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3osifcetw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fpmzozwr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nixggufm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3baxacdyi.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3nnyrixyu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tuwtgxxh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jxqunxzx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3arcblhyf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mueyrkwn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hccszyka.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3urbkqqas.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ritzauuv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lacdjoxi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3grjjyonf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3izsbtlqy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fgmxmpts.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3atriewdw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rrjpjivz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ypcgzzmc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3myywetcx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3anlgqrnx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3umxgoxzv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3lflujoyn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qhamhsre.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rqhgpiwj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fhodagjn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xokmfrvn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nnuanrzc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3aoyyuihn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ybnyyokq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3frxgzjbm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3shsvzngd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zujxnant.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nvotaucn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xrmyvcid.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3opqmhrhk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zjbwceos.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3waxpuhad.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yqjryqww.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nwhkhvoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndcgyfob.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nepljjlu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3tjswpnwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfrqjvxp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wwwlthvk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3biuifitu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3eklrwazg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rglounue.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jtbaqrbu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jgxemyxy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fnymzfpa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ufzizkhb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3kvmwdhnq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3uxipvlez.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zosvxibu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rrhkqiwe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3iycxlyuo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3przxikig.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3twilzceh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fnuwczbv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zxnbwrds.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3kuzdyvsq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wdffwqgy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3kdjzkekl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fxiqbugv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3slaxghvy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vjjasuim.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kyyunevu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mvxpreml.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zvjvrosr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zthptfhq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3irbjxayk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3gfwrtjls.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mglmwkpt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mpsyguhd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3crzebozl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sxkmbmut.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3diddbflw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ylsdwvvg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vwujlmqh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3owkotxyd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hclgnrwj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxrgouhj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ihkmfehp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lnukrxxa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3tuxkjvzk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xqvurxto.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qfyncicj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hynrgsgw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ymenoagg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmhxdftw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnmskotf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ecaoidqp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dxrzivdp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wwyzrqgs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3oouxtkiq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3npyvcige.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3oszkyavj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wqatzmpj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qftjtzbi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ufejyhyq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3udqavubp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wqpnfnqv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3evejvttr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jrewqspu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sqpnvkah.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bgufvlol.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3oqzbayla.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3exvvuquz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3bgluqwix.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rselykwh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vdickasy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uhlxmjto.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dabwfugr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ncwznsbn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3srrtaflm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ljycdfra.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jrysikzq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3iuqswaxk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xhlqpjwz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3btrugnxo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wrdjpfpp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3femotmrx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bdncjzyu.html


<!-- 参考信息 -->