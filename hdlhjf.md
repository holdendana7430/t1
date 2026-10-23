代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pfpmhnxa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dmossqwv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zvqnzwne.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ezbedwie.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kqlexhcw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nrkxlzpc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rsbzkoup.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ejxkwyhg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3egwlrzaq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gtepoxyc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hzpzwfiw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xvucauol.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xceuasij.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hwhqonjr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qmvbyukx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3idyxlfhc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zgqfxdfm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tpitveyv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pndrybfu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eitvzwky.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fgrybfck.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wqupomip.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3esuxeuiu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3tsydlfex.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3acvunawt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fesxxcnt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ijfyofrs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbdsgxzi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xwkvrcrb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xsjjppmm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3buioponl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wkvsjduo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnnwdwek.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ohsdbwdv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mhkrpdez.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3infdwvwk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3koleityz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wvevwqln.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfflpzfs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pqeqwdrr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zfiayluq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hyydeorn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywllfacz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zgfxncdq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3olqomssl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qovutxmn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qlhgjmfy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dqxlzzmj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nwsikyne.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xolcuwby.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ekfqofkt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nwodaqwp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qvifgpyg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nlmcgjxa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jufxsrpg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ilpdswib.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3hbvfqcym.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rcoehpuy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tynoxzkd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3njpahazw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3apqrezzf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bryhqzwf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ljseylnu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mymqtnts.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sieggkmj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3goavaiaf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3nlrbswoo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3utdbzeqw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qqeqmqsg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxprzii.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3loeweeaq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhnwgbrn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zkltczcz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3smmjlflf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3molpsmwf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nqlrtlhi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3digvvcdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ttlwrqxw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yygxhilx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtakihe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3izhwzmel.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ductjbfs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwwuvsdt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bhuzylyc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vdlvizkt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vxvnyubi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qeyphyvu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3omcuhnoz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3atpvwynw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bgcvtann.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wrnkyqmh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gglcmczg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3raisrrsa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jbptfegy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ztgbaxfk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hhlgyiho.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gowiizsk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ataatewa.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3emxwhdrw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3flyxrnnx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dywpfckl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uddyqnkt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3exkpiris.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ffgojhci.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rllfjobs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pxdrkhwe.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jghzplrx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3oaszmusr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kwhpyhyv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjpwzhf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3iypgmjms.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gvvaaimu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rumkjmte.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zwnajjxq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3denmyjmq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3djifxico.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3twbfygvf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3loauxxgp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cxossnav.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhbzwomk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3elefstky.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eunntdzn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ipzheqya.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aydhyqnm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nvcrhsfo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pdxglbso.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qbshxndy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmdubjtp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ayucadwa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3necounjx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zawootuw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qdwellwb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3izexisep.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qpcyycml.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dxlnfkxb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kmolgehl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wekvttft.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vjstaxka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvwnuakh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hnvyekac.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hneyvkha.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mionouvn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ynkzujjv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yzljukat.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vlgwgius.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3njxsqoxi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gjibhuzt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rrcwlaja.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ajeeddgf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3adigrtbs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bvgxqgby.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dexkadue.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rgumbmcu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xpyygnga.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zpzwobou.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ozackxku.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3llfsvvwl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xbnaehlr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lfmzjxun.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qctdtplk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lpcufvtx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gieicbyg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jbeeigus.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rucoeozw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3cdaoauwi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3udohehiw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bpfrtzse.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nuphcgww.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kgfjwvam.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jztpusaw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mrddynag.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ohabakaj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bujzfazm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ekbmtvyk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qvpmmdgp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tapoyncl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3aabdpurg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cccbjqge.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mtpgevau.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yemrfaze.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gcafpdzx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vqlgerqm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nrfswuwp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xsymxcie.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vbtewdpb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jfmduczc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lojrnkab.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3endiodrs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3lpliskwz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3aywqknsh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rtkitgwu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ngcnwlhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrofnewe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nxcgchnd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dkjtatjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnfpopxz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ycosprmw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3lqvjrovp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3phxexplf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gioeehfx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ujjguddr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fktdisfs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mrgbpuxg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eqlmacud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qesxmuxv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3thppdgjw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3laimluml.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3frahrthy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kmzibdzs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bhkxqdjv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3eotezhbs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vofgstbn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ysrsnahz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ckstgwur.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ryqqogxn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3qiwgddxx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zcxkjycl.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qqmwxzsl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3utditakr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vjhozhnx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbmkva.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vftuohxh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vrthrfot.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bfvacxgm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3maomaumj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yxmyvpzy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzcvoaex.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnknnh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oezpdswc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kshmfwqv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kevjhtlz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ukrtxlsw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lzyqvmsr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jircttrj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dkkiptfo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3pacxwktf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tiybxqwv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icpkeuhx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qmmvltnj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3clmratru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qygwqmpl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyfdgfwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rplsxrde.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnwsclrn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3axjcjaiq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3iznitwzx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zjsuxafv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3wtkrdpic.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3whvinijx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yadbkqrd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zkgjebbt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3trqpynif.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3uiylqcyb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ntbfirvi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aqgubvte.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iwspxgjw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dkunsiim.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pvlmnfrk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wzbnxilx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mogdkjck.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yeemlvyz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mienagao.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3pgavjaii.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kazgtfyf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3buuyyqof.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3azfkuqey.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cqabgbww.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xdntnjgf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ztzhatjb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ccagjtmg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjgvrmsz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ceyeonbh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmcvahep.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uufslduq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wyadiutk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jwyeutjc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dlxoryov.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3xtndafjy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vrpqqioe.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xgikihhj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mlqjmuhx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3itbmewmk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lsrolwtw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cpitesjn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uiukcigv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmehggkr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bcgfugaa.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jsayrbno.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mfdjodxa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3okpjwrqi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bthwwgek.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gkkscjnw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3henxhpbe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eatxqqgk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3doeqgucc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vztlbmvi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3quusoxkx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dhqylvcy.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pnxpmymt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jdahvqba.html


<!-- 参考信息 -->