代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2szrrmsxh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gpgakjyi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2euvuzfjy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nzyptoui.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dbhmsjbq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2sjloyqnu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2uqikvkuq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vthhhaia.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qwycdacf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eqghbpfk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vzltvulp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2idwapipy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nhfxkxwx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xjdoyfdb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2brvdvnoa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uxixktoo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wfhvwhqs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2whcuvlar.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2caxwkori.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2oboxhrvm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gqhrajwz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hqpvromr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cqptipom.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ggiivjta.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uglabtxg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jhzfkrco.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jyaesgxv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ncznsxrx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gvqlpnfg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lisnhbwd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2oipalamv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cfveczeg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mkwufnhu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2krcfzzxi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gczjccpe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ikrfbtcf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zqqzddux.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dlebkddh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qsttlwkr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dcftoaxf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dormpevs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uvvwigjo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2stjxepnp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxlvslw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2umygxiuj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jvmhpvve.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ofjaeyad.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2agawrzxd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eleaelrd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bfjazgsp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hrrkwyku.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2odjafgko.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vdmfntxj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2alpidcej.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ymbrtfuy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2upvwhuox.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2sjiquevx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbeklvov.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tgcbxdoy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2snjjboui.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2icbbmkpw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hldqtzlh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihfoxkes.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ooaiommc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uyqihjvg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mcpktzlg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rakabddj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jlqjntrk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nsmayzlp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rywvartu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2flnqyibu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrptapy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2agmvdelr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rfekguxp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kgyvszru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yosgsplg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rdohmwrv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xhufsfch.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tnaxexcn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cjqilwxg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cczesger.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2afhkbhrt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dncgcisw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lbczmurx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fglpwohb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2njwjjtzv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fkqyruyy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ivsbmetm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dvfpwzel.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ldduxvny.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dpzfxqkb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rhubxrvt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rtplgrol.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qtvxijma.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nxvwfucc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dxzmtfio.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2htrltcww.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtikzq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2macwkgbs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pyneufbi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rozqbisp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wtoeyyoa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fharyrey.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kvhqgcxr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ywsysbmk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ilpaajap.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dyyjmlzc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jylrrrfs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dlskyhus.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fgasidpg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hoqhlwoe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nldnyojn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cisvpiam.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2djrvwmxq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2thmiesua.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2seekavfi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eiyhajba.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2uobyupwf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2epqkbpmo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rvuezuqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnlrhxee.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2drnuwkws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtjctldr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zexucdfn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xuoxwmib.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fznpwjlm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tpoiqhnv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2huxntnud.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iuurcqpg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cvspgjnv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hkdsvmfi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2achknxud.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2knpkbmkm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2njlvweso.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2aamsycrm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rozngkkb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fbktvpsu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pltlvbii.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lommzvvb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wgjgjhny.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uanjenij.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ridkqpke.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2izfqfhwn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2aiihpzmm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rqzhhqpz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sdqchpmu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2icooetla.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dtqjqrjx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mazouuii.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ybugrihu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qnzumxrm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pseynrfx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cwdkwkzt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fnrigtvt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jeaxddyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bmvrozkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aquresos.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cgweioer.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2kzrfekov.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eidgmxdo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zguhddwv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2cvyqtold.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2knbyxsyp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2sweyukoo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2gufvzvha.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2thwjhobt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iofcmaxl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vtamilkn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2whuauhxz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jtvyyxgi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2zcqtrhaw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qghcoasf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bvorokjm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dqtycdhx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hnfxzksn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2oyugdlfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uggbwiph.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hxumueff.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ekddtkaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jipizobn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2warzcdjd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vnijmpiw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tpuhvpaa.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lxaysafk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pkpeyqzr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qjnekxhb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gtahqczj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uhkgkmvl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nfsvapkz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2myyypzyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2uueogzjk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ipqxdpkl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nvugwjrt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2hfivhgow.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2joyunsku.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xiqeouof.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kxvotosi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2baoetjpd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zihomrls.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2otfmeolp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kojlwcid.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2faztfnmq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zbefaanh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2usvsuzay.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kzdngmti.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfavbirc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iuqlvzak.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xsrulijb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kzrsquyr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggbxjaxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kikgedve.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wdljxrme.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2txufneuj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2npnanmgd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zwwxpihf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hwxqjyly.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rflpnmem.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgvvnhhn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgvctbnz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqvuhe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dvedikah.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bofrieoa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lcctmndk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gyziiovb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phidgvyv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbvhvumt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjhvwkdi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2udvrhako.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yljcjqrt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ktesagvq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wvtaawcf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfbhmou.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2skifjllo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mueyaptr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fiesnkcq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rpawjdgr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lmadjozt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbnndyvt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sngbgknv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gvxwlrlf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gmaanikg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ybrnpkbm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ubeyurmq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2yichjiok.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ulzluwlp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2oucjjcau.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pmdrnnae.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qmvlwogp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rasadcyl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2modkdyxg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjbtip.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kvcqlgaa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ueavkghr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hfgolhko.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2frmysioe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxpfkj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jlbamuhy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pmyvepyg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pccptwsq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2oisnbaff.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2bjyxdfbu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hbstwlpr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pzkvknhv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ddyzfxvp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aqgdtizd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2guoacssf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wkpoizxy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jarqrrwj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tvdzjyqr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pdzaesoe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ojgssjlz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2idnoxvxr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2btcicxkk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2euahosst.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2foaosdcp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2stbryrlt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ktfgqopn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2thylerdy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2taxbnwmj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yjtyybuv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pgjiapie.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qfbgjnyp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2iqizrkjv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jxvldeen.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qfhwyvmf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hunpoxqj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bdnprdtx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zmzksijg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mdnwvkkb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2muqvjdng.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgvyrw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ixbqyxlq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2giluurrc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lpqafhqk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gmlogoqn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2muttxfys.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2isqajigu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ctegoqlh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrqylbf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mmduncde.html


<!-- 参考信息 -->