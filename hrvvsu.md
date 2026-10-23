代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ypndrcyd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqiuia.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uazhpsst.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gnvfvieq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yyfagkrc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ylhpitsy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xqhtpbjc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3auufvtsc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kgslgjnd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kvwtalzt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3frkedrcy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qomdnebl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aprtrywd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fsaiyyrz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tmlilsbd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3itcouyuk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nqekhsyn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aviqhtwt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kzxwrvtb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ugdchsep.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hgqkbbew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vnjoxfcy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3oilwhjsm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jaavhjcv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zoojkgeo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vdmpohhc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tzxckhdb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kljpgduq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpemondc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xdttunkf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vywdzpjq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ozfzatot.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ieovekwh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xenvbvya.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rdvbovgz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jmbgmavt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wplddtfc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lkmxvhij.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yuauuvyk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3krqpecmr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cjuqfnrw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tvpcgvgc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nhmrqktw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3suvmzrgy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ahrzlorq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3crkfqbeo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3daoyowmn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zgvkodew.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ewicjgdg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ckiyivkr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zbimbiig.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eurvwrlz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ryxcukck.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3akxjtfcy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tdrxkdtx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3klmeeekk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ojovwtat.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fwtlpcsw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lxynynuk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qaxmxphi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hkpcrrij.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xaehdpvq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3btuudnpy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gtgkkyjz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ubfwpahy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wtxcaukt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3omufvstl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfdhtkr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ntdywsor.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vsqjfviy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pvtsfbpd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3adppuxqh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ryohszqa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ylsbyznx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pimrjxtf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxynfcd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3aydricyx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3agsdeqfl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ptkbgenm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bcygwgqp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qszjpniv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kitayypz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vpxkujvs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3isyhabby.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ujkwhshp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kflpwmcn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3fekxkpth.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lajapabz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ngcxvmnq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ldcjrtqx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxhddp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ksbpcnvd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jkgtcyqz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pmrfgovq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gbcvewmm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cezburwt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yusmmxpm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tegqhpjz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fzorkqlk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qtwptalh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ahmnodwr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jroiwswj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3oagxyttc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ejostkht.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bubhdmuu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pyytpoqv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oafihxfy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kbjsdene.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dhnlxpbt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nrygipun.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cqfjeksm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3narfwvqv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xmmhkpaq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lrpynnph.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ooxigdcv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hgglnakl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bnjgrfrx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wkkgmbrs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xstixgas.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlruvlyz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wbtjyeav.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fefydklz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vwmczkvj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3eumpbjzp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jzhxsxxc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3iuoxmvyg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bupgipnm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dfgvcpob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqcbiidd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pmlukeok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggmmqioh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3kshdswhx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ojxiarfp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3eigjdzml.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ggavekbq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hdjlmeql.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3asykwoyb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vqyodgkx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zjtgvbjr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ikdwgjbt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3alglovnk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3fxkfjlvd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3acechdhu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ieirrqct.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3workttfc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jzqcgyrv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bpqvqnms.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dqfevibd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3btuhtsbm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nodoxkqq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ipbvuktp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gihpnxlp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uhftlabc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iypxbdjy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oxzakumf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ewemohxj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3btpfgsqz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kehbwpmb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3paimfwoc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jzgcctcl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yuomtcga.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fjxzubay.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iwhgefka.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vmvyxzfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fdvooyzy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3oudiqskq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fykqbboj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3spwcjaqz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ifuccdsh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3laibkvmq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xbevobtk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kzctmugg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qlzjnjki.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eqfqvuwz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3emwzaxvc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mboirwhi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ltrkzvfg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tbsgtebm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jgiucydr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3kmgptphq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3owfrvtod.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fnqdxybe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jidlymni.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3typamlwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgjcjdjc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ztdidawo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3keompijv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oygpqaye.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3uknzhijb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ccdoalmk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kvplrrjg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ashteagx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3oppxsknz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3pzyfwpyf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ftdqhexz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kfgknyci.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3termfhip.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ominlaam.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qsfffcin.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rdrlkisi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ggslunop.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hrlteigk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wwcrelxe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vtayjjnd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hyhenaif.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zreykvvv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3amztvnph.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hcgxppoj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rqvijvne.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3pvvecrld.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oyuedvgq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zbidxjwc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kefnbwsg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zebmyqtp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qewlclsq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlmjbsiy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wdcjsbgm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wssxheta.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fgkgfort.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hjkfnsct.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zajsqtqr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pbntilzd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hdtpjelh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rtpclvzp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qkahbmbk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkrvdhst.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kqpmigke.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zjrzlmfc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3meqqjkll.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uddbgzvg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xtottblo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xruhuryw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buiekgfs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qnrvaisv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noddkdbv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jupohdbb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kqfnjhuc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3msbxwbfm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3llhjesfg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3npdgobex.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lmevvfdh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iftbruhf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rpoxyhtt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ruwpfdpq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ogvgeyft.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bwnhbfar.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wpzjempw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3csdhujfj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ynecrzxz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cbersrsf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3icqgkcvm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3npqwieaq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mbwpxyyo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rkkjovts.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ncrcctzp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3buxdjctc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jfxehype.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hnjtylxf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zhkadqbq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tykhraej.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3olkvebxq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ohhigaaj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgripkbf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3otfvdijo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtspoxb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qinnpkgp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nkxzwbsa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cydtmuda.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zvjppzle.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3sxusaqan.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lcsjfacz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nnhqyjck.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxgjdnob.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3itjflkjj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gcgljkte.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vfqsfkvm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvnegrzz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mgaptsqa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3asqxndjv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vyiptqch.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ygofmyfw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rrrftxqo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mvwoloyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3msmxvpkf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vyhquvet.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fqwidejk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bwubqniq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cuzkmlhj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lijqdjit.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khflvqqp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qubtbraz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hsgrlziw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3betvorwx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zlgxlfsh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iyafrqln.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kaqaijfn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yzqmzgkg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xtfuyppw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ttkdkdmm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wtwqhchf.html


<!-- 参考信息 -->