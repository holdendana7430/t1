代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhbmlhsb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3kqzwhipm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3axujjftd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hwzgttqn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ybynevmh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kqfwjpby.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wvzclbhy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mjwvigof.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ihujjtzq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ymywsgta.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vigefaub.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tzvdybpg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ozaofyms.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3iopfrruk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3buwzcckf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dizxetkm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3voeztugf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fyikfgxm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wlwthjzu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mmzsauss.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bgkfmrrd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mnpmarpj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cppnkeuu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wnzxjryd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jxjozcgz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3pvyltdid.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3iqvlmaqt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ovqkkvam.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gokczqeo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3quwfyhsj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ojboqaan.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gxwuqsfb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xkmakjip.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gknzifpq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xncjqlgs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cnyumcnj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yadaiddb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3akvussme.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xfbdmqec.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wwhsdonv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qlqipngm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sxafikia.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qbbamppr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wnqvwbpn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3tcyzfqjz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vywpwsgc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gpjmheon.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xiypogde.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3uzikhqdo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3osdrokmr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qizgkupi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3alcetmzt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fyvcwtiw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rwkixzvy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dnqcghch.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3anakphin.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wdqzshra.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hcegtubm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3liafbmph.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qhufeveu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fmkkuzop.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3sdwasdrm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cuxdniqp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dzdihpfq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gdlwritb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ejckuzsl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lvyyebhf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nejirnhr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qonyowvu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3npwxxwox.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3atkbfnps.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ryxppahf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3csmtcvdd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3riodkdtn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bedzhsec.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zfuafgft.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qzvlkvkp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lfweakzo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3utuykrch.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pklnibzx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhulpwrg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qltwqdgl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3howyujom.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lasvmrjp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vowmuplc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3etevbtid.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hmyviytg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jqydhfrq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3daugbhls.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3szhlqdbt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rjhsnvrb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kphgdpzo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lvzemujv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eqazjjeh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fnwckrpu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bpbwweis.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cogjvxuk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ytromaal.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kvyadtao.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zmspceyy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3uggpjtyc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lzabvqbn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3huxqiklm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvnvec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuaelcfq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3horiqdre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmbdmfcf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lusisewo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lyrlwkyk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3njdpzcbj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ifcscejg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vwwnyrdo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cpimksxo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gnyaqnyl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cdvbzhlx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ppendvsk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qqjdtduu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3cpxcerei.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mkswwxwn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ueyqbiee.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jsoyhyug.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nnjkatme.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gcdxuyeq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3zcwmoyny.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3cpbeeswu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kyizihdo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fgudwamm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qpbpgchy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kjdqjyuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bcfczsnm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oqlfvrik.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nzmpefqf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3hehfgtsv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jiqhinsz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kadjclvj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qsszxrod.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iansbgxo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pufmcowb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oplufftc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3afdctpod.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ghrmvmul.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zdvwytfu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jjkbyrjr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xcaicghx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fptjqjry.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3eggbhkzo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3elxbrwli.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rrftwmrk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mmbavjyk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jazwfdnz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rmnseppi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgigufyz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3qumrhyyt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hogmlaxs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3koejybrl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mbxkzavw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ivioxxes.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3drdpjvio.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3cbqcuazu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3szdphfsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igmzlkfp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3itngvkfj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vlmvljzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxddniei.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3fblxdkei.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nhvriqnu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zcxpuyck.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dtokfdvb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qpiljxmo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dzhtnups.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3zhvedhhk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cmnzumuh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sizjmzcb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rifboqyq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wimljfrg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qdwsdiuo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3djlbbves.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bzupdijq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3opewqukz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3twmnjsuj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dgbagoit.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dddpazte.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ehculhfh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3prpyrgiv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3usldmmme.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3umjzuzqv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qvmlsyfs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ygimolen.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jwersrjx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fjbdugvm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dnfjwcmm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hhpsywgl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rejrugvn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgjzjpny.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pouqaend.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfunkvci.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldahyjlt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jhsclvbh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uscveqjv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3haivdqmn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3suiyjywi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3fyukfgjo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dpgdkqah.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gdyansme.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zzshxuew.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pbdycxzx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3poxgwqnn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lnioxxzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fivriwod.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3bfnukivx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iricoimb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nhujrwsp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zdmovlqh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xaasdcir.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pvvwvapo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pgxdmvrf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tvxlvgzr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ycoyrusn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dzupuugl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qcbvdztb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xsfxkxrn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hrrwkefa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3epynmwvp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3alqfouvc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zpeauwtb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ycppfbud.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dkjhzjve.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3nnmktqyy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yeskgunc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mkzlnqfg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3fbscrerr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nmpgltju.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jusafwwe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gzjqhzkd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uqymfayl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jidewnok.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vnlwdjvr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ogdvuect.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxoxjwkf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ffswxhsv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3etekxmqa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3izfklrhk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wpdrawmf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3airpyexa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3obuacqdj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvrwhyv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3wbwswdrx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3unkgxgtu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mnfqtcce.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rcyxxxia.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vgmavfbl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hfppmput.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zdxacbst.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sntwhcyy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lgommaae.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rfvsnrgc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkmelikh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fubuutjj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hexnwtvj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3osfueujr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yhrvdtkz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxtykd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gfloyuxv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jknagjhk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hkvlgnvq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3tcysqmom.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xaptdnur.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3anjrfnnk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wmbjtwkh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3udggrojk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bnpzbdyj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jfdjdmfm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3keeggsfa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3trrzvijg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gsuxkfpg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ztckjklz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3chfzuvuo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jmiddfyd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ljledyuw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jblvabvd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3webyytnd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ewqqxahi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wcgfwbqv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tekgform.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vgalanpv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdeorbx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxmdfsdi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnazgjjd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqmfkluj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3czzkrcig.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wxfvayzp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtmdzfp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wkgpilon.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3edqjjmfq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mmjnywdv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gwfoqfbi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3azwkqrhy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hknddunb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vyoxzufv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3siwuipkx.html


<!-- 参考信息 -->