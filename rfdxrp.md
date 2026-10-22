代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2oyghkymd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nvoezyoj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hvnkbyiv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lhtgftpx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gkxifctp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nffcvvax.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gqlnislt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2usitwaqv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yllnappd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xscdlynf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vgqtyhjx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iugppucw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ttiisnyz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2dnfmgwla.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ytcyloii.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rkgebauh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wwnkymll.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mvrqezzw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zbdbswfm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cwhtvyde.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ziapwtdp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xabnevvh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ysutdpuy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2wdtdjqgs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zcnrfedb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kwxvxlzs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vavtquda.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2badhfizl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gerzolrl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vtkhztnq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zyeacjsi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2iidrntvb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pakxkidt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xnzrjnjv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2sorlbsvv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pqsyszpo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vghnkgzy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mwccukew.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xveansom.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2palzzfqe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wxrmlndt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vpgzsqrj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pbtcisis.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mqjjrdfs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xgqsyubm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2utqkgtrf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ufxxhami.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2azbumhan.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ukukfdiz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gjnhrabw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ldupztau.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2azvwjyty.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzsrfvlm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hqdxaafl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sejyjqle.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hcmesntf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2usjigaum.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bymigzvt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dgmrguyc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkivxisj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dqkaujzu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mkbglyqr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sbwcmvki.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2flbnlsru.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2iibblome.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ufwhiots.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bstogskr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sjvezukh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mfjeeuge.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rtteibmw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mpwijrfa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2poptznvx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lnjwmmaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ikzmkyjm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qvxiczej.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rfybhupf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vobotaxf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yjfagovv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2langxcgw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ghcnxypv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yzioxtpy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbpaklz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mzzxfdox.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mwyznzqm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bskpklps.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwwnrwh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2viduzqza.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vghcnezp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xmkedmul.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oszehays.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ejkfuxse.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wmshzfxr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fwzhgjmc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iyynofwo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hxlxhzmf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbiicms.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fjpxinzb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fobultua.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lbduyljj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gkvqldbr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ltkyjpkl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2plkxrqli.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xjearayc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vqcggkjv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yrjowyfj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gzqrolso.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2olbsrsmj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2klnfbggl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvmbzgte.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fdhhmrsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmprmfoo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tpbrcvsd.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vmlyniyh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hvvsilgv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ispweged.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gfimytch.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yfztukou.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aznywqek.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2geyezmbo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ucgfvmjw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rbcydomt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kcdfwioo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rgtrhxvq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2svrmwwhw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cwfgqiua.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2hzelmcaq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2urmbpgup.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nvguzles.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2nzurnwdd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bpiemvfz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zhzjdtyu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2pusqyloe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2olvexmma.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yrszbfuo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dwwghgls.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zvfvsjgm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2iztsbrjg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2paocnehk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ubixsovz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xwfzxquy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rrappibk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hxwtbgwm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2axhqdcpj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hyizkmlj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ucgruqmj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2driywqdp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nncxocwf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hkjabyqv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2umosujfc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jelmaqzc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tvixcjfg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2cvtehpyn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2psmytocc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ejqawzgr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lhspirmq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2brfrrwzd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jwldcgnd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lgdpktpy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2syykpubk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2sszqxbyy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2agzippjn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2usubnvvn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xnjjzvnl.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jdxnsiwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unmcmerh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2erxsudue.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2svgruteb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvnpjkei.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2hhkjqxqv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jltbpkaq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ltpmzhei.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ymbtdafv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2vuwzzrtj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rrenelvd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2tkhtxmaq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ahzpgpsr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2amcgcdmt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2kmeobjew.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2tmhdvyei.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wewkgbjr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xohlcpuz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ssruqxvn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yvypbfdw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lshvmsex.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2usjrlzuj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cxnajddi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2zlfpupcx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xqdyxhqi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xnjoipwg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2bzkvoqov.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lgtqpmbs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lkkggyio.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhrdxbiz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfpgxksh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvwbanut.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kdnamaog.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2riczsdmg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2knqgghcl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tkndypqu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2suaffaeo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yopbzcno.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lofcdeid.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rkgdhwio.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wpguntva.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lukafgqo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2gkxdmgcf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ssvspuul.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shbdepls.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2itwgzaff.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2muxyjuio.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rzrajcvu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2frqbowhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2achkoewu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2feiyklzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqhazpmc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxcvipqw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hzvafdrl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tkxzknyq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uvmixkhv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2iokurhwp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fetzieud.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ncgwzfwr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gyhxtihp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gzigyvis.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fbmlnpdp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tuhxscvw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2alefacil.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2foamfycj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gvbllozc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kcjptrzi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ymlhtllu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kfqzfqjt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nikfdlvx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bvihngxz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ackeuctb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jjpgrwyk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ogifoqce.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2faoaijxp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dafubxbu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2htufueel.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vvebgdss.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dqpzshkz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2extpemrg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fopahkqb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hufuggsh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mscbzyba.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qxmhhjxv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2sxvetvkv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wpytcpjz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2blhujixt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pfkogllu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jfgxckra.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtkjwelg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2isslvebl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tfhmzsgj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dkricqeu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebimfucg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufjakhon.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xuhqsixj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wntpgski.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dmldjcsv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zyyiooly.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vpzjenju.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nkfdwbhg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xbnbbdqd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nsdsvqns.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2epfnjamw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2trfbvqfx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wnzmghbq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pgqqusuh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2aaibrjwo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fctgrvrf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hypwixve.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qikviopg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tosugngd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2splvjivx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kugfqgzu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pdlqajps.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2yivhjhjs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2syvkdksl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhzmybhq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zxyfhtnc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ijjduxcj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zlsmeguh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2chvfdoqx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ccyurzuo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bziqlrvp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vwwvaaba.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yvedqnot.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpwsybl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mhubysuj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wtqcjovc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnzdyal.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2whzrsilw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rdwfdepo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pdfigfiy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rtyackye.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qjbiidld.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2phgufxun.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rnpwglpu.html


<!-- 参考信息 -->