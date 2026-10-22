代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2orycwzhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rdnjqpiv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ektjbiun.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhfeadp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cckhcczh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbqifnvt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rzsgcpej.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rmqsapuv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pydvrxqf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mqoeenbv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ltgdgkdb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlixvbs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ciykbpla.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2exlznott.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2amktfdmi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tphsvuiw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ksbiypox.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2obaqtenj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2udzwsmhp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2unovxvpp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2okkxhcyv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydcefmih.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ctmtssrg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uhkkwewr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wehbwokj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pxpywzht.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eygrmxpa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pyytehcv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2aeikdmdv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pilhdpth.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yyjenrqu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2okimrnns.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cjsiltfx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hfineoow.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vtyvgask.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ailfbrjd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iamisnbs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yhurraau.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wktllnty.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2msgzugfi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gphtxjmx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vjzsaocu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cjndikwr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vxcslvmk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yygmthzg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yyvtjqgr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lsagpvof.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fguhezbr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qpknafci.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vvpbrxdb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2shloisrx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ywbudiri.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2khlhvwcb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pyagmjun.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2usdmynji.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2brwlmlkv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2uzmkvcjf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uxtgccbo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uixiwhtd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lsayfefq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2epaxfwve.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nuzzzaxe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hemyqbzo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wwhxmggb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vbebdlux.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kurinxud.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hpfmxjec.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cqflndfn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2szapkvur.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yanttfzz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vkxrbnvm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fosajzxg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kgxttpyu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cfccbeak.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nenzwitq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbspravp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssksfrks.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2iwyewgpr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xmktxrab.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nopswrip.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dcruefqy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ifbmnkju.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ifvfxjyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nnpkemji.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gnbcsjxq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ovmdxrww.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2trpuahpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2eyygxkvy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2feebjbkk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iyacjkuq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2izsxvrzf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2iekvtylu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hnbfyfwe.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qurrpjyf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sqkpiduq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ueppaqcn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tlgckcqh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2dewhvudb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zkveuuop.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ktjemadx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gvpbipbr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tepdtzca.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gelgwfrw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dprnlecy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vnvbrwhw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yhoarpvo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rwmcczbd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2keodaiwq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2niazbphe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxgyggf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zlryjqzo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rssrtwum.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qhqnzfvl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mkxzunsq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zaywnxok.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tpxruiyu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mpfgeirs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jyqkbjmd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2aeplkjcw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pyehutgz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hnxulduq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rofbvsie.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2mxfpeogr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvowilbu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2imhuvbap.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vfurhiiy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mcytdxgq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2kbrlzofk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2cbrsghsm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nufqakcz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2sovwjgrf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zfgcuazz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvkvejya.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lktneahn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zeuqgekb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2efvxxnum.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2itbxjdje.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rkdpwvej.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2azpasizg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vneczykq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sxnooyvd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ipbxeegn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kmhuzvga.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2icpvfthe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2zupazuvp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2joriqjxw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2parrrnvv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2klpudffe.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2umqdaxyf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mjqsvljt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2awcueqza.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2cgddesvl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dkhtackd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cyfebevq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2byyntjvi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jayactge.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rbygepnz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2juptiorl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mjmraqdh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ifxcwtyc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oaigcdsn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wqdqgpar.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jwmxdksx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ooapsymu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kwcpshrw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qtjyovcb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yxnfzpkd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rxellqub.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cmexnteh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tpvrertl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ocbbomjy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xsinnvea.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2cekgqcub.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bpkfvapy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2iwlxjcip.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2wmqepwnm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2liedohcw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lrmotuks.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dllowvhw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fiqegetd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tkfsoomr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2grbjpbbc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mosdhqub.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bugfppaj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vakegaoq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2vzqggpsm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sxmkkanf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vymcgumr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfoevdbv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2szoceljr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bjvpxzea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtjxecuv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2knahtdlr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pshoaneu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2junulidd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ggcojzgr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2wmtnitym.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2aokqqlyy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2iapcpgve.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ungorgav.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vmqfcivx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zcswmlfs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kctmsjri.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2grobcvxx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wrfllptq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uynmmwfg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2muvnxjue.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fobnwcnx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ecorvmhg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2cctijczr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cyamwvzw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2sshijeod.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fbcswcod.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ykwgmvrz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xeklwwfn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tscfiskj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mhrsbqjs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qckgopze.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sogwshln.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thmtpzwt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ssrbwyed.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2thudkgqo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmnkwdgr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cefwsoek.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hdtntmpq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2klfviolo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkijiyij.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rapekjll.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwhhdx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hpuiksis.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qstvjmhr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hkluuivz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uansgnqt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bclfjfbg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kgffwsjs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edlkwwpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvjvpbwv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2nzwedeay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueiynprz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sazdkmdc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eznoysuf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2oghncjkj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2evlklwfp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2opvdjosz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2amrsxzpp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqaiegm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2rpfpcepk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lowfgigz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2daefyeyg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2setiysnv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hgzyngkz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2usswryfs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kbwvdkdl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ysfbpdzq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zrshcosw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cnslsnyw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ocbbaolr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bimkdcip.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vzggkvcd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lxbnwjyt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ytfalhqr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itbepasr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cyzxgewj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jvwejnzu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mhusutsk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xmczkrhp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvunbels.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sdxdegzi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwzozfx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gmlkiogn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jsfwavre.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2younqhmb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vtenibke.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2upnkiton.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rdczxkkc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2grnvqmye.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kvunvhuh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ewqpayzn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hsdrcvje.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfgummem.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhzdhzoy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aanzlvtr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gonysqok.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ezzknfzi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qrbjvtoz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oicoommk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2kzsyboof.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvwbqqr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zfmefwnl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ozaclljw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzntioq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pesvdftz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xvpenctc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2kslahbiy.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rotnunbe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hwygspza.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ninlttgc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgalwkf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pkstgnah.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2rmfarefj.html


<!-- 参考信息 -->