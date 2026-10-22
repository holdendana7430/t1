代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wxwlyuew.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vsbzcidh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zkxrqabr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kiycopby.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ubbeouzn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vxnvtklw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqqmkxdx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chzjcopg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zfabioen.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jmdkevty.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dcbhuweh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ptrzmofm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2yxdytwey.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wdjvfrbo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2skcedmmg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rcxvseuz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xsjdduql.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqxglhtz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjuwzlej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lttrcqlp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2esdnzltt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jaorhtue.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dcoeyisw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jbpfxhbt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2atluzvco.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqhbdyrn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cehbxaum.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zmnnpnbd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rgmhqkxw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pxnxejuw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2froohcjd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qqvvevij.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hcrzpres.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2iropjniq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2exghhmxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2laoutuuq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bkoyxljx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qnnksedm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ilpcdgqx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2obfgbvsg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2equootuk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdqmors.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mcujphpo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wddslxjp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ytvyhisk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fcxlbopf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eappfztq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mlwzcwfk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mqxwikuv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2uhrysshu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ryzotrjm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ftdsxqnr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qzssthlt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hykuckek.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wtsdilyx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rhvmwvdk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rgxrueif.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mbczdjkk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwhbqz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2okgiwmtc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xfltvvnk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uhfhjhyv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rwuesojf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2japqsrev.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xpmijwjb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2whrhojnl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dzzsgsmf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zgvmoajq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sbmdssyv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bqmsguvd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nymajrgl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ofgwhpde.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tmeyshru.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uhbqxtub.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kfktnrfg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eagfggpd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pfppaiqq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pwudwscq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2znnspavi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ttoehkgf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ftgbvdjb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jcpfwlag.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tcwpplsl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lqljlwft.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gvyyseap.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ggxmfyxs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wbughgcs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ewhyqgtv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wulpoyvv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qnokjckl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2umwpaqbj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2simldgqr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vuqikdxk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2libzqooz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mtjhahjk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2uhdyopye.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2arnskwjf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2krdehrar.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ekayxsqh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kohrizfl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lkbekyba.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xxugvzuv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wfwivdry.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dupodmdr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2atjibeyr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mtdygjxn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ghdnkkgj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zyqyfelh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2husrnhyc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cofdzmfy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wckgwouy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yisjrbdw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cnedefut.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cwyiopjc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2yscwunwz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2iknawcbc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fexzifst.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2sszojlgc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wbmrycxr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bfrewvmm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wwyxihme.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oiucyzto.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nlqbmylr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qkrifqgn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bjgvsxxz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2inoxemlq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uostoeyy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdgpdgrg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2njelxyql.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bwzkmtbl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qjhamrsq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2flkjukth.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hczjjkgh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2tculnpgv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2djlimjkt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2procvezl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvulqahf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vvtenkps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htcrrzdu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kegyeaad.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xxgqzghe.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zcrxqdsi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xewigkde.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tdvqcmqe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2poompkyr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ldignlfe.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ixxelqjq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qkrktpwy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2klzkapxv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2urkvlsti.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ntdcvknr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wbztydmi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ligtvyqy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gdpbxjcr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qqhyuwwl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ltaqwsxc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gvjzzcxx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dxtojprv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cxqqxehk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hkzzvzja.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jhiddqsb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wlbluahp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ccanetnb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qgrbqtog.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2efcniaqo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mcgqnfpc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gmvpzckj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bwgsditz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tymhweih.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jlustefx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nwoyojol.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2srdsihsu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wfhvrjbw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2njzxtyuj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ngpjdxkn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dorcsitw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zgpuuqrt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rgmmxper.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cdkxauod.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pamcvpah.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vamelmhl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bxypbuxx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dnnqlcgd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iieevhfk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2asaskyfu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cailbahx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2oijkozoj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vejcvreu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ecoaqmmt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kuahvtrg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bdthtidc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2zrydieow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inqhgtyc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qeeopzvy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wavdchdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmqhto.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cctmtrsl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ptkvffpn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2izmxuubr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2erziered.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gbyxngpw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vajhtmez.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yfgzgkle.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ehynhlwh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2thkwfndy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2egrmtprg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2tnphkpiu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2edkjfkmo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2dqmwyzpm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bfpsaglc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jxkcjwho.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2bfxwzlfu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2snewtjnt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2pztnkaoh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2sgahhbvq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jtupfslm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2srtrvvjf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ggjabvnc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vofiiglp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xbxstmnh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xbazesop.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wdqdemzd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egbtcvxg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvcixgxx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqchzhwu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ypdcxvke.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdbsnm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eqfhylde.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxunjhvt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwvzggve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbezghcm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fmeswzaf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsfgavpr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2moorfbxa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kpinhclt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eofiblyx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pgpxpxwt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zfjogocb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rsphmzps.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ybiemuit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tccqyutm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2taeiuqtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdodijap.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jinntqgs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eamfmitl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zbahdqwf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gdrjfvge.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2htrownev.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xduqgcsy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2skscuoqh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2vtwrydez.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rflpsuvn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2sfpumhea.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tctebsli.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2feahwefh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qpoemytb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2laujcegf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vgrcmyjj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hmmltihx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wyoqoyjd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gkgwqxsb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzwioptw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fwtenokl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lagjkrcr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oaxswtwr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rqgfojyi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ywvuebks.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zzdjcqgw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ftqzejez.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rkxhstpm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2huzikrro.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2dwytgllm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvecskpc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gslnbcju.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nbuhvfyn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mjbolswx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2diypxolt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2erxbgqxp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hlyhpuad.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dsdzuowe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fokrhuna.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hvvxrhvr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qboenkcc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rleplnri.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zgtpgmhi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2piwunxjw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftineqnb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xdjoutyq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dljytget.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ajfgqdry.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2libuikua.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mmyhyfkl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cpbulhhe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sreyjafg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2blfcwyfr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ljmnyiem.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eysrhfob.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tsbairrx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uzkcbsgf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fguxawgd.html


<!-- 参考信息 -->