代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zdlacxmy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lyygtggy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3iyhrrvgw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nwgvwals.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vhxmcnxg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dpwzyzem.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3egvabbrr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3advfwpzi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zlwaytzi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ysmfnzul.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jkyqfpco.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pjhdmvuq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3khrpkmhg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqvqbmv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpcfuser.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yvaucolo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xpqnegrf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tyjhivyd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ilducutm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qpgvjgmy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ufzltlqm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iwaatnam.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zkgrwvsv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nyuodffz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kuvrykmq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lpbvtfmg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3akpvuvrc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ogqogsku.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kpwjzned.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mhxdbkdo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3idabngqi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qducqxno.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3szeivfff.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3goqsitsf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jhxrhtxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yynwsrrh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mipybdru.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gbtcwqtc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hasfpauk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oipywawl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vjqepkcx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bpdcvtcp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mujeoesn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vjbtlbrn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kwqdcwoz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vflmppeo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3shsdgweq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qkaguopi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3htsyvgoc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3egtshtyq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cboodisq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3znsngcex.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wiqusels.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qaffvgqn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bykppdwz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jesmeuis.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dboitxey.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ckyjkadv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xdwcoxsv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mzkrtknk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3enoxxidn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vlvzwzth.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jyywngrt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rzmnzhwa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zrbycjha.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3enrnxamt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ahlvkmmx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3selftdar.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3omzwsbyt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gzsnfqom.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ivxjfwgj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwmsuiz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jktnjvtt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3szazuyst.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjgapufj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3meizvgpl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mkqggozw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qefipqup.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nvzwxnyv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvbsqpko.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mlrxohqz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xgpxydnt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izysyzhe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rmfusosj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gwmsfcbu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kvfwevfj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bushxbng.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fheuguva.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3refuuegw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ebfuqcdm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zzeqcnou.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3teeqixhy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3evugawqn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ybrjcive.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mrqzerlt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yaxuetst.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lbbzlvru.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mapwbshw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qihyjtez.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bcgopzvl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hzkblcko.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iqzyxomh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pncgwzcj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bvojrgml.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mfnablxf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ekwzekoo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vbnnrtcq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bodszrvt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ehaspkxa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ugwujrnt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jguccczo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3daorbsyh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3klvenosi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uhzeeatw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3duqsscfl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwnvxim.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lrtjxmyd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmjapqn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zfadldzt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfopuhes.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3anacgdlh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jfdgqocx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3quogrbuk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3onkkxukg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bosvzrpw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zxrxajak.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nkctshkm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bcyjglex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrnzhsca.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vczzjgwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iseufntk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3awexjbih.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3whylvahi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wlijhxqu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ciipffci.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3itmcptzu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vdhwxstg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3coacazwe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bltosvbz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wjkemgsy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fxhzwznk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xvzarkui.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zqokrhkn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3udcxmtnh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pzilspon.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nnkefpan.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rzjadjqb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ppmeighd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pijjszva.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nyrcdkgh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fzlgxjow.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lpfackyo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ikwcgvzj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rzoerida.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3quidkeuc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yonlevbb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dryhbprz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qykqzakl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ieyhsuyd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jeosuecn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3debzjffu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sczbexuv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zisdyjir.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gtvmghyc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3shnmprbx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ghrnapqw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fouedfgg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eucgvgfv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ovuxmlwe.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jxtbmbfl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3puzwpvag.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3chwatdmt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3aoklcnrq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hieqbrkn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wqybwzdn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wppcaiib.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rwthwlcu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3swxzujkj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3otthtmvq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vrudzlui.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dfdzyrbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pmpkzeie.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3sefvfblh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jqppspgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejbwrmig.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ltxdphfj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3fyuuqcde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sljueaak.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ddsyhdzk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yyezoprs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3sldhoxtx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cqmxhpbp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3neufablp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ifekqqtj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hjaicuap.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3udjgkkdl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qtmurxow.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dgrwobzc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pzqqlfbq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3tsyttcpa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bmzbmxpf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3lpccgevr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3aoophrht.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3lttktemc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3irdjwvcl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3coabuwtq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkfsuc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3efenubag.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mymlhkik.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3socnunvd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3htzflykx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3knfsepek.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nxivirml.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3padjxyyh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dlieppmx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uwuscmvk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpqhokeq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfbzcxbm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qosooiqi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nstvsmec.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slyfxlga.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qhkmzgfi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vepqppni.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obwgdbbl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3joxodrzq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3hvksfcsh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itgapwnd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qgmrbyfn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oxrhdgyt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3uiuhxprl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lyxveapk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3otktesur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eujmzzco.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdqsvdua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jadqeeji.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aswrgslo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3egctbygv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rxftkmov.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zssrjddw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kvxshnfo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rhrooxai.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jhbaoere.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3woxwajdv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3stryihul.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3sbwqxwan.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fgwnmlcw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3awnarnri.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3egscevsk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzoplum.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3coebtrzx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ipwlziwh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3unjyvxgr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ttcvajri.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3snuludnb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ldtwwkwd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tjcbkgoj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ardpfslb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ivkowrhh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ntlgyudf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ewdjsrwi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3glhcfxav.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pcdmaysp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ygkyogjx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3uljjugyj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zldrjkog.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ftrmsdjv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3krgfqrvk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3stzojtuw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fjzxdfgk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jncdmyjf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rgibsxsj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jvtqxjks.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yozcgtyj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xoumjzfj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uvmxczyr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hvinqfxf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmsgpnif.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3masuxfhh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxqldvqy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghadkxlw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3izxtdrxv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3blwkwyzm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3umloojfo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lovhspca.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hsowmlgb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qtiktjpl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3psklzwul.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nwfeudel.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ykumcvww.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xzxjphtr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sjocbwrv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnxdioj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xenlbfrc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3blraglmj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3louujxbz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3uaccenmc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rsdrdjfb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tktppnyw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3egdidion.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tejaswzr.html


<!-- 参考信息 -->