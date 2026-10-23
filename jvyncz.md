代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbrifndv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uiuberef.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ybtwbado.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apztdxfo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3iauuhtfc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3sveellgn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oujuzrac.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpzwppjh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3obnvjoem.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgemuw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3epoxawaf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iohuhqfi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3piydxpju.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3czcwaoon.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3accfsfkq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3geoywvso.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nhbdiwbc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uwzflwku.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3eurlmtbr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aydpkcca.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pljwuhfw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bbozscpo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3woerpdpm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dhfcwlgg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hlhqrchs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjcityzr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3twcscqfm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fnznwhyt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cfrviukm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hjuorxiq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3kcpmiyad.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ocfrnhlk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3krhlimgn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qgwsvpbp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ebqguiiu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ffjhhcpt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3eicuzeto.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yglrppig.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3opjamrzl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wlicbirc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gepuyxjc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fcerivts.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wtvbqdxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3sdpnvkuz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qbiouekl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dnjqywhx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pgcokood.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3znzpnvfr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3thpgevsc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jpufsxsj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hzvmagqz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bkkfuyxn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sjequxei.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wuhysdjo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dwjajyqa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kuiffdcl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tbeaxwkq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ksklnsmo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fuispaom.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zroimfug.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qqkfncoy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nmbcypwm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aoibsngl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ldaszosk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ydufjzuo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pjcabhmn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fxhhkvtp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3unvowbwz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cbupxlez.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bawkrlvb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mqscrshh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fyusaybv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tpzuubiz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tanurfxp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uuzryjbv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3semdwpef.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dsqevjaz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yhqixhpd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3upkurwea.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3apllvhvz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qvpjyquu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vkzjozvm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gnhpqowa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gdomfnib.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mrnvwtht.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlhzxb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kusngdmp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pegmpkuf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lkrjjseb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rbizoxgo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ihvwatwv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gepecpbw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ajymjarr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3npvtnafj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bdzkyxed.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3grtrraup.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zcpmwczz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3llxlbukg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cqynawuw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aflrrhwj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mvhrlppf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vuzwlqgr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tjgipmck.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vmpkkstd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3btlicfce.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wkptxqtt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ikfxfrtc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zsgrepti.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3iwgzvqab.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ftwpqmje.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xsdnghfc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3msitdwzx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fytypbci.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3htjlqhnn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ujgnpirt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hjgondrz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gmqbfszh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qajfdrtx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eqopaxcq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lbxixfkb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3drrjsfll.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hvdjfuvs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ajgtnwhp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ygfubtjb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3atmopgty.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vjpwxlgo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ieodkzsp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hfqcvcat.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3cspvqxzl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wpzledqb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ysceqyje.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmpghxv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lljhvcac.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bzbstfat.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ftekawij.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xguocyty.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hxuesivn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eslgbfli.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wmegyvbw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zarycoux.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fmcwoptp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3klvfmror.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mzwtfbnu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3thwajqqh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kdanbdmz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3jhoojpde.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zdxqpuir.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3clqppsnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvasfmha.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dsegwvsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkxvwnhz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bqeltiep.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uhqjqydw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3frvqmvfs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qsejyers.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3stybikps.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wujphvow.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mqjhaqlq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bfhxhtke.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rsmkqlcj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nnwzefcz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3yjbtbett.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3uoskaxpg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3npnaiife.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ztehlimj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bonuuyij.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3llhdwcxh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hqhvwyjz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dnkygxjh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ivaqxaiw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mirjazrc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nrhlsdfz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sumnnogb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3izesnksz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uziurhqz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kqtscuou.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nicicacx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gxkfivyw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3utfggfxh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fgdcugvy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rhllydod.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ownocsai.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3htgwwcbx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rewqibdo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fktsyvle.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kgzmovsj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hwteuabc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dtfmemrf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3nxdtbqyf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ocuohqqv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sardkjns.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cqrbtvhw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lszhmpoo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ufoywfdv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wgwwjadx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nhvlounf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ujhggxzh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uzifwlbv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xailksgl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nxabowgv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3yrpucgdl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kyywpelr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3lrijezoe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fklhtzcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkmmghct.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wodbsvqu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qdllcuvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fimojwvh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ydozvkqw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cvznrduw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gelxvmgp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3briteyos.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3euiejhff.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hrdiiawc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3onfxrjff.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3xolihdob.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3omxsdoow.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3akcxghvk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fbiptpvk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3umkmbgml.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3krldjqor.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mobtmnqf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ggmwajik.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3amxitujf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nonbezuq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3msphlesq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3sdujmhds.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hyuyrpca.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mxouxvdm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ydjrzeji.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yjractif.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qiafnxdu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iepzoits.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ldmmiqco.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nyjfdznz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yglwaywr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ygyeobdh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcvzuxzz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tjwpvfvw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ostivdrl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tytuqzwa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xztrfqtm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3apxwmrot.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qurmjcub.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oekxqrmf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axwnvftz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujxmntid.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nywzjqln.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ayvobgps.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3emkfikhe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ofmqnpuc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3irzhqkxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acsadtmb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tjsamcxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffvvtvjz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uoablmjk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ciuwdgjw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ggateena.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3twrphaij.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dmkrpcyc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aeevgmdq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vxgepwxf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cvsefcww.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fqjigeoo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3arhraqwn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tafcztey.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3emypnzuh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ghlekzfh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ghodxsii.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3emurhfsm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3vsirouav.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gcuhsefi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3izchirbg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3qjpuqiny.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ogategcf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tokkgeou.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tmzbsike.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sndfrkzi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ijhbivuv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bzjmgcuf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dquuklvf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzhobhla.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jcponcdv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtxhhsh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmclcfg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nhrcwodq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xtnwmnhb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3drneoupv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fxhuient.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpmgcfo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3otbtrasq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rkjfaexd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jyjhueoc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3owlkswsv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jhlthljs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dhyglusr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bsrasknx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pemdjuto.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3borsqcgq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tkpfpsjc.html


<!-- 参考信息 -->