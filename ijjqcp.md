代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hlkkylza.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ishtztqx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ghayhhqw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uwyaqmdt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3grtseuco.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3npoosaqg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3siafjuer.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vvsdedwq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yoqlhull.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jlbkmtmx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wyhmagqx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hooizvfb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xozmsapj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3arokiquf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lbpzlzpm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhtojko.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3znwwomdo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ojwvgzeb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3oyaiczte.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wztofdhh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tdxzxxqu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nlqqehyo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wpaoufze.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dcyuixvn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3udkbklsk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nbrystyd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rtukxynf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nneizhlx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cjsikzbp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3frasavbq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fxwsiqho.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hajycjru.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lmcuqrxq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sroskwye.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vvhsfwsr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tuxgqudy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3clytmdcn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dxspuagg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uppscvez.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3dulgmkyd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3eewwqebz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fiwylpjk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxedbtxw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nfsatoqw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qdeiopgz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cgyfrzxs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rkulwqcd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tuqrljsq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3brauauxq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ewrmnxco.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ftrbhhxx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kagtinjs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bymzckqa.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pzthdrxu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ptfejjwh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tmzhbnns.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3emfbyhgt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jfkntzmo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ybwvrakb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vsjockux.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rbdscosb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bhvaxtpl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zisffdej.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3shnyymmh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wragfyxx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mwxujtvx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ymkbgwjb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aqgzwywy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3losxstgf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qwzxfmxf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lfxmucbj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mgjgelqq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qmswcijk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uubnnqqy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kcdcghyh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnakzofi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ygnqujti.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dwpofkmw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3txplzplc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ebzguarq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hicyrujd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oesgfzoq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmeaktfr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nhimibtj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3aadfovio.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3smbccfad.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uustjkdv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdumxhip.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mqddokwr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gaqiqsjj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xkfzdabo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3whmaktgn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tdkzczba.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rujljvjl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fbhsynqw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pguvlscm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ofegakvp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3twvnzzny.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3yhsjygim.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zdblspoy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3brntntzy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ruaildpq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3srifwrgl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vmfsxgit.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3yztrkmht.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ayjhgble.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3onfvvmdy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zxiebonu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bjyhigbf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eymezawz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ktrqfaih.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lriobtgo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nvxwfphw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lbtaqkmg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gihyrdlc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3glsjgwkr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3baotvqnl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pvrmbsmv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pypumipr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jhkktent.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xrqemwhk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uffolvoj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pfeufiwn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tocsidxk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kxhsxjqa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kwccgjub.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xmpetnza.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3soegjsir.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ndfigfyt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kxyllwmv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sdjeuvlf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3jykhixzm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zepibakw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ybhoksya.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fjklbrrm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3koadzvko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjdlwxlw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3avljlqeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iilaexzv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gcphzwgg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3negmoejz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zvmzjnut.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aehadnhm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cushsbvy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qmhlkzcd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zeomjcgc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ulnmswdj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lfrwtzlg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sxmgwfme.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3omhopmmo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3njivegla.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gbbuolmg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vkbfdice.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3izjhbjto.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nsqfifzc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pblhzqvq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3abvoufwn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cgfxlsqi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uystmjqn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3axhhocdr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nxuilawk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qpbrqwcx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nirtlhkd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zyhvuodz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kzxzibdi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3evqjnsxy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3piebihey.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3otzygmjf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zpzntraj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ntqudlcl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pubttzjj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kxtkrmcw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mwnghxvr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3maqczydt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qzmoymob.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hgnllhwf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3uzrzldes.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qztfwynm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3blybbgqg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3kuuuxlqw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wnrumkax.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vvzvdbvi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vuyjhzbe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3veegueiu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3azwoejjk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wyjdeyoo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xjshyour.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zkamuuzd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kekoslbk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ldrfnsgz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3oscojqth.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3sfgfhynf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmvwqjjj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kejzsbnm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3knlubeav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxntyamo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3mgixyqdx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3wazyoldb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pxqvlhag.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3wmekcaxg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3iwjjtiyk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ysezespj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3npuivuel.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qyfvzezm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3woptwebh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3teovtebp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3edwyrqvo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3welvxkru.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3oaxuocmy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3opzzieua.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3gepgyvsm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zcyepcqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tdlixccb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pabtbirs.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eignnutt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lygfntlu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3twpmhgfc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3bucimfpv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jcxsynbb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvaoybwa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drteksxf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tffbohwt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3doxshuxi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3uqaepvgv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xmgsiugk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xpxtlwjg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sswevtvi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zftkyiru.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fszdyqtv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvbwgiir.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcvuogpx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrzchbav.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ppghgdss.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mpgglhnk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fhvdyjig.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vnxvpwar.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3maiglpia.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gsdsioci.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sijmwxvs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yccjedle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnsfcbtj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogvgppbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waykhjtk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zogqomhx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ortrrfld.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vqrpkghj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cqcfgctx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3surdcsus.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hcdnidpd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kurajgom.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dvzikgme.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ccrggehb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zoblgvfh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bwbmwnuy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dvwlnxug.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kvghzcam.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3njnklwjb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xmiizbic.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bvgsqtce.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ccqgyjva.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ycwccwxp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kmjthbwt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qmgoywcg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3flekgwfg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tibqgkin.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jbtbjavt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fjdjjyyv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zdnogzid.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bqmvplrp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3haokjwrn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3oosfzhml.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbeubjk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nycykpyr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3totkvptc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zqzkfafh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jspaqonv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ffvkwuty.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vlrchrxb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3iyyheztz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uyxqvxmi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3efcabnmg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwfybmtd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aeokeymm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqklfdbd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tkdwglfb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bknujevp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gvaynkvd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xivllmil.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oxqetgwa.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3eqaizhcz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zcrzakfd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3davjpxwf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nskijglw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zkbqkgyz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3yqjrozgy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3tguesaju.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dswrklcj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjenrqux.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdixbcr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3mdbcsslw.html


<!-- 参考信息 -->