代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3upocmmzv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yspscooo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rgigqodj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ildtoeik.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tuwuczzb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ttfpcnqt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zbiilnmu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wbxwjevv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zxbuctgv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pjynsrwy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3niggtlfl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ttidulto.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bmofcenh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3otmkcwmt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rywmkatp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mxnsqwrk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uysnkmji.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ovkuljgi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ahddsggd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3abiotekh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3piamvbfd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rmuvhgdh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dcnlgfgm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3secsubcf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3twfjgzqx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3npcmfkkg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ygglmvbr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ededpqak.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3errtawad.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mxiehafj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3scmyqhib.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3msnmzcxs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fyjfppgn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ioawwmdi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qqmjjuui.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ynplxubz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kgvdorjs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dsqvpplw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kfakxknj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vbvyimdd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cmzisqce.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bwlpbmts.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3anuqunkh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tkkgqcxq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pqqyrlxu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yipjmlim.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3npjmfwgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ppffzoal.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3raklkhca.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ymehfjpk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mpnucrbw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cndcksnz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eolivwbe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pimhcblx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mgpopvzh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hoqbrobq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ektfxaoq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yvoumond.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hzzsavnk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lwycpfrf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3staulcgj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3uowoyfeu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ioarjiqt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3satfjmpw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwcmivlw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yayjhaaz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xtkcunlh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ezzrdiuy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gyfzzfjy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3aqtjacqw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3iypwdued.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nywkzqtl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3syvwzpve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cpwvowmi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dafzwxzv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oehoafvw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oxrlqkov.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vqisxoys.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nidhnfmp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3htxggfft.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3akazdpum.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lafgmqbf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3demzgojn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yiillscq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lucilopl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mtpptldm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hxuapeqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pxzffpit.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vimxmjdp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3yftjqcms.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jmjrjhjg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sxkydgme.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cwbleegu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uvhmdhwl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hbennrxa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3whkiyagb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3delqwiqb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3izupsnra.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rbqrdbhk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ascilodf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3btxpmbph.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jzruvhnj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hdacdabq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gibcabhm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3avaawttu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vfbtpaze.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cpufaxla.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gjizzeha.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nsruzhdz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lyrivtce.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hacdpawg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqmginyp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3acntmpob.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3beidlxqb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nlyveeqw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3eukwpcmn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kweipanb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ovmtezlq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ghdoywxs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ujmfsvdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwozuvgy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gocnaxim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crqwgybl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wgscnbjn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3keyddett.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3knnesonf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jaqzhvnp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fokhedxo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ligkyvrj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3asxgdfkx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fphsqycj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nfruwzgq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3laapuokv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mkofchqg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vkgsdrik.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xrvcjraq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kmxllrud.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vnnxmbsh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tvpagtpl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3oaklmpax.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rcfvdjek.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ozuuvzst.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jhenipma.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nxqrwhxv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vedbqera.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rlwbxqsh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3izhiwnql.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3olzwsxjq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtsmue.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nhdvpqjr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qtuyeifg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qqgbdaxh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nsvrhokx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3twrqlkwg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jwemushq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uhqhksho.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3stpsujkm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hzgyvhux.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nwycncfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ztsbwdbs.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qeehmsus.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tlfpvpfk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rwcwvsow.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eqwvmvji.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qxoiwdxy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3esoivcfk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lpsschvz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3femfqbad.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gwlwjcnb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3olsehzep.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qdgrulvd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3azfyrlvl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kpwgtgxz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mginqqab.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3decjxtna.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3iktpipdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vygvxsqm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3waoiajwl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pipilzda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nddoklwh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xekfetyo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3anandnkk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xyveburc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ijoewfoc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zbwpzmwc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tabckwtp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3njfctuxx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3rzgirjgu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mldhzvwv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jjgazncu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3pzfpgnvh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3txidjekh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3yiinsytc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gbekgthk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3zpzrbiga.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ddobadvi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3leyswdvn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ewslnbva.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3zetasvqp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3uktlkmhe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xuitkxlu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vpbctupk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mlzouzgx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzzdkzjg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iskekktr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lphmlpol.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ujlkhudc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3jozzqvtr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nvxgpusv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qdnlgcil.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sgaosxay.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ixdmxytf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndtprrjb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slzsdwys.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xllskecq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lesqhjrt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kwpgeeqb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sldcsrsl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pdhdaxjc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umcskuqs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ssirhbes.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vtsidmqe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jyklqpaj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bxrtqoji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vagdjvai.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rkphqrbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcavprpc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxzgonbc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gctvpdbs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zifcpqhi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3smmoufsz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ufdyaejg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hiqhbhwu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hhjvkbmv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3gjtvvrmi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gdryrsmi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3srxccrjl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qwdaonrc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3luulytcu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qqmvbdwc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hydytlvh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uynanqkq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bkjdzsho.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xkynrviz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ccsurvpi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tzbsquoz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3bwekrwyc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pkvpzbin.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3plmemrhf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vxhzeabj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gapuhvlc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ckcciqsx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3difpmdfb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3utgrcvtt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3iwmvfxrj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lionexry.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nflcyoxb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vxizrztw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mgoncqex.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jssqbszz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3sjefgvti.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zchmyhte.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zvtmskcw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3nwghhuxt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qeghymzc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3flyivqiw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vlogxvzx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qkanbtzm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fvxvjdud.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pnmmeqsg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3beynegqm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3katpkyxo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oewtivjo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ixsvwzkg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tmdntcgp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xlecumfg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gtyaxncv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uxuolvfj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3csfneotg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3rrsvuqit.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mnwrjuab.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhnttbjs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sqbbnznt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmkwgdk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3gzezngxm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jpzxeexm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kulrarja.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nkklmdjp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dsqfnzog.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjpzpotj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wagdjlvx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvfpcul.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vfiaqutk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmaqhfi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3seftaoho.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jquhghet.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ntrhkqbc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zylwdnbg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbbxikz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qiekdxlw.html


<!-- 参考信息 -->