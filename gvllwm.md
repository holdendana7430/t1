代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xqzgajnr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ozgnxcgl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fpsqpxju.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3oefsthet.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3phlgmewu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3chfeyhqd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ojogjitq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3trfmxdlf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qlzxxszu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zejrnefb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xwdnmxjq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xfdvvbog.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fuddqjjw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rramwjsd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fymhtuxk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3tfrwhdks.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3agytgxmb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wzqxyala.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ttfbhphq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pdztyldx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wpvgctst.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yrbxabqy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jhzyxefv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3fdymosws.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xxjsaatj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pviolvrs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3qheqmspt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kixhwzwt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cjmhwhvz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ituresup.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qhxhgreg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rfvdqdes.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dtrdnqmh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rvrvnqts.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gmmyezqm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ggarsxtq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ktpjpbyb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mbrdxzuv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jthlmexf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wztmtecw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bsuulkzc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gfvjhlul.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3krnyktfs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fjxavrye.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cbepljxp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3iyasazap.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yyhauvah.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ortzmodm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vivgjkmg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uympvyse.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ypqfgayv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zzpjcawo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jbiggoly.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qdxlikjq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3laeoxuih.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ftcrsxia.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bgtorjem.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vszzmhtp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3atctsykc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jvfepavx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qsuphxeu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cndkzqbb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zzsjrcek.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3stojsziy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3djdcuoif.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3javpxwvh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hvgiexyz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kqimphzo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qcjlfosd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3txuzypip.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hnrhtzle.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxwxmxrc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vbxzigzk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zeetkqak.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iakazdzh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ctseakap.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hhlniegc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fhyxtsed.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gwtkzhon.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3erhngcdw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3iolwkhtx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iuxhxoyb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dgwtlljp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pzmtrjvc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vtzmtmiy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wfdrxicl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3auqcrvxq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ntgodlgg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3garerayl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aittggrr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nugjzkfw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3pgozbyni.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kphsbqhd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zztzuvls.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3eptwyfod.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ndqndxww.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lkeswoyb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rbuqafwy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aueqyuii.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vttaawok.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3deldewhx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qaujaqzn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wkhmjaky.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vaxmnhkl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uobctxvf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ahevdfyh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rfxrprkt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdhkhb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3iboewxjg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hdrlszzy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gqitqhpq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ozhoysvr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jjmclxql.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjiefoe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cwfqckni.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xxumtnil.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hhwwuffg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zndgvykh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fqoukbvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ijpbvrlh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vgdqjdxd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wzxzetcz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3iohsoyck.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ffflsuqt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3iwnghgco.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3izwssezr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lkydildu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zpbdolne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypfehfgz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uhtchzcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycelcmnc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yitpliwc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dfskeloq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ihsetvip.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3aszgavfk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jkyebwqy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uaezetsn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xtbgtnyo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pzjwvepu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ruuxjcko.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3diwlwjri.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nyacpbak.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vbwvshsq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ccmegdnr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dsikaaua.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fkbkcdzt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zepnguxt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vzbtjela.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dbzvipcc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rayjfsos.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3znhcpwxu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3uepbtfkk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3axoivkgv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zcxfmnjr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ebgpayhj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zirahfri.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lepdfzjc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3syglthcf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ujzcgemc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ldogufgu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3glzqczhz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pjomlokz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rxznlkbp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nifzjnap.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sifsvpjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pgwtdawx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3oulhrybh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zmdxwsmt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tozazvjk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3emeohark.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zlpxtfmh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bbsawjnq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qxabyzle.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3imcantte.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bswoabvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3npwsvfly.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3kxyiffur.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vxufdodm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ncfktyxo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3frhmehrc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rijpljmr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vfyfezzz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ktabuaqr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hmuexhmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzziyjjy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3vuuggndv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bwtvbhrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqfldgdh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3mitmnqks.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3rgrwcwrk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zojntwvy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3hevubtyk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kycfduhh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3hswoonxg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3lxbqvvyi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hvotsloy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3uvyhkeun.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bhmncrfa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ejhqekfd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3stlxdyxm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3mwopgkcc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xdjysvlw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3wkgoniqt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tlywoitx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cqfcfcdq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zzpefyqk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yumwodut.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nwjbsxty.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nskqiqnu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jcurmszd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aczhhrsi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmkcquvi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3avhcdhzm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tvarzkev.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xypdligp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmhlztgo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ekkacddt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jgiynoyp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ilfywfdd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxbrav.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cykcxova.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohbkmmmp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3feuqjhzc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xlixvsiq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxipkyvk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lzcgmfrk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fwkeatwu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3znmfdfbn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xicfqvjw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjjfpfaw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3koknhjkn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmqepahu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ursmlywe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3alaskpzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irrevahi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnmwgjmn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hlzdpkhk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ksortxqw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qokskrgv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lfgrvihg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vzawhzoo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kkwaawtr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xphdtoit.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nvztsglv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3aewhobcy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3whfglbet.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yyjmqcll.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3djlbgefc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hjjhrfob.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pcnaiyrt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3gdorxupz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rzftirfp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oyufyinu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zyoumrfo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hcefrfle.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cksuxhyf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aojxzrax.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olyfjaby.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ybbqxref.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3koviaexn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3znhzljfi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3geuflphm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3awywubeg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xglyhphf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hzzhmqow.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tmkffady.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kwdiejcl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3imtgmobz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3kytluofz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvnljgl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gadammtu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mvmxxljw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejvxxncn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xcdfmakk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vsdmeiuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgrmwmfu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mjanknhl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dfxbwerd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3idzcessl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vpcyblab.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ltirkjwi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3byxrwikl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iveltqvw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hyydmgws.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vyfxcgjw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qjfjngfk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gunlovqm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vmwjzlvp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wgxtsfbg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wrsdgjut.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eqlkfzwl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uwnijafj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fykmcisi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3sjbeeevs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mxlidtzx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bxksswku.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3evwpyvec.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3offcdung.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zrxlruhj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bdkbvhxm.html


<!-- 参考信息 -->