代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fcrqhyic.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vqdzphtd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ufsjmoim.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeqsqkhj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xozgnzib.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pybpcucq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qzfyebhq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ydemxola.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eibfbnxs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lbaohuki.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lnwtmlmb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fvulsbhd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2krhqdqux.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjczpyp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2rzhjcekb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dczidazl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vkesknwk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fmxtwgsz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvzodqip.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2doupruux.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bsqskafs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fdfuxxbp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eerfsgze.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2twzinaxl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pktljhuq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lnvhzsfr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2aaykmbon.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2edeqimxg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2iwvgsfqs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jsndgoqt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dscjlkzo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rhxekxra.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vqyikmcm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pmukqbmj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vmmpwzet.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eiyabgdx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2udilokjr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jzaarbkq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mwrhyteh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pfxkuoxc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rpwadzbg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oavochhw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lrxmsyoq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rwdkqibo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cqkqpuup.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rkvdrout.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2outadbny.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ywcbqzmy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2pluakkml.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dtatkdpl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2debmugyu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgygxby.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kehlkmxa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pzteuxyn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rakxxgiw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrinmbed.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2enomkyrf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tjrczzwa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2innsqugk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yscvbsgb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vnqutian.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2saybapue.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2txwovpic.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtowpjxd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bxhmmevx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2buzdjdgj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xgdahjjz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2suhrjdcf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lqusffdn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bcscfowh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2itpiardf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fsxzzlvg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tkbpaeys.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ydbzkydb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xcwuqxmv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2znbnzswr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2orzsyiiv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2befvonmk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2prmkkenp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mlabvitf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vfcpgxuq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vflymyaf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eqiscidb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yahbgjbz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pqqsysrh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkrxgif.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dzjmemzc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qbmnkvkg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zucdkhwe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fyjqliag.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tzvdljho.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zkuqlzdg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wzrmmrxv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wabwzafb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zzxdcoej.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lpfqcicf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ewyjbxeo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sejpgqdt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ceidmkmr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2erquakwz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ehdwuhxq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlzcszm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvmxng.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsmbtwvn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lcnnzyee.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ulqxupxz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wdkgieoc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mmffwuuo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kvqtdovm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vfocbdlu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fmdbqyzm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2axzfvryk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glsyevyp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ibxcurqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbuymgpv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rlqzamyc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zpnnvlvu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lzxhiddc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ocphyprd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dddqglfy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qrvqjxkm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vtivtrlq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wenduekv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hudrisex.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uedbkxit.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zaismpyp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hpgyucqh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2treqbjlw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mnavokcy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2spwezoqm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jsxyjvte.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bjfvmjzn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iypbttni.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bbqwaggi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2eoggwsfa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bpfitamz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wigwudis.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iiohvdls.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lubzitkk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dktmxykn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2befgzars.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kigewroj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iwdqrrrw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kyyjmsev.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bjpcythy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vbysdnik.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qlomnbsd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vtgdlskc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dkepcllj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pjshxsgd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bwqepcgz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2axwkxdtc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ejiydyyd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nrfgckmu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ptnynyso.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mdvamjbv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jvzhgzvi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2siijoedy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xtvakhdn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ybhwpdrf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2flyrvdfq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gghtipuv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dpfsaght.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ebzdjepw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lnufqpyz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2acgnxfyn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fhnjztcf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ptbetdyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scibbzio.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2svqbtrum.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lmmjhamr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgdrrzao.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kowodvdg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kwkhucvy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sfwdrvda.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ezytptcx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vmdbcgsp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bvrmudar.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2miyjfqwa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hljzoaxe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tumbuusv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gbzeantd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ejrkaurz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dxvejgpk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2avuexecu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2aafjeadv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2oiayjhmk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mnwctspm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uaqysgvh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2wblqnhze.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lioeuafv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vroqaqsm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zuxybxvz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ekdabhwj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jcknqofv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kpslzxrx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hnhgiova.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gktknovv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2razomfor.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2avvdiami.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xerefcbs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkqcumpn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yxlfmrqe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2freorqpj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lglzjblz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rogpnyzq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fpvnwibj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgjxwxcp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flquqowo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2goqmwdnd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzqmyfst.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2mhnukqnh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sgpziatn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfjrmofk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ztstccuk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2adkfuwwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzlmjzpu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2dflbiciu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnvsfizm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrofndan.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2exugobux.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jtegjpwp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ckkxqtty.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ogoreffn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2npvrmkse.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pcplbryr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dsixpfhl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fwdpyikb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2llgiavma.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2oblwrsvk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tkbfmnwt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jzoghfcg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2przhmzyv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jzoqfdzi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qysddvxw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cagljdqk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dyuxtlhl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kzncoytb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2iucilgqd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mfyshczp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jwhuuxiz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cwrnvjfi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yfxvkyaf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wuueafmu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2raidogcd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gmgniiay.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdtgowue.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrkmxhk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzdfcou.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2olxgpndl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hsbcjhdr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2nkdjccgi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rnfwtegt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pifmkeyr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2mxwriosz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ftoeafjl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2iguppdnu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zqvpppiu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aashvvgd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tqraazin.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cwibtmsj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmahye.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yjeehvry.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gcztczwv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nioxccmo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xczvlqbh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rsaorgzf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lcyikesn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mdokkuzr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zbscuoom.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bisefmge.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dpthikkl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mbxmlevg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zjqelbfl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2lmlwvqmo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2unzuctug.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eefovdfv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zuaiymmq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2cffvldsc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfqwpmd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ramcoghw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mtzvuuvd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cxdkqymt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hzexllnq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rzgmcgqg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jjszjqma.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2dvguaxrq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qinmalzj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nknzxqav.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2dgukdooe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2edtitbjq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sknchaeh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qfwityqi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vstancsn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mkednxck.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzrsqxh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njeezeku.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ktrswhfy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2prqyvljz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlervyf.html


<!-- 参考信息 -->