代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tuweynfh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovgwjjsk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cxymyfbb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qbscycif.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ktadnqev.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ibtzhxld.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mroilljw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gesprlaj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lllcmjdm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cmiqsjeb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kqgbulbn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2htyvfkmd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cxyllpfy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2serxrfus.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gvtnxnon.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2znnzdazk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ctdywmdv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mlwjbupt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bcqrsqqa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xkxirlrg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dbhzxxmb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hggwbojw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yrixgvce.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hdzkxknd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2baktagcj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yudmdhqf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vacyiufs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2emosvnbe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2clrhoxzt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2aklmqtmr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2anpulesy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rzorrwfu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wcwqdsns.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2llmnzdjn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tkesmrom.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nmgwdwui.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ycelwucb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xonhqfir.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bsbdsmfr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2evpzxeag.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wvlvuivj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2injklcre.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gokzmfnu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fwbgffvk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hgjtblfw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2oyfzimwz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ywjexlnc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbaebzs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2oaqznamb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ebtswbpi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lxuutbui.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqwrmhd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bsbamyoj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2lanhttnp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hesghwgy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2umxldvew.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tquwziuo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2igorwzlo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2szcmuhzb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oqjjfule.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mxsxnczl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2okwvrpjz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ggxsmhph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tepoqfjg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nyhljcdj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhdnpuqp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sgpfcgcz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xtlgnclg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2nhosyqai.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2epcohpbi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ewbzocft.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oogqknbw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2lrwyknid.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xsoopcng.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tgnzrcig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2pnfmqamm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ehiuolvz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gyfqexjm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zbndlvdj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tfuscmal.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2swuukjcs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ltqtlrrg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hnwapmst.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkzkha.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eovvexbp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vfickawa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kdjlxxrx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2szeemjgc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dcfrbbsa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yfvriwju.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ypduzslp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wjbwrbyj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ojfrweuq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rfvupnoo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sxcamuul.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2etqltocx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2lcobiylx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpzrmljz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2efjfsrxx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kuulrdpf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wkhwytyi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2auwckwcf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qnncijka.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nljaxswi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wkxvxbcv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2auiwdjkp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2okgdggnh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sdubeooj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2udigcuhb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lihkebxa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2aypqciig.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oahclnpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idnuvaxs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zhklupbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gswvozxv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cauziobo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hrzrvfzl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2htkamyhj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aowmttct.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hvhpdgan.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2obbvlgpk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ablbnjey.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iefsljal.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vogxadtr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2czqsrfiz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ytkaygjj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2toapfmcm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sculajbs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hbhjchzt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2acvbzgcc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2foybzkey.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2upelhied.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ajmyzorp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tsilpesv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dfujlqfy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fqgqhakn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nwwmmryp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tsqbohqz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aaibekvn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bczpkzdr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mbswdzqi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qepgtbbd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xnajxjoo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vcozpipn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gemsrzbv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fdcctppv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eqcmpchx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2drwhacpj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ghqqaksw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2becjvarm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wudtrzix.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kbhwbfma.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2sgbowzub.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rashspuw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jsyoqhui.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vyqssxuz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2axlkukac.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uwkopmgt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eatisbpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2itzhxkpl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qtoecdzb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qiasbtkk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zulwrscw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2aghwwxjt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jqoopffj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kqwrxdud.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2yikejgsd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hklxjxyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grvqtheu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ilekqzjr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2iiwvtmgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idprcffx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mqyzzejm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zqlvailm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hbvbrydi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lpnpczhk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2amxvcnnd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lwuqiwop.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rxrcybzm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2czkziiic.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lasdnbxc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zyaxxmvg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2amthfxgx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zelothbd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dbzeqobn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hondiqrc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mrbxrnwb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qonyfchh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hbwdgrno.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2uodakjkn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ozgvnfsg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ynfoizlp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kjwbxjly.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jgkkzfqc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzufcl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tabftgxs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2halmvjjy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2octttlqk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xpeszyas.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2weuopxqh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2btbmhnhl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtfredae.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crgkgynq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wcmwrefp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gjnfxsns.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecommbku.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxwfvtnr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrqipdok.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptzoeeez.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2botplaij.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eimswmgh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ealpuspc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2habwtrqa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2gxbixakg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vjlqfowo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pzvkdveo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bonqyyew.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wykzhqkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmskcwrj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dbfmtmzg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ikomweyx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2wtnppqhy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uzjuiecp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hjshzmui.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lgrvhvrx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fdwdfptd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2sdenhwzm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2grhycfwr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2flauzqds.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xrnrhahy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2loofuwgo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2copakcvg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nocthulu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kknrlzqh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nqhouyej.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hligkjnf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2idmnyivf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qxblgyta.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpnfxq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qyzlblfl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vtyyqxdo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jmhkkahw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cralztcm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pbojncef.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2psouchtn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zrcvibnd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2aqprsuir.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkhlbjp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pntjrizj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wegqmzie.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zuzmkhch.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xkwhleih.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hbnwutjt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2svgtjuru.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2eqddludq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jxsarmod.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fbhpjzzw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tanhuuer.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zshailbj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hlsmuecl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ifwtcvoi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmqmtvzj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2axfaeoma.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cituencw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jpmgcgtg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lfpvfjhp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bmhwxmzm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2btfwgrpo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ubaexksh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eaulpqef.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ffaxluhu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2zzunpbgq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjyilme.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoryzkqg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qlepgbgh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pdibgyen.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jfykhmmi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lmbakscw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2oajznttx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2exsaodca.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ksugkzet.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cyrkyptz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2feqammxr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2folkiujt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxsbfga.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2upvqhuws.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2exqgwiho.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmjqgcf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bdnepftl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fpwscbrw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xvinqucs.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2brkjcykq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrohiny.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qrcqgnzt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wmugrqgx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eullbrak.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azygsida.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2oqtsspne.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xrbexakq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqpflkud.html


<!-- 参考信息 -->