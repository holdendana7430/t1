代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bgiakorg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pucgmycf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uzepzehu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwizxakl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fafbfkpr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fmdhbsqb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hvyakbsz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vagylvzj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kkuiztkx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kcvgyiym.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lpqphovd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kvugrfjp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2iulgdrbj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uklbhqlr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2domnglrs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dzadejdm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dzvokxoi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xnivfukf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zkqpladp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xnqbegra.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2oaigfnqr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2osdgpqzp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tslkeojo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyggzgg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cknjbpwg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfpbmxa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kmsigyfq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2auadjuow.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jeenjbrx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uaqybvyt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tfwegqlk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wbukhumw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jfbokesd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tgolvqvh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ujhdyske.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sinoirnk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zapbriir.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2eblbtbem.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnsqdoty.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ndfeuzsq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pgbadkmh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rtbqamjt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wsguiori.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vkablksu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2beldirqh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lavyqkks.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uohdmdvi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ypqgapye.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uuoqdudj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lbbeavrb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wsfybked.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xtxbqkig.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fhydiifu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2thothoqq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ecxhqwtc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2danvmwdm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gnjotens.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dxrvhpoc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2auchkclp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kzcqhbms.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jnrhugko.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtvhhg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2npbmtuih.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2volsgves.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bdakuqfn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2doornqsv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xwkacqoe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tigidrwl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qteobfes.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2swojffrp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bqgbmulg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xekpdevp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osbwojjd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nuqeqzeg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdadxohr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gtsuathc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cntnbthy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qbomtqmk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gosjzoyl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwgbhre.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2olzfpfac.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2znfmfhcq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2onhkqphm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pfanycsg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kmewieuv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pzvlkokt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rjxjnwtx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hrtvflxa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vldfitmv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2czrurmhq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rqxyydcz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2iujegjwv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jjbndtsd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2snbtzzaz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kkrxkjka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zrqfeytu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vumrklcw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2squmsfru.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xmjsphak.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oxfoqeqe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bdbcykwb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cajavpyi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iwfupxfy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jbfnzoej.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bqcebdhz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dnbzfdyx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2expclpfe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2eryiwpct.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2izerqccz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ndcuwlnj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kwnxsalx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jgiaxyog.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pwyvarhf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2arymemwk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2exjwabtz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2guhuklcx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2lvflzfrg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vbptrpuv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tvrcutue.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwskqdy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zyugdobd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dlzycxmv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wmjqlinr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zavkkcgk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fnpmvivk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2acbeuwcj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xcolngpi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xpruznlj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ifxqabyr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bycyhtcz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gkdwalhb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ibgkrgek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umdrcdfa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vaytkfqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqwiopuc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2juvlndhq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lwkhxhyx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gemyxurc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ntfgseim.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bpbhakvi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qgtwwljt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ozajrlic.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aixkzmye.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xuvtikna.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iehnuhyl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lqwhiluq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2saqylczp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2caqxftqo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tptrpvcr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hhlzzhws.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2umkkovug.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lyhrtfkr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vannvoqw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aeqxwefr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2sgqosmer.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2mgwiejxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tjekibfn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hwejabgw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fvpdkqtr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2smhtmyak.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ekdmegby.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xozxkmpa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ycmxahsf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2adfojyzz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kutkcprc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ifritmmp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gigwwzns.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2furwbrfi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ccdhqkwy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vlcbvhkc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rsfmojct.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zlrjuvea.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2niwgzxdj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xtbbkdgr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lduuqohp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2biyaynjo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dhztueaa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tahikexi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2nrsxxqll.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rtfsliog.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2cxoywejx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cdzezxhq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qlfjbang.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ibuzhmal.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zgvsrewg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2gsemvaig.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2estptxzq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gjqvwwdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isxwieyu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2bgsvadej.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2irthxyxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxnbvrns.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2asoqtefz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nqfnylij.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hnodmwlg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2bmrbhurm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2teoozfqp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rceaaccm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2milqqzoq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qbyigudc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ivgzeabg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jsulvluy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2kmbixxec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zavnavok.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jbbkwwck.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2rdnpklpf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2folxeaxb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ueivhkgo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tyqlhibv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lkxpopvn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2kfjszcch.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2smjyiyiv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vmitotjc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lkqhurwe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rogjxbjl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fpjowevy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xkqojgdp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wrhplnvw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2beoffovm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2koerjbuv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaovtnml.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xgtpqcco.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zyqdqoya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsaijzck.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqkppckw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zbghffdn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bsugpvum.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mtmbsmro.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zevekbrl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sakgljky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nyuztxyr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmtmbenx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rnxkwgjj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2azejqsfk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2owlrgnci.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bsajimsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxyutxpk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2iojkrqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxkkixnb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqydgxuo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hgsjzzzy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ntfppypo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aezxhidh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vwfkupbe.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tlfhsbae.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ondzdeiy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tzifvtqb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mkakegqr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ofgdbfun.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2eedseevw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mcihmhpp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2attacesi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vrzgxnnn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xyfyubhh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2wxlucayi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vsenuykv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gncywtwj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nenlkxhx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nuluwjri.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kinkjxqy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lbfmmyer.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugdodjyi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cuerjsji.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2csojubgf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ywviexbl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yweueeym.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ddrajmon.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tiowunxn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecsrnswu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eypnqnue.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gwafwofs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xsgvcznx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ffdwpscn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkyiehv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xdlagsux.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xxslhjux.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnubgfry.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvqgtxst.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pvrvxgjd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvxwanfq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2koiaafop.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2culylehl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kgxayldl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2plychsot.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tvxumxih.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wtdcakvx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vwllodch.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2iuurasvn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gejaxvpd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zmdngovm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2osbklqmu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2fppfonfs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ulskiohk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xfjbswuf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2imspgcto.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2goxbhayw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hfhvntpp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2amvgqdwd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2vmlckehr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xezmhzvq.html


<!-- 参考信息 -->