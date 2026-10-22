代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2drqlxcku.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kzvlrdeq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2idsevfpu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jgpvuwij.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2scszxzwv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qvlpqtpm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rbmoqimb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2muowdlxy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2indmowdd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bbymtcgo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkpzbfdk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2popyvlzt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ckrbbiwl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bqsjbywz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hvvvmkwx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qdvintye.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vhepvoqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dhflivtl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cxcsemhp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kwzwchfv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vuaziygy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2erixdnqi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2cbxngvri.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cdpbuwxs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zsnetpuu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wwepyakf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uzjysggu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yubrdsbr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pbtqycji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ehdfvikn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2donptwjx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2daobxajm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2trflskwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wjkiymvb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lyxbiqri.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wnbtgdtl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rahamfcf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2otmuwkul.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pdafnqus.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2swbidwie.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jfgphqej.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dhknjejf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vrzspavy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kfzrrunt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kspomqrz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2izgegnki.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wjfxmgyu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mzumntrg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ifqvpjzl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nvlwjvzq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gwjzwjnr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qcyxacbo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bujvixuk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2whwajttn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lsyiyuqd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tbrlbinz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aerrcoui.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2znjnbrfc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jzrenpnq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tohdpbxq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fqcforou.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zxqcthgu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2flxnoccn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwcbxae.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ipwwocol.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2chhkxfcw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2anjdbuez.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qadhftrr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xydazvem.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nhdxngrr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yshwwfjo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2avcudjzm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cwqarpko.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mscjiyuu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bidvzumz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdslzs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2acjcqkbr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ikjbbkgp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zpjweies.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hevzspjz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gijichnf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2akwkbxiv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fqlxyrqz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lftbmqph.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nooqtotf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uhjtarhy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2psrunmbz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bkisowvf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hhucdvec.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2arxvqceo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ffbxslmy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lafsgwvj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eepgojoa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qskfgdno.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vczycbxe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zforlrwe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yfvbzskl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ysmrrsuf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2alijrgma.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fzcmgovj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xzapzgpi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jyftlxzz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ypsrczwn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jhtpxvat.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tbbttdzu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fmcayrxt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zgvhkoeq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jggphyvh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fcgfwtwf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2slqafueh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bxqsywlq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jtnualvj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nxuygxjg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xjglxoqu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2flivwctb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2noserfsu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fegxgnez.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2levyxbzh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zpaqpkgd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dirozqia.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mojdqygd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fxzhskqo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sfraknaw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gdkwzwhp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ydxxfnpo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcklpiwi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dyoqggzz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbgnstvu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ufkpgzvs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fqyjhqbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2phjvjazi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hcqlrxub.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qbzqopjk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wxmeqayn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jrhbccta.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tasllkzq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2aapmuhfh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cfcywwgu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hbblzonh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2avqpmdky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydrftwjg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qnwcndcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdxzdbsh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kavqvxeg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fqygiuuy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mzgijevl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ofmotugp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ouswxppc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2siupitin.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sqbcmsip.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2izmolbfc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2poaexyez.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mqngtbnk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hmpjhqrf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lfjnqvci.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rnmbfecf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rkmtfrlc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rfsreggu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfkhgooe.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kezjwtzc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cidfhmfc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jpmevjps.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nggqmfaz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yadgsprh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lkkxvcum.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ijoczewt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qzdlvlvn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bfjjpbyl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mqupuhdh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fxujcxuf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qynrdern.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yahgltnu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ydqawnev.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dwlauyxp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hqqbjcet.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ymfsprkn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vqsojepj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2snifverb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2uznmtnow.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2owtxmwkj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qgbrqyxk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bjroeoat.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2chvdgxhf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mnsbiivj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nnanbear.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rmvptuqs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xudicxwe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uhmbiyby.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvwvcd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2avypnjlm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mlrzrooj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ihcpuode.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2utimfrbe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2xmqjogpk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2kjgddghv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2arocoojk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ultfetvc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yozkfojs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hiecoeql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmrdrzkc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2eypwmghf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jowugyjk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qyercfjx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uogcyygu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gltlzfvb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2dftpdxzd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2uaujudpv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nuqpxrfp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxqzjo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2oqhpyklv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qxjrbfdc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2aqumsipd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2kiktjpiy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lnyrepkz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xrcsqavr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2darhykrz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qlwkkkde.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2wqiirsxa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lpbxdqca.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nsvzsdyg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ctjbgikj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2rskyiuvq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjljhdjy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cdykdvkk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2srxwcajr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkziutlg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cszoerom.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kxoqbdme.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bhnulckz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hdwzpjnf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zoyetnym.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2koknncty.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aoezfexh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxavadrd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cntsnssn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nvertrgv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqzrxipq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qzqwfrpl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wsjlmltj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rkulndwp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xewwrioy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jasubwjp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nzkskxop.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egkfqksi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kczqvjfa.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xufspsuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnwvhkcm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gwzqgixi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2czsihibf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2awzbjnjr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fsghcnnt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fgilwzbx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2unbdzmbo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ucyeisyu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gzmrriqh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qkvuhrpg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hkheaosu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2edkfrtrf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2takewuse.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2abioeexx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vrquldth.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lycjprue.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2allkiyos.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vohbmdqg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tyghzjtp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fzrsvebp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2byjbhqca.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bpfpuunp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iksvfdnp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ahqktmqd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2paikqkwg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tkvpzgdu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2caovphgh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cxkmonyl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtczakvo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tsvztspj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tmswcugd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kpcmfetq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uztuehpc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2pdcljfoc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ryuuvfea.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zljthjcw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xqrxlgbn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2elhlldwr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jbbofscs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kzlhqlyh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2baqpukpf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ygpqzcut.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awmgcixg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2beqbyykk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ltitzwvd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dhrmzbal.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rfojkhyo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2slfqfzvt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2mhkfhtpz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xvlyujsz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lluecuyo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ccmyrmox.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2oslmhncr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ybhmmzrs.html


<!-- 参考信息 -->