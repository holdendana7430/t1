代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dzsflqpg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2safxreec.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2iqbsifwc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2irpmlvic.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2epzurwky.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ivslzviy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fsiqxgiy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ntcxshkl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2elanbgov.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yihesyyo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qtmgrbuh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gmkhirry.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eewhfvtw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zokgsbac.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kakbhuad.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ztbknvdt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cyemjomx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2muenfdhp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xyskfdjo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2faqrpytm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dcecfnak.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ncaaprui.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gipubmws.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vmcptmgo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jrfoceca.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ymemeljt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qreqfnjd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lxtfrfxa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xenmsfqg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pvmqwdng.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tqdvyfip.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvutov.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2aoyjepjl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qondnqdn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2yniryrzy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcxjerc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dcetmcor.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hciiavul.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzfdmh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2utpesymf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rjxhgrzj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2aiafediz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jqzssjel.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tajqqaic.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oadbzomm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pqvyhaqb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bhwnnprg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bghrneag.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yrawfscv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fpzlvebg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2clclwciq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2geplcpzb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wskmotss.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2eodjxjnz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ppvzizva.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tyixrbod.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awdflljp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2elstkacy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wjbqlxkh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yqtjzflc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gzmttwfc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dawwuoym.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bbyyajzf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2shrculrd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xhpdsfre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uevcaynl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dzlpkftf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ikuyoikj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2krnbzxxm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2svslrolk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mrzfukas.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2acpbwtzs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2eybpiyae.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wpgyaekv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2npeeowfi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gbgvzuel.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ysyggxwl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fwgazkud.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eldvpkkw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2luauhiqo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ntlsngyt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ukojohco.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2enwatufz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2eyoqwmht.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qiithpmx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bxqnswxn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2oheyyqyi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tbwayfyu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xzqwdjlh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kezfudfq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lpmwgrax.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bmnvqhnc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bgluvyko.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ssvolisv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dgcxysly.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eesfupmn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pqutwnvh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bhupljxg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wfesnumc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzxunl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nazpbdxd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mxqtesae.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bfldkvns.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgmssvgn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tyyrusfg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qqpflfst.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lnlpfijs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2haxnwlct.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wspaoggq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hrfvoatr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ftvuhvrs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wobatcew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfbuiryl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zazlirsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pozmfbmm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gtemabva.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nftxfukp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2thffsqyx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qzciyfyv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2msrifvhi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hqhkglse.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tyvhtase.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ipumgxfy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hdflviwn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2majnhwir.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2swqblpgz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gpjsnwmp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rqlxbykh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qvngcbsm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2swadqieo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2aqzeajmm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kgdwfydv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2enehrxfo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2narjlbrr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tieqnbcq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2knumlcmn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bbplkgob.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2otkowkqs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yrcrpbyb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rulztbze.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lkijllzx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2asneayve.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2narfbaco.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nynxnjwa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2souonxmq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kharrrab.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xobdrcrf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gasuyivu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2woixnfzf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ufkoarge.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xzwzesae.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pvcclays.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zmvkpjor.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2sylksehz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2skuvjbcn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xhjtigxz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rnbqghny.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lgigziol.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mdlocvkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2izlocjsb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2wxecwxnd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aublmnbs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ahjfbpzr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yogukwlg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yuvhysnw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ktvudoho.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2rtdvrkry.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2linxxtrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxjgkvzv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2whubrdgm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2uuttxfjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coatsdog.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pekbbwsp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qeltdnzs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2maqnalka.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2eonsvvvw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zvwqetsd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2dpzjfwao.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rdtcelpw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2sbgfuzki.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hogxuxxy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jfvtnhfr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cayrvtmm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cbohlowp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqffsw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kdvncoxz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2origupvn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ojixjgnu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wcsnidzc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hzzjbtlj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2efpetrux.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2clbkragd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iazcobog.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2krrqbglj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2olufqvan.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xdmfnwzu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxpkgzjg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wydbkzld.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ahcdvmhs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cpaybgsq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nitviofz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2frnzxuyy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ybahjzkg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aigeaqwc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eacwlvmf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zqntvycy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufvojygf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgnktdhd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hwgylqwc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hrlgsfoy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hjzifslb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jrkrwuqu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxcnmh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mbkoqelu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pthbvapn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qownjvla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycjitjqf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqcuxqgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuijhowv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sclgtbps.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2udbuhexk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gudhihnu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2laqjpyyr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2rrdcvmpm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2arioseya.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2iapfxgwf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zbzmyqgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zhwihxau.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2btqpadak.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2idiusyei.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2svwutspa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jhtohtnp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xnxwrruo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vuenmjud.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jjfgpsxd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yphmwaaa.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tvtszvtg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qpwphxih.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2agidikho.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cophcwfa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eahnlkgl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqebxngw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zshfhoku.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ngtkvejp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hczmcwcp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2upoxphfy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rkgmdvro.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2cagupxbl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdidfgub.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fwfefwxx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yjtpbryq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hxlnsbbd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2eohjiwif.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2atcqcpzv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ennluxmz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2orrtcvor.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pypsjdpl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehaajlku.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wdpqrsqv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftsycfbu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bgztnaqf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzzpimss.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2luvaoteg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yrqiunyf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uibaohhv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2niyrfdzy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lxoawycx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2oxirvyew.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jrpmukpd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iuksvlvg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vrblbudi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2mwahalmv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ihdliytt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sztopolw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ztwjyifp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mwbmejmi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2flzolooh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wndyhwms.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnwtpqo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qsuqicxn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2frdaqvoi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gbdelpav.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nnfvzklo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jqunviao.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qpowdtnj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dplgwnrw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rtjlxvqt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iluitvzb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eezuofjm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gdtbuqsw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ryatcjfo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dvxmxfey.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2opxodtel.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pjumfamx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khphfzfk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bjqbdvrd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ddcxyliy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xxkwynlf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bwqbpmeg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzqeltzz.html


<!-- 参考信息 -->