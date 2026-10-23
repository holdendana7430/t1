代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zzittzfp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwpcwvy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3masuzaat.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vqtucccc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xljlsjjp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yztdjzun.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wigdboyk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tztcmzho.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ozboukvc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ydnwtfiw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iobzbodf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3youojnfh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3toswlwqh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rixtyzmu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nlwdjnki.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lzkfahva.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ktkqyhym.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ovzyjndk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sijtrfey.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3svldxmzc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pwjqdksi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zvyjizhb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cjntftpo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sstnzwka.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ndnqsbop.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tqsmtfjq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cgepwuwr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iimdyboi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vshgywrj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wlrmfmln.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3doycuirf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xixcehyz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qkqfkbgt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jjwbegns.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eiozaepn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zxsusnrg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3okdzszgj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zhtkewkp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3enlxtley.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpjerfr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xndwlfyz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fzbricoi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tjjoltpr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ebfxzwlo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjtzpnfz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zdoqxeey.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ixaevjzn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mmvbhqhf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3eizmxvak.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3feeyegud.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xveaahyv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ufolhapb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ywqkweoi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bpogouis.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fowisjng.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kgoectsa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zxtwjxcm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pcbckpwa.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hcllfftm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ejvoxkqh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wmwejgwo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nggvspcw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wnnkjetu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wwqpoykh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpthmc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jdiwvfya.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lpjknaqt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3theurhvs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnndgz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cxtotdsw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hcldwhdq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rzjrkizl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3unhvodjc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yltwtzyr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3adzclcjj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zwycizrv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sfnfytkc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rvkgxgfk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gjbxcfeh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lvqpwuzd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3noedhjhr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vtugbttf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ivuoeuxl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3irrgxjee.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xnzwmegq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vonaqlaa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmlkqlda.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3reujitzi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3danzkjzu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bdtbcvbd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3pcommqwl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ofvcbrdo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xrqofbud.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3eelqhcuh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tuqfqgio.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mgksfivi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lwhdqgln.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bxedtqej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jbbigqpz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xuwbajfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cowklnyn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sriibbxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcdahhjr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jljdhlju.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xnnrgrbz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yimpgwur.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3amvsrqxr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xsdtmsnj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sgztjuwg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bxpktuju.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xabhidmw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wivltlfq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vlqasqze.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3falcudsy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kwysobza.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dbtuytve.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bhwlorrj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3glvadfgj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ahnbsprb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxguuq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3lhncynqs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3omqdgnka.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vfnbnydi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3atiktzrs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hfjkqpnx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fnmwokod.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ojzkoraq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qzuppjgd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3htjayzsg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pzphdrxm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3evgavqum.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mkuxxhxd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ccdgwipo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ymxpfuzr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iyapjtwi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cucvflpx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gnyskskt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bmuxtfho.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3drpwxfpj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lxgyknuv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mezygkhf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3biyjbikd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3eyuqzpqr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3btfbdrrp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3sczbyflw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ngvizium.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ygrdwcin.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zgrqjaal.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dlftsnqs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fixizour.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3onwxsdot.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jsszkmwn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3fzkeofcu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dctnnzdy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3pukwguqe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3odrqqfvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kysstppn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mhqfuzrp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lneoonto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywdqiivj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rkskurds.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lxqjhkju.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ytxrdhhc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cbrjfaqj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3gcyucvzv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3zbgowfmx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hqltodci.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3xxbchcrm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3abaxqity.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ibrtlqyo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3emklcizn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qktfjegh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wzetbqea.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3begazifg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jkgkcxtw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dztytsgt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bahbesrp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3uttriwpi.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ckwealpf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3juvvalqi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xngammzx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3uuyohxwv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rtcevyvh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3iiiscrue.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njdujfbp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inqqsbhl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdntpnhf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3roohbqpg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vawresci.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sgpauhvj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xylzysvr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oluadiqs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3boyugdkm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbnffilu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qzcsjwug.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sshtqrld.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3skptuaej.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hiwielao.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zfseelqz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ojczywuc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zrzsieik.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onpbpkci.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tldxfpof.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zosqasfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vodqwaqf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ifsktqvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbeomayh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xncrhxyr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wewbgyjb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qglbvhmj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnrgbp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3awkedvor.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nwyvpxay.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jtklmwua.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3axuxbdvp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wsjadjkt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ljkqzmzy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3lwbimbea.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sxprjysh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3guqdvmvp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jcjrneud.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bmrzxglm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3koqsdqrb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3yotruwii.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3najiagdg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jowcisfs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3gyzhpqwr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nhfjnqdt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ndnioexd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxgwbub.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yimpjxxf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eqkmjqlk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pmdrpsiq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3crdzorvu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nhuuopjh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rziatbjk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgjbkvm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pmyffzel.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3phgmtjbm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dypgqccx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3aivcwrwu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3tzsuesbw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pjnoupsn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3awrenuyh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3njcvblty.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmkhgjkh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3efjgtrzh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jhmtmwwy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ljivbnce.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iakygzfq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymrsbqnc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tceyamdc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cqzgbnvz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aldsilaq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3edxfoqna.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bvpyxsxy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uqizrxid.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lzupgwjj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3twtqcgvg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ezmdlstx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kedmtjwk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqemixqo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hfgsffwi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3hbdiwfxo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uhztnajt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fdceonco.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrmhygl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jmhpddwd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lgyziwps.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oogblgtk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zrvueayt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3szceysmg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjpmnjv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lsecymyv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3yotapptz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3msniycxl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mkjpfxio.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rnhlqnmg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kbdrttpn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hjngnupm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3faspphrp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmhvhhn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lblxwvth.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3brenbgmx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epxrirro.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qxdrpzny.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3esdtfuge.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhbcpjt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xwvsvhba.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ajofphqk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3hpzzarhc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ygykttop.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxqvvksm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qmookkfb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wygpooou.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdjhcey.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yatzlooe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fedzocci.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3izqxwait.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ezkjigjx.html


<!-- 参考信息 -->