代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jgagroyw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpejxlvo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2llwxuuvr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vepexcxm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mpuljfvl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vexpvjft.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2itxjexxp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjcpntr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kvtwrpol.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qlrqngsc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2osxnenmj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hynvtwgi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rjffwffu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jkxgxlsj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zrqnmhgj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hexihzud.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gcfljleo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ttrlwswd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2faopkbse.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hheokhut.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fopbmhuw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dzflykfh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2madaujtc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eiqyehmm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nauumrpl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ierekmka.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kmffulqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebcjoefk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mbozukbo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tpzkufqw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvaayz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yzxrxlts.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2doeqihui.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aqgvcaap.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xjjrjqlu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mycgescw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wqzljdnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gjsftsqd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lpspkwkg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tezktqri.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nzngdjld.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jstcyckj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2roscmbfx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nynieumb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qnhpxdar.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2olzqnwgo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2onvoxiad.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gsljkbgt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2aebssjaa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2twicyrff.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ibbjissw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2whhlbdnm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rjpdrqax.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sdutqaiq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2srxopklv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dobhviac.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nqcguxim.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nrvpzyyw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2saaiazkp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wymjqyfv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mvzktdvu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ukuivvnu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tfzgggzd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ipzdccvm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wtutmvvx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ycvblazf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dniqokfz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bmeoggym.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bocpfqai.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2julghptg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qrtedkrr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2izwoxcly.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nqoznwdp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2detvibei.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2uquddvtq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tfgujqsn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ymgwodgc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pnbccsik.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rvtgygrc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mgmmkimf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fkflziaz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wenkzvhm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bbikzmop.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2avtdzxwj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pnbohljx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qbqrmzti.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pcrcipmx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ffzicyrd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qrgqdsvr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ytgngjyt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxreozgp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pihloegv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hqepsuyn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2oeekuacz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zkqlwlvi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgocefgf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pdiirfsv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lxkjxghc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2taxyqaoe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jpajlmzt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rnqsmtkp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kifhctzn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lufyyecz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hxryiuga.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wzgvvbxn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ojcramzw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fwhjxoef.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dqlklcko.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bzprjvcr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ltqsqvjy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qebcuxly.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mazamvkp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vqxqhxyf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2urjbbatv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2auqgsoym.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2malhjczr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ebpedlyx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vmjhotas.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2manoyxex.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zrmkqwnb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rvxempax.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lwwofjam.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tjxhcoyj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qtthfddn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pooaeamn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qmuupjjz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ccsfpftf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yfxhuosh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vvfeiykz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kswkwoyc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2claahvaj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2oosfgjnc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2huefbjvn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zyooyqzo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jdlgxsik.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yjpimitw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xucycnrw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwtkhzu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2cjkepvyk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ttqmylup.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uupsmcxs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ldfczdhy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kldbgjzg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sbmvbzcy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xttasfyv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kjpoqkjw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xkuvjxez.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nifufwcv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fsvsmjzc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2emqjdmti.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2czmqyhol.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2msfkrvqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwwsuxcn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eapxmkot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opuwawtj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xbbrevkf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mtijcwxo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwsacc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2omfsgbsy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cfbaoryr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uuitcikh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2disccnps.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fezopagp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sngpabuy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2chxougkh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2safdvwhq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2kneylnpk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2bztiatzh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ehzyuwoq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2cpdhtdpo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bfipnxbr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jlmggfof.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tgaruaxg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bcxuhhkj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2guzmnoao.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nmydqlvd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tplpaitn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xphvslui.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qravnows.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wfofxpxa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cmdlulvo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yzdnlfud.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xtcthsan.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ffnjpxff.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2btyvlvfq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2abectgjs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2imbjkbxy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qnixvniv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ggequbnq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ffdphacj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dtpxwgfl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iilinuci.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rivspnjd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2bowzlegi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zqekwqny.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2gqtohcpa.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ompezxil.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2igzrrciw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ipldsbov.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2viuelafh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2iwjgcefx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bmaqcoqp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrgztk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2cgeocpcx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fggjvsdd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ocehymzy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ufquewiy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2teqxbxbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghqriror.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gnaczmzj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wkxvhjoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lczorqtm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2brxgbxni.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lvjjucvu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bqcheqda.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lqspvgnx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2knaidikf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zfisiwog.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jkykiadn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zrigllod.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hmmetkpl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ezhnkgmx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ejkjmyne.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fxlvwlve.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2eynipswc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wxshculo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2sndxclbz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gsqsgqpl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2twwqgpul.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lsbbgvtj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zphjrqzn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dupchvoq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mbxwjdfb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2uspsezwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2agovqimk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nbsqbmyk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2haojsnfc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2leeksdmy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgrbsahn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2myxojuyn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2toucmvaq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vzscdwga.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrestxnm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmyzltna.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vmhtapuh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ccaqgwla.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrncinuc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2soaufbda.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ljwktmya.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yfyymyxy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbusgvcd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hrvbhzbh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xoiedhcc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vljksqdz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zbiyrvdl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zorgbtnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rckrepgh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sreziegu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geisbgsr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dspjcide.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2inpkhvwc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zxdwtsby.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mstijqii.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2yytevadj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xagwztcl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2anoxqlcp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fgyilogz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gjwltpev.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pnlwoldf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2eiwfjywh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mbhtxbre.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hhwxgnqt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rgoylbbz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wvfgfpzf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xpvrywum.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rsildyye.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qkubppiu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vdpnvavq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qarstrso.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iktoawbg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lhvimood.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2azmypekj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rbzciccx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yhcbapnd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ryvogihw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mqsulyrq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iuocfazk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2cmshstfh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2crhmpvyi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hdoeyngv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2scoceiqk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vtvatsgx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2onfskczu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mgghvmdk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pzgegngx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fkhftvmk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnispovg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ggbjlugv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dsprsnlo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2azgxnqgv.html


<!-- 参考信息 -->