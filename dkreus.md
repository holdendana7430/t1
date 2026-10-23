代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jktgdyqx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dyxigxdn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wtelpeun.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbakixhl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3idwfooff.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3idbxboil.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgfxgcef.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hbqwwmkm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3sbiwcxmu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3irtoajxw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cmsosfuf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nvgkaokv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nabyovtx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ihunkzgh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qdcitnkg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wugnaqkm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ekgffywu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3trtwxhkb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3doqexrcj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3erhxycog.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ylievdxi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrnhyapi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hjnummic.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nojsncbm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zrvqsuyb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vozpaoeh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xjgmcosp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ahoqdqhr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nkwgmgpr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3izqptlvb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cuevfdws.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bydoinjz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ufajkyxq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lxufqrkw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xlelyyqi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hfferjhz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mgnuytzb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lysgnchj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ooxkenns.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jrkhvwff.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3oioxjabt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oaaerjco.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ejknjlit.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wfsdylor.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tbencwac.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bbinyxml.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mqoyzzev.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3etkdusda.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ainbswlz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tbnhfujr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yoqgqcoy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3aeeggfeq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3apidomeu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zzrvlwqw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hyfdgoao.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kqdgrylb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ttarizdw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pezpfshh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jdvfqjod.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sjsnmlqq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vihjmpma.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wkitpzbt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3lmqaixjr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vguajofg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zmreegog.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cxaijdjx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3akjxbzwr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgswwqv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wwzjjbqb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cagkahyg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vvwaiokq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xyvjfccs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lfjhzgid.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3freuwgrv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ekbybgut.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ukysrlyh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wkbrynjs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dhuaahyp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mfvzttaj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pijiueye.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3cptxjybf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lbttgeeb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3knbsttjg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzlxwitg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qduulldn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ssbgzxye.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fxaaoqpv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtdzekf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ffwimrub.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3afvcupdn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sfbtdzov.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3blwtxvim.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3utnlopss.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zvhkoynv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uvruxryn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3celhngja.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hkrqrnou.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxsksmke.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xafpivna.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cstxokvc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3prsueffh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3osbipxgr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rfvxysiy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3agschvhz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fihpjqgy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bmkpgnhk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cdqqwdbe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wdgumhkh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eyotijpi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mnqwyheq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fgwtlxfq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mzkaaczq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3htyyvdmo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3atlkfmqe.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czambwxh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qlezfmaq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qcqlxpeh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sptvpmpy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3whdkxnup.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qahkbykd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3urekytms.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mkndbjoo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ciqgruqw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hqowlbub.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fzouhvtt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3aydaxxfw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gmfqaddl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ziydwzgn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3rwiaxymv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lcbkciiw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtqkivxp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zohwyakn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yerysvky.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uzgiifxl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ojuiojbz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwqdqfcr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3feqmpode.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aigucowu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ghxkzjnr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3etoqbyow.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sgscrbtt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3whtaxvrk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3winpmtoj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qtfkndnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjxeaclu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oaoakrac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqmdnkyd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zmmxbzqu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3otkbzchi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3udwclvwf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mwwbfxaa.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjyqnk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dvgltjkb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bijzotse.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lsuhmxkb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ahkzdift.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pkxwemqh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3irlricqp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ypohreoe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ffrmjikt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hjtksndl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sronakhr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nbtwsaof.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yikfqzhl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kohzgawz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sgvgrfrn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3abainprn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rtlcffdm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xjqspuki.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wtgcfgvr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vhvadkwe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kafxktcl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wyebtxhp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mjawtdrz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ugfrvxsg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vxcxxpwk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lkpfblgs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ywjvnvag.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bdvvvwht.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ejkeuuep.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3axyyvyel.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vzlyjfzc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3eknpftep.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kcltpacd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3oivzmige.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dnkmwsob.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3krewzeqf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vccpvesw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qzwmsuuu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lakmznlr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ehmbxhov.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tbtlkhiw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3djvpyioo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uxcmjcrq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gkzzcygv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ugeokoti.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3butslhzu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ytsfphyp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hfsedbbr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3gylnxmnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkmvrowz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wjtrnzvo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pmstvoau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3baotmmsl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3fstfzilo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ykryeyeo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3igqknzog.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3xfpthpej.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fpujvxxz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mnwnazjq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3yggcmykg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mgthhdwm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ljclxubv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3corsniev.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bpovmrbh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3veurqios.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3svmrdwta.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3yjybxxgj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3eewwlfre.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vlmswuab.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3zusgronq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ulnxsxwt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kercciqn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3apfvcvnb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dhslkdtq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3yonlhiqy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3knqkflrk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oynpucft.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qrzhijao.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gtoqyjuc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wktcyxer.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ditrlnvl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uolunryv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oouedjef.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vsvrqiya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xawqjskn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cptwmszy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3geifxliy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zewkdgro.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sdcmlima.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wirawsxj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3liyzipgv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3knsxbksx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3psuvbwef.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ggqczokq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3shioczwt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lycdqasi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqjcyrpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyaowzqy.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmywtplc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypxxtibd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nfwamwlq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dsdznkoj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qrpjpjmu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cnvekrjb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ggtiexyw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vzwozaxn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cncpkmop.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sjfsiahp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rbzwlhfl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3rgfklbsl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xzzbtcqw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xtowxcyf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xzrbnzwb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ebskiuyt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3njwleaec.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hduzqavk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3efntxouc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rbdgwvnn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3whhskjyw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fmpikewm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dfmrdfuj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yrzbxubx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qftnigfk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3guygebdy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gyysisxi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ftvbndpu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zoijubai.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3angcopdn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mermcasc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dstgsdww.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ukcrukxa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ooeqwqsr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hidxtrou.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3pnavcotp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3caeqwxbt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ndoqtpbz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gqthlayf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dfskfqlq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ykqagfwa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbelzkdf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vcvdlsij.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzglgzkz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yycyprrq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mrvragdv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hyrgjyjg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ngdanxqc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zswlqdxk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3anvpxcpt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kjttntuo.html


<!-- 参考信息 -->