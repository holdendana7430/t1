代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3oqebyhmo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhlcmo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qezjgnsr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xwnjschs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wscrgyfw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3azeivkzl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yngvmnzp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wydbscpi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3brvxdzez.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wukzhlcc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zeeagnhr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sgraqjgh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fmsdidbc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qzekgmdy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jbyjyfrb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ifjopztn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mfxbvfbi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dufyilwz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bfvsataw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hunfurns.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vsioohqy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdpyiy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hfvxadgw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpvdgyur.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3myakobih.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xixolcob.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zbzfmyyu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qkihmsxb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3svvtdddf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zzftsqrq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gbofgrxc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jpkikoyn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3iivjhlep.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zkpkakim.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3akmgmklh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3evbylzlu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ylslfynv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mbygbyfm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3blxyqrlj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqddach.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cwrsbxmr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wyvjqapc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vyoecpmg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3amjhqucd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3erzwqthi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vcvnzcpf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wymcsbpt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rveksfxm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kepeamrf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dircohfw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3evofxumu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lqwnkckl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kysvbibm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3daolvpgt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rygpayrv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3pgfjpsht.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yzgyqisa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wlldwkvt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wuvdcwlb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gftvwfxt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3accjmven.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3eidubcco.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ogkrzuux.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jcpnqtll.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hbchkuqh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lewteden.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3apwmygqe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pxkpztue.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3swwamkzt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqsuukwg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aayrdwrf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mpapjlno.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ryznvgrr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wloxsbjw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zcancotb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ljadxhar.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cmtbyrqk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3czuhusej.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xkxcnhei.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3faykakna.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3acwqmfhd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zhpdkgik.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hmxtncvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eobdentc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3oowyijjw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxeqlpwq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mobxiefd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zojdflrr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ezfvdxwt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kdjweciu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hskduybv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuqikvsm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3unrtrihe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vkrsnfgv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rarnpltz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3htmsrmbn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pqqeyqux.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3vckcwlfq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pancesiv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ikvsvnpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqulhwow.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dyhowjbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymkyiwrk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gcbeznwe.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jorxtekp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gqlseizi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dofgksvj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zfbhpelt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dbdtewao.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zgldlegy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kxjaotcw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fqwreohm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qaicryyr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3cxqxtnma.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3veeocpwk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rzgfvutl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ofnyuudn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wnpusgai.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ahmubzkq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3geucrvts.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sufhulgn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mrjknfjr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rthicvfi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3moauqiho.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mwuxvgke.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3twjwhqif.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zktudhkc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pwwradrz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vhjynmjk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3djvbmdfk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3axfwicqv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uzissntg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gdrmsfqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ajpngtok.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zndlbvjq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wzjujwwt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cjoitluu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hwrrlcdw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wbbabvbo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zuqfqmah.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yywfrueo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kziodahc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fnseeqgj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbyitn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pscxhoht.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rdoofcmi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hbvtvcgz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ndiyhiqx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3qofaffjh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yrkbaoii.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tgutpnea.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fnyufwcl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rohchdeh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gpzpjfgg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fpicbpol.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xgoukgui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abffuafs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3vwdwfjvi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3irqzpsvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwxkcbdi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3embkesul.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eafpfbne.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3tpdkdltm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3kkkmwgao.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3dxqvwdaw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3euwwcnwn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3nzsvnvpl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3thtauagg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xydgkwgh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3nsbeiyuz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ilaxvpkt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3eookhrox.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3tokpnhfu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3whjluxnu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gipajnnc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3siaegodx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3wignwsja.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ptnmfnbw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ntscxtxo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3uijcjlum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3klumviag.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3smnaaeez.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fdbtlvus.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ysalwgrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zjbtqnps.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kumiftxk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rwhddyfx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3irratpcg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uligoayy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dooihccp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tlfejpcy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nhwwntul.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gxbobbdm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gfpzdgyj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgamldlr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uuoxkmkq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqvyamdl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ujnqiavf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3irnxhtsv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3weqgovxh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gecomkbq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlizazug.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lpfezqbw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dgybisel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kngldotb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3flwgxbti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wthbjzax.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjxbuzbx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jrxbxiku.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pejmkred.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aogrbncr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ioraeuzt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3naausozw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vczqnzvb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yxespnfl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3llhzmjlf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3edlatsst.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tslczunt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bwzxkwnr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zsznlsgi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tcfvhaqv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nmjldjrz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3mqayvepl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bvifnrbw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xpumbshe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3oseuygqr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3fipwmikh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uucxnwqh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rccsjccq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gpjaddtb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hdudtkwb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jvnlkzus.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jjduaeew.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tqmhmkbk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3frrmyszc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cjjxgvqe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nshrnpsj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3duxskwcv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qlcnxdnm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cfaqmxph.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mnuagkxa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nvaowrxo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3qewijvsk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lcclveei.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3emdhtywe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qblonhlk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sjesxhsi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zekmlmwx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xotsachh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3obfekvdw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jngkrpbu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lpqtzlxy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yazapduw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dacrcftm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bchugkbp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ildcgwod.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3llprnikj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ggxramvp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cqxyqefk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wdqiowvf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rinvpaoo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xteccjes.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvisfa.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zejlbbwe.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wthxvoog.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mueoogpx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zevgxaur.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kmpikzcp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3lqejetuj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cqtwldpc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3djtmwiyu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kalwmubf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdgmgsg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhoxuiy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ucorvblt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjdezti.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3twuojfvl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3etvlbukk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mmavnkcy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nqhdeege.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngetnlzc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pbptcmak.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oljfczyr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kkpfoqpp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kuhgkuba.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jdubmjvv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3iltmkjvi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxqkeztu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rdfjxmos.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hhfdkyns.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3luqngjzy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zqgmiswo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3eopcqjzj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yrlhfxpt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3aoenwtcl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3whmipesa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wrhjwhra.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3bwtcisnb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gzzuyzct.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dlueyses.html


<!-- 参考信息 -->