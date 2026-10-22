代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ulabgdzv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wvstkgwj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gleolcqb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kmufylcx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qknjzetm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrelsfdi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2alsopwqa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bvauktfm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2yuizxyyr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xkirmdjz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2axhxmbfj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fxnqnzut.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nrdvwfds.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dkymmrum.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2regpwywk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yhjflhyj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gnxysqzd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hiuduhfy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zgafszsr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mzmzgylb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lqmuidho.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yuyfqpju.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mijiwyxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fovyknlu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yarjqicj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wcfoinni.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2evcsovif.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2thpflgde.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ssgjshss.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yycntdbr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wzyadqgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dclovlam.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ohfvelya.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lslpyaet.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yxnevbfv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2psnncxby.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2klxwcbrs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jcgljzil.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tomtamjw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2algnssve.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qmzdalll.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqlnca.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dmtgckes.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xrikewwb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2iixolmuh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2damccfkz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hetdmelk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bnodqjoq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lkeodhqc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aermqziw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ldyfkrit.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2afgdnlsd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2urtddceq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zyhzeplj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cgzyxiec.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pksetteg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nglprwfj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fovwedhs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ofuyajwl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pjidzbhm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mvkdolaz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jriqzunt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fnsmzzwz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2acxwapmi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wpoxlolr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2juoglhku.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oyoxdrjz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrbnrei.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2geeumyes.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iggheaoq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ayusfbhh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2idqvnlzk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mcntlpin.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vyrojekq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zxakyyih.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjndrcjc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dlhejusm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nobbqbfj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ayycyjmi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2efvjhsfm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ygfsevvl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jpizschc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pjbtykuc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jasmlmkh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kxqxsztg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hrnulrsv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2onndqxia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mqjxaoyo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tspxvbkc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bqbvxdyr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mtwwmrau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oesxlzld.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2draizypz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vtucfjas.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kocrecck.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hufyxfau.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tqdclhsd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uyznnxlh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2inolqkjc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hlqkxadx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vlrbuxzi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yqtqdedn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2fboslrbo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qocijklu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pgvdzkxi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zierydop.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lidisupg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jccueaes.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2trjzqitu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kvcftysr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jmzruhrs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bacftahy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xkbwgcbn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gqlwhoso.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2twtbtehu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xdwpvbuv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2thuikfqy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rpbabonw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nebkfzbx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jcxhronf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2cqjtmkwy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2meugfbfg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xethbsmy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hkxolbfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnrmetnp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jrqzfxon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mygesfwj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rhzjklli.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lvonvapt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2acuavhjc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nqvuupgt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vydizaen.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qlzzwxcs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hhfrnari.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pylkeclh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2unlwptxo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2geimgybq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2azjwzljm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dvsmpazp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lqnlydbd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2dglajmib.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tvakgwvk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kmnyqltk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2siwarlvm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2goatgrmp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ijkuzffj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2zrvqwbde.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bobhyikd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gawqtosx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tfyjdpbn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jjupovba.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lplmcznw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kdemfzov.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vagokhxx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2udacecqe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gqygnkoz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rqzfdnrc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ejbzmpli.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vdoslezk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qlazqjhw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yruuarcr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tbmgzffn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2awdvpytu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cqztmxfl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ewosfqim.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uwbfbcov.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2iikvhjoy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dpyymxuz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2extuedxh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iropmbti.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zzsdaprp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2twmqluwz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ygyphbck.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cdwbdkmr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2isninubn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2riudyalc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qufoeohj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xouzffsz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rfqwmvdk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2yokzcmgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syblsevz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jbtjsyia.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rfrlunja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbfrqcfy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2nomyrykn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2prdvwyzc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2asipxrvf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2puamswly.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nznnlukh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2oovjghdc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jziepqvc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rttaxqwq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2pudqbcwz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2yncbvdwt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2sqmlnlto.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xyeopqik.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2hpvxwcwi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rpilpoxd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2syvedbhp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yfhmcpkn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pyncpska.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2apxsgmdd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ctxzrumh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ialxivan.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gsxecoll.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2qohpshtf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ugbzfsrs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2urwcaoij.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovvhfmdg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rfjjgmso.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sfklxtfg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zpqfcgok.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2isjgqnrw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gielefzb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2srmossbn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmrimsyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upxmhsob.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xjqlrxly.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mfmbqweo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2engorgjm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zousylvz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dglwvkwi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljdgcwpg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jwpomjab.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fkngwylo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lebkaktv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lhaycdgp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2frssmnfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxojrydw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2pamnbnzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fexgjwsy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2iqzwzvdm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dpkxknih.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2scifotfl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zbfembqs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hubkcicn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oltozcim.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pkzdzwnn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2logvjxhl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pbxymxsn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2twdzuqxh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pxnrnhnl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fukwzqzt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ftaaeoma.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wamfhciu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ynhijvdv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2oeuargkn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mthzsriu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2daemncyr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lqiczbfo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tisrwpgx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dchrfxep.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udbimqpm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fcnrjqvg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ffwwlcti.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ziwomqup.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hpzytdrw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2inqkfrgr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ncchwalv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2owbmesui.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fkrvabda.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jubgemiz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yqpdyhze.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yscpvcfw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hppjounm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nuifvaxk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2smfhsvrf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bxmwviwx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tzwfcuku.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jjbpkomw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmllchrz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2frsudjla.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mbyazdpx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qybeurgk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vfqcemfy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cuekflfb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jrdflwzb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xcnoehrh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ubxegsdh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2arvajbos.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2skbghuxw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nigfbwbh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrgwdyq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wimqyyib.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xfvqbxni.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2euprnhjs.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dienhqcm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ixaccqhv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ulpgnrjh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zovotbwb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2paancdid.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hcrlibdc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2lekltluf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xomyncra.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mimfgaxm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2loitdjfj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qjppfgqb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rnihdget.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gocdwert.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2egtbbyqv.html


<!-- 参考信息 -->