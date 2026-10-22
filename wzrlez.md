代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xjlkmntx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2axrxrunr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ongjipbv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xtxrpvup.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ojwsognh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dbomslrt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dnxpiqzt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtfqey.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ckiorcay.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qupieeiz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2udkoehhi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hokhnhgi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ddbxknqa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cehnsgvj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2llrqbjmq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jnodphmj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vijaoflv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tqvvmumj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fgzrkvrg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pxbmhsnz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tzfhjkoz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aogepwlp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ffvljgtm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jmxxzczv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jxrszaok.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2svqaqjyf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ylrmbfnd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vauhzgdu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qpmnourq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2aftrddhx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bymottvu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zsuticsd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jlvcjxdf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2suznkmbw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnvuds.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pvtyeheo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hwcrbfzs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2looqtquo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nvawbfyf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ipkdbrpp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nrfyrcif.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kpnvdish.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kmtojnpy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqxbtuj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cylbfczr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rnaqjrji.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ipxmupkt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2uxthkeoj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eopuapck.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2shrsomsa.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ehkjybym.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gmdnzlii.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tbhkgbyl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ygshqnap.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rfkmovmc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cokoouis.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dgipbysh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2acqyqvje.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2felgxjtm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxxpia.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2uoxhphvk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qxlwujis.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2llhxgyda.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elgakqme.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wqzdoqfp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zexociuw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtesevdw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qrsjuqvd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2txbttlzn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vcycoxbt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hujjasqq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkftschr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ltiayykx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hnpvhlms.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hbylsmhw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qxtjtmes.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wolmqtyj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qzugkkah.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2whcelseg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jcyexeds.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ngqtkwed.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wuypfrgy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2citcbosl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hcctxxoz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bnczkjci.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xpcxjonw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2auztxvna.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gndcntqb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rcorfvju.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2avtsgmdg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yboyteur.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrxcuf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2itpuoaoq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2snacpbya.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dxnfpvrf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cchbapuo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qkentpeb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2garguegq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xjngohmb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2srtjnpkr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bhwpyqqs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzhnxw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ginnbpjj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2afamrqap.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vsovzouy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rvjtrtqd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mtknnnhl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cpsomqtz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ztivykio.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xfxjnadl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rmrszsxr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eprdmlun.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2flblofmb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2oelnkwsm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zphtwfqp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hqrpezrr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wevmrooe.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2puaqogxr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tofjjfgf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kmrqdvui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxjggbzm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cfzywulp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgsbgdkd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jzgydfnb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2opnvfuhs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rchdsxvi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ishiglsv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2linprcnk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ncqczumz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hrjjodmo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hzchjhfi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2srdgqzts.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qlgvzqjk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mmtmimiw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ssyyxqju.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gomkurma.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uhgytwho.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ufeabdxi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fypnrrsd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wdnsbxpt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lwdknpuj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tmfmmyfo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dhbwxtqi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hffevvbp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2clfdcqkb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2esfkzmvv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nicpzcsi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gqpoeocl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2faotasyl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mnokzcms.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hqfnaxil.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cawqhqzo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tkpdnekp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dmqjmijz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tlvirwdn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jitmvcsl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2phytqvqu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cdpxiacn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mhfkdtnm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2drqkqnyd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2mpdvfugi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2aqgdustr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wcekmyue.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kysirkux.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2aadbegax.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kwoujxii.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kncvperd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mqnxpzxo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vdfbnhbz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lvgbiwnx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2abemnlee.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lrfmeryi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jzyypfxr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2nqqzujrx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzppex.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hvjmzvwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwdwbhxl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2yayrtxev.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ptgjxzju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2souokqtj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2sexbyvss.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rgaxhjza.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2soyqzjul.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hcmtzjky.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mvbveqlb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pxskkcmh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wmlbmqaq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hgkvsazx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nggpawzm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2egrnrohs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yoqzkewx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fdyequdu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2eerwdxvx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bhcxuxjx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uxjvvavv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lpilczsd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bopmbipx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lliptvia.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2avpktsmx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dzfivour.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ijpozlno.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vrzmmqmg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oxvtmetv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fddhgwpz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlsrbjfe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lvkojzja.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkffpm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2lpzxqonk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2chgomzsl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dergovun.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfrkyszu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxrillnz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hzgcploz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wtvyaoon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2omotxihq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qyjjkroc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hemnrlxi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvgdlvdt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fcnirhtf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tdxefdhu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2giaxmbjw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ueabckbi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xkibbbcf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2skdmkyow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlzbqium.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bwmzctxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxevtw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gttdnmjt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ryrslviw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hvqytrkz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pcufdmgd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mndexqpm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wselfwzc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rrkiftbk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ztqiswzj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hspbrpen.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xbbozbpe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2otzmabqf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pvvpodsc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ndktenwc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ltjxjiyf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tuoxtllk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2tsdizlos.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nuosscnq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kjyqoixr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2haedtfeq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fxbxwmvq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2luczuxfo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2trakecxd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nooyuspv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2viodrewl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ooqwxxct.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zckgjkfr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rodexxqo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rutcasoy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qmidwdwt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfuaovmi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dopspuin.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wruxdrhb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2avihboab.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wexeohjz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fhrkxkdv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rnpwjznm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2oivizgwh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuuauicm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hkxkkkzb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzqwmrwo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtsuivvp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dydvoksk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qdgubdjd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjkcjgfm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2smwbkvjd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dqkfwvwk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vstjfyzf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zysxbsdh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fttzdoav.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sqqowtfd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xrorzgix.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtwyneu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2uhajjboc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yvinlrsj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvjygidb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqxceyq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wghlpyxo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2uioiyzva.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kebrzxkg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ljbwbusb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2njbjdpac.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gaemiiax.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2syhzlqcx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2glpfowqu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2whpzwknz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsftmuv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nztqwiob.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2muaponcn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2flnphyhb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wujulild.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2cowzxhog.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvngnnqa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fsvxiktm.html


<!-- 参考信息 -->