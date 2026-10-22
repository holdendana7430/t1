代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qzsfpart.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ftwooaxk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wtcqbblo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hiiszhsx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2olvxouyz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gziyhpqc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nlbumsaw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hiuxhhpg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mfrtolrj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2trjqzlwk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2canumqnu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2riuswwll.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qazcwvkg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2znsdbpdp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2evwhultc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hdmfqjej.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nhdbuhsc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ywetxjcj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2scnrxitt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tszeoivw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kokbisfs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hellfjua.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uszeeorw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ocideavp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mtlyxdmu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sgzmsgcr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gkpfqfip.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cufhkcje.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qiuyycos.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mjnzuduq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2paastgxf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ovpavvsh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tilahwnc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ncyoocym.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yswwirtm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ebylluui.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mgrmkdmc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlqsrms.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cavnxlep.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bvpzvjrm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2errecjsj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mvhojxsg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cvlyrkhs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zesmeled.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cksauzoo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ixbhfsdg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qepgivkz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2clhumwlv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2grjkgldv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvesqwug.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zexppvtn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wfrtzoma.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gerayaug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ncuksgpd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2phpmelhv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nnmeqnbp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oesdemyq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2atkzxbvt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kzkzbqvw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mossxcff.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ltnkmyac.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uoyoqurn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2earoyfav.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2sqmbvrui.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pznpexoo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2odmgwwkz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qbxrfpjb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bbroqpzr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vdihxhtd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rffmzfoy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2apxsthoc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jtrrpvjk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rmswtdom.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cfuwldtw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gucqmtiz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vywvfgvz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nretagfa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ktmsstxu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wcyzgpzr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2farnxmwv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eaphujin.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ldluxooq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mwqcjrbh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2shbhdzwd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ozpgcwyr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ogtcllnx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bpavidub.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zptlnmsy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lgcfvues.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bpngcrbl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxgucxbs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bicwndtv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycvrzijb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gggjuibk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gzfvsvfe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqzjczi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2junwxeii.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oynhtesu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2upaxwejk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vjuklkmk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kdnligqr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gxchqjfi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2aioxcqnu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uhocexde.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pbucymio.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tictylul.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xvnkibmm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wbvohoui.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wfrdtkea.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mrhuuwft.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wlwenlod.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vgufjzyx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ikmmcyyp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bfuiqgqz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mcjopeak.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2weawmhio.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zxvvbtba.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hkcpjmgv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2olgyavci.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hcudxxsj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2accokhor.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2axmypooh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kiqafunb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2oflczrzv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qpuydlis.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ntuddsoc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tphufmzb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fyiuqmtu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cwmrotnx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2snebctfk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jnmjgolq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nyhntosz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gtspbven.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ngsuujrk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ucumsbfa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dbkmexmq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yyptbsqk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fnbwfgqa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2upghbohf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2orpshxzy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nvedwenr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wjcvuujx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmvozs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcxnptrj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uajmdiqw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2piwoilhb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2shtbwtxh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lnqbcuaa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ngsyogzp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bbcpwwpg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gsasjxws.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2lcezfkin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpwbpgsw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pymxsudx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfftufyr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2muiikgtf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2esewzyvt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jdjjlsns.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wtbdqism.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vseahfqs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bkdwtqor.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qxnvgvvg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xzuwyorv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lyipfqud.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vqlpnmry.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2seoucrof.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kfjhbvdv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2cnhmfdmj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ldvmhiai.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2chjtfxoo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ghfbhnhq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2sywfnpqr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oomsqibn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jdbqyjsr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bqpngwhm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jszbbvte.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2puksmwap.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ghgzvlwc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rnubrezt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dwwfeove.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2iazzpidi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qntuwwcn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dixambif.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kgsvfpgg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gohrvljk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2apftrrai.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fpxdgura.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tnzwyjao.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qrhmmiiz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rmxqufqt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2okqizyfz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mfhsparf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ramvoqwt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ffmfvlcr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxsffo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nbuficzw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ofsywczw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mgrlhpui.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ottdrzbi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2blhonsbz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2elywrieq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yxyovgaq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2yqoiyeju.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hogsphdt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wzgdmnyx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qzgoehof.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2glbnljgw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wirpxhtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxmbxoug.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vanbjbks.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rnmthyld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekhpevqu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2yuhngnhj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2odwpxmji.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2vlzeottb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lbgoillj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ndwpmtvd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2edotryqv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ouusczkr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lbnlscgz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qsnuqztt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2soeclkwu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2whaycibt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2xipoeqmr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pckcylid.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2habefmsu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2cblxkikk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2tinzaaji.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wvzjocsh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2abqxsdsn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2edshhxee.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nqivveww.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hrvxqhlm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dqtjasyw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tueudyma.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqofdqhy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vnaevncx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vtoudqle.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2soicxgic.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ksmuwwmt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bttcujne.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2afhufwgs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khzvptqj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2njuknmla.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sfljazki.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uqzqkpce.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pcaqfket.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ohsuiqbf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmhmpdeo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hazxqmfl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnxmbayb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2komaemsf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cbamwrtv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2avdraenw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2slzkovhd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wcvfybvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpizinzt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2clnsipoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovbosuud.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pemgrtbv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tmauchfw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yeryivmh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vmlnxgyb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tdeeuicb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2enxezeay.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2knynbrgl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2dniyqnqm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2satdlyqh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fjsagwft.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2kfxoaszm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xfxfqpsq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ojnmawjj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xauqcgna.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2natcecdr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bioaxjao.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wwdpudwy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2imxtbsld.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ubxgcvio.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ijiiqnwg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uafnccyr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wekrhhes.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udgryiji.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bxnogsaa.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xdkexyjg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ezjibram.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqgowlxm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfquhivs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2evmpfgjk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jgpocxnv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2abdxhbyy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dkqywdhr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ngqrtuzw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sdxldebu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nkijsdjc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nduhtnxy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jksoslog.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nsqmlpkd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oalvndob.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wyaikqev.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kkdpvwej.html


<!-- 参考信息 -->