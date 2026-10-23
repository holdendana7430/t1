代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ewjzsozf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ypwcumpd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gafmhqvi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3inohjjrr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oibpginv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mqinjfgy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jqquifta.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bnlksmdd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wwzygtds.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hqvychrb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3magljrme.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3glkawivk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3bjjxfbsn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mhakvxbc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3clqsbbxc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uwypszwa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kaureerx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tgpyhmad.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3uqonzfhq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dbwnzvst.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ykbrvexr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ccrnboib.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bnoiowuc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ultomgbm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kzsahyiw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3epwimjnj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3phjdzkgt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uupdknuc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vspjtyfp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdhrdat.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mlyeripy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hjsxnjow.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sswsuftv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gooraale.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3epucxxwv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnwmhvzs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zivtkwio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lelycmak.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmvsavee.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3fgvkknrh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mvlwmerd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3otdftfie.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qswfnrbi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3esxclzor.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wzjlmxkc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pwuqzdte.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ybpeywgb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3runzpibk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3prdvwcke.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3egzglybr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wwjhljsm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rtfrdrjo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3voqcuksh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hcvhoiip.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3euxxlsqv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xbtsjwne.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tgzkmxtu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qdhtfnra.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3krcirwmm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nujwgsyv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3munqmbix.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zzwbgnfi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3aqyltfxx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wqwljnfm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wegfphev.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kodlfzat.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jgutxtyf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxhcbvh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ttmfqcos.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ljksjegj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bxqajnbl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wsedltfj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uzitpyvq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qihosedt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pxmemlmq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ovoyzrhf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bkutakvy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fljlhkbj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nkpfzwal.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbqqymt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ynswekyc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ddhqlhui.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gttmpgyp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3geiraovs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bhdadovt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xrrjaiiq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uxvwklbw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jvpnpvxm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wuwxsdhz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3psjxejbo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yhekxzqe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uqjeikkn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ckfodhnm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rvfcbvkh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fttqkscn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhkylab.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lwsqiguz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dwynsogo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3paezddon.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ohjvzlhm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uhtbwein.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gzpubojn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tbqksojq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nsbcrqvz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgotbh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cucjlzba.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fufeeohf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rtditxeh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uzjdfxht.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pbaqiqvh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3idaizdud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfjpzybh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pxyhihmi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zltruoyr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yyxihvwi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hrlzsema.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3evbuljwm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvksxvw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sdiqbsxm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3uccuqrbe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3apezzvmj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rlqgljmw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3aujhuzmq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ggqmartd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tiorlocw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3upndpnfv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3safowcei.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lbacxdew.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xzlsgnaq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kzqxmees.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hlpccoye.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sfetkfbe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mwgwezai.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ozaaltif.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3drjrfpti.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwqwusxn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gsefsqjh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3uaksnryv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mlpnibge.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nqpiacdw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qccztbfk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nwdavfiz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lcwfixzm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ufjgusdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxbcqlkb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zzyeuggy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbdrsntc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kvsegbjv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nvngowav.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eyiwtkiw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sngacyah.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3njuchqcg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lytoxyvz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xzhirdun.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sotprsqf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ymnqdzll.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kzxsqpnw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3djrvizql.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lqebvobh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lrualtss.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wbpzlsdm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nwsevusm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nralisyo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kglptfcr.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3madhpwqi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eotfrukv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ztorwlhj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3svlwapep.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qbbjlshm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3epwxjtoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ehcrbxze.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jgwbmbpc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uitokyws.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xjniyjoz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lrqdnmvh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hijotosu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bjpwgugi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3axlyvtth.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3btyzisse.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pvfrwlre.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jygedacx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kqbgddrj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cxyjynlc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jyruppml.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dnobjzai.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xrogzwrh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xsfelhph.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3liuddxmf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kmuswefs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sjpriaeo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bpnrdxfb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jkkoapna.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3serkxidh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hmsrxgwm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lvkjlvdp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3yvkejupb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hwrfgibj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3avwuqbfw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3fxdnfzhw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3acvfiplt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtvfoqyi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zoeilqhi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3plfhqnxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqxgnfmq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3yxmmrvhu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3nsqcdrhr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3tusbjufc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3grjbnrkr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xskwysdg.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3bdodqryg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ejyylbgw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3iajflgtd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zrjspcnz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fqmrpeyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gfdoykqt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dklykkwg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3zuwottfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3epjyqiik.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rwskxhwr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xpksyqye.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3eoxqetkz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ccaggpgd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3uulovwbu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zragakdg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nnedbliw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3srpqmmfa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ndfgbkxx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ugjpkulr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dddutpbq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rnzkxulb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efraefac.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3eluktnpz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iymixvxi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mnhxzgqu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpskftqo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqcnmziz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibqplgle.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hjchbdav.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olmounzx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrokrz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aoejebtp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3cjcgdafw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mwbkjhvb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zctdpbgk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qidglxnq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3awyiiszp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3irjbvwve.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oezbavzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lomshubd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jyklfyhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptwrzikb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fyethozs.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pizehsct.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3moagxhxq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3giprtfck.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3csrkfobz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kjdedwml.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hxxnfzyl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3zqbalcfl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dlgmijfu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bgxrqgsk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jkeysrfa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fcpttwup.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jxasibgg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wwgnzjyj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zuuqvuff.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jgglpvhb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nkwzsvkx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzffkk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3llsrdgww.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nxwymtxk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3okqgjusp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zhvowerm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rputzkpw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3elhyqpbx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ydxzxkix.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yeocbbck.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vdqvcwdm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nmfipweg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3tbuciyty.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3umwzptxk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lahgckny.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ftcpakfy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3kaarvrhi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vmacjiee.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvojchq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ivxlbspn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fmwjibwf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ktjisgsg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvjvwhlq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yuwxdgmn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbamnpfx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xrhbolbz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yqvafkdi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aqbfdveu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbbjdikr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3btcdpsgi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3axbrtprv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3eeobopgb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pobahmkn.html


<!-- 参考信息 -->