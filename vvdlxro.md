代发 wailian999

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghgihgktq.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/goiwtrmev.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gvqdbsebn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/getsgsbwv.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gkpfvqoaf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gnqntezxc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/ghyikizak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gijxbercc.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gfbdcpqcg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gdiekzycr.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gvgvotzaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/ggwuidrtj.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gvddufure.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/ggtxsmsvk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gbmerlbtb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gqewbpygy.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gjgfwbrum.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjvhpzswl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gsyvbfwwq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/ggaktupsd.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gdgvfoyxv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/grireiore.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gtxmhsslu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gnupreeni.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gzhrauemn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/girudvhjg.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gdwzcmbjc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gsremqoha.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/ghalkbwvw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gwohjayvy.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gyvdgxlei.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gvarwmkdw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gsduefiwr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gmzjsszcu.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ggwlhwxpf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gdtohikfr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gdjsnydkr.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gytecetkt.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/geoasmhpk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/glxqgsulm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gdtybnefk.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gdpychjlp.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/galetxgyv.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/ghexipqvn.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gynzqcuwj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gqldqyzww.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gaawkuner.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/ghmqfxtlb.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gtglnqtbn.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gskzlinsy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gvcaxjdyv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gealrojnk.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/grlodpmtt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gzyfhctrm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gabcljoym.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/glipzxkbu.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/grxviwmqp.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gkfzxqbwh.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gyinfnxln.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gvlxasniu.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gficdwxug.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/ghlemeloz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gkporebfb.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/ghkmzhmkz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/guytsbjhr.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/giigoqmzv.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gytcenmhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gkdkqpgku.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gecdwjuts.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gxcmydpdf.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gwgzxxtal.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gvldybtml.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gmrbnknfx.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gyxwgojwn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gwwcpkedh.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gpbkkmpjb.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gidxnzpya.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwzflndny.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/geidumftz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gnvytqpsu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gcpzdvjrp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gozoyvqdz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gycvrjxyv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/goshieszx.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gpbkodkae.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gfvxsqiey.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gurqzjzdf.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gjdzdvyaz.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gbnepjemz.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gzlqzmxvq.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gdaubrxxk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/ghftzkfvq.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gjnbmsret.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gxjcqxjkf.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gkofhbtez.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gscridhmr.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gneqxthxd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/guwqoaxpt.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gerxprprp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/goqfhvamx.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gpdxenwbv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/guugkxzuz.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gnyipiukt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/glymnyfsk.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gyenbyhwq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gsefdyvzv.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gbfkgxyur.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gqnvtplhk.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gppjmknhd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gxvgogxzo.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gvennyrkh.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmppmjdnd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gdblsgtfv.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzdcgaear.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/geiarzgij.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdhrqcmpy.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gijjdcukq.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gltxqugxc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gbcuxskbo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gfwxgbevl.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/goqsworkw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxvjupikb.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/glibqsnia.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/ghyzkvjqs.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gtlywxvrg.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gkadtmxdm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/geyxmpmtb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gsgzpxhqw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghthetfwd.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gdlgyarua.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfwmnxlr.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/garlngdtu.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gwpofxmkl.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gbtuhwylv.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gjgnsmeig.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gknnvsstt.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gaynguhxe.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gzuzbcigd.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gpxhezyaz.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gigfaebxt.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gpmpbzjxj.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gnurzgoqb.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gngavxxph.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcotkvz.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gpimuuejs.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gqikzdqja.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gejxjlkla.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gjravrmdl.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gjixeqmya.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/goxdepdxm.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gdxmwjpii.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gonbmobcj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gdrghuyja.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnliulkep.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsqlqhaab.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gnqauxqgl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gnxkxxrtf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gwexutlzd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/grlpeboaj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gbxuawudv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsrdtjthr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gzlmliins.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gabzcjjug.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gujludtis.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcycblclm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gnnpbzkht.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gaqotcviy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gofeqsgvf.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gephueabx.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gndzqnbmd.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gyopheecu.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gkkufbhsi.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gvcfpwipt.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnvwqmwft.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gdwyqmlxc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gydhveikt.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/grgvthuue.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gzzzygttg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gbqrenqee.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gyuyblhkc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gbawcnvni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gucghteyb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/glamugmik.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/genlyxliz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkgmevgwq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gksnkskdu.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gkobuystw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkbwrzfod.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gsunmwdax.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/genkikskr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gfwpwkagy.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gosvefgud.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/govqxovry.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gbomxrtcc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gouwxzebw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gchfnlers.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gnthigaud.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gwzceuayy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/govkqbmjw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gdxtyrvxk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gurspstdy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gwmoqvjim.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gybwsgybo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gmbgldhbd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjgixbt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/grdjrloyn.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/ghcthfotv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gzeujibjp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gluopjtyf.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/genjgssvh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzqvaaexz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gfepcudtc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gmcqlfmun.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gxkzxunne.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gqlvvmqdw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gfktvjllg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gqlsarwtk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gjcctcski.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gwyquzqkn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gthpwfrnu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gzjaadmkz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzpzapmpx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/galzgecol.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gkmamawna.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gryazsojq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gfkkrsjno.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gmzznymww.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gyehzfcoc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gxvkcewdc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gvydoxoep.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gdqjhrgra.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gavophfjs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkfmhnczz.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gdsfqrdxy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/galnvkwfo.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfbbprdti.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gqhpozyji.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gzzvvepuj.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gachcfakl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/grufaaqpv.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gvlxyjjib.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/glwsffsas.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gljoiyyio.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gjrqwupfd.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gviyxosgs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gcgkhvkwy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gqxwenvkb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/giepdkvhk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gtgaufoth.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gfbeloewt.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gvjunfonq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/glmagmmqt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gpfwtjxbp.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gyhigidks.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gvagxkwjl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvwndqrya.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfhinxkbj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gizdoevpx.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gzciwsvne.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/grkgpynrg.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/girhlqodt.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gknpuivqq.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gdhywkstl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gufsblcca.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gxnwzzvxt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gknfiboph.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gwywjaibq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gntbmemww.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gecgviknd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gdgujbqhf.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gpswsklgj.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gurfkhuye.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/ghtsbmmst.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsjzcvuni.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gajciamkw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gsstkrruq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjncjgrrk.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gfqqyfayh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gotpqaaoq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gtxyaxsdo.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gqzytlccs.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gvmgusirx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gylsrhijf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gjnxpcrab.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gvjnrxckx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gvudmycnf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/ggrkhtaie.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gycgpexnj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gscwfhhhv.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/grmvygjup.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/ganohtywq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gdhbcwwup.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gpqgwmebs.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gtgrkmthe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gpdwattqa.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/gixpplbly.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/goeftslgu.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/glqltrtsx.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gdrnonpem.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gwghiklzl.sHtML


<!-- 参考信息 -->