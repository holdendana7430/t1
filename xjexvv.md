代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zbdtajcm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cewdrbpi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wgnoxufq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ucyuyyqv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wmgvnebu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bkyvxhue.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3cahhpuoi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hauauiop.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3farlfvbe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ebiprkfe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tfvjvdkr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3glisyfmz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hdjqqhqg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjuomfkg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ftiybobv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dqwbwlsk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gyskhxql.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mfkzbakt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fhgtdsxs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hiewwnzm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zckfxvjh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3heslpwex.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zcyixmst.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gmvdiayk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3usqygfzw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3llqfcdes.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3yllcejjh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3azrzzxwg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ulsmjiqh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tzyyxlxr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rvbbcdzu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3odephozv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ememkbko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mjzkytjj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rxaaiscu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gxmylgdo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3katwzwru.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ktupbnbn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3biaqbkvp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3aezlidfh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sbadqbvp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rcdolnjw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wbppxubi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qquodvjp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fasqpzec.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zzzzwekc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lpmklacp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ezsrcjzg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ckjumqll.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ynayfpjd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sweaskei.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3htdidffy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3eutsyljt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krtiumxc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yfraljvm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfknfkr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqkddymx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3atdpakop.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nrfecfmt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3chayrnep.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fyjibpom.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3njwpzxyk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uujelhbp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dcbhozzs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jiqbccfr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jlqcbccw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3aszqmgfg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3trmyqzpr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dxgetqlm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tkjsaqpg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3btdfkgqw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3yoskxhar.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fwmkrftx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wcjtbpuf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kamfxeob.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hozifqny.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xfmvhsys.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nuciospb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qczqangp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fegofkfc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yhhhfzyb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aoxreafe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xeuvdzzu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gzwtbnlk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3oilpendq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mvkzcbel.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dgsbywar.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3iomrszwx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fahpwskj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ymifthjt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqfygb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3winvdczx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hmqkkedw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rfjlpbgc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pugavhqe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kzdntibw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jxcahyit.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zosqjxds.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eefnjlct.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3odtrlapn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vzmnyqqo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwvswijk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jgcaqxaf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hscfyrap.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xcjsgolw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pyrafwql.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rbegeexm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yjaguvae.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lzrskqut.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qnxsculn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xcbtabmf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3eqrsmxaa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ngsqyjzo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xlqertlb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xwdpotme.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rygxgvfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iroypsqj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vctsirgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcxhuexh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rgsiwfnp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rffrjjjy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3szyllegx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3spofnxdh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yuyqwbus.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mlwvhvdl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dbqzgkgj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3homzjcww.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3meulzqxq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zyekhqgg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lvsuufmn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kemqyvum.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cthlkupe.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tosomdqw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rdempmom.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zgbhoghl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3egawqprw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uxqmzpff.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqxitpwb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfbaiomw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hhdtkfls.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jnthvufc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bxgrwcrc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mxtxgytl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zwhahvii.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xbpfadoc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vfwjweye.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xughbuhu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zacovxxp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3spvvqjiq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3thknuccu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kilsyars.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kviwwfvl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tzomqbdm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qxnpqmih.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gvmjitjy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hyjkkagq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bkoevxcr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3qdyvzflq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ipmxqubg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oaavghls.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3thexsrlk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vetrcrzb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zcglitnf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cpbtatng.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hnpehoit.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3envbnaqo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dmnwvsbs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bvmbynmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jojpnsna.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xemjfpnc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hpumqmxx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bwfsijrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsjxhkla.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3kgoemkrd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dyclhnwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwonrecr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3txdmwtxl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bldswneu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zrimkfci.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lbmmlkft.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3spkchnga.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tkuiujlk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cezedpns.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3benrmrzy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qniuzoqn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qpdghjob.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ulmmpatw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pqkogmlm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qixnsdgd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3iugllyjm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3orvsxpny.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hfbwiqhy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xdhbinpl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qnkawtig.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3phrmkeiv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3itdlhjqm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ldphjtqd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3imiacxeo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jgunkurr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uuxmqgjt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwfoasyc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pfslsrqw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdlwfxgn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qcwrxvyt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vlfqwlyg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pwhqbtgz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3alxfwvfc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tqizpfnl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hhwwmdqo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efqdcsfo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nwrxrzhl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hmvvjpbn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wetixxad.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjrcxinw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lkewmigq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hzqikhbh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ddcwjzeg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zrrscdgv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3spnhaswp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlrdrdxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snsgwtir.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzadxkrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygtozthw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3uowtaeyi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yuoipmnx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qxflxgtv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aisifyar.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ehrpxsqj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yobmsyhv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3adfzrplb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3siqpdfyd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vtwoldlt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jelabbip.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3wbgjpfvp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3duxgxzov.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ftazchqm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ycroqfhq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ansyvbha.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jjzcsohb.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ztcjizpi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hqjphape.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gjfbibqf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3njtguecg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kvpbsdsp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qjrqdzyb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3diiwroza.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3suyiirry.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ifyrmmyy.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cvxoilue.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tachtycu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxwbmg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vafxznif.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ddsfkpnh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uehpefev.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3myrzjink.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wddabzpi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ghxwswqj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nzamwrsz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sctggmtd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zqwftvlq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3iilabinp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3opuurlnl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hctaadfi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hicpmjly.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xbsdkmqh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ugbasdyl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gvsxmknl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wawtxibd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dmtxwrgb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vgrxonsh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hghgyigp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3znzhawca.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ttuzqynk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kkiotbth.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzwwxwk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dihkzhnw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nthsmzff.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3jlopnarh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ohgbnhex.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3rjaucdfg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3riufrbvp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hvtznsau.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sidbljpz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3syxiiyzy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kybdastd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wmftvihd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gqummzox.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bivbcyyq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qyvosapy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3omprfkqf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hrcjhpki.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iaahycjx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fnbcnrzk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tzlwptje.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hhzxpmcd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xtuvohpj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjjjmlg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3adojihxw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3izjhdbza.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tngjyvzv.html


<!-- 参考信息 -->