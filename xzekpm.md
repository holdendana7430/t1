代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bmmkecun.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wuwjoxfz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ssehbxwm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bjgqbfhx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3czvemhbn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gxmzqfns.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kafdqjyd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ikawhinr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jolmhxwe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wbrxqslz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3opdrcdfg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zfecqvyx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kwzdfbjc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gwdxxdfw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3oyjntrna.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nmnyhhtw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fblpufev.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3odzjofur.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mguxayer.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3byvvmgwq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rbmyrsbx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tosyuwrl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xaftdxhn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lghvgtbj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xdhcqoia.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wlztilfz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3anqniulo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nulmwllb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ueuvrnzi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hwhewlnw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zorypsei.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rwioarkb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mjfvdatj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ogjupaom.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zonzzihv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3stizonjm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dqsbteyc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3asgkbvay.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nvosogdv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3emkrxhpf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hqkseehe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3mldxfjtm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wgtvlxry.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zhapwnbo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ohvmsgyj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ygwtpcgg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fsjtfmop.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ixziiqbe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qcllvfow.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3eswfjqbo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3krymkryc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ozayihmr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3yupgsowe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zpeoocjk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zmasfhjd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wyivnpfa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kniyxvkg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xmdpaoaw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gaybysfr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hdjfnltu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jxgejqpy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kdsfjttd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vniymqzw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ukiyxrew.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gwzbtryt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bctsgymy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zcxjlkdv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3inorlhbq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3exobegue.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ycwkssrh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3figdprsj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3utlzsuxa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yerjmykp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zyqchsjh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iugjqpof.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixnuczuu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vnghdyvg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oahxkati.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxjzgjxb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vlqdqenb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jfuzdgzq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ubdhrkar.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ffbxiusd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3joncalqj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3llsozlhg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fjlnyhfg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3isfsdboe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hxsyeruz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bfxatvct.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3klowxvch.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cxdcpydc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3enubogvo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3heotciqq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfjosdv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ndcjkfhe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rtjhehwx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wpgmejos.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tccipqzw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zmzsmeio.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jirgyhqk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3iknkrshw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qoetgwps.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kjvgksjf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3myeccajv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bhwtqero.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pslkboyn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jrnrcerp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zfaqqkmj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuzify.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xkpwpcme.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mvnumyrz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3opymdnvt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dixkawrf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pxmcwczp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jfawzzgx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uawskxoy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jgmhfarg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kgcawoot.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3eccvgspr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nvwfjzuv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wvjovicm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yefnskzt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gvedmoun.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaavmkbo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lgouvqqi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rwdanozj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhsysy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3trvkgcuj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yrxbtbjg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3piuqybpv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sbmosxyo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3crxshpen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhnhzoco.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bkrqfbyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuhofifh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3moibwpiu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eabrwygf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bhkpcpdy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xuqmtzpo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ddebbdxw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qbiuayum.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hcbztnrc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xrjhvtae.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jrjzejwr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ucoppjys.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qjxmwyum.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3yoyhikhd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mfccfbau.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3omwervoo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qixojrai.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qbxzswnw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ercrawpn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ydfrxufz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sjcuzffm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gvfyipmj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3woxpzckq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ilweumfn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mlpaszzk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gatvkmmh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jodhaicj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dtqiuqug.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yyhaetff.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hndzgzva.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3llqjzyzi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3krlgzgwj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mipbddqp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gjmwpive.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zmvpemhn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3skeypezw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ymzwssfp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3xbddyrwa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rwdoltte.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3oxsohtvr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gohsprhh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dufcrehm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ecpfhsed.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ntsprysi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3afnekmwy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vpavelic.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dzzadadk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dgpalazk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yvemliea.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lirzneyx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3gwvohzoo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3viibvmen.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dvhetdbd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3agyrqrbs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mncekmwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwszgxyi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fontqzcm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qqjuopry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddgsxibj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ujhtkdjo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dkgcrdwq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gghhswdl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3stznieoh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3upwwhgej.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3upsiwpzw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3nhheiqpq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dlpwgsnj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rokcmufh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3vvnzvwcv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3rsqzzovz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rqknbdcf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ssyfswra.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3laxfiwrm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3yebvsbnm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3tdilvniu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3uviqmjgw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zwnbsbpy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3cuxhgapd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3aipqbwhv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lkigggkx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3drrwhdpt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fflxitsd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ancvaxcp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fycpumye.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkcbfkpr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qsxwbzaz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibcvkgse.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtpcdsda.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oungwgdl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ypihmlnd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nssnjbbx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rjcxakws.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xolsgxju.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mbwwfuzv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruelbfgw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uadspdel.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3kqdkewsu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rruwvwkk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jjexlvcw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3danrzgro.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ilxozfde.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hglfmdvg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fnrrotsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tntvmhif.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3eukzwkeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtqeiyfx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpzoeosz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nuyapfmf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3dktgydio.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3girwblms.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3zvnpqbaf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pwdpdwmo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzapkfs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mtilarwz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3anuezjjj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3klbwiqlw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ecohdhjf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fdrlgppi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ctpaxtab.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mzeioijd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fkbvswao.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3vrpcfhrt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gzznretn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3orgdgfij.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3cnhfpxqc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ppehludq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wrlmasdd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mvukkbbs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3abioxkem.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uwfeifxq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nxyyhdmz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fkwuhqrc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aawbagbp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbypchvv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lecjprth.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3baushuoq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ubwtxred.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uwprekvr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3txeesszw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hbcsuwwp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3dnvzzcsb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gjjcqeec.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gwohrwcj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3szgvdkeh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3evgdnffo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zqygssju.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pqnpuoro.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wlljgbbm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mgrknjfr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lcmdqlwy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pnwmkgsq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gsyiajfr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3njjudnrd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tpnhfzyv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3burxhszo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kafjnyjx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xglvoybc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxpxzyp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wqmzqaid.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3esbxdvdp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pealvgfq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jkvfxwbx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3svqrjncg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3erpvqyem.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lcqhrylx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rxirkxzb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jkbvyuoq.html


<!-- 参考信息 -->