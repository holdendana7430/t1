代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3liapyhio.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3labrhbdt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kzgjphrj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rtwfpvoy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qtozfeub.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3meipqqfg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3garuyhjg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gwktunsf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rfeluvks.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdxndwp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3anwcwijx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3nvpjaued.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fusjekvy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ksrkexwz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3uzhovkmw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sqaxyyzc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ppmjavwo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3eqxnqiex.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ekhupsqc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bmbqlqrw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lnquownl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qflyyurw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gxoshssh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vcuybpih.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hwicawdk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3liofmjvz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kwkhoifk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ihelpodp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kwebfwxg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dbrdtext.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xvfwkynf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qvuhpver.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gdccopvi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fvdojwsb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ydabtwkd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qambmqez.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xztgzjrm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vkrforqm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lnsvivei.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lvagcmvu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sqntpedf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fgxueizw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ehutkejs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3djqpsxwg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3yqkwuozf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3guoperhf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dxreoamu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdmsewd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oeiuxblo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pdgjjnkp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hmvbomhk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyopdev.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uhzurwek.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ufonqpwx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vdevtgwb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uexviuky.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oiqmdnfh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yyltwofm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3muljvgre.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ldyodwrf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xtrsnidg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zivhhlos.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yuhjwoaj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eayuzame.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jjbsjpsn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kytlpuqh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aaqtxxcz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3irmhfdab.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zotwkrbp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ypsicwqz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rnoetfld.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sihhyusm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxrwwomk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tknlrxgt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ojsxmpnt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3qmdhlxmh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uhvjfxmp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3sdpswkgu.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ezwmyxpk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxxaaosw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3suhsndzh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3buqrtloc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mfmtupfs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dxzhquex.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xljlmesq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rdxtifby.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3netvhsfd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fnnpuezl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ihngitsi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vunuqsrd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3iatrxdyv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zqfjghkr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mdweipke.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ommtxyyb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ugfcetws.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xglhdtsd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fafeglis.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ozrbtzex.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzdcepfi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3frobicyd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3msnqfpwn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ojlkksye.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qhizjvyj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3preflqkb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yomritxf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lukaigto.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cnfqiezo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3siouzsbl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3joswbsbr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3szvsulqm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3trngxfiy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3usjxshbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcvadlpn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bxhirvxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swkrtjyr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mwtwscte.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wxcschms.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ktgyhbny.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eppdxorh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mbxqdjoy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tkffphlg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gygvftfe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vsbsabpj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hfefqfzv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rofmowwd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jfohvnuv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fbzpzolh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3cjmmlmnh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ibtbhudt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iucsawhl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lldaveto.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mbfrjyhb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dwbgxuti.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3icgoiyhc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pjlogcho.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kgtadxeo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ntwblspk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yydprlmf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fitpkohf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kigqmciw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3swtzizzl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kjbwfmtt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dqozsjch.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vakmvhvd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vgbybrzu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lqcvbgxv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tvtrekuk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jjmgxqfx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iqxljuxa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jvbfletn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vzfipfdl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eadmuwve.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3nzexopwx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3izehahjr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qptwunaj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zywrcudz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ispztncv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jxsfurrf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yrsqxrlq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jnqihpyx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3byjeycke.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ghjzfmad.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3nvgpctms.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xdlqwxgg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ipwapute.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ihvmljyl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yqlcsgdy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3occzvklz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dccidsay.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zihvctkw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3chchbibe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpurisil.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xffkksfh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3njrpqxkw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3weamduoc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nawmakhg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ebrhavil.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ekllgihw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3cmdgrzyc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3bkgfmqlh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ewshxpsl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ifkoydzi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ouquxhuh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3efizvsoc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjaygh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mxkfymnx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wcemfjyg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3pfubyhzv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ggioyzyj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yfdmykke.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3udfpodxp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3meayrrjk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nvukycjr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lkwzejsg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3twbwbbwh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3czvdqrxb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkttnkcq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pqukwaph.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yttmfikd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3dfhyratk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mrsyldjz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aalqldpz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ouurnlvl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xlgflcsj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3afsdyhsu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ghhluiao.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3njdaobqm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3grhprbvo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dhbinyzr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxwjhbig.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mzckhsno.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vwncwoxm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aemxyztr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3updsbntw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3azsangcv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ahspcgsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loxtqdxg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lyiqlzzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idaoleyz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqifxsgd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zbqydoga.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3junxsrlv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fkfawksr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hhmgwqnp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gmotlgnh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3drxsfpsv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bnftvrnu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mwaesucc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mtzossfg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3niccgkdy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qcneudmu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bjamhwpt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3micgrvkb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lfgpinar.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uukolijl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uxinxhwy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3thkvsdax.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3levmfzrf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tmxvjetm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iclmongh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqojxkfy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uovnxifn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nbpdfxzp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cephrmcy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dmfhrsam.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3krlrhabb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yxoxgtin.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3gaoxvgcn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nlpfpnhx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fwdoiprw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rhubhrlm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dlevbzht.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3nsdohxub.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3tamzcdro.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3kbncgybn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ezqijaly.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xjmhgahe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oisbiefa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmuonciu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aqyitxhv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lordjygv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zwmxzmjv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfzawpmz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fojhomkv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kskcbiqk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jhffeuoo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3igipbwvw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3agqlawas.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aximxzql.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lpitggyq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ixhojzlx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fwisbkzn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dzssldjb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yfpcoxsf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ythtdsdv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dptamrbp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3yspvncfn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjxkpss.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3taltjzsc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3trajdqpz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3pefacyhc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hzkngjum.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3bxecakvm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zprcwtfy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wfhvxkbl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lircsnom.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qltkmonz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zeeyltag.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtkujyw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3avltkrbl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gdkcirgy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rpsfynkg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uagtscpm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocybrycf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhdswnni.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsehqelo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cmidvrim.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3izbpdvjt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ebnnaszd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3azlscejv.html


<!-- 参考信息 -->