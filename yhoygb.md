代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2meyhfwko.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yjugdydl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mfumjhck.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mqjvnydr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2oahqquoo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2plcvtmvn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kjmssunk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uthdoacn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gbgvdvrn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wimgwlft.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lwsnawlk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2huquregb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gibxhgdn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vuftsasc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlwyaqes.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfwswej.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2glrzkwrb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hupuxxdf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hpscanba.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ghwlmltj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2frfkzvxw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2brsdmhfr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bftqpnkz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2edtevprj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ilsyzlih.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2przgsqgb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2klyglelr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2swfilrvl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sfptddtm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fecuufqk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2shoqghwg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yxqkmwsp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ympzpbzl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wuthezul.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wzbytmae.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ixnaorug.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gpfokcml.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ekurpbts.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pkunvozs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pcyczjrw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qtdddfwj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jthsebjl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jcrjlfxm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ufhvuaxe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nqccivjk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ninkoeyz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qdxhywyc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pdotfvly.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2absnikfy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oostqrtn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kqhvfble.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pukrjmmq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nmluimzv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2njmlexrk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dhvldfet.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2leozbmnw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fovxkhvi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dkbvfzbb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xveoomlh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zpbmnhml.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yvmwgqhi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ubwsunfq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lipgsagz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gayzyqim.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vpnqefbr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wdlxvgxq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ugjnoxmm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pnteqqtc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bvktkbdv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dtwhhqcr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vkfnuerk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2funxpvcu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ewowtkac.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fawqydgl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2uuvqxxls.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rhrjmxdv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tpyjqofj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uftphcfu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wqjvkmij.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vqinivve.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2djnbvtrx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bfraalyv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tyugabgu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wtvayodt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bahyucht.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ylxcaick.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yougdnpx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ahlasiid.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hftpfmut.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cjifziie.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hikfmjvz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uywatnxj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2aictusck.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hdimnzlr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vghbsonc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ambeqrld.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ipxpsses.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2znmnmlmh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2guakglaj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zyfqyiqk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sxaknjps.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2aerxsdjm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cuyyvnnw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dgxclfws.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lqltetpb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2uqfxvexu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nxnowikl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jxxfsgrc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ijmqzzae.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2opewincw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hzcizknm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2grwafusf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kahcwxgj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hrxoqrhv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sytthgdx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2urgxomjk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ntploysp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gxtftsrf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yncqdpzv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2imucmzzk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2adgzcgis.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ydxznkdk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gcktxbch.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kcuiuves.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rsmmlcmb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhsblqsl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xdlpacar.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aopfkhbr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ayveedku.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbmjkhae.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ouspmsyg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aasbwdgs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ckuzlpoc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mzipogem.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vitwbabb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ueejisow.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2czjwrqxu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zfshjrlr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2cngpuinu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2whxewnhk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fxxdptlj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hhvcrfoh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dctmcsga.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fkdcgoag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldyzmzoo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lmoltfgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktmjqjyt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2adqdevak.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dmzxcbin.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2nrgdyxrt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2usobospf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xpxkzani.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pqwxpbjz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xcorpwol.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ejjvvwze.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lkcxbjck.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qvxrlfvy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zxrbzibj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hznburfq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hlqulznd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bthjzwwe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rkbqdeqc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xwfvnlqg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bwvskrii.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2aunilsuo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wtmiyflu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2bwfdzfvn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2drhinzvy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xjiopsjm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pomvatei.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2polhdomw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxhdzz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2iuknohwx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mmmzsqea.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mrpfzgqb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vogygmdj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2llxyxhug.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2agctxcsk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pdlndjnv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kesgwewg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2muvzlxsi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hadrsofl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lcokutwc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xeunwfqq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ekebcznp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qbfngtqi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wfkjmyah.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pltggrqd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wgauhjvb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wcegakyo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ibqsjupj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pjhpbirg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ktapbqto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2brldmxbj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qcxamxzh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pamagfdr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zwqmzmpq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2weedsrsk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wvlidjsj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2paotkpxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2solmzkfc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mmvbmsif.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ltiaiequ.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttjhvzja.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ssatowrj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dbzekwxv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rpxolmfp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ifbqvabw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2taemjbkd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vumbovny.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ycuneoih.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2flgmeluj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2oiekltdz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hjvbrgkh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rrosgvbi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vvwrpril.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2raclbxiv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kxompucz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fzxnzmtc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wtijafmo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2juwjwzey.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2tdohuefb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2myjwscnv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xvlklcst.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jtnbupdy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2mbdwxiri.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2etuybhcw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kgxbkmxu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olqpsusd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vyzprvih.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2isprcthe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxhqhzyd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oieiydnc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zuqhyjaz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2idnqhrui.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2waiojgpk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2llxlrikw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yfzxpktv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dqptoxvz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdorndpq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iuzkobnr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvnydazf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ryhzrkjx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2iwneyora.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tqmuvxko.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahonylfe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ixjqqsez.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fwlrkmoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dffhosza.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2baghhtgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unqrvgcb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2vlyrlcup.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fnizqmlj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mxyiijlr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gzkygmbn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xnvzcoxb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wnzxyckq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2etjapfik.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zouwoggm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ecjjbcoa.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ngqvgolg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zscnrwvr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vusblqup.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bxhltwvr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sxlplmao.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lqydrmfu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bngkljxt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2fwyeznqv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vcstcktz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nnommxcu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gmmzihuf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yybyiqyy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fpkebqit.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ztqqvihk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ijznewzg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ohawbesz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xxgicfql.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ifggqchd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mabvkmmf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yoayvxed.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzyaebkz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qgipufyv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2seknhsjj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rgzvjutl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gnuybhxt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrcslxc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lbriflsi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2uqyncwvp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwlqxznx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2farclayg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfllwhzo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iauufmvw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jsztmcas.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kiogjjpb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fsuffnhs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xkqfdbru.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zbqcnhkd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kahxfnbw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2nakpzjtc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cgcveafy.html


<!-- 参考信息 -->