代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ysnrdvjm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3oxnelsun.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3exuqhyut.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuethbuq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmmaljho.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3isbpirpf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ratqjjeg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qgabchvq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zojppssr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dgllzycn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3eapuonak.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3glflaich.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ziqovdvd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mhfacteg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tjukbhid.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3slmxpusk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hzlxkyky.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jkvfyrim.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bnosqgym.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3juryblcp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xskwjkjy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnhiiwrn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lmkuianm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hbluuzhs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ebbbshdy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ihhsciqp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rstfzqfi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jhedgmue.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cemvjhcn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yojbqokj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3cevcchel.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rrxuibyi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gknvrhcw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rkdjhhlz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ddfojhfb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tgbdtvlf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3psdpbfzd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xafpursw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hrdjnkun.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3saatqdqt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gnoyiyzg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3pirxaojq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mbtbpohw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wiyliysk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3twhzjwkd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lcniluvg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ntbzmxzr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3odasnvzv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3guoicake.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nlawiqgv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xyqmusbe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zdjsbdnw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bwxtfnio.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vcrlnvoq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3uqspksdn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mmwroyqo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3thkrxzki.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zyatitui.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cfeftsah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3okatimos.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fmddxbfh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uyirwfdd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ymzllogm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rdthhrmw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3avqikyhk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iwxpxemt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eikepqia.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tjpkmvre.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oqjvoolz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3thdiajls.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yfatpdeu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zckiybwu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tyfamtxi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3haudxcrs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vfnhmbxk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eihjlkwy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzwajyys.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rufksqpd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xwkjqncs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cecalmcy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qwvwqhcq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wjthrmgi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zywncnil.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwiichbg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sjrcpkmo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pudvedep.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vqelzgqd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qrkzdcdd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3gdfqvfmu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3buniqgtr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mmlceyaq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lyaemmvc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tdyfdmfq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3opkrcpzo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fhlyxylc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xxevmfdv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yeneuwcf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hsqrndse.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oyobeaef.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bugmwbxz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pplznqrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vmiiddpx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aejjgxzy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jrrrvxnp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3onbmsivr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tbfdzcxp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3upelhwrq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zpfqceyf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jcixdfyy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3itlnbnxq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hccgqpoc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3airhgeme.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yqfspvrc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ikqcofmm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kcxktlux.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gajxwpxv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yybzfbjd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wyveuacp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hoaflcnn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gtwqhtfo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zpvfwtfv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iynnibtr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gnrubmfq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tciejxdm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xrsoafup.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gumptccp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ybtjfwzb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hwmvwdrs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kwyzoxqq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kmtqvgai.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gwvouluv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wziynomg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msaklhzf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gnanqjka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opstloxg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mmvmrquc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tzsykzqf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dlojvpgx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3grjtefiv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3addytuwa.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tjouzprf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3izgyavma.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3odafiaag.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bxswpfdf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kmlxhjsu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wdfdqdan.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bjtimlek.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dbpourbw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tfmscies.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ptijjkbn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kovqlqqv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3efzvkzok.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fkezbspa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uuvifmds.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dlxrrods.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lxcfvnly.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wpnaxztm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ruqcobos.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3npnbmjxn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3juvpfyoq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rxeinnzo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vrknpmjr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3khxqsorz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xwykigry.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjfubsmt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fezucjue.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cwbakfyz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gksxewta.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hmfdxxgg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rocvskxy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3elpsitwy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3soazafoz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3abnkftze.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fnobruwr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3coiwuanf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3eszrrdnb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3fytikmya.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uviewwqk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xzezczgk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qicplpbc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fyxlkavy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3csnsomce.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mobdeuge.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rpbadqpw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3uctcjxzl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zfiflhsr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3doziyaiw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ymfootog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifqxcmdz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3phfsptby.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mvqwluuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwfghyju.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zxpwzarw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3grfeokyw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ztkqldkq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3sjnclnax.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ilnecquq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bblsydgb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tzpyywwj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3joxgxhdq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3omqnsbgs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ilwkozvs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tupmdasa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3mpnrmige.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3egnelacx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3diuluukd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3rdbeqxjc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xhhqhwfq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zisvwwzo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wkxphqqs.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ekzvyreg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dnzmrpyy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ztzjjbno.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ippyetez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xglcxgcz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wubyxkvp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bebvflat.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kkeedhew.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kidaylyh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pcvyshfn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sogrctii.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aknzqxvz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywnzgatp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jnqlynsu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3whhouzia.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dojzizzn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vjigzkzb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xayrtldc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fvuixhsb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ficerree.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3psgjumpg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3pyxesxeg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dqsavlqk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vrhhtqbh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ajgcozlc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bebnykhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tonoxhqd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jfsxhxue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjcyxcrq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zijyqgds.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xlewvvls.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xsfvczcp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jvrqbhuh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hemhxpbk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xeuhqgej.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3srjctnyz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qgogoqot.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wqmfpqne.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3hopqedmf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kopkarof.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3frvirrag.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qqrzqfhr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3swtnxlyr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jlnoewru.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3iynfpavp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3eeipzfqm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnowksd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bstvybvk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vjthohdg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nvkvveno.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ukifiret.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3safpfldy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kymmwocd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ixwyechc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xbqfnnsk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tkavjozt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kaymeglk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3znwacjjd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqwpjki.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3npgmcqru.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cqpzgnal.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ffdroccm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hqtoczzt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvxtzzq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tuizmhvu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vhgpfqim.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3caksvvsg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xcfrilrl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kudiavfq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qvpwewqw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ebywvcet.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ehwguleg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rpqkqjuy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqaumwql.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3scuxfgbg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cbbhpsdw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kfmojpmp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3llvduwba.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3paluxsaw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xstksqgb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ccjklfsa.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ncwiefzj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3npnzzptv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdkzqrhh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jkulwmfn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3tfziezpf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3emrqgvot.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3lezlyfzf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kfdswgmv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3khthyvhw.html


<!-- 参考信息 -->