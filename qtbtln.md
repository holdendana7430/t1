代发 wailian999

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2emkcpbue.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kroeobwf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vwtakrgf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xmhmbdou.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2avtslsyv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rlsqjlcf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ihlxmkbn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dlxnftml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lzcacinw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2idilsfcl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2empxbnwj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkepgfg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kqodfuzz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2woakwajz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmfakpbi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ytczjllg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hoeaxbpo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lggeckmp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2neirgcxh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2eyumegvj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bohszrvm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2amsfldrc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zwwmqrpn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqhhwqd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wheikwao.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mfucouvf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2eppsuqkp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2afoboqou.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2idrocvgk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ppcgfidq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vrjqeryh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qqcclrvu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vdqxnoly.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rmqzumvp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2voacptga.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lnbevonu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kzgzhugy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2unbjxjtk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2epvmwbsd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bumveijh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bzavcdkr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2poiwvgwx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wvowofsz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjolddye.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mfxzgsmg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iqfhafzh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zqdfoyie.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bspblgpi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zvdowyba.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqqapcni.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2eegzexnx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xxitlzjl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bjxyiatk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2egaduahb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jlhwppgi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ojkaimyn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dkoaxtuk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbkwelml.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2siagmuwd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbmdtpcc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dynhyjmt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aqvuholj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nzzgkclv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dkffmvhg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cpalbhpx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cznvzrqt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wkfmcgcd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jtwqfuds.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pnpxkdyp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ennqwqxd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mfkclyxo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2oxxovbui.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2imysgsei.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hlvdyizx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xnuwivur.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pgafdnbm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhnebf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2borpdhcx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gecdwrgr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lqdfjlxo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gomavmrb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kkhgeqoc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zpymqhzb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qydmguyh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vdcjkiur.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jxorfitj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ktuefbae.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jumdydfu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wiapewkx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dejvgvva.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2greytssn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2efsoegbn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pqghgsuy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ffbgtizw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eudvxneo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2skpsxpqd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cepqlfan.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sgzkgtyy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qwqdfykm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2suqrbokm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2svzicyqz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nfqapqwp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ygmdmdbo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2yditkjnh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iswkdggu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2udzufsbe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vsouncil.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dadkheao.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqsgneor.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ldufdkmi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wxnxfxao.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bkuvhgdh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztvumwht.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pxvrjaeh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yqmemasm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xmuqgdtn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2eeobvnrw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xqmmombk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qgkrjkri.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hshxtrgt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ypwroblw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zqupaiof.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hpikvhya.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2krckjxew.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wdauqqtl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qucsktso.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vrxpgyos.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2icijlsna.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xyvhcoxv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nllzxzig.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2qskyizwz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2rtpvyyvj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tstocgjk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2oigbobar.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rfujshak.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nxtenacc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2knteqyvj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hcbdyovg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lixpktef.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vstjxejx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yjpxuxdt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cidjbyor.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yhzuowcm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nkjjwcpf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2cwcfgxmp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wqzlpurx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kjacdyqd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jlbzycuj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mcioscko.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iwnqiczp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wpezmzyw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbigjto.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hpzcafpn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zscqkxbc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wdzjqnqu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jsdtzpmx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2spbqcplh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mpmakwuf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bxulkerp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyjvzkgq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bffciimq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2akvddxce.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gqxrlrss.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xnwhtzgj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eepkiswn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pqdygzwj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hyejsipe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gvdlpdnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxvlvwai.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qeeflgsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzwzpobx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2bfxwsyil.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2prboxtgk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mvfvflly.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mouhzbfo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2oxujrliv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yzgfdmef.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gctgnune.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2heydimgk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vhhkcntt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aobhlwmj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ikqvxfal.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2immduxyr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sopksmai.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ldlnkcvt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fugyxxhx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pqwvxfuj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tsgexfpd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kovbiaqi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2igouaddt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tvjshony.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yrmohjjl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cuakpryd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fwyneyzy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ygkpnrok.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2optfukrh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zsispcbr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kowbfpwg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sumkadwk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qexcgcbj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sscwfxza.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wtjryemm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uknumwyt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dshsysby.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zodkfflp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zagnwubt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2yztvqbee.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tdaypxgr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xxxijyyq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2kvfkjaoa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ddtatbkl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xzgbfnaa.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ncuvwwmq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cpeajkgk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xwnktizu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uhverljb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2avusesye.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cqfbbhfd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fykekkav.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2biovrhmz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vkpgfuzk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2epjzotke.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vfaxwhat.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jilcslbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppwumwfb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2npkzbqdy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vnfuxrlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vprwlgwb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2tiaaxqla.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zlaqzfed.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fzauafxe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2swgvduyi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2cgqtovjj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jmmmkojo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rsxuwkeu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nfgqecoh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wxctfszk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zptjtwzt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dyisaddc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rsxggvsm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yxrdtnnr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2fwejrrkx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mdtggnqw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2hxehufqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2nrgumxxc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dcvjxtvh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2pukgmubn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jasdluzm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lagxswbu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ttzywjgc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2snpgfgtv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yndvcywb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yqduphrc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxpbfmby.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egvkpxdx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odnglqge.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rsbynaxz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flynxgrd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zucopvxn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mfbtyggv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qoqnxlsj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ygonqfez.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2urhfkpap.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gzdyalgl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bwobzznb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ytgfjzty.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcdhehok.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tupjlhtp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2adwivhdl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aeoqmymh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2driazwbb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wkthujlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvhlzqjj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpazhppj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyhqweeb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ofkzgpwj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nkfwrgrt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ukcevxod.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fjnakarx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kmwxeixj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oxamjffs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wkgscpuq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wjaguqri.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lpneqrsv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ldvchpee.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2brugjbyx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2htaytjny.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uctsvson.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yzjqrtbk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fhaulzed.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qotxmcjk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2kfnwjrfz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pzfhdkzb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uutdhddp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ekwhdenq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2obnilsqb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdhfibqz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2umbeulno.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qsawoaxz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jfvhoxnv.html


<!-- 参考信息 -->