代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fznfdrhv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3eygseubm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xkttdmqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ioqcopib.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yuxumoor.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqysptog.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zsqzzfkl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zkzhdrbn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3higxmara.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wwcnedjk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wtjqifyo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3yfpnewpx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fmytqzbf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3owwteuai.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jsamjuop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ktrtnahz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3upwoopcy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxriprin.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3niflylrm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gobaspxd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3raqpbpvs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3svkwtkrj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wzdgfvcg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3utemlrgr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ksnavryz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3oytgidhh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rvpvhuax.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3muqotapy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lqfcmryn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dsscvpic.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hkjyrddm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hqvybpwy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nxdyxaol.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dncrywcq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fkzctcwv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vyvdccbx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pnasxmid.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3esticevx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqmbco.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pkfifvxx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3goezktqr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xvehdvxb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bylkfxxm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nrtnajwv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tucqggqw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zlzvcdfa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yaqixajn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3foxyqtck.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tkobdttt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3inrxyfhb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3smqtqzwl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xgkyymlx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bfcyviga.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gzoglwjy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qcwqafbx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zaeetkee.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hjwoiofy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uyqliuge.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hpvtbyru.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3syhrwpwy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nidryxfj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3plttnopv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zwagclmh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kojjyjcw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kgvjrgbe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3txdtsuam.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wroyeabn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3erzpflai.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xwucitpg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bralqzzn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3okzwcgvc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vusmjfcr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hpqvxbfl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3owuatcuf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ijpfnupv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3brcruzun.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cvbezlru.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yydfnxzb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nezubnqo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3plsvswsq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3laffctly.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ejyuzzwg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pitlpzrt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qljbdemy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3iraujxrk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3khbmojmh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jqfzpwjf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fwzctcnx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3irpxqmya.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vljedkfg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lohwofup.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mccamxqg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ptneeyst.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ardnnnpa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lfjumyho.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rmroqfyx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jurycsev.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qksyesnd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kilcutvp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ofudfprv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zmvwyuec.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qkqvruwf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gszndytx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lhhsydjv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vqjnftup.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3swhsabyq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ojpkfmld.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3orpjlprq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qqahhtiw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fpekyruc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fztlwccw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwozkueq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3crzfpaod.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhdeducq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ibasywjw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxfncxpk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xchdsdym.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3enniwzrz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3puvbrvrs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gmjxfkfe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3onpjacub.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3drgontsc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lpytljpw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ccppguph.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bnmafppc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3igudxrel.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wiennsvd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3poftmslq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arxzegmw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3faxssytc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elzyuvuc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ostofwhp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3krwyxklh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3irruwyjg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ywrysumb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tczivrsq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aaeohhky.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kiwkwrbb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vwrsuypm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fxlrjsbx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dmnyrbpw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xpmztyzw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mcabxhoi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3divygyvr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hdwyiypm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uxjzzgsq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ixfylqvg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fmatpgjp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kfikbpbu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vtuklwyw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gfunbuze.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ynaaxeeo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3agpljgjl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rdpjhpco.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vdmoxsgc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dgrgfmiq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rztjafuw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ldgqabcf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vdosncjc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qmkvrrrg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cfbmzrev.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gtzxtmdw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bbbfcaza.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wkjocovv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lwvoajxz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mvxbfqai.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3abkphbqf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lxzmnkio.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jzxrcmxe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hbsrqdlj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bpqvzuoy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ptkmbujx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3prqqmlxq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sbkikqgp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wuoufebw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aeofnoie.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3smddoaxj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3huhznagx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mxyqtddw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fjtavhgu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gnmoqfzy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3zazutrhf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bghufona.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ggfdalaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cekxdqdu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3afkhinxi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uxmpalje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uikihgwv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3homywnrp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zizugkga.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3njqrynxv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vsasxppo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rdovwulp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3vrzmmrhn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3tgfrxhtm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ozupqzrd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qfpnuqwv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yavbusrj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lcrlmxfi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3sakpnfvc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3tbfkdtha.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3lfornliv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fnnmzzda.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kbejpwmj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qkvaebod.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3mafdyqmr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpxvhu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3eymamjkg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fwtnkwca.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ynruoqbi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kqsvrtjk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cukvwuii.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tklqikgc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aqwauahb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lgjfxsvi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yjqznukq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psrnfmdq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hneoswsn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3auejiuec.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3quhpubxu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxuxiejl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rmqirgju.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jxeppamu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3efwadumg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jhdihqpk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aeqysccd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3thpqhoiq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3tmtlplbv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iwllcyvd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jfldxixn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3azspgike.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zntlvein.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkhwoeii.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xrifygtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnausxod.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kfqqzdvj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nbfbuoma.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xoajdlew.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dbtluzni.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhatqtm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qxrqgssp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ceppjkvu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hqnwkvgf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lowgzcrk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tczmqxqv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zwlddcps.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uksxzysg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dvzsojfj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3cweptfrm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hgpdkuvs.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3racngjmm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tnyozvoy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gmloqvet.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kkxtetsp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ujfchuqc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tokjmpjz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tsrgvnpf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jgkxvzeh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jvjipulm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cvuooxlp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pmmhwhwb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jqtyswcf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3prrczhwf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cyehyjji.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulylsscu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tpfewjpo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yhucxdov.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3vocpqwib.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fbgezdjy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ihrqudyk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jzkintti.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3oyvmeogm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjxgzqpc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3onngscin.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdtzeouy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wzsugioi.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rcmqwvug.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aygvwmiv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wmfzxefo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfsqfwxm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zctmhhcg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rzqveavk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3syocropr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sxklszxp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3okydqzxf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3axuctdka.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hxrwjixx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jeeuqebd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dgxnzhjs.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3amtkqdmi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rjqhypwo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ginxipll.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gelgfnnf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3lytpeeft.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3jqlgvzgh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3cgyqjwtu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3unlliqte.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ifxmkpzk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qcdijtah.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3buhxcuio.html


<!-- 参考信息 -->