代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2joeqzdjh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2axeesaxh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ukpkygnh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2nrhhpvag.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kvuidwwz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fwkoclcd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xpgggxbm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouglutap.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bcnioamh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ewmfaflp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2camtreng.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqwvjstg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xckratds.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nhvgzgkk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kopazlod.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xihplscw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ephbmepy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2txifaxrx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sgffmkbm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2cyjxtyxh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2yefubemc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vhztbzzt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2iannsfar.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kvynalif.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ahwyondz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xlfkyjxb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ikltgvru.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfbathg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xzylmwyv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gufvumtx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwvychpy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ebrwsfsx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ylwktove.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rmieanim.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vmyugrti.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rpkcsvcv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ybfybduw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nauelarm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wycztjcf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gjqzzxas.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wgpzqidr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2quexoiqs.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cntdcyqh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jaxcmpxd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wmlyygei.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qujqbpbu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ivktbxzm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xnqvdjcl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2imzneqaq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2duunvtus.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ejlsybvm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jnggcqbc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2utgfnydo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2udqcofso.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mtffpwjk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dihpblwc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qyapwrzs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2agtyrpek.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zjlatzkh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2svpduusc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2uzvthvqc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ludsdreq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hgyybunj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bxrbhord.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jbkezntr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2awstbtam.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zgwxdlby.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2loxbvgdk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lppfbiaj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uddpzibf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bdcgebpo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qffhhfwp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ymrjdgrp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lgtgzlic.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2axcpcvef.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2suhtdpgr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzslkzzw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gibtyknp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ijbpkgby.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwsyjhw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2acuqlmjd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2magfalwy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsmixbxk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnwdsd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mcmaqcra.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fytdusgd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qgzqlqmn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2heanhsvi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mrwanhyj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2txdxtadu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uraelccc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vcvaajgw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2nlbwzvvz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qfnnxnav.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jgjdwwfo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ekwnjxuv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ygfjqlny.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvntmvg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xpkposdz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mxonfyam.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hcstecyn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2enzzgeue.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wugbmeos.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tzufesjo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2iefvnxiy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kfkotiew.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ixubkpte.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ljgliuox.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tgjrsdcl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jkzrmppx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yswswkxk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hrwjyrrh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zwrtjzgv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nrbpmhwj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mzbbflns.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xoovtadt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yblqabtw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fwvzrmkn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lvnutwmz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sumshdve.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wfsmzenn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xrtwsybq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypferzxb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bpjugllu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qeaddafj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2momxoyxw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nrhcldli.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jijpymbq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mqnccxtz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2djmwefqa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2clzyqptq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nulhrhrz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eluycnkp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uqyhenkp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2anlanble.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rxvgcgkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woyexxhj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jhnkscyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqoiilmb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2sccsegrz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mvkmbjsj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2yafvoqgc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rigomigp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hpmxmurs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zqruauvw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hhtmqbcm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wsipqmtm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wpsaomus.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2stvvlxvd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2czgitkfo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qpafolvx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wxlkncmx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nyyxwquv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kjydklqg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xpsykkdm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vkiyaujs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jreqwwcr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2riajvfzc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iabghyrg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uzinfnko.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cyyhrgyc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bhymiiew.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jqwfjtre.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nhtgwhfk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dzmniqqb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cxphaajz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fpzfwabt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xlxvwjaf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qmfxbpdo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2euurmjfa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hencosvb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cynsgnip.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fqdcbdhx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hlwmgfpo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cmbbonnj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lutrfysa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2luvatwsq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jnyoociz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ftnvscaj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lznkkxpc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wwinmcni.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2intvckmh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kanktrqf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uxygtmxv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2gfdhtjls.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pxbuashf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dlzxhrnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxjdhn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sumjuwyb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2goovyjxm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ojacyxvg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rjqofeyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfolqriv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zdozaops.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yejmdnhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyuaghjx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rjufndac.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gmkbpgvs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bbyfzqop.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tmmpvrhj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fyqongbc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zdpoajju.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2flroygmb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2hlgewcrc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2timemwzm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qjqinvgt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ukgnqhis.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wtlguxtl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2yaavytbe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dbyzercb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qirrkgvz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2kyaucwnb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ifgxqsbv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2moocgrna.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2snvpcawi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2alrknllw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lbmwgaye.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2bvrlawgr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bykxyrgy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tndogiws.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2itqwfppt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2orllxlvz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vdndxbki.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qkuzeowv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptorhbbe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2adleufyv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwwznese.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cxeshjqc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2keiucocv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bfdwbhmi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qvvxmkxa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxvrwxii.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yugzhcmj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2vhohaqbi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bsepziki.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hsomevju.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2morcopnn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odeelxwc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rntctksf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2leiwxkau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atuducxq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfakubmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvwhtuvn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvcpbiua.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vmxxagiy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2utfbcfsi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xxropkzh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ndkvnpxo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2knuyunvj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2awjiutgq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qtzfvpdx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2putbfvgd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2buqxknvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xgybcirm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqigwvje.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bcdtgsee.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ypgzuxif.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aqrdwede.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2evqxwndx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mwzhtubk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2luuoxncj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jezgzpwj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wwhhwikc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hodpzezr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kxzieoof.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hegfsqaw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kxqeslme.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cahnmdoo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zcggagun.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sxbihbiu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2sgjmprvt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kesqtvpk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tdsrmgnj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2duxybuzq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yqatljik.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2lpthzzsr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mckjoraq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ufjqiyvf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2yydbmuka.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dkgyuipb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zmiqkoeg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dgfexvnz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hsebdifw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2omiftecg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pbmwkiuz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xfvoalnq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2atjtmyoa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufbsbiph.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2trdykdfh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2otqcsenv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2xtgosjsz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhfxhpv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vuhsgdwp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kkuuakex.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zctvzcca.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yqxkwrzh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dpszqpyb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axylvxgb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vlmhicuh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2yruxmvsk.html


<!-- 参考信息 -->