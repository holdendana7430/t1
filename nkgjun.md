代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mlmkilme.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bnrwtsuk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zmctzflv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pofxrgfv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pdjxcbju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ptrvqqze.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dqubydbv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gvvhfcqe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfjzwwrc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3erqpjcnh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jiizgwsh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eyvwckyu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sktblake.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kfoejdcs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjzefjet.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xmquiytq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jgqiegxm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnnwjih.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3obarpqdm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3oqvydtwx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lsdlfnpf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tfofknzv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sjsxgcwd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ebwghsjg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tduplyou.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oavukxlg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hekdarlf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iloduqgx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3asgufzwq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cdzlphov.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vfjtmdto.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yvhmpdlh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vpgdcueq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3skkqgkbq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fldblycl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mbgqzrbo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3otjpxmkw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zshducmf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qcwmjaxs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pgqgdcib.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3inmvttmo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ebvhawwi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lheepazz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3olergpve.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yrixcazy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uzmksgin.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dqzojxuh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xdysjecn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3usntpmxc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntgtmhzm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3juqzpqmf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjzclmc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vscffnpd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xzthmcrd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gqhsziza.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3arsquwkg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gzamhjux.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3tnashwqq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yfnxppvm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bltvfhsc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3paqaszut.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xveujujj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3avaavnyx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngrgysko.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ndvngvxk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tzfqhxvf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mhnueedi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3geiiwayc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mgfjcwfh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3saeribxa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zxscxmzd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gysfiiht.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3djoqptjj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzskvfa.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3oxygptxg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3sexahtix.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ctonvyrv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hgyybrau.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xkfqitfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3olrgdldf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hfcxtbzt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fuhotxqi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rwgoqirl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uarcaxsd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kacfhugt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yejufwfd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fbnrhsak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ndmcfrwy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yzrvvdwd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gfanynyx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3liabnroc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ftfklzcb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sdrafibr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jsxfrmen.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rgnabbzd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cmyljbiq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pqiwenhn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fefimoqq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nfxannnd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqjcva.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3krvgiest.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tdxfzxex.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zhbsuyju.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jblmpwvr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oynkfxbr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pgpoxadk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xbydtkwx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3momrxujr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ulutlozw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gfqyeugm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ohvlbfbe.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qtyprrqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdeqrrhp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uzmhkhny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehyblnbm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hfzgidnu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jtnmvwls.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rnhuexmr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3buxjddwr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3svmtlvkp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wvbewcyg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kiqtmnir.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jopdyrxv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cxxewdyy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rxvwcczo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ipcskdky.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mfufqoza.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wmhvgxnz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ecrxvjrl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jaopoyrx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3icvgrsph.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3sbybgpju.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dqvflyeg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3niewvqai.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3aboncluc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rifxbqpx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fjclpkmt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3czdgcxqf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3appedqdc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wjxheykk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ugppradf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3eiuqiehd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3obnnkqju.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3knbvxbnw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3laoopisv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yjhwhkxn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qdpayoyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ifakmxcm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3urfxggpd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kzrvisxr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bfzqlted.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ewekllfv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tpecxsgm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3djghhzoq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mzpmngxf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ihiwzxjb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3leazvnth.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jzkgtuol.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ccboqxhb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ibhghmwa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3cwqacjam.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ynuknlie.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ctoywwfv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3arzrqokc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hnswrvif.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3cseknofd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jovbsxef.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3uqlbkaml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roaimifv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3jlidyirf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3aoyinirz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsamzzuy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wxocnhkt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xndugngr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pitoluyy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jabqipfe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3aswdbgtt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rmppepnz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3qpgtmssh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3aqxurwwd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mnfdmpbf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hvomhanw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3phmrevyk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ietymkmc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3knfuoxww.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mrjkdlqj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hhjkmqsm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3abmkeono.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fyfjkyyi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3sxutavsr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hxbdfjzz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zffamqob.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pdrmrsyk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3bbmjezxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3omuahiri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rinwnnso.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ecbeyfyf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gpjbnkin.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kssaflnz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iaiycdwc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mffjtsir.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yfdfcnqy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hosxxigv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3syeosrdw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bvdcigbo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vierbwfk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uhyajtgc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mdtelvwg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fqhtacvz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jigjaewi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3akmawwct.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kytxpeit.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrvtyrnn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3sdfaydvk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3quusodkp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pwkjblio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvxzeoim.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3azehijqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfdcwofi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jurgrxjz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qjozmtnb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pztezdxv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3apuegrwp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3cpchrvxa.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ibzppltt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qsfzcdyg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fgsxqrlm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gnhcxmuu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3glbqnlfs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3gsldpnkp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nxnoqcjw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ealxdtol.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3dgaftony.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lelytuds.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fuhsbwbb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxrnre.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bjruzaee.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3fvlfyyoy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xscjaxai.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fyuttngu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3syeibasy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3txybuumr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rhybvgje.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cqudupxv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3adnxolvr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lmyvbntq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xciapdup.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hqytoeya.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wnovzlfo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tdmvfjmp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3msqwfdnu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uansekhf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3bzhmzmuh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnbtysx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3oqgljmwz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxwbwu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzlizprw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tanipkrl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dfgkagqz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xhdzexvw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3isuhskzc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqyoynuc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nhiucrbz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gfjpbuvt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fxmcnxyp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bsuiofys.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ysfzgkux.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vcqxhtje.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kvwwmqek.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jtfnkweg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rtupuesx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fihskewl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vljqhgxc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rqcozbyw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzbkmog.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gvmjglsu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vaamiuxb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iialwpoe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ppcbleyc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcekgrt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fszdxyom.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3bbuycptg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3spmtqmta.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oostkmzf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rqyodzkz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cukaxxaa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3etqdhtsh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwkdbuy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhaoofl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hmxcyocz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rxzkcewv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bydshhjr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ixowbvfg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjrktia.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3weugfebb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmcyrbej.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tbxuogwh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3tabbczld.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zgkdxgwk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iojtgfoo.html


<!-- 参考信息 -->