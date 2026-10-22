代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lqylecgd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lgsnhfyn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2afbiznkf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hpcrdquk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ijivifrz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gtzajjan.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dkcfoeuv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vfzeupjn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kfqxjkav.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2umgfrdtx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yoiyutkz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zjtpddgt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wuffuuef.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sflmlfsr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gtngeudr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qvqhqolz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cuymzrcm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2megicxro.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qqrnzoik.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2otkptshp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cjntguzi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ihqvjfyt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ysqpwqae.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uitmiuit.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cxxyzlag.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wlmkwpdg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cxekomfi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bjggmsfy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2aniapzey.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dsdmnnqb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqzuzu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2caodaosq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2noeelysn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2idjemltd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bgafgpqr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2guubdouw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ijtabndd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pootudyy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ekqbcarr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tjnfynvn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bxepwsct.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2coertofd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tpkkduuh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rydrxmrb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yfiqhkey.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jhdmakhd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2howvwwup.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2whelexjg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fmvjvydt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rbbjspqj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oyesggsc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gkzdhvxj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rmvawcrf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2slxfofqa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2avldzppm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2emupzlzj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2skyvovye.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pmzinybp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2okxtlkme.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rovjtgku.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2agruuged.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nordjnql.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2khuyxdth.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2svbjjdar.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rzoemefk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gvhssyfn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xxjmwbpy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2giblsfan.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xnxhlkdf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2oseyuhpl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2senalihh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mqdjygya.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2euzkfamp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zlnzrhwy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2szczwiol.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fmiheuqo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mvboghek.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ohkozxvr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hcutmzgw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjuljgv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2apppwfgn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nfopjesr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mrresmyd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nvpkuvrk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2aufroryh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nghevmut.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bnvstxws.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pupcvbxn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cbqxdqyb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxzlvc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cpassmoz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wokdiyuq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zopgjfgk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2suxjpsgp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdlzmuqd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2eixzwsuo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lgrcsgmb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2iuvwmklx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2oszrkont.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2aiidfogj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iqyxnsba.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uacykgej.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2phqjexvu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2padadwqu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tapjjytd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lvkqsbut.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xmjexeis.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nctrxafz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2daiiepxq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgqbjun.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2axgbscxa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ymrgozjv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rxxxgqzr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zafycuxd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ljahljwo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2lkcaqgxe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mlsmmtus.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zwflqimw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ljqffknw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2smqwrjdr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qudrrfed.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cpafmggf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2trvgvclf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhefrkl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gqhebuoa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gbzqumzw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dkpvtljx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wiqolqjx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2scnmrbil.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2igwcbmpf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wasgfaoo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pebygfwu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjffcd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wlzecosd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sqyovpka.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yhlgxpad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iytwofly.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dhbgqcms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byohrfvu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kyqnucsl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xtxctvfk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ayqkeqbz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2moterdvk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fttnakbk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zympynqa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cbvbwxux.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oooziumo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2evoigfow.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xranbkyk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wmcsiglw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2yuyljghn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kqchoemf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jpykpxfm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jcofwgwf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bosnkjqn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ooitrrhu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kdgcrzqs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jawzdgth.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2eyfbgnst.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2znbnrskb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uottzktw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aaachbmf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ekdlpyqn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kfmngnjg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nrkggyhr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cnohdqry.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ggsqmcoq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nsyrijvy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kfifhbtz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lozzprko.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vjzvrfdm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2paetwquw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vdqefhvq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lvariypf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pihuttbt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ucurwotj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gxzdvnxf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2edqdtnum.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2byrdpnlp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2iloyvaoj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bgrpqslf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vvthdawn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2skvgewcb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dfvlshff.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wsfajesh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2afuboqpt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2umgsrskv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rsfmsouh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ayentszu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2aagjxkqn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wrfxsdmk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ouoppweg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdurvnuv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ckndfrqp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uyjjnvft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pddzaoxz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rzvnwxlx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rqvwckmv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gjmauman.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gishxqru.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ntcskaav.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fsonxhhj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xapgaueg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qshvtfwb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jjlfgsmy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gkmzbkop.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vwbnopsv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cewsqtev.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2sackjeqm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rwdifmpk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tqrulozs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2xcillmyz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tswmvuzj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ocxizfti.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2hyoytrgi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jxarqbcs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axdjgfxb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rdyelgfz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2azdizoqx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xovknkez.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rdwphbpt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wanjdqoe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onlwmuhx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cfwqehft.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rynrqyvz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wbclvozp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqxydbu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvjthkpo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqhgssgv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pskdsrcz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jnmuerwz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gulnadqz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tkwnnyfe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kgcsnxaa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bifjvsut.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxvehscu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amzouenc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2glpgixgb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kvjjbrpp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2drtrjvpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjbwlt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bmamuxii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcpsfvek.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfnposmc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dwfsvphs.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2klrshebb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oagmpphk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2upcnmgdk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kzrwmqxu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rktiebcr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qslfhnxs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pckqnwwy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dsligejj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2onkagopy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oxbupdxq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qzlmnqli.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dxufcohc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2imjqeimz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hlttvoat.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2bhnhljrr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wygzauwo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2dicpjupb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mchwffcr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xmhsuuyl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tlulsvrh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2slasiddk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwmqsncs.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jfbcfoxd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sxbrujei.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2arbwendp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2atajkwdw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kvaipued.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jjlqluev.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uhperjbt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vhtsmwwo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2pkxvjmvc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hugrmfzd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ohcrxkim.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rldofutb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vmibqslb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjvbtsoi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hywkncuy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xcwywkdg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjvwqaqb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qkbxrekf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2agtetgnb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iptergsl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2laadeoko.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yvnwyazn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hyqchken.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gwldoxux.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rgcxmhnt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gdsivqhs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nkzvzyxv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2sxmjwraj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ffgdixxf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hmzfvjsk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sgfgknvt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpqvkoz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2clemkgaa.html


<!-- 参考信息 -->