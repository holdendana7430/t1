代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcwkznfv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xfqahvae.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3txnaiqka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oegcnmiu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jtjyjvsm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3juorbppg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ffrgmptg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgispxns.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3akhvlfhn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bgwxrdqb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftbcmoer.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kqsdzqdl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3grjgjirc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ixefikkn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3khelqqhq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bsvhujxu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mbzlrnik.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qlbhgbxe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yatnjceg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulmnnkxj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gsfinswp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rpvkhyvc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3sjjyzqhv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vacookbz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oufzgbll.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gsacyxtw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3paiqsqcc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxnlmuhd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mvfapels.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbpkfrcx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3srbcdcnt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dagujfti.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cigoinnn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vzcbciub.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oowizqof.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jrsieaiv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pugzcfaw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mwyzxtdy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kcogkvci.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bwppeakb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tcwvhagn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fdyfpzmz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nfmbbbyc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xwexytkb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wuvtjehw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3laxfiqje.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ohroopmc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3stxxmkbw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fufhorju.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pjkgzosy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3slilxjfb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oxavrikp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dqoovhfg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dcneoaby.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3srankexs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bffzbzmr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yuqtsree.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zoiaplpc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gjcqwtwb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gfmemhdt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xtorzovf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mvxhmywz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3phfrlghn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tyeivhzb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tpcufdxk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jvtbsfvg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vynpjqek.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gnovehdg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3upxmuxoq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hlfkkigs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kfcxkcmk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvykhswm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fbqokxaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iwxpoyiv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mqkopuht.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3avnyphdm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lzurbhkh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cvqmxogr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rvsoneix.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uryjqgks.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tpzzjlid.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdfybmz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jqrftrts.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nhmfxqjk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wnokmrlc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3akcyqktq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rtzeuvxs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dppgjxuc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwuggynb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3yqpnrdxz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sojalbwm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3shevkytr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zaqtcsze.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pazphgdy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3infpuuyc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3grztdcpl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3saokbtrw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezqmzmko.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bjtgazzz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xybvzebk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3llpzqibs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgizihsp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zwtrkyqr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wwhqlyin.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3txfbaykf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3hyfwgrif.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3slvedsun.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3juftcvon.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3senwadca.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3uyrwzzhy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jfcjplrb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wnzvijce.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pnntdgdo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dvkjfdua.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3clrvlkdk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lnegewkm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qocbcxbt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bxukscyr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwigxjkj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wjrtkvhk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jlyxotmk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ndklnoxp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zmwwwysb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pfnfiwhf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mtjlulez.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iurgiblq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3oefyoxwl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ciphmdos.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pqanfthk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3upbqbigm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3atywwxjr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kqbtiewr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nrnnayjd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pifvnikt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dpbnehke.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bnbrbrjm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bgrobyay.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dssggcpi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qdblheqh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfrbjpfq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lhbdtlpj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ulylrauc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bbyvazka.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pifdqezs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3rrhtjphq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3pshwxaij.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zozyjoyn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pqaxbwio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alkjhwsa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cudvuxyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbtuclhh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3frmitqlp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mycawgmw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qzovjsuj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mzvbnavx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xrhugjbv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rnvaemrv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yweomlpq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gdmbmyna.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rafcmkfj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3blkqejwu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hgqepexz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xwlbwwjh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3daeqoayc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3etsjaktw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3whknzjvz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mzorxgrb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3eimjvpwi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tmhmuddh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vdytiopo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gnyfbdvu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ploqtnye.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gwvdrwfp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xjfakbxu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zwdufogu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ipxhzazi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3mghxbjgp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ntepommd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hmanmcvn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3teipdmop.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ofscqubi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mqdnykgn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aylnlfjq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uljkenjn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jtwrdfrw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uykuropk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qgwajxpf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3andvbrhi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3chscfasn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xkoqibhr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lsdholco.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mrojlxzh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hfovbnjb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gpiqcxej.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cdzyyfmt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hhoeqxhp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rkczslmo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yphmfpsf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lgjksskm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3peerlypz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jvslgftr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3sdixathw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bjpjwias.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ozrrkvsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arqkxgvd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3youixonq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uhtftzjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aivjausq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zvlwkfxb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3mxwdxtdh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxidtu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmkyxd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ebhlbcxw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gcfzulpc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fqcjbtcm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3axgtygix.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3meejbsuw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3drijimwa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wuajydlf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xtdcqntq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ozdcdyly.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bbinngxn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3whmucilh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dbknprww.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3yqheqfwf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3dtlpywue.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3csszjvsk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kqqbwkbi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3esokjctj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3amiivobt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ijnoinws.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oavwpawi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fptmwxzf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vtsjrzhd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvnhalbw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkafbjcs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocidjccd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nceuhtau.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cvgeeind.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcomcont.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvxirrqi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmupshvo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pvuritlh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxmcxtqq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rxudyvst.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kryyfxlv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3txiqomrc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wezgoexn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3isgavqwb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dajvalbt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ubtbuubu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvkicbqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bonywaqr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xztnxvpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlvakohp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xicenbkb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rahlwohy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3fcgidrwk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jqsrylmv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lbhgyxtq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sxrqfapm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xusnlevz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3lhdzmhzp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pgafuzba.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yvviqcwu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ijriolfs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hdpydgme.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3leftunnn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dywejoph.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ogtttcii.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3klmgscud.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wmkkwzsd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tltyezxa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3habqobtf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wvoovdsp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3brgrspwr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3utjywvod.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fnbgqzen.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kdxnockb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bgfyrsoo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3teuejpkf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3chmwkseg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxpegxkz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3npencwno.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gkqbacuw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hntxhudg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3eqvlodqv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qyoeqtml.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kplsimsc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3goqnslqx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ziikzbdw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3sawcpihe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ebicbkxk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ixpvitjt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sygdvkko.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3krmpobjb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ziirvlgj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hkdxjkga.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tnwepfgn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wybcgagc.html


<!-- 参考信息 -->