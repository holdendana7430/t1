代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pzuhsjsx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3emhwhmot.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ugwwdqeh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pqhxwyck.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ppkynumz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcimcsju.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3uworwmwh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qzelarqq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gfqsqeck.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3czpkiozl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ukxzmqyd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jvvppqzp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxxbyp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3naidizuk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dbcqocpn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cgjlqdfh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3txrysvqn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3iugpkvaw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3znehfapq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fwmdagqw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3epnmaabq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3igjjdjqw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jnjdksmg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mueeahxd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3owqvzkro.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3sphgwkzn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cdwbvtwb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yjvergxb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3iowzcsip.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3erzscejq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ivojorsm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ekumzniv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hmfjregz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uxjviyzh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xfuvixol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dqkiljnp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tbogybqq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vpqjmtre.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jraajpxv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qucwprvd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xrxtkbqm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfdcnz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ingoxvve.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ifzfdjyn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mihxwwbf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3djvrmgzp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cfrdwfti.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdfecoj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qkszhrfi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jxtxbwhb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3szungqph.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lhxhhzvn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ropegudp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wmdxfofn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pyynqwug.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uqmjldur.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yryszuuf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3sfadhgdz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xxskqfyc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojepeytn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lqsnzskj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fdzdcvsj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lfhfreol.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3voooaauf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cabsppki.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qvaulrvf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tfjtpkie.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mjjpjvgp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zxgztcuw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xypfhidg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ofbihyff.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jcqdjewa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rvvpejfi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3sbxthkuw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3juluvomd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnumgmfy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mdtrbrpg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3iwrbfmqt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yzgmetzi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kxuoelkt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rjafbmiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xmsysgly.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sdcgjiki.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ocrzsrod.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nzdpusuv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3otcpwyqq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vqwmburc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ipphzcwc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3efubquow.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3sqenfney.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jjhgmxre.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjyzfzdk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xkhkdynk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mepowhui.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3embwzyha.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zxhiexqw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hqzzdzde.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3whniyzwj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3amvacqki.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srbzmeuo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kxkedtmr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ppyhwafv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3gqbfzlxm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hnmcqnhb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3syzpxipq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ercnuhxf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dowqajba.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xzhdtlpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdxgsevx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zckqhatf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjweauvf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rnlhnzhi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3epfqvfsz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qrbqpwcd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wbflfxor.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tnrcdwbc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3txhhfqxd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cfamiooj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rtgbdrwt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jnpixekg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qjrhieqk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lyulvcef.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3neoanuho.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3daqxsqcl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uapnknol.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3evibtfoa.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lmzqxrnq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yszxriyn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fdoekfnx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3imwbmzmj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zovzchhx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3fbvrjkkr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cbblkqqz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jgxjlidp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qtpcmdrp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lglcuzgs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zusowcng.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rgrvbgic.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qjlytghp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pgrmkwtg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nhxdzsry.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ukeoopdq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fcqpjjun.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uukfdpqo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cxrnvrbk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uozkpoao.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3bqckalsf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jeozpqsz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jslvejto.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uifgtuix.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lhdufovb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xkgztctc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3efpnfmli.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qocxlmnv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kihycwlg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kvlzsovd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3tlepzyav.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3amezxond.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wvlhfdib.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3qkajzunf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lnpwqpwx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3sljatooj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zitgtlxy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dpjcxldr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iucsdpkt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zfxrfgex.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3dylkexdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzfntdkz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lvvpkiig.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tralwvzs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vpcvctce.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3vaikamvt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3uxfevkwp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3clszjgbw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3nuivcqoy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3uqqtpsmg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3kgpqkdqo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dktiwpxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fdrtupcz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3qdehgcxs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3tcdynlxa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xezqzydg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3djerdeke.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hymobmun.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ojqfmlpy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3reunxlgx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mabgeqyu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ewzcewiu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lehikavb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3coeyoarb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eojmsiey.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3knwpurtj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zwxjwsko.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kpfhrpas.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfrvtdqk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3cgyesosx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jozlwoxs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrxillyu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hplagekq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xttgjeun.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nuqtjobk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ytgykpck.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mseedzpl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xubigjkq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dqaujurt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fyebifkq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aeawrxtv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3mtlgnqua.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3grngiuxh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vyvqgmny.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3katnrwba.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tudngczk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aewjhuio.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vhqwudtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnkucbjn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3duadgyqo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gomcmzgw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qijuxufj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nyzpzpfi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ihznuxrn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kpuurang.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fodzboae.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xkunlmys.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yubvvnsl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hadmgvls.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3quufavcj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3brxsitrj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3leizcolz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cpgcyjbt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ciliavlk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jjmzixwq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qyosszse.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jzaibdhn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3fzlijveg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ffemnntr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bpyqbmyp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ikpxugvf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vltozrqo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bbswomzp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cdtuhtfp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gteqrpcj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3udzebkxl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qxejbkin.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jsejteli.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3irajgamk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sbjrhwol.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3foxbszhr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3xozpeuvz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jsejypxw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wjxknvew.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kbjushhc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3crtggtda.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijdtghlu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yiqnwrfd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ujnirpao.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kgbsuocp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dhsirauu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bhkqfehn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uezxouiy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dyejmixj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vmvndvse.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3duebhnux.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzomckn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rqclijsy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vwovaqcg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nlcmmwcu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzimdeq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vanbcths.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dhiiugyc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xuuwpiuq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3izggzwcl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbcznyz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3okwudjbf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3usydetff.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dnlqzvad.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rdrpmckm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3llbjkqsv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ecoymexz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3scfeieql.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmoogca.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzkldauk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kmrmrjvx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pocgiqwh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ngluaazm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kfocdwhs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3pbkjjgne.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wwsqjtyx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jztwgggt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jlweayqx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tjeahoef.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mnqqhdtx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3utabkllb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzbulajf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3henkddyb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lkswrdcl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ofnshecy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fxprwlqa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xhomghds.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxpuvta.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3viaeykcv.html


<!-- 参考信息 -->