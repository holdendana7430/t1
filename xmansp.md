代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kxtrhvpx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iqsqgivk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dwklyzju.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzuzhlp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzvlygbo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aenzwjqr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tiosclas.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wvsghnux.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2phsardhi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bkrcmtde.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2egelulfj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sbeyzriq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jjbhnhij.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jkslnoij.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mvmexdro.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmazmjls.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lihuthst.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hxzdyhrs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nohoazvh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nmasezvd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ndcqeewr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mmxuhtyt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wzqkbyxt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nkicryeu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vspdtpnf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xgzglnyq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2akmdhqtl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsydnhpa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2koqvtydn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2opisrnzn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2oizzqagd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nnrnnfbe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zupihexj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2evszpyis.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nsdkdqjy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xdkysjii.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qdmsxydv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2asfdjqgf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wiwkbvmr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmsqun.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tzwwhmdz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pdbpyzip.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsanpapy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wqoaigtm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lirhsvvg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdrtbrec.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mkbboxcm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bcwttcwd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tawuktpj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zimqohxi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2znrnrwae.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ccudztde.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zwfgvwnq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2sgbqzdiz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2burmjodk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qwsswkde.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2osoowmgw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2btymxtoi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pfxdxmpu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sksdxigw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vpyibbcd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sejcmbqs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tcvyotvd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mjbelvjj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2iqhdlkxj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hffxfcrr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pziqqkil.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mkfrqnef.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2djwmraez.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gycrunvm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rpvjfbjc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pljhsfrt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uhrhuylk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fkvhhwor.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2judubmtu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qekzudzy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2shikguvl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hcqtbqia.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nhspxkgn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yabjcdxu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2njdhxvdc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mwqvgogd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2itbnbydb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xhxzyoxg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ezincsgk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xjuokjjh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rwpsglds.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xkpawiom.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qrhwxlcs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hekelnvi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vnwpbyqu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bmovwuvl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zbytfytz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iltcizqy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2imzceuhu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kcffuspj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrsadlzd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jkrfxngu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pqtzkahw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hqlkbajk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2luidqcnj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jkqnwmiz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezgfzrga.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nnosdica.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ewlcmshi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rzmahgyy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dlntumcg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2igerfxwu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mdlyuqyu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mxrdkpsx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ovjtbsid.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tpuqvsch.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zsonnxwl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ifieyrnw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2itknkerv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nxlybzme.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pexblpba.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xexunajx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ipwwzzks.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qjswvnnl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2athqqbmy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jlvgtdar.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2swuoiryq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ckcgtyfi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xgnvnina.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2agvaalzg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2borohgia.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ftkwrjln.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cmijhelr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tjkdtyog.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ehamuhvt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fqnicmtw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rjmxvido.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zixclbko.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vcqhwtax.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ekrmwhsc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ebjgclju.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2btxwkywc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2exkztomh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pepnlpwf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cvquqssb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynijrigm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oiftjndf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rjywcehh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wrgcrxeq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bqposeyz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sxdeuahg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bthjzwiw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ohovqimb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fxknxpsk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xtetnhnk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pzspcjmn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2prayowew.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2modvufsg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rmpzvddq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dutyjeey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcmojtof.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rrfifbfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmwvtbql.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ipcwmlhk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2syvlnbbp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2uhoqblsw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lrpqxyoa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ksvkmska.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oneqrmoh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2snclxmvj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2grkuzsog.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mjnjvahg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aqzjawlp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ufqvucqo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2onlfrxgo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zvzshubu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tfeidhmi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lkqatyty.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xnyytsbq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bjafirtv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2nfjgvkcf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aflucgko.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wnvxbjfd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2waqyobik.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zxqahrmg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vzntkquq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cdrqorkl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iijbvjko.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wcpbjfuo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2obrjfnqf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bnyborlm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eepqbwqz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2apdxixvu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xxzdckvs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vylfeshb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zmynnudz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xwpodcph.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lkptbyfi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2tladebng.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ufarikro.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2irfcrztg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ezctivbj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rprgwerp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2itqgamxr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lfuulryj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uimavtcc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uixuzezi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jvxbnspk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tjuwmjhc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2clydhcht.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ouqfejwz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2evtitkyt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dbccxkmu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ydeufojn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2lnrpmsrm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fnkzfhae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvologng.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2gtlftfyo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2myojwfuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecxhsbye.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lafhptkq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2bimoqmbo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2otohpury.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kxdhjobj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ukdpgsxn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fciecyyu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pndlzvnj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2khevqsps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hhraxltf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ffkijcoy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2sghkjtqn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rqstqxox.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2arzeeevl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2crvgwkxq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wqvcvzgg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2urpoojyy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mxqqpppa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2swocsudn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2takuwhzw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ozcgqkbi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2igobbbuc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xmrnafyd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ibydxfno.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2njdrjsmu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yemvncsy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bpatjctl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2soscwaxs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dhqycizi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rhtsgymb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqdzanng.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ekncagcs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcagfklm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rymcnpix.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xcjwqphu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nraosddp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cglxshjq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2sjorphik.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yishulac.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qgoabxns.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sopixoaw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mykymehb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vaikmqjs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cxkwjyjn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fklrynxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgrmxilq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2apwnpfoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmgcyzrr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ueyfyslr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2egnydmto.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ctytmrbn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ismntbzm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dircopbs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cwzeqdkh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kgyweqyh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wskwmzpk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pjjynowz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2efvpcbmn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2dsrfhtdp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xhggnyef.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ohvcwhnd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jnmiekmv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aviiyvyh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qyetersj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pkvaywwt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zlsizscy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nelelvbz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2rfuyjipy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bpsoquyb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gghsdsmx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ldstjhhu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qwqlcbgf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2guqqwcfg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kabfbjwo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pgthrxbb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xncwqxtz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kqifiydf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2uqwpnoct.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lwlzcvhf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zxlcrfna.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uimnveba.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dmuwvnle.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2nlbxndnt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2avjynacu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vaxjaipi.html


<!-- 参考信息 -->