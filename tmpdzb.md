代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jfkiqohu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgglldv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxvfqymu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gxsubbmf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jrcsfvov.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2chtoblri.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2sntgsood.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ckywmzme.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ahmstjcb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zymjjmlq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rfhtayny.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lweqrqje.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xeeudsqz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wwhmufse.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rephcmnc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eldkaupx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2scnhkrxx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iggpvvtl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vqgjiflp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cgbfnqgc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nmrbsjiq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmcbgfcq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jlezefhz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yorihzbp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lrvetcuo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ccrhoxoz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rzgaaucu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gpgmgooj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jrpatyqi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2msypxvkh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oysysndg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2puclnpnd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vlhikbfr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2loqbecib.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2txittjwc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2exmnthcc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fzqgmlat.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmgngk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rtsajipb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rcvcvfux.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2raxqdzfs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jjysrwmi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sbpblvgq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dtfmjjmr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ndcbkodr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fyzvgkqy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kdyasttz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cwnxxfjt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jhdqvipi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gsbuaiyq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2odgmubbj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qmalypbr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2llqgcica.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bzazmcyp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rhjrnnhz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tannwuxz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2koijvyjr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bxreyipq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zdlmfbbs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jmjxbbit.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bopfumbz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zvioltfn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cpvhdefw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lsogpqgy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hqqrzvkl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ztbssjqb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cikdgbec.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vdmtmgxj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rprbutbu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jutnporv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ixjaehav.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tigfipcf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lkwnsdtp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2wpihmfgw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yribhinf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dapaeoqi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2qlcofjgn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qnswevat.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hnfqnmbd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2egjxvivd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iammwtyn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ocsbciyk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfxzmo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lhpduahv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzrmkugs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mjovsypq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqitckrj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jasuauat.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wwkhiuoi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xydcynpa.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ouvudibj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ingxwirl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2khjrtirv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2okajerdm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qhghhcag.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2egncstmh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jnsxvsbv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pujqsapi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vgsqzjcy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jmbmvzrn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wsntjmiu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xykbpzra.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uxxwrvpz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xmvokeki.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2grueitpr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uchetkqg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2geosrsaq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jxrgcxpj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qzmfgzma.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oadqzhfb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aaacnqrt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2iondcfag.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tuhlckmi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuktihw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2meholjuv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rvctodbj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bnkkevsu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ywsiauiz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wnyhcmcy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ypgpuluf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sonjcmky.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ktpztarv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bpxqyvmq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2msfolzli.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qlrsrtzh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssebvlhv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2njluvrdk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dlwhepvl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pnseatjy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lesdrpgf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2brdsrozl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gqocmiuy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pipaivyx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2luhvaanz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sepyxjkw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xvtyxzqk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2offiluef.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sjyzdjhu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xbdvyehb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2uviwqqmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lguxkjoq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hxhsvpij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfmudzvn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2nifzsalp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vsvjgvcy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cvvgbshp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2alzeisgg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dmackcjv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ysxjaeow.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xsawkdhx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ugpuhkvt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pzzvonft.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ayjjvfbt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zgiplybr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2akcovdwj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yuhlmtws.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hffjyfcl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ithlvfou.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2picexrcj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fqwqngjl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pxgkcitl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2unrthfhm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2twexnaqc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bjrwtrmp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gsdawcet.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gaxvbsld.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iyuasham.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nksqheve.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bjovabrc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dvdqgmhb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jpipbudl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ypscibpy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qdphqtdw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jcyfwvvz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bllvddto.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hkchuuku.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iboofvhg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xtnyeuve.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2atunpmtt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2akivxhxd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ticyptfi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rdpjyphq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dyykaset.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hwutssaf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2auqbfvqg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uknvcosv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hxhszdqz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nzobqdoj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gaszaxkq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oewcwmhu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mvvygkcm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2blxibwav.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vqacmefi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2epdvubyk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2axiadviv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2trnpjccm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gixybiwy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ogeygjag.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2owdpymjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hskseeco.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2mcljgsdt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bddrejpu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ovmgmriu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uifauacp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lualbkcc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2cgtnkefh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hfkxyssw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mbkasfyv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2uwcporok.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2shvwestd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2goirgqpo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2juwnkvxa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yvxhiomy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rcvdxvkw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mdxhhqkl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2axcqonct.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uptmggri.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2uxwsyaep.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ueqvvweb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qzzacqpg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vohzwlom.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vqsbtqjh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2obfvnuqo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlirpqnd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yzkmbmgr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cgjchkei.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cyvhfwab.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqrcbvlq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcobieki.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqwgbjaz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2shecfubj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2twaekhxd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pcufvwqg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jyscgjbi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kagsxgxa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ruqhfiob.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vixhmqlv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2whmrmsdq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uppexpfv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jqduddti.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnelbsls.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbdtypgw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rffoansm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wdrfwmrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnamdmtf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2lggcyatd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylfrjgyw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smviukui.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2corwqtfi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qzfilslq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jtqbrbcv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2gscxvsst.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qbkttupc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2agavvqji.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2sxmtxgak.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jgacyvfp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2axyljktz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ovjurshu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lysrluys.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xtxtfbkk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fxogrfex.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hqvnkmqq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2adebvvuv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2rriqxuch.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xkgybfch.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hczvshvd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2hbuvhfdy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ugjihfky.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ihfoigtp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iquqhltq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugdwfsnq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yfchamwy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sjlveeaa.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lqmxzqlc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvolzydo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2azqurtdc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2abozocsu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqsrsb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rjjhmwbi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bfeyrayw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mbdmttlz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hbhjrsrs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2sstbefah.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2knvyefmf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpdafjan.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wdoyjjjq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pvylsmky.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eppeyuxl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhtwvuvh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2utsvayhg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddnwyxkw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hzxcxlfy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jijagzuw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2czgfhofl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2avtrxrud.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eoweramh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rrbfqiws.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jqaqivkh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2otentaxw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ukykjldw.html


<!-- 参考信息 -->