代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jttrqwoc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lgznfqos.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yaaitvwt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dpnacmeh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qpmlmzph.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zirzjoom.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wzhjaoxj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaytputi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xraehjsv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dvjqkute.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3shntwpbj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3slctfsoi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ziprvqnt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gmjucvrd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sewuvunn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vtgqjihm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tqjbmhro.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ptlczglf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gtnpurhp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3isuzdond.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3axfwwuay.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nhuidiso.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eanqcbvl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kkhqrspx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yzybsqic.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3beiscjki.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3trgdsxwb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gwjbcelk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mfpdbkme.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zztmnkco.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bmyusjvk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vhazcaxh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ztbhdzlm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqpqogbf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mtzcstvu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3aqqvpayq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3orfvjhvm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kezyvhxe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eeibdfvn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fmatxych.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ylyrqbcz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwfipw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ydkccyrj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czmfygwf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vkxsniff.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kbznuzth.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pjapgoxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nofzuoqb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ektmkwlx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lqxlefmy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wtbnpvjt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dxizrhcc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wujgmbca.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qjrzxsdh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jicptoqp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qhryvmop.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3smxalhhc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbfolw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xnxvznoy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xuzqsutt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lcpgmxnx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ahgwqrqe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uoeqroiq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3crxyvvks.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nowygynt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ifvngmmg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oppbvvyl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3luzbwptr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xwpurbbt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vbouchov.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kxojzxgs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3htetjljb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ejgovcdb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gxpzcdyg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jwzdhihw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqmolnt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ycrqyzfd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uggukcpm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cmlbeazl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tontodmx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3oaqlezrd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cgjqxjzf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ztyqizdl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ykwkjczb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tilfohwt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jrulmysl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wawovwpa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qauvltry.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3krcmwfuv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vuthatcj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ityvrmvh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqerkwdw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bfczesbz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wjqqqwyt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3krmntgum.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaominzf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmdxbaym.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kbivxqtt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hmpzugzz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nrygcemb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ljrryhui.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hatnulzw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jgikmocp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zhojdeec.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3oqajncwe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zmynhesd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pdpiktzh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kmzeomqa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jptusava.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yjigcajw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bidjdzkm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xlultgbf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kdypyspz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mkgwxlwj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uzdooock.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xirpnpfs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vsyrcwns.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zgbheycv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3imfczfye.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mfchkgnl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rnzdywyr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ibcxjsha.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ounikxbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eqyrfmgz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3amhpmhvh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zrunzymk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3zrhgmoai.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qjddpylz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hxrptbms.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mguzfwkn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ugopigwb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nrzcobfq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iiatxnth.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3brykpfvh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cgtsunez.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tmwxchik.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zucrougm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gfiescyj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nabnbmtr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rskifond.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qokcbrev.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hdelgkwb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3waiavxzp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvudhnlf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iosboudg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xicgyvhi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dhzdefok.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ybmuofys.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3etwvkfih.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xbbzfgfy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3smjakovy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jknttunb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cidgygtk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oayfaeax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxmbmwas.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3brrivcle.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ubshxsvw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3savrwcpw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gjkoljps.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gtbwnhou.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3owjnmlcc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mgftyjab.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vmrjuvds.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rtabuoyb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dulqcbzj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mvesugts.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ugfrtiex.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrfspa.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3czilxxrf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cipcbthx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3apekccvj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qqdnogne.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3isgovxby.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rjrbdxua.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3brxuuvgn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cegdhkqh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zzklnbyv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3osmgodit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lktwvrgh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3iqxbjxdl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rgqewgug.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3aulagelg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hujukwcx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jzuizjjb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nblqttgd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zwkxifag.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ipgsjvia.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qcvxuxwo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3htdpndam.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ffoctzvb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ktlahdii.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mppyfeyb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yawpwpjf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3wkjfojyp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uolzsbzx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fsndktek.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3rpvloyve.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3egxsddgs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3okhhgyxk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kyazcuir.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hlidjwow.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iqbcgpcj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nbjszadt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrbvck.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3juzjiyvq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3eakjuebl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3okdqchqb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ydzcruks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmflezzt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xmcuogun.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lccqimna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydwgxksm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yxpmwcjk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mctmlaeh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wrovtbhx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fjzcxzaj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3lztaxeuj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3uysilufp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3yooczefn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gnsjlahl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ymdoajff.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3iwdrkbcq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wlxcrvkn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wxfeuzje.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hoexioex.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3szyffias.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3txqcpngw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wzxkrpou.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lzekdxpy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xnvwrahm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ygwgyzgk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3caodvdeq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3urkvbvpm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3gcragmbu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bbzxpdmt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wymengbl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3stvzeyhf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uyltzxvv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fmxocscv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ykxdgyhp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ecrjgfjp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zztmdrug.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jbekkkhu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wezfveny.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbekhufz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kmmrccpk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lpswmpcw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zlbwkaes.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yainswrz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oikueizd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlevnfcz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dgbjraua.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nmvazblt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btdcnave.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bzmdkrcv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fbgrmbpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnpvrztf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3votyagkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icwaqnnc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lymdzujs.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yaebpihq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rrujfbru.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rdftrypz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3kvjjqmdk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dpppwuho.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3syjppkeo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nypbuwhi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dsnkxyld.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fwhjsrwq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qqnioxoy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3prckzsce.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vxomeqwo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qsfmazol.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hsyspvxl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3lmpvzcdh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nqtkcrxr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mrlgfmci.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jeuxqdkx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xbotjtoi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hwjnrdzs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3viuhzkib.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bpiklwte.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vvgjpftw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3yipqmpkv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xlrbnlbb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ujoopmjw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvquarpd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kkidtmcn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zuymxctw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3eotbixfl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fijyhkde.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bggyfiht.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ksccjxnl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3tdigfqck.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pimgsgeg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cyjpjdjn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vuylmdpf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zxybyrho.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3orqgnjaj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3crwbgmle.html


<!-- 参考信息 -->