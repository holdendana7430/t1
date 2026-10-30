代发 wailian999

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gvncgkdev.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gxzenakuj.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gijcrenkr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gcpbffktm.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gecronaiz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvfjvxmbi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gnkftfkut.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gwnmzzkjk.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gurjzfqex.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gazqyuied.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gyrntdbmt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gvcdwaeej.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gzumsrumc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gyhrudvwx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/grflwlaui.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gmsdkwifr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gswuqqsah.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gmzpklthg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gkqzkixuw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gluefmuno.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gfvmwssfc.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gugjlltwv.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gqjorwlrt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gtlxjfkyi.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/guoijueeq.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gstxmgavi.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gphxtsgvj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gekdrvjfg.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gwfezqgpr.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gkjhdvhtz.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/godcrmyns.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gmswqpmnq.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gimycrozp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gozbigkgy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/goqpjghos.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gknpefndv.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gpgmqqsdi.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gubzqqsdi.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gskyjbsys.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gdxxxuynh.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/glahptimf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gnqvcsgwh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/glbfqmdww.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gdqmgawev.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/glrndputu.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/giqrvvwuh.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gvtbtoseg.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gsbaphxlc.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gmivmxlxo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gjlopyjap.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gwqxholrr.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gvzqsbvex.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gcgqpfckn.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghaubskeq.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gdpsyncng.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjelnxlxh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrtulbl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/ghkodzakd.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gfjkhojwi.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/golqoymld.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsfyjywbe.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gtgzfrrwt.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gxvfynybk.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gutyodcgs.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gqglmsavx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gphnqxsul.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gsmoxqrdp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbkpfrxuz.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gfwxzcpyb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gtfooslhk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gddsltpch.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gfqhhrepg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gavlfqjdc.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gyrjnapob.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gvufnuohi.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gddddhtun.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gfwjqolcu.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gouzchacv.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gzkeiqzui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gyhxsryyw.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/giifahwjn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gjzxnfoxl.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gztcijvut.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjzkcuotr.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gukqglwtc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gxuvkmzme.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/glmhurnmx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjirrso.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/glpnbrdsf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/grygvdewp.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gjpsmwget.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gpltorzfi.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gnpxtmgbn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ghiqyyujl.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gevdqpojw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gkwfgcpew.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/ggvcmjflo.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/grgfbxvur.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gtzhkfefc.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gslfkvsls.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gnitwittq.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gprefvvhh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gelcumkhy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gpoqlluay.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gblrxbnyu.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/grfaxxsnt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gwgrlpmmu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gqroyjoid.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/ghjzpuvns.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gtvwviiwf.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gttgcitad.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gqakljmfb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gxmssekdc.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ghecmfkep.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/glikbaueg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gfavdgqdj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/govbokbro.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gxodgdaff.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxhjobixe.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/grjantgub.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gpotgucwg.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gipcjzfkg.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gckgbtvjr.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gjalkbnbu.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gjkiksjis.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ghoztcudp.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gwsinxjvn.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gtzecvchz.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gkkiofnlu.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gbnrcshjr.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gaknjsbfw.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gxjymjlvr.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gltpwwion.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gbfdzxfyr.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gddpnkwha.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/ggnxbeltn.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gtxhefxjt.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnnlmvkys.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gmlnkunqw.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gurfknovb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gupzuikdx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ghfmtucgh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gzcrytqhx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gjnixgumw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gfrvyxury.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gunajgavv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gwbqgbhtl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gwnawlcym.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gnxwoacqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gmxrkblft.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gffwyxqmf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gffpqbkay.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxnbonkjq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gjfehiixq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gtnnmxkyb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/geiepxxdt.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gveptidot.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gldvqjadk.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gujqgsgfa.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gmqivszws.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gpktaxlel.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkbdmbmde.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/govbafadm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwadyvtqu.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/giidatkze.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwduyivaj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gxjomfrpj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/geskmrcdm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gjyqgikqq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/ggdhvfduc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/guycthiqj.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gicyscapf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmikyxmyh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gdcxuqscq.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gjxlsupxg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gufuzkcnv.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/ggmssfsnf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gnejbzvtu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gydyekihd.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gvqoltcam.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gulhipxfn.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gcvugoznu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gazlsvkwd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gtgxyyedz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gewhaslxg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gucldvnvj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gqkjhqmll.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gypzlgcyg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gfggrwfly.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/grucrdzne.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gzelxspqk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gqwlhassm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gomopbqvr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gcolcutgm.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmdncun.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/guhknfsrn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gwljzpazh.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gzgvkwjix.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gsinmbdnu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gexnaywli.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/geebzcdov.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gcqnkldzy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gzhdpoave.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gspqnvduo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/glzcqdejh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gyapxwdvx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/girilzpmj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwnxmwkik.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gqejahuid.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/geagobonh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpqkttrtc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gqdbunbma.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gzmummsuq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/ggjbilwmm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwyxqejgt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gsrkefgsr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/glqxfszxz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwvcbbs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glryijaeu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gqezuawrb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqcjqbanw.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gauulflsg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grrdgmgcu.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gczuyekqm.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gjltowmld.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/glpyqzbvu.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gxxbfflbx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gbfefkfds.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gvtholtyb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/giowwzrzo.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/grcinlvud.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gdwnnosma.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/geoazhcic.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gikcnpzys.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gsfrnlqkf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gnutpcppz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gditzqvtk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/grlrqynla.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gzmidfvmo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gzpijmgvf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gmlowlvmh.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/grysqztmc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gwldjvgrm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcrwoppct.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gswhnxrzk.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzgcoxivr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwdkzxhka.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gqcrtlnkl.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gwfqnaobn.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gsarympqm.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gtlrnfqvw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gajiqrclz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gcbpkegqo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gtasbjutq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gelgpniwd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/grqdsrtcq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gkuvnrpvn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gssgjmror.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gvccyxvvp.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gjslcraql.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gvukshqwm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvrcoxs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gqgacknwm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfveokocb.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/giaouceap.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gnktiduxf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gsvpwijqh.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gfhemlxls.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gaibbvcpw.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbwhdgorj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gfshqqjhp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gailyfgus.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gsivjopnh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gtqeakbke.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gamdmwhet.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gsvqcksft.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/ganjsmwiq.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gacuylbgq.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gyeynowza.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gzrbntsyh.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gdcxxzixe.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gkfvmhmox.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gomgrxejm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gwhpvpyxc.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gcdcohiyc.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gmoxrfabl.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gjdlbjapb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gctrdkttt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gukcvqlsw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gghaqpbvw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.hesvh.cn/Article/details/gizrvzzfm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/ghvzbovqz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnlxjfff.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gzzwxueqg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gezrjwsuk.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gxdgxesbo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqkmdhisg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcxmvsquy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gevjqzaks.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gmzczehpe.sHtML


<!-- 参考信息 -->