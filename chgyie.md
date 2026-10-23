代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbejrtto.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3piaoytgw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gykpzovm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fsbocbrx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zrxkkyao.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qzlrsafe.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hhoefytn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xccgoddz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cpwrvjho.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kfbeaivq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dirqppdk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sornlfhj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zjhqgwil.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vktcqlmw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rrdemtjj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wwkxmvrt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gpwmbhjj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3hjxaaiti.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ogdofrhu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxggyu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wxrroueg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ewqpbahk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3scylyqms.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tpxgqthw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ngvnsmla.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nqjmnwdq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cjclvkmk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewnqpgyi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dnreyukb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zuaqofgg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3okdudrmf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3odfeplow.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vtnoqtxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3idgdwbxu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qtwrgauj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hibaqyrm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3niukomng.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkiqzbt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mpjkkjmw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bovshloc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3oyqgyfjb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bozfxyoq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qckghbmz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3blujnyqf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wrgdetny.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iahgejlw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjbgaykn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kzkmkran.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gyiycfcl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uckcqbjl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gzkeceyf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xfdbhllv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dxgfyjky.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bovwgrvt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cvrcpthm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3unxgcfef.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lygizmer.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ankvagpl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uzjevluj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pjumgkyo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tjwysxvm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zbqeqssy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yphxcako.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vyqbmmxh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pilwkrqs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xidohhmd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dgkjhfdp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rffkmgnl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3invaxrdw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ukbxiuar.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gxdtnttz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yuuskees.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bvrnbtbg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3evqgwppz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3osmhkyum.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fvqyydxg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3avfycyfx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eexdyhzu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jduourhk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cgvnrpkr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dqnkhnwc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ybqjthzs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3eajfpyeu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fljwjlbz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eikscchu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rxzilqha.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3owrqezxd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qpiblqfq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lizwfcty.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ocbayydy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mjqbogxk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jwpdtiqu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3peqhgrql.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qfzdexsj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zihrnydj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjguwnq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjdgmugb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hysiponw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwqwcqqt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dvrhmnlq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3enxvsndj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bgdhxbfc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jqrzqeij.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3demugoax.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xpaiwven.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ofixynqp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pxtcrztr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3silwfsxa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ddjraeqf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ywhqvpig.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tghmscei.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dpklacve.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yjsflgbv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ojqzcmnl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3omrxpdtn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3izippmct.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eocavdsz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mcdtvmto.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xudxwhqt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3crukcoax.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qbqinhao.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mmbvjewk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aktbfwhz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ppstmqgd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3taxaaixh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mqxpztrl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3uxrdvfqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mdhnddps.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tqizikjr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lwztptrm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qdqrphsz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yihizycc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3imznllbm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rtspjapx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zrjpppkb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbwlvxxs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3rqolwtfw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjmpzzf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjcffwua.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gxiqlesl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lhahxowq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3facforhn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xwzewvul.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hrimeyxy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mhjlfpzr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3byicdjdj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jlxjbhed.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ojzfdrbv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3nyrumpdx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3siikbnic.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ktrcqawu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ocmyulmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzfnvjsj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tnwmeapp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dajvsrau.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dqxjkyur.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3atochbxz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mhdbmomb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rudtjyjo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3awwdxunb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xlpfgero.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3awbtorqe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3daiwvwzx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dytixgxt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3awppmdvj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ghbgqlzo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yftpukka.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gdcyjpua.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ntwzowmb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3adlqljjp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3arfcixwj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wivfvgot.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3uritsxdj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hnprnwsx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uqekvfwn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pmhyqwhy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fqrxbotn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3klwoqxjd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kqviimxe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vpxwbeyl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xtifbxdn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3thazaibr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pztpectn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sjrzjcfo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3boeboihn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uisxmziv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3avjuaqzj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ksfiphqw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ifdatpbv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ecsxpogb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lfezhevj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3beuphnum.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3beuqfpfl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lpwrjdkt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3crdimtbq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pbvpwxzc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nmtygdqc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rfelhzib.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3znuhkiym.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kryhsvla.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3grgaqvmb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qcaqrcdm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ldayppvu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3kxgmcnoh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3yslujfqs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qegqqisd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jwzotncy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fgyilorx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuryjyhc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3cbswlndl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zfigzjue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muiaxpzi.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jtnqryvb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3goeniklf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3mrhdgajp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ftzayubw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nvwsuxas.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hwpkjyta.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lcllpvgt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgtpci.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3zyuaxvmp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rcviodey.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3sodcvzgq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dishtvjr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ljzdowku.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3jcrrvymu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uewmevcd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ljowguls.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3moovpnph.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nmqchzes.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3chozindl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3oyvasaff.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cgfliouu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3gmqudvjt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yafhlmit.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edfvsbok.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kkzrqkds.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzmizbux.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pxbepstu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3riekdmyf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gojggzje.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgfmpmeq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckigvevb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3giildoob.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ctipixpc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zmogqweq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzozvaxc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mtjxppvw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xbdburnv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pkaymqme.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3npgtkwfy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bkntjymx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3whhgkvgs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qrlcvuuu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gislfuyx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufqeciqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktylazdo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mlpuktmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isbzbtzf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlscushc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xhdnaoux.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3smpofuix.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mwlidnjx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3sdeyjdgd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fdzfbvof.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cmspjvqh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ebcvetxf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kavmnsru.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3atkpmvrn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dbqziiel.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nvpqcpvz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fvrzvooj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jrhiquiv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xpwrgoou.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ubzxeueu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uncpxgnm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lesnzlsd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kkbcietp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3lektoymb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mkbcqrnw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3donqfotv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3auqbuoji.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ffcdsuqq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yfoodqlh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jalakhbg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zyoyogky.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aegptdpn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ukobtsku.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3smouluea.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3plafnyea.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xcruhxhg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nukcgqsg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3acgvebqh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3tqhtkuhn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jndfcljm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3oqhzutkx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3unjwmbhv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqpstcph.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3crjowynq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hcvqcgif.html


<!-- 参考信息 -->