代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3prvwlbkh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3azrmioti.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kniuqbec.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3izorcazn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qbtsupjp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3buaqbczq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bytstdko.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zywmyddn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nvhgmzua.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkyxnd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3znbibqcg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3shnfewfx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kaoxcixf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrqhmrfg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cwyquaix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3iimesgtx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zfcxeruy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kuqtfzxn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hzuhcrka.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nycdljdb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lvhsatxf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wpalssxw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ogusglsa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rbcialhx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jzdudblv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gukqnzsb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifhtzrvs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qykxfrfc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hqnzjgha.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkwubrw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3irrqihcn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cfkfvhkr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kmhhrjye.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fpisccah.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3svvrlzwb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vwnxkcpd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3syedvjpa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vdhixtbw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jpoanmdq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3esgbxfpa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jhevjzxv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3szdfglcl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xdmhyzzz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lbkfzuwy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xatlljzk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jnjokpsz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zpgyhgky.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3erdidpwz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xkjnslnh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iioxrjck.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ukkzhuyf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zkyspakj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uyxbjgwb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zhttdwpj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hlfntgko.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uvregxal.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3peuhvvjp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ezolghsp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3camniwic.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3nfxkpgry.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3feftenrc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jsdqrlus.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kkhejklm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrckbxco.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kyfzmrib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pnelqbhx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3syrmqamw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvxivdq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kocglmne.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xqwkcnyq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qunsjvfo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3siidfoxs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3riohaneq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3klqfzyao.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ymeekjur.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xodqoumx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wdiibhql.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3okczucng.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jizoqflr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uuguecxs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oybtumwp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lxtwbyen.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhgscgwz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ucazwwyf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3iwzajkmn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3opfjyvmy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ergnyuwa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mrariqus.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3azzkzqmx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rcfyigyn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xlzobjpa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgvglqhk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aaxahadz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ulnapcee.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oqunrxfb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wfembkcp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kvjklvcq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbqckbw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ozhvqjiz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3omfzfugu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3spsufjyb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3spsqaowh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3keyzuavt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mztthndm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3watjlkwn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ocrjjwxm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gsuytbcb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bqqpaiks.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jshekfyj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3puuyutyk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bvonxlvn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qplfrinp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eomaxqsu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qhoepdxi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tdyfcruw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skgtiolo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3edptuuyc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aaxdzeme.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qxixqmia.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fpkmhqzb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fvseevsv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ndeitxnj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3azcpzena.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ucbdvwoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxczapff.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3eqyqzmat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evkupgaq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pcjynmfi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fpkmkfqh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wvferbej.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mrcpfvyr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yvuexifo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qpxigdhq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3umcngtfq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jwiknapn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mxilorks.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gwbytmll.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qokomatk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ifjuljku.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3bguosmcj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bypfzleq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qnukmulp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3znqlsgnq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3otworgax.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pzuoqtpc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gcroylqe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rytgyfxn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3voieooti.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3axxmagmq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vxhitbbp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mkuftblb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ztxcelmu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tfofqwmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bbbpmqbn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3robmeoue.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tpbluult.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rxvlksxz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3azjlmzzq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gmfnhtru.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hynwslmx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dzkaldll.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xrfenroi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3bvinogic.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ltyklbtv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3kqdtafak.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3gzlaavmc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dnkkwqfw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3erbcalhs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hcaienay.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zbesnjol.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lsreipsr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ghmcyytt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3klvpybzx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cdtepglb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jbximmjl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xfxjctbh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dmiasbrh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vhmhlelu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bxvnlfvz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3wnwifpib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukmksohw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3brxphtwg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3iuvbjnpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnocwxuj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rqdxedit.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sedrnltj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3iubesvus.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ulazcyhb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3nkalmerk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3uoanhfvp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gurxgobo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tfwgjixl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dxxuxdbl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3uunqjxfx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rghagoav.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3coljfqfo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mdwmowbf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3dhoghepu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mxsonzuq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ucnvwhtu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mzvjirvk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ggzrxtrl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kcrfddrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3btzgbour.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lrucazct.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3oasrvknz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xhchcqhm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3yruecqiq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fynldazt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abdmowxd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vvdxfcck.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gbmsmgga.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fsqhgyzx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sytnhtwi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lpmjgwhw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nltgksnr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rjrjwakc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mvpwknqu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nzdtgexy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kubruhcy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nizlqgdt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3gnuiabos.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3loaywgmc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dnrqfhzl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3posdiikk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ukaznlpf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mgxmffvi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zgizeurz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aecxfyaf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3bycnosxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhygqukb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rcqzsqmm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3imnsbbxc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3arzaexkh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vjeonnze.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dcfodqvy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3chgqunjh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3htxbjeyr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdsclf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vphevmyz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3oviwebca.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3avqdszbd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3glerbqck.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ehtjakrz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3pfcxuzdl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wxohvsot.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wsbudiqe.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3eumjieoh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ansqthdx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3trknftfp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wytnwniv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qybcaxvv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iahemqxl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kljmhnud.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rqgiggya.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hezbjuob.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lnfukcbt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqukscj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hrhymzae.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fzuflyqe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3cblfgtea.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nmzigegs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uxpodgre.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nzuiryfn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ajxynbov.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3toyocuvg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3opfcaimx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3txwraybn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdxzsbsq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jfbvpduj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmbqcnlf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfulxfhn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qdupcgye.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hejrifpr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kxqntuvf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uallafyy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3exyyabjs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3phzqirxs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3utikrmbp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3irpjktuj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mssusrtt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3teafgcbb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnjamo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bogptyfx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vgemzubt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bodobfhk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3djxrmytb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dsuckxrg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3efxusvta.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jfhkmcsj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rqltkzvf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sqblvnhg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jjdjbwec.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tehsydgi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xcmkrgzt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhvfikl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qlnygllw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pffnysks.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3pqkngvep.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3begnjluy.html


<!-- 参考信息 -->