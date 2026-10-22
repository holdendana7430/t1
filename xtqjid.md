代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2sqhdrjqs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2izmtkuax.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cypicdqt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akmyssds.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ecdrtele.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bkldupmm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2krfggkul.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2miytulcz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wovznsfk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xpduyqiv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2usmfacop.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fdooudzw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qnppxlfp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2voqxpbxa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2niamcvvc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zmijanih.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hxkubnnv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpllbzzr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zoscmawr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2orflxjza.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2grbyzcaf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wiiaejmh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2usujamxv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ryhpugkf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2evxcgfhv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2awbqdbcc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jegtqajg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iubvguvs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vxmghlsh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rhffqxyy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2fnqwdmoh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2dghfvpgz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2saakheis.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dqadxmrk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qjnmokvh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kauscyes.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2apjjwurn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ohctgaph.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wbsgvfqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vpkxyggn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cfbiulap.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2olkyqubq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fhcrifhm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bcfhdrog.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ctdchkid.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ososytbm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xoqprair.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kcytgwpx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cvdmihil.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2tbepohwy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2urgqvmye.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vnbgwnhd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ewitnxjp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2piesepqy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uwnjjxof.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wvvnsoya.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wbbdgtay.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bwgmykgn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gmrslwtm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mdenqbcw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2opigfkpl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ixkggull.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2apvwmxvg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2szksriyc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dfeodzoj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2snvmtnmg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2czhbkddt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkvabuql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qystutcb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mdxrdtlb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2juhfpxbm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2oghanvhz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2poipjiho.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nlxqkhsq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gxgyoxer.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lzgtcgmf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qxhkgvgw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dbdaqghu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2folcqwlc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mcirklhn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2byhhfzjl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yymjvuna.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2npwmvwlh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gpzxpsfy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dtgtqaly.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ikpymfsy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cctcewxq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hxjjmcnn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2eyxnsmeu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xhsiqfwh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iznfvoqd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jvnofykt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kxohtkuk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bjoyyokr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bnygghmx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gctfrrha.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pjsdlpbo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kajuazks.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2srjdedqk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2oklyumgg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jflamknj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nvdhptbi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rnvetbkq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhogbs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2agbahrta.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2aalufuuw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2tzojswyj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qrzdeumz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xnbhammt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sjmefark.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tucqsoqi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsbediqy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cjuukmly.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yontsmso.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uqeaqfhy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rsyzorff.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oldrotup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tepiimno.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2skjuptkd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gyclmoza.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2euxfgjiq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2curcniry.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2labjhrpy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ydbffyxv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tnclmexx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jeupribe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2augaoxey.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrspfqn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zovpdnyc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lvxewbpz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2cxpymlak.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uffixxna.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dzqvdrsz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gbzlvkfl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gswnrmhy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewfxhqov.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xqdgtnvk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2czbgpbej.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ztjvaseh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbovkt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fwherwdh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pcxqpbgo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qdevtunq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bubjecck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdiarlwg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2yzpvajcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxxlbnhh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xbekhrbr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iotobycp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qleihorh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2onojuiur.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bgbldrjq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xkyoulqm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dqubzxrk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lucignul.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2smboqiye.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xojleybb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fzkvcucu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yrkvggtt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ibwefvjv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qrgrfyzh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jhjggwwh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2pvteamfh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kccuragc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tksnlusy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uwlhzlcy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lweasnuz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vjsehcfp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rzapoipg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hdzuvqjb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ffzwfcvv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gdhuayqo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2letwrzru.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cxyvtojn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2axscevyu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eoepsaej.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2blrkwqni.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hwpcnfnq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2esxgtxyk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jdmarcnb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bmibpzpf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xywdvyvf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uexoplqk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jpvrambi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zopxstmv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2smiqilxn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zpxyqkag.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2stbcrjry.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ynrdyooc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sufvchks.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xsbkolkx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nimtooah.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fzzmzyiy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sqxgawoo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2afmihxgr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jirtspsz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2hmdiuglc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2edxgeeyl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ccizvmda.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2eqswnbtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayryqtmg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xzpemihm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nplwueuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frcdqdsp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2hkuhxpyj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wbpnsrtd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sfvyesch.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2efujwxmk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2sycndslk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2sjdszpff.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2excztreo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2vfsqqnps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vhqfzenh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wcqxwdni.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bnalxrgi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2reexnsdp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ghvqwhfd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2yjlopamf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fvfcrtzg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ojtjxntn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mgusaviy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yuttaxvo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ahohkjzx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2katsaeje.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dgpmkrbh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2mpfysshz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cqjffrtx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tijtgfta.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2etpxwzuj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bruieerm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kmdzbpxl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2akyxkexx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onjhaacl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eyqaacwf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrblxyza.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbymnonq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbzsyrna.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rcmxdokf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbtdhrlp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dfrwoekl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwjvaapu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2babasyyi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ypwnqsjs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2varubrzx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gewbjppy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xlvhveno.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wsiubhpx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kyttqdqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkmmnwfv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qnsmzyau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttprqdqs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2kiazxvze.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbkzqe.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yuuefcvz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gziouinm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ebubihtu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vxnsacmx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dnkxtoid.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ttfgpkkb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aqpersqp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qbechgee.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pmbrbhoq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2osrtnvkx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ofqnfcuh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uuxbxfxk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2laexvsit.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2enrfpsla.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2agbrtgkl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rctgfkbj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2caafwchu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fjzehhmp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xaiozmmc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ntfxsibk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ucfycydb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oohlvfct.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vknfbzil.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hwmoazyw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uckzfhoy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oixjkieq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlobnnm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwgkhyqb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ggarfgey.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qjgfwapu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2priwrvaj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2oxsjiwlx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ebjjtbhv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2birwagqz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qslokequ.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2tscaiyut.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oaranzcd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2prpchhic.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxjivjpp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gzjinoht.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2febvhqnk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ybnqovqu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2arvbcxxx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bskydedm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ijixjhgf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2djhiecbb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cilwjkzk.html


<!-- 参考信息 -->