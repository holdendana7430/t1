代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3soqhcfmk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3aglwkpnr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wfjwpbev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3edymaqvu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3eugaxgkp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rilkupgj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dwcsdzjd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3skzefxge.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kwalekry.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pymczndw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3oowesquz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ounqfrnk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lgdexalq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fsspgtby.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrgold.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3txubvtvf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrakwy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qlehrwte.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gnrchocv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3trmsaayq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dtqktpqg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tbyzdbne.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tifmvfov.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kgtatiee.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sjsuhoob.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3waptxptu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jqaahesr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mjmsryqi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ryteaiuz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pvbakntf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3twoglzqi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xgtattce.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pqkmnwkc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yhbvhrsn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aekixtwa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pyspkwgm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3otcrrpff.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lezlvgyr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tdjihocr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3penwtamy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qczdirnd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fvfitnlk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qxpuyujs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rccvcsrf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3buvdfnlk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3eccryexy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wdljyubr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3sivvdcob.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3afetkrot.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zzptnxpx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ryotuhxh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rrlnvyts.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dzmkrpfj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qagubuqv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3twxtiqey.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qxnljqdg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bsnajcmz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3onfeqypo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gnmiuipx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ciydxhly.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mcivbryv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hvwaases.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tujraotj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3clpxgzxp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pcjfkbno.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mooquokw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jzhjguwr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsjdvrg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3igypvxes.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zqviyefj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3uyfrxxfc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rlidxjyq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtmrarcd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3soyxeizr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bxnktxis.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vxbegrtx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dpirbyae.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vvagzeka.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3imtbprej.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xgftqkqd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3eeutfijw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfnlgtyp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3liqkurut.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3brnfsnjw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fvlpdqxx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yxoadcun.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ijpfiwlu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qcctofub.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nfnzvolj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ddjhkmbe.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jifywqho.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fknrajvj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ouqpfaip.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dyonshkl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jhwspyhs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nwpddpxl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jiempecr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbbbsyhf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vhnnsmsk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3soltstyg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vfjuaexw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qwepblli.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mtomehbd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kabvyyso.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xenzivgw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpquojt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qahunaow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rdqwjoqh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3emcxgkmc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rsmamzbi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nozmbvoi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fuvededo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yntbdjmf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tqmbgedf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lwqamlqy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xvmqyvcq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wozmrcyg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3npzqyqjg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hsjibute.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3bxdtvxdx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lwctykrz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cwxaftdw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lqnlyogh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bibixtqt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iabgizxf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nnjlhqhg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wygjgihq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yjrnbdax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqbvbc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ihvmnkub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tprssjmf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xtsllyqz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wnldhwkz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3repqissw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uuldkdbc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fzdbrjez.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ntnxncpk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wwjfrjvs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nmzuseyt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3huhvqdaz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmmsqw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3cnblrsvm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3eblaoehr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sucreqdi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cjgnxhol.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gznzfnvy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cfiwmphn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qszlhguf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3deztlhyk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3twqonnnf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3emrkuiti.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hrfxwtom.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ddekvumr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fpuaxwde.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zptbumai.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pccknkuo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fdzkskbb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yrrttguf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lytgzfid.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wjaofeqo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sqjrkars.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xnwpbqpt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ljhpvjav.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jvplqfcw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hhlunkxl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3piidhmxh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3azfhlgbg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pupxnznd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bxhrfsol.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3chynaokd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bxwwxnoe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3syuzsuhk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3uahjlyqc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3petycrsk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3qyolkgqx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wyjtdzza.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3celebghi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wonfmqfk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hoftknlb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bmgudpzg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3lgdxdkle.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ktwncueh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jsgdkzlx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qufwnobm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgdowwgd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dggjpslj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mqivfbgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfsauxmr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3altnnsyw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vxzppajl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3eglzjpwb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dshutjjw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3empagutx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3urhralch.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zafgaisr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yvovrupz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xgrhxycb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mmlevbdr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xmsrerza.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uglsgbut.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3uvcwuusk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3prcfjlmi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3invvumlg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bgarwsjz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3skqmfstw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ttllnljt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3nqdtawcj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hjttjvmp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ylisqndt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3afzugbrt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hpktggbh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mnieenbc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vrtoknyw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zgcftzfx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlooxrji.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pqugaylk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rtggmgdm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnyolplf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ihradaoe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3alnrppdq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ewvvvcnz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sdvtjsab.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpdlwiig.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oasgkmgo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ajmmlhvf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3fxhevdck.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3izdezths.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dtmhdxru.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3reupzykb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nxmfgrvu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pmgqgyvs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uttyqyhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbqbgqhm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gaaeanxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ustmdbak.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ediaftse.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ivcidbyf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3krafwtch.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bnauhoto.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nlbfrhuv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3auboseyg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3opmnjiwl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cwhueyyp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aoegcphx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qggqqjjk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hqwgduhs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3baloldci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rerkedrf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ersxyave.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3njvwnejd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3okkepced.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qlxwwwib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rkaadwtz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wpbmmcgz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3uoeoftuf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wbawjzir.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oenqsphb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aqjdvjjj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cwgarkfu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uytbotvx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3stvujryp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ckuijwwq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3goxxrpyx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvzkix.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hyygflep.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3npozdjvh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xbcivhdg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zhxhjdkx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3felufzfp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3valaslqj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jkrirgfh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pmxqpfro.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxhqpbjb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lzybyacx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zrwnrjxl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhvcyqgj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pxbltbiz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lttgeyiz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zojtgeyq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umzigsfa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3paficyod.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xtfrytve.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ibgdeuca.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wkooficq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ycpvqogf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sjkcbdmn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdgcvrj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3irugtrcq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvfxnpb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3jdxgidoz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uglyvbvf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qenofoed.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uknjhwdg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zidgdomr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3prnfmzkm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mkqzkodl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3syocavmn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3zwmojtoe.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sbzffvwm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpgoonv.html


<!-- 参考信息 -->