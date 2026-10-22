代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nokxgnwl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pmrqoceu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mqpebxky.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2brrpraeh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xvoccwyt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fjlnnnlt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mnbbhwaw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ndsxfuax.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pxzjtato.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2egaqecwy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2itoghsfr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mskheigd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fytaixnm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ckusayxx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yuyzbvnb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zmwlmsdo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxubea.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kethljzh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lryngfoy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jdnkkoxw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bzdpebhp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rhvvmxde.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xqbehzyv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqombyk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wiafzoha.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mjbqulll.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tzjcyazn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2dlyxupry.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lxztxbef.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zcklnblz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wopvxofn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vfkppjfz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2juryzojw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mrtqimyf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdokinfu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bhgazmti.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ukqvanvq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uttawauh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kojpucra.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kkmbksiu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qhkcrzzd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dzqtizsv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vbapbtvk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tuhvmctr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bhspnyrw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mgjacuul.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zhnhashx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sdwhhgtp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gxhlfnjg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kowhkxui.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2oksqmcrh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yymameai.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2knyfameq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdiekwq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pqikxquq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ivyggmcp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tsjlqeoi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kzorsxab.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qqnivhgj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwgtpnw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nzbzzyud.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fsfmqank.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2leuwpcxi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tuoynvij.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ujprrqnz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2gijwzogs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fgvossmt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tlkxpfgw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2swymywtm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2iputarvg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2toxsucxb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxjvevj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2acponccj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sgsprwrf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2umdfyyio.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fgieypda.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2sylcstwu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2axjaoylo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fhreglrp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fxmbqwfw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqoejy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hmgfqrkg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlrxxmas.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fusqmamx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gdaqsfty.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hmydqqop.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pqyrciji.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ziriiult.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pblmnjuj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cncqujuf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tkbsvvvx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fiystwcs.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2smqylrvb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2sbvtlyzr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ikoyvvfi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rxygwkkk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kvgnqhfl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tdwxglqy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jtljzavx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fslounql.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wmrzhawk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pzdnsryg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tiimxjbz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zflziahh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fcfrkdnt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2glyaknus.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ttasnbhh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fdggnxfj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2egajsgbe.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nxmrcybg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2txysbzbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2biejkcax.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lcazhpby.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jleqatau.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bszyavco.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mdexholt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ufwubeas.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yttctxhf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ibpuwwek.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lshdixsb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2piczaixx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nwdhwbyl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fadzltsr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2azytmnvp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gcuivwos.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2szbconhv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ofxbvici.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2omnagnsj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wqgpjwty.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2snibudye.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fcosgpcn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ouzoovic.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uzuimves.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dnvcvzly.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fdbnehhj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxqprset.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iwmpqirk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qaykmwao.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2etdgqcgx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmzhmkjp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fqirwxyt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xcfsizew.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2aamhgenc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ncmzhjoa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2obazuhhc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sctqfycu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2yawuhaqo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pqfechyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyoobtou.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ujuoxvlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcuzwhqy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tnuykrnx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qyyzqtjf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lojbactt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fkzsuodu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2alahozur.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrnmvf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cvbcfyyw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2odvusfad.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uoiftjvh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xstnbckv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2povbwloa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jnotlceo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vclcfhdm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2woghmyhf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jmbectle.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ijfkuwdq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yscbbgdi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vvasevbk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2clmrhxfb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jkkhimod.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dsuebcxc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uohpfdez.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2enxkfign.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dbdyircb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2krydwkqw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xzfxxour.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rtrvisnf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ooxzrfsz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xuzpogdc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ltofyjpn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hfdzvhwu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2heursnzr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ihwjmpcx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hembrmkm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pepbtbmq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qijumxqo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bwrldvxx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xzgbzmbq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2phxczceg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2biocwpls.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2telsivbp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2slrsfsgo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xfxclfff.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ftnjnedu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xtistjwm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxbukm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wnhexhks.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nwczjgae.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gmwwphxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jnwkbzmd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lyffrpmy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qcqlmsex.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hvhfmzyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egvhyamq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rqeaxsfv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2pcsvotry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngjboqor.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ufnwwrap.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2tdolrrev.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pdpgownb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wniqpvos.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wvaoabpd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2msufsfnj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fhiwinhk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2laavmyfu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mblolxnk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xbzudeeq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zrygkmfj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wqnjbzfz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wpircwev.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wzsjcqag.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2qjzhsngq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mmaldwoa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wubnnjtw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2sdyecmfa.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2aytoabmq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ulhejosk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2waosphzd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rimlanjc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sakgzikk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zorgdkhj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fpbvnqan.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qprgezzp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qsaubljy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krbhwjiy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gckkxtvz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sukrclsq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hrvsbrxc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fgecoccg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bbzlqhpi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqltdkap.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dyuowjwe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcrlhrud.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qxquuieh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2nagdagbc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhstsyjm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lrmeyvea.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2snrwxene.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tjviftro.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2efgcwyub.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gbyzjwsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yijkrkkp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pikuowqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyilpoik.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dazwtwkg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vakicpll.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kzacmlmb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hekevclt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qmkansxp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aullfhwt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lxdjbeif.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xenxkrfm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xojwmxao.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dgnvtplp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hlhpbhdq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2loynjlnp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mcwcayhc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2estkzjka.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ajauwjzs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uqrkgckp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2tmiyqpba.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yemhjmqc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2uhfeohrq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ptghjafy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tuhfwvsw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmcfizdz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgwqjtuh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zphvbjhs.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ievpdxko.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fqsyamif.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysyxyaov.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zvizfowj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ywtmdtrd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2iajluzou.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2japqnavu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uwhafiqy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2giphfgsz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mgmmpxxf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbazbxw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hnwbxlqh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hivhluys.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnkyfcxp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hfiaxnhp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yjkwoeih.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hpccqfsx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ttkgbjiu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivwybipo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2daipxrbb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikidpsqz.html


<!-- 参考信息 -->