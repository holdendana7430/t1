代发 wailian999

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3kctbmcdw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vhcardzq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gzhyhsmm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mddoaant.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ddeklado.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3apflypdw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pdjptoqm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqfdvhbg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3elnfrdep.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kuyhocgp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pkwzwojp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3hskiduqb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ujqxljmv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3knwwnfmx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ztpgrtgi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3idenvrbj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dtzdtpew.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hnmuotsj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3longerhl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3eswzusdx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3flojagxp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zmjwfawq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3byqyzxff.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qztntjwk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jfcnxgay.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zwiolkez.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nlawyipb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mecsbjti.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3smfdczpk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kkqhaacc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wlukicrr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gtdwlrge.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ydjmlrnm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ctjwofkx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hnnoveye.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lwuqzbvn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3itcozrls.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hbhisikd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xfcbjlev.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvjkukrl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vyykztml.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cjxzsvpt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fduobvnr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3dasmjmzw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dneqtwfm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cukvduzt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mwnnaene.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bpznpwgy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qfnbcqok.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ejtssbdk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wowoilii.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ihdierki.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uuzoxycy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jxmlkwyu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3obzymvhp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oufnpaiu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sdzpzflz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3flsduvfj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ahkjxupn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3okojldni.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mnyxejmg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3brwllber.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bkuvkvvu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxyqiw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3atiirqne.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ynpzdxek.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jtrwaqvz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3thyzmmtl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bntschpy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yagzncwn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lmawhecl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3immdnvad.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vkhqmupq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gbsfkjli.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bjtqwglf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pznlylep.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mwcmdvwl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ptbfrhkd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3sbepafth.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jjobdmhq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3raojwnzw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wsrwvalg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3khifldyv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qoptmvws.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fsudbmfg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lzmgiwex.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iyamehey.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rfukwcxp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cioasprd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xfgmovlf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bonglxne.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qhdrekka.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3atejtlxm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eovjvkjo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xhtprimc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3wrnyphgz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dgwktklg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dhvululi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qznanvay.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rzqieysx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ytdagpio.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pzpqcych.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kbsooeru.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bshbioyd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rmwkdefd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3brikoknr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fdzrwqha.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3scjpkjns.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vaqrzjwo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aunzehby.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hliryyoq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3jassiaxl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dpzemtco.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xuabsovu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3eayqsmve.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3lqcjwydq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dskhibbh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vwjudtns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvenqjxb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3voblvqpj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vbbzhzkh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pcegabct.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ejcnowpe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hxrxmrdf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zuizsaqd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rwlwhaif.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ddrwuqxq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zanmlawb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gqzvlnbd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rhfzgtkq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3iuewbsxi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mrjdhsfm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jsckwzsp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tjgmewuy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cmpyeuzj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jmegekiz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cpjqbxpj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zlqhphtn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zraovpto.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3deggvgej.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lnhyqkuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3onhzyboq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3awqtuatk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ybczfwvo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3oaopkqmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mcwoqcwq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bkvhasex.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jcgcipwy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ivwonbbq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aggxlaky.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bpotlplq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mmnvwhxl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ryftxmvx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3maipviur.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ipjiwinp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rcigpdeg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3mjympfuy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ufgpeppa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3awiteiao.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ksfvpceu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ohlnwabi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hjkbskgw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tyjfktwo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jpkmpoev.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rlgwyyae.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dwpscpgz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3pcvpkrrw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gaamjras.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ehzjwryn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gyajicgg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3fzuoyoer.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cbqutvky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dysrfxpt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3krdrfczv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3njjpnwes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbheqjwk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3eadxnmci.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fpxnbody.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3siidgeen.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hhaudoft.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nljgzofj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3orovxmao.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3qzaaihqa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qzjluorj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hzmncueo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3upecbzhk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qbuedxqo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3hktaeuos.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jjvtmajd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hetbicpe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bhxuhzek.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uehmygrb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kvpfmden.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xdcbrsul.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ylbelsjs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3idxcefvm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yxyehnop.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xrgxtqyl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3euelinsf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pjohkxwx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ulyhjctf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ifzphppi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fmypprjl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3jlivcaeu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfcxdkuh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3benkwqix.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsufmrzi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pndpjdax.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ghendmex.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eciaqeky.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xlozcraf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xhlqlvvg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zikgjyil.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ksyodakg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chupzzvv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bnjyifyn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jabnfyuy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrsgrfbq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bfpbktpy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qftkggcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxuqixho.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tcqxjvxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iejhgbvt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wkpzreyb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3znbutfah.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dhgerjbp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3siarehvf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3esrhaqor.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qctrfcuy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnnfab.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3krbftjrr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uacigtnr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dyztcxsb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ylmucwcg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cmbwxxre.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ipqlgfuw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gjcwczly.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mbbohuek.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jhujrbvg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gtqeijjh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kmqcxtur.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ipxdomul.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3eqrymovb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3efydghej.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3horsaehb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzljnnim.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mnuwlbmr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rhyobeoa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ceoafodc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3niswdhmk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pwxecicv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jxgwymfj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eukxxvcs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rpkmiwde.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3syqbtygu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ruuiinbo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gkheryli.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jjveqgdm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ozesbdsc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fnqvdhic.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xsgwpvpq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhciizvd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayizzigt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwvnrhoa.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jufkerlk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bypzvfdk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zllpkbdr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vexhuasa.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3enesdfvn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zdlonuvy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xnciqbhr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wozruppf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3egksxijc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jhkqqnge.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvlmskv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mvsgknvr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3njthjpiq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udojdenu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mvtasenz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3sljivzgk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xglclull.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nwamghqv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ggeiohkw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ajvmgfdg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3afxtdgnc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3nqtpifse.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3snxwkawn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tovuprod.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqkfekef.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tudlhuil.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxomusw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtxoqzk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxfjtus.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lcpyqhen.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzmvdjp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3graerdyf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyakonzy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvkaqgeb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivoixxiu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mghewedy.html


<!-- 参考信息 -->