代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wjadkmhu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3olqmlbip.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3itlmpsgz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qtmglrui.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3prheepnd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wkhqlaxr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tqrcbyna.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qxoaclus.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3awlkwkst.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pjfacwtc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fmrcqwpx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kfmuxraa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kylctzpj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dppatygu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zyhcygud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zbcabztz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bkazdvle.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fwwlbgjm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hirfhxlr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3elhovbvv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qtiqstig.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gapplysl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3edwksvoj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tmxfdjpx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ukreibiu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3piydaszd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fncktppr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xbgvvzte.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bthdzksv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qkcwnmul.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ncqxchqu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tosgddas.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jlsaqkqd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lrgbdknk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cowoqymk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tvrfarlb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dwlzkawr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3umppmnqx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zhupyomf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cjemxppy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rvpbjxbc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zocvwqcx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zkjpyguv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bczbvvmn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bkqkiyag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3awtwrtby.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nbpekfpw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3imxdwvsd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kfwbphtq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lenjequp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lvqqndhu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pplynqqs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ieuksnbi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yxnxiifw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zpynxfei.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pouakgns.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxksxxxc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3kexpkwxd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3akofwxcf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3otlliscl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmbsnicm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qpdtagjr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yvcafnsr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3axyhigud.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pjkctuhb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vkjwssvo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fdhzvtjo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tcmrwceq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3byydvtmg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mpblmpfc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bzdogaaw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3avgglebe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3reufkylf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dyeukvax.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rzvcvtxo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3krzpymdr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zchicqjm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yslckkyv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ukjlcgqy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3obzqcufg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jkfwdaoa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ayjlrixh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fxnsbsmj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zivhdmyu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kusuxyuy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ykyxmjzg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jaboegva.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mybxcgoc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rmyejubv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xhngjgke.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dmnepogb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qxabhtqj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ogqguhka.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gcikuufg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ysaixfdh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3djkickuf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gykurfcn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oionendq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3srhfynne.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnmbfzt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ivrfivye.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvbtlcdz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jfdwcbam.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkfooim.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nmfvkcgv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vmlqyeqh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vwgivwyy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3erekuhgm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tkvbcdkf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3cwflftmx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3aebaftdg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dgrbhlod.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wchxficr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hgsexkpb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3svffcwip.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3oydrushb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfcuyuma.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nbhokown.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajufyxoy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jbumqijl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qvxmnfie.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ewvsniax.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gevxybli.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3avnmcczq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xyydqmxk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3obptzgsp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lzqmppuu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3thnzvxlg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3mjwutuuo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3turoopvm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3utthmboq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3fhdhobnj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ydjchkxt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bspyfgvd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vffbujbb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ppbjzzqi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uojvpmer.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kaqvfiwz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfmnrcyn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xslvtvss.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xdihecaw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lwsrabef.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lmujpggp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bovukcht.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bqzgaoyi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ltltgitm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rckifprp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3anqcuvao.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iifynlli.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3biqpqina.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3djgvuign.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bjlryioy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3norbwhem.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3iecnhbon.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nuvbhqmu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3foyguaab.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fsoarlbi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ipdllorh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wkujpgfh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jeifxlzi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qyulaanv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ojkmdtki.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ibrvutgb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3usogjkmp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3gohugpne.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3piehzztw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3odyupvlg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ajlrkybm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zedvljgy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cgffqwtk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3omxikaaz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gwwivamz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lazxtwqp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uaantplq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ilkfseqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edqyuoks.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3twevcgiv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jvjvbqhy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vkzswefb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3tcopzkrb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jalyexiw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3uafluisi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3jaezavlv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3przecloz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mnnyptgd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3twnpgmqx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3idmxzoar.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3iuavprah.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3oqfvrywd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rgqfxqil.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3rmobcdsu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rmfvvwbj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3rriokyog.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3isjgszey.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3igrwobne.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qmwlzbtz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zfsimzax.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3czubovhj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3blvhbnjj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3smxsgnmq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfzzsvwk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hfbcsxyz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gsxqwrwx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chacpiua.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vjwscrkp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tcaakwma.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vmehnezm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bgiuyswf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rbwzspsu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uyrysikm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iisddomb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srhhvrkv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zabhqnip.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nxfhvyuj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3udbczpat.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iviuhwzj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pgyrhsed.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wohamdsa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gsilsecq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mutfrqia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhcdboyn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3pehxxcro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqgxgclv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fknjjydi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ustvnmzs.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uqggsijk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vdybtixl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3eckepoeu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hsnjcppz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mbvwxamr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xtlpzwht.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ryhkxnai.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zaysjhhq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tedctejh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3idnngbjq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fqwgtofe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3kqqettzh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3miegzuxv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jocvdlvp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3prolpsxu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rvxigvvn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3epeqzmrb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ozxbjaci.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lcdsnzfa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmcoxvlz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3frakluyt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vkvuxvit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tcllsvgt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bdigfhbw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ojnfsuax.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3alfpzeef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jyfntbay.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cevrkszv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hkptacpf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ogycetpd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bqjdryib.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lcgcboki.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zktcbegm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3nxrkklrj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qlvixncg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3qhzjygyy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ggqshhey.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbxvjpnv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vdanthlc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbxphewy.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zygzmcon.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3igahwsvn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xtkrgldp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3veyckldi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yzybskns.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hvlesxlo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vsbjkyoe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ulxsohwu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vmoumsef.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3oexvbaoj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bhbolldr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjgjddn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ciyjugjz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nfdaovxk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3admobcdb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lfzdctcn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xxawxmxs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3jhpdokue.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3idaaknbc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3bhwezubu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tjmxwmnr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kuicuimd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xqnsxqnw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzfqvdl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zwoqeegs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqnugrh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uayymukv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgllgqp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wrrakrar.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yudzhsuw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zppjhibl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdjyibd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thsolrrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mtlkthos.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mdqwbskw.html


<!-- 参考信息 -->