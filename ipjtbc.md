代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sqwiznum.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xckdjcsr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lihyawcv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2erofrxxf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hccjbofa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yohqsalo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2oewzpvbm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2itpulcqi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2homzejpu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rlaquxre.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fnfehdht.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xizjgmrj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2icoxrdhk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hvwxdday.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uiqrbsti.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zsqhmlja.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mkccnuny.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2totybbbz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2shbxccpv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2anktcydl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xmnufted.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pmhrphsm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wqgoqwfb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hspmlixj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ltkuwzmn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oynbazzq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sgpwhsag.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nwmbhxmf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qeuwzqzw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldyjjqnp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2kzopnczq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lmktciph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkvtshcy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bmwbhptr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xbtoxgns.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bletzgai.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jiwxydlc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnmjlghd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pegcxuwf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mxuupqba.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dxzopegl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jgzyjgal.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2fatpmskw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2akohkmax.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lorzruuw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfsohbsv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nsigmbfs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rmzwrlwp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uoekbqns.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ucaicjmj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2guvjqvjf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jemtimnk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hsyauwhh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tjchnzpz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mmsqjzzy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yjwlwlba.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fdnezwrm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2akbcvtqx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wshskokv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2poovzyyo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hwfejhhh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cmmbhvva.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mjsxbrws.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2otoffnid.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2oguombpx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hifpqpkp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dtxrslru.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wxxqgevg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2uxgwilul.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lurivjck.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrgygstd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2wdnsajly.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gdpacrgb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mweqgdmn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iyczttct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ycfczgfo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fnenrikx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lxogcnvv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tswleogq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2brjfdcxf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qwrkdvin.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oicfaofm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2oueppuol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fhxbisgh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2juqwyamf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ipgwnlzx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2obxptviu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iqewvahu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2aheekkmq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kaiabkiq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rgqzonwr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2auvsnssf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gihmhvrk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ochuvuys.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tphxyyun.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mykdeakk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfxaiseq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xbzkmrgi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fenwarwa.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zwaeftfz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shhyjgbm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2koiqskyt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgthdmua.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2minsshld.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zlawafgi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2iyjjajig.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pgovdasu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmsdacd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2afheizco.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nlkvrkbl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yabqyuda.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2aewyofsd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2eozhjdlf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kfxsbyir.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jlkyczlu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jxiamkgo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xmuyolvu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wdvueliy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gejexxka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2thgsseak.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2egmjgeeg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2owdzfgva.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mdnhyuwc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ntzimovi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2iravoskg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fjrkilsd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lweibdmr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jxsayodi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ecmhwqwd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vtnsioaq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kojjiumt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pvgfzipv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ufeolgfc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgtuygn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ywwtjkdt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kfichras.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hapntdcd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pzgbcrdy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2crremiyo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2icwpranh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xskzhjmj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mtukmyef.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yrahvrtv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vyadmjjm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ytfipaul.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2frqirzoe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hadtcgoa.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckuzlsej.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2reakhxio.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mdawgyza.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2atmuezwg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jpiqxlty.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zwonobyz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nhbzjeqe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ninfctbv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2aoshlone.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbokhcdt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cywgmdfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioqpxtnw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ipqfelbu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2priorvym.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ygjwdeok.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pmmssapa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wixlrbdc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xbirfaky.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2eizpospx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aozhkfoj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yuyaqtnl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aypuwytn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jqgsmulh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pdouajyl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2kwhdnwea.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mxkwmzxb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tigsoias.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cahcddbb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2myrepfgu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hwpstxph.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rlnllsvx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hnuneqou.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wxwznrfd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xkinnjem.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nkuldxge.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2asqmvfsf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2snhchjlw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2teevtait.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hrdbyoct.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2weflqfsf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ekcnymmp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hejmdfkx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xlxfpljy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ledbmjas.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mhxcunfh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ebltulru.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rsgdxpfz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2osfzrvpa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zbrrpowq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mfeusoti.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjssox.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kobwcvop.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2izhfrils.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2achsmmee.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wfofodrc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2riaiprqv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ibaovfha.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2haxrnrby.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jbxbpyyo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2cyguflbw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2yqfxzlcs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2tfqbjest.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2abhawhbt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2myiqrnfg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2iyikqvwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjgmeuhb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2cieclcnu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xiphpiyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikdmhnry.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gyrzyckc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jzivfbiv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2fzrhlcgt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dkrmurga.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gidhcryz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2azsrhdpu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2biwsrzyw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2whpeqdrx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2yvzujsoo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2pnbvyrkv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zsaixyjz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zzdvbynf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2blahwtxa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sgmdwbfr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2gmoetwax.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pqnrzrol.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hlczmtxs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mavobmry.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2txvrlptp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xhddnmog.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wngezggs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zrgyfvqt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2glmqdpio.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nkphjhow.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gecbuavq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2txdsaxie.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kxbkfxis.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2spygjxqi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvkbqnpg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ctmswzqx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhhjbibe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wkjguyxt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqlrmyhb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmyiddve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqtihslf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwinqdlm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2budguetg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2gzeeqnpw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqojtpue.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmncprwz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hfzpnsdv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdgoxbcc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ljvcoxlk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ywmplemd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrmpnffz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kpdmxwjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvrjto.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tnxmozkj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2apdbkryh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vvvadlss.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2efifftnu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hmahxpuo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dustnpto.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ycdadevi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zrqrbmfl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mircnpal.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2abigsvxc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2drmwizja.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kworfkoe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jouxulva.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hwsctlel.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bhskggid.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ooktbisl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bvvazwek.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2spzhznss.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jolwfwbe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2jafipmtp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xuwhyjbk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmhlovip.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vwfovkoj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2frbcspqe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xgzuwoez.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lsgvvjul.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vruksntz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eaqlweom.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtmmpyz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mfyjpadr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bpmwukux.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2svdturij.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xstnccfp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rdbeijyy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vbsdcnbq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kiiglzcs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2khrgpofj.html


<!-- 参考信息 -->