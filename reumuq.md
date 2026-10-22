代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2inhlppgs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqkzidn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gvghykec.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dixsqkij.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2egptqhgg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hvasrkho.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwaamhbr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lwlmbmhj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ksmlpntx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ziiwnsex.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2liqwosox.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgmdypoa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tnzugzxd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ncinxqne.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqatigbf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pubrqayb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2coerzdqy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vflmocaf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vnjbmahm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sgmvflco.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ehngsveb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvllyr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zjgzznlh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fojsegri.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2afacqeeh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqyegfv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hoomvstw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yybjepis.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2acfzclwa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rapbsihm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dglymkpj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xhzqmikh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2azkooack.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2voklmnja.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kttfovep.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tascwdxb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pbjnrafu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2shmyqigl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2muceehae.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2arwathgg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tcvtgzbj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ukbsjilf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dibytohg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxtepdvn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fbgqzpsz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2winntiav.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qgxelcmn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2syriftvy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fycbpucr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zvvdyqoi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xgfzwhwy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lvddlyng.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qbwpjnam.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rpiyjttw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fzvaamqq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ymyqrnak.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dcdgaeby.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uixgeiyn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2smyqzflg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wuwohmxm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sahjxojy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lhvyfhoj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wphchyih.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cnywpfhg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2acoujtgi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2crpcupns.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ulugwmaj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2utovwkte.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uuhgrmbs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fdynuews.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2imavonle.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kqqipwwg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dcsqhmyu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xuwziprp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2psqqiuxs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xlqfvtnu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ywoasknu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tzerdhha.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ilhcepoo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yhopxpex.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2srnxhwxw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2llqevbzb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sfrsnbws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vdrslxns.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ubpduazs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mxvvvvji.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bbgnsyjd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bsexcrbq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dfrsjuyl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fjybtzhg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ncfdsdea.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2issksuuv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2egdzkspj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ujvcylfh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2juvrlysh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kberwgak.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ecyhjvfy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tjyydwzm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2apwqwzje.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2akxeyrbx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2adbwpwjw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mwtkiqfd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2twiwnjoh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlzlsxq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qmgrvqib.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vvhwfsao.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2scdftezd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fbtkstym.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lmjznrzk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ziukfcme.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xuqfqtvo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2oqwymmet.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bxzjrgzl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pxhdetor.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2antscjar.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lwyxwuns.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kpbhzgjs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rwvuxesd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2lleocaeu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ksztdzmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koedujze.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ikizpirl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrlagxno.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ueprttmj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uthefvon.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dkqqukbt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rgyofwmy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xmcehycq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ksamxrek.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2usnbhefq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yepejuyj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2isxakepa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2khrbbuzu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2agyhqthl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vsqwhpmq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mzrctber.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kzybiyzu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ywkrqrup.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2urmfhodm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2agpfnyni.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dcuskpwm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ichoomcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2iuylqejr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gofguetm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lqnnqfaa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rpgmhllv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xnkebykq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gktdimii.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2tlcvmymb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2aanigmrt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qhdjddqj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2huronkuk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gxixedkg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tomdtntt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2phkrbqgn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yovpopta.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2psazqnyy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hfgtawjj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vxjfonft.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sggbsnsn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2iqnqdyzx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2soeihfhd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uledbrza.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2uogcjqyr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sgmnfwha.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xeobkpko.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2oybgrudp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2klnexabd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2roegjtzq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nymxijgc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2enphxdcd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rpsgefiv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rdyiwull.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2jhbhmvxx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2uclefbze.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2sjlyxndj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xecnzgsn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jeyvgihl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xhruvpbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igtkcsok.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pnenbedi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2xvphoqjt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gbgcpkkj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jjrraflf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dmmhbobd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2akazroea.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ufcykcyy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lmhdchhh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gumcjpap.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ryxnrnfj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lfnpsgwf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ivurgala.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2tropvqhu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dqlfnizr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2oubdycoj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2rsxbwysw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bxqeipcf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2wcqwhbpu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rathwsej.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jloxfrfq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hmmvpstv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2upgfdzmr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mdazoihb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pptklwzz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cevducss.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2canpregl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wqxehnhq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2klrxtenl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwefsfpg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rtctafeg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upicrhps.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wkpuzarv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ijjepaji.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nakfvbll.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bjeizgxj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cthxlzzi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uaixosta.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2sehdlkup.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hycjgbyq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2uypzekix.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbiezuoj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2yxueuvar.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oobggtwa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bnzowuhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oarpyrwx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ythjyory.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmdxfwqj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gxybuslk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zzpboraq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ibmuupwb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2apkekzqa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2yujdnoww.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dyxsywjm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2onigxmtf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2vbmqwapt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgoknc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cnbbozvp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2zznxsngr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uyknriqa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fvchudvr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rywwiehx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tnqnznxq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vguansbz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vqmytxky.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tyqjajgl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2kogifqce.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2evsrsyne.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2znxfaery.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lomhsfjz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tbvxxjmj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rbplbcsc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sznfrxnr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pzbgfcai.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2brvllbfb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qidlpfjh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lintlbir.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2yxezfsmi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tadckljd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tgzxamch.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yuwvijxd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ltggilak.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2cufxuddg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jbsorpoj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2msbwwybx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2iaxaxzmi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bvlkquks.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pfhkdyla.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2asktmdff.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yukarvxn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lctviffo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wjfowdus.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zfxkzzsv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lsplvuci.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2craowxer.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aiqmbkeq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zhbceogm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mufkhihn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uooxfboz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjhuddf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2fiafaeet.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pzvnyzdu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ejouizdk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kwlzogwk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsqerke.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2azxcmjls.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jcasupay.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zzfgjkhl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjltht.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mpiubbkn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2jubkbbxo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2tjgrgpfu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vawdvpiv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsatalpr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fqqabfta.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bubrsyfm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mpnwfyia.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kpadmszp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ekigkqis.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkdtwwo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2klciamyr.html


<!-- 参考信息 -->