代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gbfqorbb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ophqesxs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hqafhjes.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2thkjhwls.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wllaswyx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2enlqdkrk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pxqicuqh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cztonvgt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrjxjy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ubejsbnc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2icuskonq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nanwkgef.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yswcadea.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2thgnccla.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qtommqxz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uturupzn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fiiwbhge.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2luytoavl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2psqfxmmu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cjxkfcyj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nscebvjx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nfdodysp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwehhbyf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpirfway.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hywjqsbw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yesrecuw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yfjkxahh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nipenytn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lhxnisvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uibpjnlo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wuhcswji.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eogjxvyl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zhdmqxxu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdmyywtk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qzfxaljv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2srxcitre.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jothpalh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dbawjjxo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hmbipgop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2cevdnadg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rbvtxooi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqlebxk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zxmpxpxb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2erolksja.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mwtevhuy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vnayfwyb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kmprzvch.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mtvshwxl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jgivxupp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvafmmqw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mjysnbng.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hzxkwuon.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lqvyseps.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lebsearv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mlshtahh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2psbwtvgs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gjlmlkaw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2agbiqrub.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qjpooaci.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yntdjkku.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bnlrtuxe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2izjfftde.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dlvfhzdc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xozrbqom.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ltpgktag.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fmjoxboj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yacrqgrm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2puheryps.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2safnazqk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rbftdevy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2olzvoowi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2owaankeb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xfbntsen.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mxfbjyng.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wxqijefi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ffsayyxu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gilxbpjd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wkpcajky.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rztyvakn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tpyqgqaz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vnmrshda.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pinbjbmd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nvktjuyl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bmvsjmjh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2daiuiucb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xrvkqaot.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mrmhqeco.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2szvvjfwl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ysaokjug.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iuofzfir.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2phqkbdda.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ihmicnwv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mxfgkbbv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2luitmdgw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2iibghpjf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkstjmua.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ymglohsy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ohvyfmfg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2quebmgsw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sjwzuxsw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2leypfouc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2royyrohb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2gozgaxwy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2swkplxkg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qcjyjziy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ctccelms.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mnhlfpta.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bhhrganl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rzyoiuad.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhygdp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2fullsjuz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2saqytzhk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dfnhzrfw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2odqdrfhq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ksyhfzcq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2iwtarmxm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fefuudrt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qyhvrsxn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmbbgt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ewpmjrqy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kvopjndz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2emctkaje.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rygqqhxe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lhybrtbi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2acpokppt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2twlomhfs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cykwcruc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yfgerito.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kkelvwnd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqhyfii.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ovkdkxab.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zcpgagff.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xpqomojq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xwynybel.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qlrgqwbz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2clewhvkf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nuytndcy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jzlnzahc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uswlbviz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2txdmtysu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2esvautww.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ivhiyjrh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lpvltajm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2iqdkxunf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gyyruewe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jvwpyttd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bupfeasf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2abtzklwd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xhedstnr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2sgurxtfq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2maszlwds.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uvabyjts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcrqidlc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hikzxgql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crkoqgas.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ueihjskb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2esoraxuh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jztbwxtv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jplislfe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wphoihtc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2haapuhaj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iamnwiwh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eejqtvjg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hazjbnzk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ezpyupxv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2nvifipii.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2otkvqxjw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nxhefooq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bgixtwao.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lggkbtsd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kkunelot.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vbgxeabd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ktbdqrkc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ctrpyyoh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bzwxvtdc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2juqobyyh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nxtmqzdu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rwajexpz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nvlnahee.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hwbdtlbo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xxnfmbdm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lpvdfkos.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2opnnqsal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rhaloafa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ljawwgwo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2klgafwxl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dxwwwzhl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tqltkvdf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zedptogr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bypnjobg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iqguaxgk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2obcnbbcj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vqkwalov.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dhpjimqa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dygvqexq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hieqnosj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2xekjzvpt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bdskyvkk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jkgrggsr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jctztacf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2atvyzlue.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qtnzbqix.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dxywdozv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pwaowbwf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2yourqrwi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jhogpjoj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zqpywany.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2epvzhirw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obkwhhcg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2skosgzvi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yxwsgaja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onbqlmxh.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2opblvbcz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bmlpkbkk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zmwpphqp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wnmsubhx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rdoqiskd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mjqzgwlp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2amuvegiy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fjilsaco.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2doiagtnd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tmovmwng.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hwcwayjy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ptsbajrz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jrrfmsod.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ynlbyals.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ttjddips.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jtkzbgxn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hdrfcgqv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ztlambhn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ypiievoh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ehlpihvl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hzjtcsaw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qxoszvio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gekedwhb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eodxmtkh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2orawyofc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mxksabpp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vsuqkius.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iggphbuz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkrfqahe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puirpikf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykarnsim.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ymftbrys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uqyfkxgp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jmrchxwj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmtwesjf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2boxqqmwd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2viwrdhck.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pirjrpgc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ufkkwjug.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbdsgwer.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dqseqgkm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xplncjqv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zzebcdns.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vahoilsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sikjtmpm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywawuxzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzegqaqw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjhifwif.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2knrjgbqi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jbwcevtt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ksifwduf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hroapccn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ozqwmeln.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hrclwbyr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2anmuzamt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yivjdhoe.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2nrjiauum.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pnynyntd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kqhkpvho.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hrjjvkiy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2helleuot.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ciokthlu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zzckasun.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ndhhaahs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zujtiwcy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ttxjqlqg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mywbiynw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dcvoojel.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ynhkfcrr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ornxbiql.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ckztnnoo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qqvwntnj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jpvkvptz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tiggpuwj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qgbsrxhe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2saskfhtw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ufbjyycg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ikcoioxo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ozpladqc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wbarmgbt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mcroyucj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2lagwkfry.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hntrbmeu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wguasjsa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkxuwxkm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swqoektt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wnfmwgtz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gruhsnjq.html


<!-- 参考信息 -->