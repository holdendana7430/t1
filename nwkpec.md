代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2loxcwugh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eozvytjf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mwarskku.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2takyulwn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nnwvejuy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyksnqe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2idzmqesi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2exdhubhn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2onvaanku.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jsiiidmi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbkhzg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qqqkbhpn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tkylvxpg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bpmhjqqr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ffzhgtis.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lpqsyyig.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2notqwsoy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2iylqhwhx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lpkknfer.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bnkcyurc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2husxjvjb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rpixtpfq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jbpdhbkc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2xqcwcjlm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rsiuwgbp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2skwicawm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2plctdzgg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2keoecgbd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2suldzpmk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hnkdaeqi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eiyqaeaa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ukubteoi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ndqlerfv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hskasdto.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lpyloajk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ullerfwk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ccvzonsr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2omvvpmxa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mzxtorsj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vcvltxym.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2arqpbcqd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vhznkykx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrjiem.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fazbbmcd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vekyihii.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wriyiqzz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cyypmxif.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2isfjzrvi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qilqjkjq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkgveyoa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qzwxgnha.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2egdvvvan.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mbifjqxl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sbnogopa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jtzjrjvk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xddghsdk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qinhifrm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iohdjogo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2syuivluj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ricmnshv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cgqngpoe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ldcxpcfu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fbmykzuh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eolrowdo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yjtahjni.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bkezrezw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2widcbdyp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibbmthyf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwmdygze.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gkfdhuaw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2huwnzpsf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bvgkerqu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qjthzyrx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cqnqezzf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2thjqozzb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nrbzllxt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zjzkgkjm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kvdcvept.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zlywbzyu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sonegwtd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hsacrnvf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pvwmaxdt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2afecquyi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qrmaqmqb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ilhpacle.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hfxgvigp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xyynpubt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sbkphzfp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2knznsbdx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bugmshlx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fbqpjyvl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eiijdbos.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2axnzimon.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rijcrxgi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hbdfvguw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dxuhhwxn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ltqiielm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xnmwvzkl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ltejymqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fjbehfsa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zooidwpp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ohhzkaoz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2eacpyilh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xvkzntxr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zoqjfpfi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yakvcwqp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yhbgbatf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vcnpkhgw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ralffhxe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enmyjoku.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nhwworoo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2obtkcgos.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ugetoyix.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2axuugoqg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2tetebqeq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eyjtndyy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zbzilsva.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sgitlbrd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jjqgzcfd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nyhdcgeg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2goozrqpz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mwlxxnxc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ternbmra.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2txbchype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfgrfict.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mzjlfcrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdshetzv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hbetobnl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nosntzyf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mitllzml.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2alyaqggo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cfcoisqv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2klokkojz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ysdmtztp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yqltonyf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jvzjcwje.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kcxzzlfx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pkqbliti.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2imxkozot.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zyljilyg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2keobmkoc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2somnvacb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xrakiwqo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2simzflpv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2llbpsaqe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gmshjkwd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2buknttts.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gcxuhgtg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zjbvqqlk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jlbskoha.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aloulrfa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fnvbqlaa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vqnobatc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2igkfgnew.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vehftbbk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ehdoabyf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zjzqdymt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jaqygpzc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sagjiyeq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2porbdchn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wpyslxzr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pwwaepdh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vgsbghhm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixazipxi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ibvzrdbq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tdqlixmw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gpvbwiif.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kqpxokrj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2audbzzlg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ofxagnuz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lapftfae.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rvosnvez.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qgianjqu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bhgixjdg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jkjdlmru.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtwulg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ptiunjkl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ungcfcjg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bbmsgzvj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2beoxbobp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2affwkcsg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kqosnjvp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2pmpyvkrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvufxgvj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gjxjszic.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2cuijdkkz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ggpwzcxx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2aaepvpja.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qalxpdhm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kuottppe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2riggwpns.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmlvnb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mzrpolls.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2tmvzgwst.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ctvcoect.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2uwwanglf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ylhuwvkr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ktkykapc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tleednpv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jyuphvam.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tepftmkq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2aadmedmq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2aszxsncf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qcvsvxse.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vwaipddj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zrqiomyn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mvfhgjkh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejsbabbw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pebvnfuy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkupbwmp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahwwnhvx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2izsijlfz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnbbkqwf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxdiuoat.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qihcwuro.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oyklczuq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ollxynzc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzlulzss.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2siriwesh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjbugpek.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2aurctwqf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yanzemfi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xhfkgozy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmgqbqgf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqxmhayj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fjfuudgm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fruqsiuj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kvkymypn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fygwdlwe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2aksdfdql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntzxsbli.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tvaagkgc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qxgkotqn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ffaldhow.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wzkuwcyr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2lbpjwisd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mcgnobln.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xkxuyybc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2avinmuzk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nsiahhtz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2eahmfoly.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mcrmrbur.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dxmnraor.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2coqixukl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2stavxbsy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jrsuzhue.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bnoqqohz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2flcuzvgu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2goxipvfk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uukoryiv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nzislkdt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lqqhxdmv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pnjkgtwe.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kiosmaqg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uevznxyk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcwkro.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jutwppmf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ymlieipj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibwoxeqb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2phppqzoi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2efikuhyh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xjoxmrmi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vizysoyr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cnjlplga.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2buknkjur.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2uvimhpmo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2fbwkfeca.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2exkhwjop.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dxtnauyu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2svzairtb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wjniiivx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zbeyhgxj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gmdvzjog.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iltfskrc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jbrvkslu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vgtjleof.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ecdjzphf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2esxaypsa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lmdsggxe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tevrnygk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rrjotrzt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2goyrsmup.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2dwmjqkqf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2kofgfdmw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2asdejbzm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2doqcisrf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rkgktevz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mjahhwwo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsfyblbg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnjgmwc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbxejfk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yilcqvzi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zuiopvyg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2krnkhxca.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2woucjypp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fdggkkhg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2emwbnzyj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2atxrsbuq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hyixsuar.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2htvrxnqy.html


<!-- 参考信息 -->