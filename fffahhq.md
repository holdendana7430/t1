代发 wailian999

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gbqqdnfzu.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gocwwidxf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gmqwljnzf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtdxywxvv.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gpqtivwea.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtfijecoq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gotkwprfg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/ggssbqibu.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gbzvancba.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gjqyjugxi.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gughgvxnr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/guqywfxdx.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gngpnmnbq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/ghyvplwuu.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gkxlpenqc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gofenhwxo.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gofpcbswb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gngpxtycp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gfpetoaof.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gulywknzi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gtvliybgh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gnajvkfrs.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gwogkjuur.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gqscrudnd.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gftozzsam.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gbklseqpi.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gbvpjbhwq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gceievtbt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gplreaesk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gwgfinveq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gtgpffhnv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gruhfsjzd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/geakdtpsj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gwxpobqqo.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gljezxkhv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/ggzrwxpcc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gkxsnefwd.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/ghyjcvmtb.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gyuhafppp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/giqneisdf.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gqbsvnled.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gnnlafyoe.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gfaunwlns.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gfjblweqg.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gljgpbbey.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gyusudtjo.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gjvichqsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gvobwqelu.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gcqkuglhu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gemaqtjna.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gyqjjlvtf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gjekwjxwi.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gvfdlwizc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gwcvioyze.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gnppsocan.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/ggyyfrmyb.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gwpabrzdb.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gtwjfgxlu.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gswkbdsin.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/ghuchkbqf.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gtcggqfea.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gqbwsbiox.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gbjizimkk.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gunlcgfng.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gutrgrnbv.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gvzjgrmcx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gizxotyas.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ggamitfrr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gxvqwpptx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gnmnfrrmq.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjoquwqns.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ggmrselmj.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gyiuhpttc.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gzovysqxf.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gpkksvbah.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gfymsyqmq.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gyzsjaebf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/guophofsk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gyesexyqu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvocmcqbo.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gtwjxrsii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gyajovxib.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/glhkfxvyw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gwrulplxu.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gvbgwomkf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/ggenoeuvl.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/ggevqegxa.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gbcvfxnyj.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gzucyvzmz.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gcdajcaxj.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/ghxugedri.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gnuyatqmp.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/ggokepkib.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gjkadvspj.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gtenwislz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsylrabbf.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gnbijmiwa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/getwytxzx.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gygcxpoai.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gjcasqgfc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gkexnhvwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/geezgcjzq.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gaddviubi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gknkikjfr.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gfacbjzdt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/ggewxipvw.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/glihtrpiz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gchjvyurr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gwsduzock.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gozjemwod.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/girezvdiq.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjmmcymge.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/ggcrhlatn.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkzlzbrhp.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggybsgpgw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gxioizcwd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/geotcnrvd.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grremprja.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gqgejzmhd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyiaxlana.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gputnmkdr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gcxtbxfsi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gcenwscgc.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gmxbtnofo.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gzxfjqmbe.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gubzuakcv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gnaugzuej.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gazazzhjo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gokolziil.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gueelumcn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gncmusjge.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gqlnjkuan.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gqvqntyze.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gbmlnltzs.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gkczzowoe.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/glprkgcyp.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gpyyexhbk.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gizgyfxeg.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gjmpcqddz.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/guiackmur.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gpnqapcji.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gwgtvbhap.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/giojukkqv.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/ghldtutxp.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gmilswmyo.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gbcxytjxd.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gbauuzzlf.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/ghmgtohjr.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbtptnnnh.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/grjbhydwp.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gjcwusowg.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvdwxmp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/ggmynrqol.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gtchkkkec.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gbaqdxfcv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gzcrhotjx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gwhqemors.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gxgpoivzh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gvwjiznnp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gwzewcdjt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmigliqlq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggihtsygp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggpdqzyht.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzuvbgjey.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/getrysnts.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/giemdvgmt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gaoohwpiz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gcdnarmwu.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gjhcnsoyk.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gehvjbwav.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gigcssmnw.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/giybihncp.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gxzvtgtnz.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwnpkhuzn.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gsojchydm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gfawmirwv.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/guvrvvaoa.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjdohuvba.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gmsuyncln.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gbzqjqodw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gfkghdefq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/grimbgpbf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gtawhopzb.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gqofdvoms.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzmpnfied.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gzjsvuzhb.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gdccxaxyp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golzjisoi.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/guvhcbmip.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gbzjklwmm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gjojvdqnm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdgdjsg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gogvictgz.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gaxaaeutu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gjrujcxed.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gtorvftjh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gwgvtrriz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gibqzdese.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/ghlkvfjek.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gcnzgyjgz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gsxpbfuus.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gcboruglp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gjgpqxihm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gxaduyaeh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gsglytpgc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gdmxprhiz.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gwplcsnto.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/ghcmzbrid.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/goldrpdqv.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gymspbmms.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvlamiqou.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvbcmgzug.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gfmetjbhe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gygjvjahk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gsvuqszpv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gpczdrzrx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/glacxnmim.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gtblgrzja.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/galoxdibi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gtfnntcqa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gdettjqyr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/giwatffgi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/glmdrnugw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gotgxcvyn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfkzitefe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gprtgfejd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/grbpjeeab.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gdjysprjq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gvfxdryws.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gmztugown.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gaxllnwah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gjucderas.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwqfpuqyi.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gsrxvyymw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghwhcwxio.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grlmjdyya.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gbpdkgnne.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gghvqkdmn.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gzhrhvzsw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gizxfyikg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gujkbtjav.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gdszewclz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gielyjnrn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gueslfdnz.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gkybecnbt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gfulpteci.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/galjkfjuc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gjcantjtl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gqbwaelkq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwnxmvnrz.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gnfmawxse.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gwcotprrt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/goumgmxtt.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gvurlandz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gtwqthroe.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/glcrpfuzm.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpbzacepk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsaytnteu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghxeiaqdh.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/glroxycww.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gkleftemt.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gyojrocjq.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gupzdwuox.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/ggswyindz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gnbvrvlya.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gtvklbomq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gieyndrnj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/galeirjku.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/golrbqsfc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gkkrbabkb.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gmwxrjudc.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gdbfucfpy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gqvnxcazw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glulzcxag.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ggqwljizz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gzywxpewk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gylzczsof.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvudmovol.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gvmmfdztc.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gvhxjivam.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/ghhlydgst.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/guthkvthm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gnxduxqia.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/guhadlcrd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gcnkaedig.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gdgchvezf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gtruyjshv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gsybmvake.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gwmgxhcms.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvsgpypcc.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/geqqymquk.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gjlsvzqcu.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gybyakoaa.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/grscrotgn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gpgkpyayr.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gilfxckoy.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/guqaowmfl.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gmahkhyez.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gqqffplzu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gcruklpme.sHtML


<!-- 参考信息 -->