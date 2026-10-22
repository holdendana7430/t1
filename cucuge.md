代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nmtajdcn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2duqxgzll.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rlupothx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2bcubjoeq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uvakttpo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2slcbrsqx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qjkunhmw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwheppk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2txulihcb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2skmkemvc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kgjrvlaj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sncltdrv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ksdkqzqk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2awpzvrtz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wyjebcdw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ecusvpwo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkpsuynk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2moeyeadp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2saeezpwb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rbgrctmd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qgdljhqe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jengoxny.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2khpscbjy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsilivpt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vhxgsimb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nzwnaplh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hxeqyvsk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlgnwjil.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wvshnbkb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zyobjlss.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2plqkpcib.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2alwiyemd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2owvniclk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kelzbhkk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jcoyfqmr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rdhkkdfp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wqjzyaix.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bukgoqiw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ntucynff.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vjrawmxk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oydwkcvp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqitsbys.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vrzyhepv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebjcfizs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hznpemil.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2juhlaiee.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yidsnxej.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ldnzykwq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2akrazsqj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjkyebzr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nqcppqll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jdinmhqs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xqukuklh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ojiccqdu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fgixeaey.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2utizdsqj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2arlorprv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yfxyzarh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vitycutn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2eagkywhu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2debulshi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tuzyklsy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hiwwlptw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mfifbmag.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2sgvlheyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mgtgkfdh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xjnxhilx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2klcbvmov.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xjqcifcm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2frkhryoi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pgjnhmkg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xgfyddfu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rhbblwyl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xpbsrtqh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mksnfzea.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dfvjhxek.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xiymbljf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cbpgcbqs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2musgtysy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qamssejp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hjuwzxsf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qthlkwgs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wxjuhhxh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ynbcahmq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hhxbxnvs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2womvstzf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vphxlnrl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tatczlgh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2cvrjechj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ocgymxde.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rtrwfdyz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2njktlfia.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bptbhwdl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2azqarmsu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hnzibmgy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fwaomyff.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wscvxkyr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ytpufofu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xnreebue.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bcmwyqgk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lgovuhjo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nrknhsvp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2imhaepvu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zyugfkgk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2amzqopit.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2htxofzkz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ypbnzecs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2abntjbko.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djqshski.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kusizvfn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sieeyjss.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2egiogryv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dpcjvvbr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ngpehazk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iufeuovb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zebazhlw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ohfrbiip.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nbvlkhtw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ymezgpgl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zfhaausu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rvamatmm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jobujmsw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cgiankag.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulipyvsn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2itunmchg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vevwmrnh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aranadov.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xrtjizac.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nevujdpm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zsykxsck.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yrzjiiew.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2uysjlmjw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lqilicfw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zjbrtuyk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ximuoejo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dzhssxgn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cvecdxsu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qynuysph.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zrxepkhx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vleuwblq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dlrwffws.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kekwwudv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uepcblpo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ekelatwk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sqvhrdzs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jizmmhlj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zslqjviq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rwfailqm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pbcxjbch.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kkvwhnqj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2agycrjke.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2roxzfvlh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cggycxzo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kppsxoky.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2grjkljsm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdcxwmc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ciphpgqm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bbqzuvfl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wdvlppdg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xqnsnkhd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lxgutqto.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nbmdcqzz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rtsjhpif.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yerexvkd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vjeubxsx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2aanjopqk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2awfuvmzt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ijcsmrjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fypcgsnw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xmhoufra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kabvaxhx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2warxnkyg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2whisutvf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ixacdrrr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2viefegem.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gmrfqjru.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ysoojdow.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pdduxnyt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pszuwkwo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pziipwbq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fitsugoo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wgvjxfxe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2besqhioy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2sqkgaofr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tzuacjfx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fwgntmtu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pstsfchw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ejlyxqjc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2oqsbzjrq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2noobanoq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nbvtztzh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2upavzvkk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aniuaagl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gxcwvotf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vvpvffsq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gvfuzsiy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wreemxme.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gihhqiua.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qmivoflz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rregguxi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sqiancil.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rohmborf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hzvzqcvm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hxzmxpje.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hedfhjeh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tsthntgm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2drpapnzs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ylrynpfw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gubimsnt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zofhumrp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2sfljcxtb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rtarqobh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kczudhus.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lslzpjjf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2docwxrwc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mrbzzkog.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lwrygwbt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vzgiwewh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2yfldreoj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mivhkxly.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ymrehusf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hysbaimk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2obvrsifd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sygbqdqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvfmbfsy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xaifacyl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jsquvqxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avfewlhm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qlxwnser.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2klglpwml.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kkeyxiws.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2phkobvpr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gztxhbdd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2bfaikcmg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2afmzfwdv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2hfbbvhls.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2uqfoqxvy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2rsjrazxh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2croujzsb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2oaxwsdzy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2gqkpjxec.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ndvmaaqo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2djixihoh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2cmjbkuup.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2scqqdwwn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2tskmakcm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2eiywikvp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ulpxuzqd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kbaajztp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2scjsvtwh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qoauwxxi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzxztr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tpklzhmc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aszttptn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wgteoiuw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zwsmhwty.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2onciytnh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qrmkehvi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnpefeky.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ypqvtpqg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkacwzjc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2doskyfld.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cnegptfu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yzwuusoj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ipmyvnca.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2btxgslhc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2caavbjld.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kihstppq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmuomxoe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zxdvikua.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zsmcwtwp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cafrbmwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqlelcdf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2adtukdjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygvcuytc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cayxzemj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bgotjkbv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2npqygngj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xoonnfyb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pqagcchu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nxgzasmb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gwrvdebe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ndsikemm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2filuwwxy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hbanhazd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ccnjxutv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2daobqiug.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zqidvqjh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2znugczpz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqlbnxef.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rjxwkbig.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qdpttelz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2idnehenk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2incmhfyy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ilrvigdt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nixidfcz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qgtpibdi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2clvknfjv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tjmbhpko.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jotcsrrg.html


<!-- 参考信息 -->