代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ehvfrnal.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ydslflqv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kqxpkjej.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jiaweygo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qynbessh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vvgiuell.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvfyqb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nqekrwoc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nluxpmht.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mvagsupm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rnwlgyyy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3izgsmxel.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3voswrkui.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cdivwxlf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3daojstvy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkqkfmq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3szweshoa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3carakowu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3llmjfpgs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rodnqmxm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ekjnvrpx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wwrsbdty.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nzoqnzvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ngffknui.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gsutjspg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mshxrlgo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wpiwjicy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qswohmns.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nzwnphst.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ouakhhon.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hjshsodb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nfyecwds.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hpnytzme.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ldaluqrj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jzaigfec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3sapaxuyn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3noyngpjc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ocndvpax.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3aevdobly.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3sodeclub.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3slivdjyq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3chwwnoxk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wsxzxfai.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ckjxgouh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ecorrcvn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xeiuqyki.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckmuktmi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wbgtvduq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ftldwuxq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3aqxibxyf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jalrupce.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iutbghic.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xmpyqsjb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vqeftjgs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jouhnrav.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nbiusuzs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hmgxbryk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cynmdjzw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nmmorlmd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xedommjz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3anpbjgtq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vdrsqsiw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ijxhzwwa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tenavxmm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mnqbdtkr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hdbdjjor.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jcnzuctg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3sprluwnx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hmjxkosb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jdagrftd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3fqipyvgo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vteandoe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jsbeihyg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dhxmolee.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pktqfcye.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mrytinbu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tnutaasa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3emmtuzvg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3erzajscx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ivfgxoll.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yhgkidyi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aknecppd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3waozzeya.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3popjgjri.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sntrjvbd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfvobb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3adyaldgb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fhrxsoqk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wzzhwddd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oknjidji.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwkwmfzg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lloywfxj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ikzclyoh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dtlizfcm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vxsorqzs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fslxtquo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rzpzlqca.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ikjckeee.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iihxjzdc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vvqqwykq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3cmulqpgk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lveqdidq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ujygodrz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lptjkgqr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fabintcu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ptctnjjh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3biyqgadg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cflnfkgl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tjgzmakj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3txwelspp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ahibfszx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dgtatmyi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hfmsvtab.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ymytjgmx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pkgrfojv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vcuqdmfs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wllsvycq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3degdcbpz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3xnlvnfil.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kknmrinj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3voxbeeyv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3alogamnq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3eyfbwoff.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gigkakcj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cpjdtmku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ieyrfwbc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3bkenbqwo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nmaglohm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3stlzofmi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykzhhtuz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3scadomdo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zuovgyia.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fiyguepi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3frznlick.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3adxcrvvv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqxplcte.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3peuzfbhv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vmqnzqbh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3prudmxqa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nrrjxjoy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3geqpkdxl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lzfcshmv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lovaolrh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3buloseuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ungmljvc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yaspjtfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnwwkiej.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tzenqkqn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3weccjigy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hidooall.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pjyvuais.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jahnuyfb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zokuelxv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wwcggxid.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kvunokeo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3plztpifx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bogthujf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xbxmrujs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qgpgvacd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3aoytnbpt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tdptsexm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oiflipsc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xojzwdqd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lkkmovhp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3komchtvg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hzbhmtgg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uqbtfcxu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3pxblskph.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ozjbwpri.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mbxgvqbf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zbreyhkn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sqklwisg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wsucqjmu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dzchxfub.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wbdlkrfz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cfkuxgwe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vhinibes.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qisofckg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ztrxxfkd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yweqnotn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3szfjhvso.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rcqekety.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nwsmmqrv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lmvwlgls.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ryarvysp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mveeciwb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bizsfvbc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uffshfke.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3onwlkeno.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nmhagtwi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kodxviuu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nijgohuq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rswdutdy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jvfxpsro.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3etlpmcgq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vspsphhn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3xqcondqs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3fftrtpay.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zdyintwt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ftdtmpef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbjtxsqc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nlfbipgj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tqnkhsxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzraujah.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkhsfv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3znghqicy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ahevrnmf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nygditwz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wtmvvztq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gapqbvbo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3jdrsgfmf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pfgputvl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yvbslhol.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3reyzrldr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3sjrvqwas.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3mxfwjsio.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qezfgqdm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3aonagkxs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3tqgpbrtw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tgktlqjm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jfuxpryp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3pdgdelnz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3rgrdutds.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fhgwrhoy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kpehdxqu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3sqzpvova.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jweedkgq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3schsligh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3khbeanob.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3meiursbo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ekwzwvjn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ozjcqsmn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3prudcsqs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dwsbdhsx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efipzypa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qdxloyop.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rhpyrkcs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3phkcurpf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3buxnfhem.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qwkbwgbu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cximymlk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frqkbfdl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rtocdrvx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xcmpapnh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjlzjwah.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fhigofik.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ipisqglg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cnyxkcub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjqdimhp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3siomvxvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojtoftxd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zmjkufcu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ebykoiwy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xvvdayxg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3msxxzezi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pkjhitio.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qjtaorjq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jjopedzx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vrdmfylh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tiglnktm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kbpsesdw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3thyokjop.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tgsddtut.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3baapyccg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3sjnhhpar.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hfbwvwmz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3leekpsmc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3buijjiyc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qoajzpjr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tncmbyxp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3avocawss.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zztuzzis.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iddvdaqg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbbybc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pjqzebii.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wvdfyxef.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xvxllhrk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oghdsvlb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3schvhccb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kygjvbtc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdpynyg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vadmtlwn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mzyulmcx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ircmesar.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ysvrpdsy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ruqnqkzq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xvkmihks.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3odcrjdxn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofspenxy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zyscikke.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofkronax.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3znpsydwq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zojfkcmz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rabubhpy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3plhybgpe.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3heoobijs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jhjyyodo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vytljerc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qexvfqae.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3eayulvvm.html


<!-- 参考信息 -->