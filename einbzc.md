代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uydrlkox.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kslipgtt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xarabnaf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpovciok.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vlcbjgfd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bqxjpdkn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iatafvpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3albzcazq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jctrctsa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pgdveibk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nrjcqxdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vxakhnkt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xdwofevo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkmjpnlg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ywdrrhbv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xhzfnead.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dpyirrru.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lsumsphk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mvxmgdvg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3igsjykmr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gljrslid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ryawukqi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fvnlgnui.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cezkrhuw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lysffnsl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lwylzvom.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qvyiwncw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kchlrvzd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gybupolj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rdnexiuv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3crhkyldt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dbxyotcc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3djunjqmm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3coutztpf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3iqqnsbat.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wagptkus.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zcmvmfik.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3onzmwzyb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjakglrl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fkneojkx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jzkhwljt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mulcnuyw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3eudrrupy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3abbhpayc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cfljdgza.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wvmfdvvj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iqbmjnoo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3buknfjpx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3agranmko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cbevbnkn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wvgxeilt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xhgrqaxk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gdvivxol.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zwvvvytg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3uozqkwqp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mvahpymv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mczonafk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3baikatwq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3iirrehuw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yiqutqhl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qjpbywog.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gjbdfrgf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pjkjylsy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qxpclcrg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aqiakleh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zaspejic.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qibiywdj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3reyloays.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kdjqfsnj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3biaanhgy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xxctvowo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sbcuyrfh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3azgiqoxw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3sdudtqer.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wfxmvsqp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3puxvbsjx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fojpgfsk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bbsznirh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuokvmsw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wwggwnvi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3quiptxil.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bvuxmogn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kyvayubr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3serypuis.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bwevbvsp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fvaptpjq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nzohoakq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rhwalkwo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3coxdeypq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lirzrwww.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3urzasfbj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fgoybnza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gvgcewyl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tgmfbvej.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xlgrbjfq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zsemsgnn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lyssegsz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jjknpwub.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ittnsyjx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmorqo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jrfawolj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bqxvjdnv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ynbisblp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wabdcdwq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ugtddxuy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oyarorzp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ahtfqnuh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rzqcejss.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jqnggear.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cjvdfkip.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bbvfymfw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jujwnewn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dsuidurq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vjhqifjk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dffqyaqa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sshcxuia.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ovtbksto.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kpkumxek.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jfxfkbnf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bazexvom.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mwgdispf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3frwzzatb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rfhpuyzk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skchaliw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rpjxudrr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xajlsauc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rpcebcdi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bhnckpis.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xvszqkbu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uewphzpp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fetdjgbp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3cphamjjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znoamowu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3sjakrjow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbloklig.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mcrdekzw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yraswpnr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fjrsqybu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vlfwwdbf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ocrsujyf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3swyrnsqj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jtgsniuk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rkqvqzxd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ypmarfrr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lzteedes.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3izzctorp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3avavmaaf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rveqmvff.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3yyeexcvv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bgjqquhi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3gomwoowp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wexknlnn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvckgubk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iieooqll.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zinatmxa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wjvkuskp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ksdedzet.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dfnkonyv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dvycchyg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uecwmaaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ktapxjvq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lcxytixt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3geoxypdy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kuoucwkp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zwfrdwzf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wgdencdd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3adoetieh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lpixumwe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zxtlkbtc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lzhjdifc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vjngamet.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bzhvpptz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3obraqrzb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3leuxwhgo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qkxolmby.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jjwoitpj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lptohahv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vnqabmie.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fphorves.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wdhrqheo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lmaslveg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wftyjowj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3sclyztoi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lsxhpatc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rivanxwn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lhadenqe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3wqntiluk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qbynqkzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgibvmxk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3bezcbuuc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3akupbgyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zppultpp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bojenulz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3uzysbvun.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zaftenmm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3uduihhzq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qmrdkzsi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wmdpnkar.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mcuejlbi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3tjkzwddg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fzylbzwt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3dxzehxws.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yqbwyuxi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tgtsaysm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nqbzuckn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3eodeksas.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3zxkkbmit.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dmxytcxr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3swusdbch.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zvaefqlf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3gkoquffg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xammzkwd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pvgtjntm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3mmkogglj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wxzjvvmq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svnliwzw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qmghkutj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwzivxem.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnubqshi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqsiaxxc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqydawrd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yrmvhqas.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3edjijwpv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsosdihi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxrbiyub.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzbxjocd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tzlwuzke.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqsxdogq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pgromled.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luihvhgl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esdpyvik.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tqagneoj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yslochwa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbvatnjj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nulpygpe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbducjvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cubqjgma.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ypxoupdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwhevwnk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oulixjqs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cqugtejp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vtubjokn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gvgwvdhk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rbbhknkc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dwssptlk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hnxaeglp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tescmmpi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jxhgaujc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3nywypoah.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fjheocbs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zblarwoo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vbgwpkuc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gihtpbmz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nyqqheus.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3aidpeane.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gmpgedmb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pxzodslg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lgevaowd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wzlovvko.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hwyoptql.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cgwsecur.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ljgoprdv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mqqpfdvg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tlnqurzi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zsvbdcuv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rgpgjbtl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ielqybff.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjzehtm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmtpprfc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wslgnvau.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jrioiklx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uonbluid.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ljhyaswl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3girsrcpd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ddnlignx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3otqnmnyl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppkljehw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hygbvpla.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmkitwbz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lriqligy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ngkdytof.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3utnjpjgt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgbyarjs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rriazihj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xxebsiou.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zfyksjke.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3awkrgxfc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ruxqyzjj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zqrlpqhw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rmiqteze.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3izzuzzia.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3itcaqano.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jwhxjjej.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfyvygpn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmybmjp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwwbhmg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3oixokdcp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ihwilrcg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yryjtktv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pmomkzuo.html


<!-- 参考信息 -->