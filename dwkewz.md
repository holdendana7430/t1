代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kuqdivmj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ukpcbvml.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lttypmag.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zhlnmjcq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3thauzuor.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3sdvzutfb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nlrxswop.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wnkjyipp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pknssjyi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nfepzigi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qwknftqq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uowasydu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pgzsxvoq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nbkmnnuq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rybnibst.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ywdmxatr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zyhdfmrl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gopyevmx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrfmvpmn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kniedmhu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wevancag.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnwovdbn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3hsrtdkjk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3aixjhpwt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tqxmzoyf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eukxhmwi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cgjdxecz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mlwjfuuu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xljicdht.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ofwkznaq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qdixbhsu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3urwgkdyc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rlnmqyiy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3azwqxwjt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xjeasapw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tyscwwnq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jolrpyke.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wjscjwwp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3glbxlavb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nogsdrol.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rwuutuwr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aeiepdqc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3utzugxod.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vvdzuwtu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3euvuprly.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xzxnsyrf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hdnefjzx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3daviqagw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xnekztmb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rfneygps.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sjdlfjgt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kgxdypbn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kimmxdck.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ljtjjcmj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nberajsm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gxngaduz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ftjthypx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ofsfaics.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gtghdtxi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ilxdmfia.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rscbennn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gypkftwg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pzlqwmjb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mwjhxgqh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oegceudb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jhwdyhvd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qbvdpyum.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jvafgegm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zmzeivwg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gpmfdsqg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pustjuub.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mixehaau.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wfnhyekc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ymrgguoe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mvhvjgsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3evcqbfuf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hshafvfb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hypjobut.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vefieoro.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sahjazjr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lmoccoxz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vaepedph.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lpqxvxiw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eldjprst.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wklfvsma.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eogcwlyo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wldhpoih.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pquobxcm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ewdxcvhd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ctigrwsm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3czpbnfiz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdtxcuiv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3grqqolyn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3agnoqsju.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxplrhhy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dejvjytm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wllnbpyh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kqkxunbl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hjfiykvc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kfohpcut.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ailemtsk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jfnwymfq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3idqcells.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ujytwyxq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gergshcn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uycndlpn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kaiiyqcd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sreovvis.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ieeknyfi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gmfanhcc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ukarilze.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3visuxasz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3oajttzln.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3abjzvfsw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jsayfkyx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lrlgulxq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hzmacqmf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3alsgtdfx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fiivhdbc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wwalnhag.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pbaxwaza.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ctoxrgfb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ptxzxtoi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cihtfexv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eusodqvo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cdymytog.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3udkzxvlw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lcexkdik.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fjxjogrx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ihyqjtca.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3oixhxrpr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aibzbhhi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qtdocxov.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbicoeoh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hjqakyba.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hamybagg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wavpreqm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jmawsxea.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nafyxoyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vsljzqgv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3stwydtnc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ynelqeyg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ghstwkey.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nxcxpugg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3inxageej.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wittectn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ejxuclad.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3tnoqpojn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwrclaig.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vhbrntex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjurnupl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zxvfaoke.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vstnskse.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zkfnhing.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wyzmeitp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iqobyuvs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yrrmvwua.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dkzuvocu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wlsvjqhm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3idyjzpmq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jvuywrnd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ocpdobqz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ihhrzuyg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ypsuqjyn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xoxfhurj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fdqutojb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3oinbohuj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fzuzddqb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3osrhvdoq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dwdrbdbt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ulobenrf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nhzeqohl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uwnbmpvk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nupsvrlf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wvyoiyvh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ogkszyzc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gdpajayq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xzdplpmx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gptwcuow.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3revostif.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wcncwimh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rktcxezj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mftvkxge.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lllbnsym.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bqhiysws.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cvturmwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zzhccfki.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3swsxqapw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cbxtgrmn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ucrxbgzm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3lzpyquvv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3eiwbltzd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qfqijpzv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sobbfrbw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fgcdpbib.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3txqhvrin.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jzrckkcz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tgxiqzgb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tzlcetyx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zxybslzc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3uvfbgkkn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qiskekii.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lezfdkqf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jzkqqgkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxpkhdxk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mfofjaqv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3grcbbfli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddwqpzqc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qugmlltv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gycoitni.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3sqcukmva.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ppfrkfen.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3krzvsnxg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tvxzlflk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cotyutev.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pysjhfzu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qnxczwuf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zivnifyt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3paooibjz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3duoduram.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vgxjrzra.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3drzivxde.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3hurontdh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xxvhzsjq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xahuaudh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3evteqzxg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wyppbqwc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3bfyztsgc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ajwqkxjk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zyjtgmsn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ymbwznvo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ghvsxtkd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3khjnspla.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mkjmmupq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oxkgdhye.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ixwixzmu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ecojamkh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eucbszyj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3usjaxjzx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldiklndk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qfrclvln.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zixldjph.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvpcwckv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xoevosmr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zwepihah.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mzydtzhe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ibciucgj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3kczkgyuu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nuyzeayv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jtmggnat.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xciqjyue.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvjhwpfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezsiwbjq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3otsmjfdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akbhqari.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3buuwugha.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lfiqlklc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gnzwsytv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uopvgqht.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rixnmanb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ldzbywsu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lecfavoa.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3oizmehky.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cbszhgxg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pdqaljgr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3klgukctb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hhlbpitz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vtdgntij.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mhrxpqep.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pfwjncjs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rdsizvjg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yhvewvmy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bkbdwvtk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3epqvggab.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3oakzkhyq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wleuildn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rolhsbno.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3njxjotve.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyehcvws.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3veibeyzz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fvahddcf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qyzdscrv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxwxphqi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dvfewjlj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3coawbdjg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dtxqjvng.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ixkgwygr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ildjeary.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3szfzbwlk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3boqlycvh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rabklgad.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rkchirbp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ytzhyrbu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ifrcqjkx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdwpdtes.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tncwthud.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kopswelq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nrlloqpw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzxbtgyy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ayqicilp.html


<!-- 参考信息 -->