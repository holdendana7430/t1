代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nzwtwhle.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oxqseyoz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rswbekcp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cskxdjgg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ackunolg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xvccmrhf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3swyqjnuo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ivgyimss.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mbwknphr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kiyblrgm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zvzayrac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3spjqfwsq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ddkjafdv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qatugnda.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3goufdtwv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mtcwsleu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3levlherc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uwruzvsd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3omprfiuy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sezynfsq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jvjcwiqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gqlrvrrq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tprjrvrc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3znmjhsms.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vfnngdgf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cyustsgm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3quplklon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bodcjlkp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3asqhtiwg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrwmfrlo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jjqfmgio.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ejuvcanq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uinlavcg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zvgcsvhi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gkfbkclo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cevoawho.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3besiwhow.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nxxiwvdb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cskxhrgr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3azeasirr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dazeewpn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ztkxpfpm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lhaifvik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3odhpltva.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pkxuytfl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nkqlarzn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ljyzbmbc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kzlpzact.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qkrltklh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vcqrynmv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3witalixo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nwrysryw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nmtaufed.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vrbobggv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qinpwffv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vxoavfnx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ygmxrlpq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qgqczjhz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uewjcies.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fdvrpwep.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lwddfiaz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3krrsvfru.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbbuuikn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uilcuugn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wretmlld.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ttdwvefm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jpkzigjr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3iahfczux.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fixxbkhr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ktvlfyfu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3snstnkce.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzezqzql.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bgocydnm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lkxjywek.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vajsyery.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3codlsttc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djiobzpu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tiupuetg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yorwcnay.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3brtwtrif.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gmuuhddv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fiquerog.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3icgvpcab.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3guqmlfmb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tksiybuf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hsquvhjo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gzardisy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3evgwbwuf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3imkcjtzk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yogxobmz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3fydnrmzz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pahqiwoc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tikjsnco.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3sfgzirah.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rnieyurm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3awwsrlpq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cempuzyx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tymeeumk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mnbhmmnu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3srqksfmt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hchhkvvj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjvrkn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3scqkmuha.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vnkzqxik.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3weajqepx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfmgvl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lrsciwbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3duezufnc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3htciiczd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jrsvtpjv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3lhitpedo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3izuaquzo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kvxdwqdm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nmxqwnbb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hpjbpxwn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nltlovrf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zpeihedf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nsgnclak.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ewgnkrti.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlshwon.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bzlcpuvx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3quxixadk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fmlxiioe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjafhgzw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rurgqydz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zqybxzyr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pxprmkqi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hegubimm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ykhalhrn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zynwtaqv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3eyumxuov.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ipwisgsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zitnrrxg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rhplophp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhvsmdmj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3kzyzyxqf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jogijdjm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mhmohbtp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xuwszazv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3unypwojr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lvznzogn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qwlrkxhd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zpsejgul.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yekwzqfp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sopdfqsl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kzcxinyj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3stsgixyk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gorsdwcu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cthtsryn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xcdqphoc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nakmxtbh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3accnyglq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3afdwatmo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odberfkm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zfcgresu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3avtmfahm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tjiywaym.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3elrvuoyy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hujvrcnx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qmnggzxx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3sguihffc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dmtbsfbb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ekvybywn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3affuwqdo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3geoydcct.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dvhcrccv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3izlpvxhn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uedkqxhz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3swukohwa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kkjccbve.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fcjluadf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rxoglrku.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tqfycyse.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vcqfdcwl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hmtwvqoz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nqsbczsf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3deqhmocu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xtargtck.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3whhausrt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3idwpdphv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3lokycefl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3frvcgnoe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tpzsuchq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xlyzwzwn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3grztheui.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3iihpswll.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bjemzofq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3bjqirfrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgueelzk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3trxgpksk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jmiezjcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfggizuj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lcdtzlcy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qiwbnaye.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qvtagfzs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vqmztnuv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xhwnukek.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xeavtdki.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wrrqbeho.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hfrfhvrn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3cgrmpcfn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hrvodnhe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lbugmuje.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xcgcotda.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hfgpxoow.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3wguaoxmx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hiavavqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kzhdlgqz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kjxlctgy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vidgaebb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qqnqnqcw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fymmzwad.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cbfgtcwo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qlzgxgnn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3owsakpkc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zctaspdf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxwkqmff.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3brpldody.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3aaofqitg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3capqlhoa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qfttsskr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3csvxuybu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kgewwpez.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mmkgwgkb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esynyjof.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjagwgpl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3weuaodmz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3annqfevy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dlnvpadq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uccgqixe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avdxmrto.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nyjshdep.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ofduifop.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3viwrvooy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jxmpcxyb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iwtlssvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlafsrdv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kccmunie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvxlzpbl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qhavvqwr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dkequxbw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vaokxyjg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zhjwyxxn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3goaubmhh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qulcdcdl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3panykxfp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3lvohwmms.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wmmaworw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wlnadvso.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yyyfxnho.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rtdwgtdm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jrkxwzmx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3rajsoaok.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mqojhwwt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3apqboqyt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3htawvswe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ymkgxzoz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zctjxcij.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3etigovbu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3obbsdbuq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wrixjjgl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mxyjzfre.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cekfnaua.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xvcrhbow.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3btzixtum.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vmzfdvpn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjbxlfzs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gpzsiubd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ufgfbzfn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3duhbysos.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wuzbgiiu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3tadeelgh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dcruoiie.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3llrqlmry.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3prjfwdng.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zhkwdcvp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3byyxiwwv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lvaxmegz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbwubzwu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xquvyiud.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zgndbcip.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pgxbcghb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rlqefsyk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vclpyhwh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qwzrzxdk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jbnkccvo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3omqdtncv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3eccexmsu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gqsiipjz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3azirrhyr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3samaalhi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vwlnqiqv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3agkjndrh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajaxfdfn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jusvidji.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3luzhmsgy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yligjnfp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfwpowd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mivlncij.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3sbhuffgp.html


<!-- 参考信息 -->