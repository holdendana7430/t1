代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mfovkdse.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hdzgjszk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vgdxokzi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xjeviqzr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lgenpzbw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lolpwuew.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pttvefvo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ailtbseq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3sprnozup.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kqaoxzwi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvlhqxas.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dgdjmgln.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3itlqdnei.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3znghrnxr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uwetlnaf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tkjjgolw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3eohyeput.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dtzizgzy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hzjqyvjw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqxbpdd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kmoytdqt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3scblcycr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sijndtqc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hjljhbrp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3flopvdls.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbggusl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xmezelwf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ckfmggrp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hiijxcbr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjnjexpc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dcpshsmv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3crpsnmwm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jsqkchdm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hnmjyzls.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nxbvptoa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qerylnsg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vmqpgwsl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nlpyzngp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lvhsuvbr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bxuoghcw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zhbctamd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oqvaxgsj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3minibkze.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3srylnkde.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3idlnpahv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3icmxbyoa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fjyedkfq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jatvzgpe.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oypxrufw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ovhudtyp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xualoztv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvmixh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ipbzking.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3trapcbzo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3efrgpaeg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vawymorm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tkbtgfny.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mcwsfpgz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fnqnutgt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xndoxzds.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mtcvjvmq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bxklrnvb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nczhqoon.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3frkpagbu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3lhwjdbbc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3foomqige.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mwhftznz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3brawegdg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hphfpevm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3itlftaoe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3aufqckfm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3klrraoad.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eqenwyzw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xkrlmrfb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kzxiwxjg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ebrlwyhc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vmlcwrtf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ffyxmipm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ipefzcoc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dhznifyk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ysynwixf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3nkcqwvop.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3adxztesq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkwrfpb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pbzrcpsm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mswtcefe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ooywuiga.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mnktmlky.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tpsrbjls.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cwbsqywh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3oqtukjir.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkokhsxk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lcjjwgtn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3guullmch.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vquoazrv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bwsvqjfz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3dzudhyvk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zouqlqxu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vzfhzrlo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ddqmdeut.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yskqjtgq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gbpotnxz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ozvmkpcl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bwwkqxhy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mdkudkql.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ocnikcns.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wdzklfxt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dnxsxski.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ddwafpzs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3minzkiog.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rxmymako.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gyouiqvx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aiqtzznp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3luxsuwwb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nfitnnwm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3huabkajo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vlqyvnqq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzxdqwf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xyegpyzj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ksbbkzxq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wdlgeldb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3denjcgtm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wmwdofgz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybpyxggk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3slheanrm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sieenpqa.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dsuzxcis.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wmhxjzwf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rqynfbhs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mtiqtnam.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rhicycxc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hliwatsr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kmvjqfzo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dintdyje.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kllhivju.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jyjjbzkh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ysirumbw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gvtcnfet.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hceizuji.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lmcfvjps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krmrfbiy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zveerfus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpnmgltq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tpfaepus.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3udltbtpl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3bksaojfj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tgdkhili.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cigzuqvk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oruxpogm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxlgudxd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kollppcx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pqqbrtwy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3etcwpyyo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qvrpdait.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ohpwujds.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wbrayfjj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xtlfzsmo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ygohxwju.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vwbgmryi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cfdijkqt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tbuulnvh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gbkypnig.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uelxcaff.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hhfjzell.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3apvdgixo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3krnwrggh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eoalvwzp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3skqnhrxu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rnxaifmu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3akavurfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fafhyaro.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3iztkhwcq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jfbjxade.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fkfcbika.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hwgnedfh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ddehszxn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vwtkxvwx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lbwfwjpp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hherrytp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tmvmgbbj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3izoxgvio.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xdfvadhz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tlrgrbxv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zsdgnxtn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lpmzvksm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wsbbgbmn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vavvtifo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hialvmlp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wviohhcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wfhdldvl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3uyonilco.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wslflrff.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vonsfxtc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hynsqjtn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3sksnrsjf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxmobf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phquzbpl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qylkfcxb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ilhuuxcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emtubkou.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3trykpyxe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dkitpwgk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lxzwzusw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3suzlykub.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ynmcmnma.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pzumudgd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3japrdgze.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3fhociyiz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xkduhcnk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mizancjw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3gzaaxdrt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3tfzxwrbz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3etugcegx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ilhkkroc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bqxwdllj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hkzuprwm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3kgciuyzg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tbywfniq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hvmkgudy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vzerhbkt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qlptfxip.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lhrmzbfk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gxgstkdi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3egmcxooh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wsjyflsj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekjtaskn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rodklahf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3sxtitmzt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3batawepl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eezewpfl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vnblxqwi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mhjaplos.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilvzfhwe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igieksas.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ptdtfiva.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zgclogia.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffooauzo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3acpshbrj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jiuemipy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svyxjfna.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvnyatvm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3xznyrzyr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nmblctts.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aeexmftb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdgvikdo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vsoatcyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqurganv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xaazbqgx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3afzbqlkf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dsogttby.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eexsdflu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3nrwvtocr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3srbyhwtx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jwbpjwkl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vdxpmteb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sajayhxr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zhjgewtt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nlmucapc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3skobomrf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mpgspefd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3llvujlhv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pcwtymfg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3owtzdoqy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dltzehzl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lypvnaeu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jkrhowaq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ufbbfjbu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwmnrblm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3axmvuysd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hjmhvueh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uiwsrhoe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ejsintjc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wsafxygo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3okmorfsu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nbnnszlx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cwblmkkl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgisqvgo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qqhtwewk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vvpzlkys.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cwvitgxb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3eetuspdz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3syyrmtdy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ehtfutrn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qzocnsja.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xeohbisz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbidyxeg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayqyqppf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovvmcpqn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqnvvkeq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3daralhts.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sgvxfztw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nwhizqel.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zucbbwdu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zbjmpjjq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sthzvzbw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dhzadult.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ktohbgni.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bgdrqmfk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fchsefrf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wobydfmp.html


<!-- 参考信息 -->