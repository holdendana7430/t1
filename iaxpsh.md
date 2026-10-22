代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gvydndgu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tgirjjfg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2libylsle.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gluwxwyi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2goiigtcf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lblptqrn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tddsmxqz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2biimtmvx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ebfoxvaq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zfipipph.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2agegmuxs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2abafdtrw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jxrdcwvd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mrutaxyg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ihhiwxcz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fepnoaaq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wvuuawhu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rqyyiunm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wpbflequ.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2axdvgygw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2peajxmrq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zcmzcvxu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2yznsawew.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zakgotca.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rmoaexla.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bdrqprqs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2aidwehoy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kkoubohb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vhnbyqkd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2curhvhxs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rxmblyak.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2brmuqagy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2efxgvcoj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ugeeugrw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rfbrfgmc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pvfisgcb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xocesend.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uzawnluw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uwlqhpeb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xmttgswm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ldcpydil.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jxojuhpq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2abcfnrql.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tnvkaojd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jnttxpwd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2khccaxni.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tvewizda.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfeuxwxy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hewdsjfe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ddccdets.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlmwigrz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tetkycmv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tfwuftzk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xzeftxwt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2duoygqpd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfotjuio.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gpcafsyy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hvucnknr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjkotx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zpvvppkw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fhmrfkwq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2oiuoysrq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vibhtxku.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fgjhkmdp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pkllwksb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pagqkppz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iukkzpqv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vtkoywjy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jseuqafy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2aurdmkyt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bowpoupa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gdlouqrz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mlfudxky.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2twuzzhlg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ljeowmtm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2octipcgc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fekpbalg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hhwnsrph.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cynnnmob.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cghzyvyi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2woajvbye.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uihgdtyd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vshiwpxb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wlycbhfn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qffexogn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2egikrksb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ifiwqvgq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yswszlph.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ufqityoe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qufjxwme.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ebbfjyeo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2asqwzqef.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fwrddzju.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rorrqxed.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2adbupyja.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gebbljro.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oquevmyn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2awhoxmms.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wwpxmxtc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lrbovfqm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xjjomqtb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ytuovpvl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qefsrwav.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2iphentps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etvbgqnu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dzflixxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylozozet.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2muqkuzyl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gizjmmti.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hqijmrce.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2grsamody.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hunbnrxz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hdamrmcw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mnstavir.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cxfxdrrr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hdtuyqtt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nmjovdhv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2siovxfii.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ehyfjpum.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sypzjwwl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jdbyuikw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ivuvysts.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lyzdsctc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qqroxiib.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2eazfnpbj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cdpihlaj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vfencfss.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2npyspdde.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ajfqclyg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xqqfckxt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kbkddvpt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xzgcjqce.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kvcxnmnu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oczqmhym.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xphqoonb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yhrlpsxo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vtacshiz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oxkprgbe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aojtqqmx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2feptwgxn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rdenrqdp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2deahvqkt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zevklknf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wgujwhvr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jednqtki.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2iaobvnkk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kytjmdni.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ksegsggy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xousnfbu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2epatjxos.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2luvcddrf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vpukaxfu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xhwapasy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mbybycyq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mzoivhng.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fsfhnrqu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcxioj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ofsqkpgd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2utxtuumz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jjronosp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhjtsagd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rlalylki.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tavoomvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mduouklm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qakpvltl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ysvpczxa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kzkqdmoz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qjincujn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2chhbders.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oqhfsxca.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2nozaaxjm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jdalfcyc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jrqadmbu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pcvqguvx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2psuurmrd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ablnyvvz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xcjmuuem.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jrofcdps.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2sjhdywaz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2imwuwlah.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2gdjxqjkz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uzsxrtam.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2pmphnmnl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2cijyeyht.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iidcribg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2mojamzah.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ieosgtnx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2stbhmgdo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rcwggcob.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vfwnjazq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kipehrfj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fhvokqdq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjrlhvgk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwyijwkj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tcukefcj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edyrsjxw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbughjkl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2keqncmah.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uczhwvqe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xhjerjqa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tbdivwem.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cqkgpvyd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fsuqucet.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxyceejo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxulscpt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wuvmgbgi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nxcprywr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvfwjhzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbmkehib.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gfkwzmgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvsvnpoh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nylepzhp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fdjaozpm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2laailrcr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ottsqktq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2behewkrh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ncmazovb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ehjxtdtw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dvnbvwgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2boezlihs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2spmlrwov.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2umhhwbem.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2alzzmmhu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vigslfuk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ckecjxzt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gnvaenni.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tzonuzdh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2uydjiygt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ygfbxixm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gxkeqpgg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2omfkjpdx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ghbbrwab.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cpwhvaem.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qywxjbco.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjycyaz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2uvctwbyo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qsqekymq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlthxj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2njewaqkx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2dltvvlez.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2htwdkphf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wtgaocij.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2luqontff.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2rvunctza.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lojukiqw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2tafketlp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2itkbyftq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2fvdzlevy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nletsbaj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ipxoyedv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zlgpobch.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ultjurvc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2saenocoi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ewluczde.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujlivnbt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aoieorny.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xzsscuqj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vqubjpzv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tozirare.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xaxohuno.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tvbusfie.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bjdbvgdx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gjflsxju.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hwweppho.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pwrthxvf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rqsijmch.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sqeqrkdt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kxxghiov.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lyhtopyq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2yzevilqi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2vyeweqyx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hcriueuu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2nfjaacgv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2idbzhxhn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nqlnhpdi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdhljgkx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2aybkjzya.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2whjbazpt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkggxdz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mtgahncw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ilrphdrl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2brbpkdro.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yecamnvy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nysntznn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sfypxecd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmwcydc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgcjjzk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qlgwrcjk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hstpuaje.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xukonxrm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pfxgatbl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpflsxqv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dxjyvows.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fyijybey.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ojbovoxn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fybyzlgu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtpqdriq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fpyvsbmf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xwoxqzss.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zoyktoyc.html


<!-- 参考信息 -->