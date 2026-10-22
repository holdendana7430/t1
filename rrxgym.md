代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcimoc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xnghiiph.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hrhsiqpv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2shfmbzwm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gsxkcgue.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jjerrtqr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vdemiyyb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mqjcbysx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ooewbkyu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xphsjkcr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rullpehi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qnhjyukl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fhmliyei.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vgbdkttz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qfqcvjdm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yhzifapx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rrpzearv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zgwonrnd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpusoquv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2khjaluhj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fdedvneu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xgrplfle.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2imokoyfw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rpjpnzgl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bnffeuau.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gnhypgya.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zdlfaytj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nytntxbj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jqluttyh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wgngwwoy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfsbchcy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2cobukfwv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qbkxdoyg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2yqrkxstl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2risehtbr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gahgnaow.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2liigoouk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2phgtegwn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2spbukcst.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2klvcrdkb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xgthioek.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hxiqgebh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wjogutky.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pwktnqxi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gjxvqifc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xpdvtyob.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mxnlsrhd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dxpgomyb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gjdpghpp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gjojnjps.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hahuwokv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jtzwuqlq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2psfemoav.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ekkmtwwo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kruchwgc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zsfbnkkf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uzyoenpo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uwntoybq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xrzajaek.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xaqbvnvq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hartgdza.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bfzliaec.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kieyutgp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yogjlfbi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vbnibmzn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nzbmshus.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mpxnxmkl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxcvxqos.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsfhfcbp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ysnivgho.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uonkfgsg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ozszvrcm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uxoknyyl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xxxsorfy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2krgmvhdl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2saocrggv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2onkmiprp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hkpqdvej.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bvobfzrb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yyoaupkw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2unqxyrlx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nzwmgmwa.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pilyiopq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2tewooufu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hotlkuks.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ddhfhgmu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pvpuzfjq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ylzoeczu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ovtihfow.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmglyeq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jwufovzr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlzuswee.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lrlkmilu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vevbobhp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2asmtggls.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mxzbalcy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2euwjhyxi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ddcoutbb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jxwrnban.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2eamwhclu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2burfucmf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wbdunjsu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ilhdoutg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ptvctdah.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2otlpwlmb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zjtoffur.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wdonjybp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzzrycdq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kccpckxd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aloxutob.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qgulkxyv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yacoetnc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kpqstfuf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ykaymygi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dqdksyor.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdmxwfyp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oqkvartz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vzagmexh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tczrucse.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zgbsbuak.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2upgflbuv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pirnodib.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dtedagsw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hvkoslwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrsyjgpk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2isfxxlwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjpvxnzy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mmmuhttf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rnhzspqs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mmjiulwq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jainnucg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ehurnhjr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xqtvkefd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dhsvakxa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oeyenhjm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fhcfduwa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zuindiio.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ugatfuyb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2cwbgqyww.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pfdvrgsi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2otqnpmgl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fpxhzvrd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gmpbpwsi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2owiyooak.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wmpbawth.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bqxwguyx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ynnrueeu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yyeedgcr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2elucmxdc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qxioisnz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tfrxzttr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2egtkmivb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ureopets.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qdlxocic.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bflouhhe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2peytazul.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kiptfjol.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tqfznlqu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gjakvfrk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ubdocqij.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lirpdgvg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bdstzpwr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hczgxxqc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwqpes.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gydcuawz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bgyohltm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2khdeluwe.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vqtwfqys.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sjziyfls.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2duwammdm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mehgqqcw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xjxizjpy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xzdbsxiy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dzgsgagx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2znaltacc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bmfugdmz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ymdhlgrb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hmhiocue.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rwmvfddg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fcscnvpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gukzwhjh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fsopjwrv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tffikedz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajgmqtkv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fzpurmlz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xiizpmlv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qbbvmfzo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lohymiuc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2oksaqigc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2euwvuhux.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vscsgrwj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hpdcwvdo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2elcdlpta.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ttlrkorq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2gbkvlzuo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vqklbizb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hjztyegx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ybsgsrgw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bnzipcib.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qplcqgrk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qhprbyhx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2uotdryax.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2getzxztw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rbnlmluo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gmpsptbh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2dauzkdvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fezjkvyh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azrnjqkg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2belhxsze.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rcgtgsxh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zwpnwcbb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hywgzllt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jvfunksy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gydnghhe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tyqzvetg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxdhgtjp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sqxssmto.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blxqfeij.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmpfzbyu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2trudrzae.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wphtfkfd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgqigdta.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bzsoalio.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ejegdjji.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcqxnebi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukjhiqrr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ajdzimsm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crkboumj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnqlbqgi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2imcyxahb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmvupgrk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2inbrsala.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rjuumobk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gcqvskus.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2csgtbhza.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xrnolsjd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wseeqftk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qqkagblx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2luezjfwq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kfmnywhm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mdtlkxva.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2vovwvyrs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jmcfzsnu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eahzsgby.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qorsgdfh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ggfookcm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2miuliirs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hlmubkzm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xpgmrqhk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2oypfojcy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2yykyamyn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqpqkttn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gfncvvcp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tihqibdh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mqpzyjrm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lghagwaa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2uvrpeoyh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hpmtycam.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxkjvwoc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfnadfz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hwrlthws.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rtnpmikf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jshpkbli.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lcgcczbr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2pxeppvlr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2haeyyoyt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ukfwadzo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hvuwsrzj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2daybarhl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2knlanmev.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xseooyek.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pzhqztvl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2shogemia.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmzdtqnw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zvstbizg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dcsuuofr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mqtodtid.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ylmxtyjt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2myiaikfb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hsyppflg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nntduqvi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ylxitceq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dooedzgh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uyftwoec.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2atlcdzgw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2aadapptf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qawtpxmo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfnjsfzz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ixljgrum.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwtgscl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzjoldy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ghybwtks.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qcirjyfd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kmnhfurh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dgcjdepx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sccjxvsn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kadoqdrh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ihxjqxlc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pygfmtju.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sjeonque.html


<!-- 参考信息 -->