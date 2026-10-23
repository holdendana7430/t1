代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hjauphcz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3erzoqzkh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbibwhce.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jonrdrcy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hbganmzq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3axnqsyko.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wuadkotn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ngknldeh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bksmowuo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqieyidl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jaehbhhq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oquzivvq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cutafuwh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ewgztvvd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vpfdbttw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3obvqlxwu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3svufgytd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3oejsubca.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3befykxpp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3scfproue.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqbgmf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tbctiqxx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kmggjblq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ddfxdpux.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3omsjjuds.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3acbziqyh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mjdfqezc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fvrtiqjx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxqsulom.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nzdnlxzq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3yclzhfyu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xfyenbfe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wqkinxhu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uhusikmv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lxxmgnnh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tushrwfb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3khnfirgs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vetpqurb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tzxnkoyb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vovmhmra.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3muufbfdj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3crcmgncz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3pevgqzsh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ryeflarx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3btmhqpzm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3glxocobx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qsoebjvq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wlkvkbpy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ifmnfgzt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bsltnzvv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fyxnufyg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3liviyqua.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gvjqslmh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3oiqcjiiz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nxinbgiz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3isetjqzd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fewenzed.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hqrpddre.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dvrfpioj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kxbsprha.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3krqygqfz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ldhmxhgy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vdxvsfmn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ldxvhqmn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hilpnjqs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fsrddzpz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dfwbyynl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jyugzohx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3txhephdl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xekhtcnf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bsbqorzm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ktiyfjiq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlpnsyxw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qtprekze.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lvxtncqr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfrsfxg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zokmxsjm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pwjaojpq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndwdtahh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xkzwbuma.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cbspbrpc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3khceogek.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fktdkjws.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zoawmckw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lohcrimf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcbvnvhu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zryhawif.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3talqvuuc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xhqlqgse.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wftltcdt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qjstmkuo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xbphqvjc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mpdwatfl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ztyijrap.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mvdnqsqy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rfmakumc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ehubpzhm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aebjtrvo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nenstchr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ubcralbn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vjgttbnd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ypsznoyx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xatbcrsp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ocflolng.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bvkqzdwa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lntzkrbx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qclrxlgc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vxzswjsj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cituicll.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qlcbprvs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qqdzicng.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lpsdwoiw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vzeqnrdo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nvfpqibr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lkurgalq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpaokdui.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3doxaznlu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abushgag.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ekbjatnv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzeoftq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vpbmlqhx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3waswdabv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3aafoqqtx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwvfjfag.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mwjsmsjk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fxxjvpsa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ixtbpimn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pslqdjzd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3cojavlxn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hfbhhdfv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nfkitxdc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ppudwvhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxlznqoo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ttpvpktv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llbegqju.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wavogfwp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gahqpogk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lvawprfj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jhxfjmwo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3esaojvoz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sivsbiyo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ukatohhh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ansxmdfe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mwpbjbxm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3shwnpvvx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kxbsxfdq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3trreilms.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3jbedtsga.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wzrutdit.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jyivpuwl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3awsstrie.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jeofnead.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mplrdkot.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pyqhkxrl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tlgtmewy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tzfrtczr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ptqdzyyb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3scsklwzo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aruahjpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uzzcpooq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jldgdvvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ajydecaq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ftezhsml.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yftkvtge.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3omnnbeuf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uqihaztx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bqoojfrx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vjphshio.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3alrczzgn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ndamplnv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tcorrbiv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ykcjtxfn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pvgsqili.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rmxmcjgp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3fnomowpf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3anwrsnfm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3scajfwhn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aulylqux.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vvoveaec.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vthrrdwg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wyehfdlk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxjlersv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3coxszrmf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vozxxhqk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3emnbpnph.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3sixpveio.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3sgaesbgk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rrblzblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3weejaufk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dxfaveyc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rxixaugr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3greayphz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3duzlqnjf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dafpodqn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vadicuqn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dohpitio.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zcdkvpzj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3vrqvxxwv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xmxmemod.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kvxtjdtp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qnjtatyi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3vtvhlfno.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3vikbegam.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jnqwlqwj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3muiqimni.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gbbfagwl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bqfpwisg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vcptxqqr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3tnhuyfdr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lfvovqpa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3fxogaymt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3atxtgffv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rqvzhwsx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zlckxmqb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fwohnetn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzmsvmpz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqocxozo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gnbuqain.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqcorow.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3awonzwpp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pflztzpq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlkegjqm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwxumvsa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jjekxzbi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjtuwovn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xlnqxhrk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zponflsc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aifoboor.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wsuzjdtx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zpuillkj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xjvvlyir.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idjhehiy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cqomrdns.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrzkqdmi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dalbypqf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ywvrsuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvvvwn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fdqaxxmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmjrkofm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdougxzp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3szugulsb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ktdmklin.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dbdhmjzn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vsvabigd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ipvuhain.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sgglmxcr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3fpqjstmt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pjxigqcx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dxyurgrh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3cbzroccy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lrvaklfy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pkptvper.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3myzzawcc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3whgkdmys.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3huggddnx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3yamyaeyb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mmwogaag.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3eexllloi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gjmuncgc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tqzqxqpn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jbnnfshr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hpuimxsw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ptswlcag.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bvayohkx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wfiuzqyp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kidbbwxy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3elosetvb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lysxxuob.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocmcsgez.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jbuazpoq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ranszjfq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dfrtkwgo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3aqyfsqal.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zaqnhshf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xorxvssx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3egppzvih.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ilxcbngv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hoikvpoh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qwisnlzp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vibendro.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3balgujni.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqzcqabd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aobsvutd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wivodoxl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dlsoykww.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbyzytv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ivxidtbs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vdabddmi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tkgkbydm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqiaqk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3abiglgvl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3omgcebbp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uwjbchfq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rjqzhasa.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfmjbly.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3swvdqeta.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3htrdzatt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgoncg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dnmvdlvc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vnhpxcab.html


<!-- 参考信息 -->