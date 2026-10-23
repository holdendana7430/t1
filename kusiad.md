代发 wailian999

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ncgqtkkz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cifkvtaj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3illmwkqk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vktawwkq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nlpsdpfm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xkufkuss.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fulysurq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3laoesfvq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3emmomyxu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivrvhpmz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fkvonqun.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3blbaonhv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kwqbrrip.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vdoafjfw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3epmonycv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rxjdkuwn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qaihebfw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nweewurv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xrzhkzyy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yjadstjq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3olcilfri.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wsmdlqua.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dkjgtbmp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lwqgiivs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fyhehste.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3woutgslq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rsdjqpsp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mgfbxeee.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wprmxdmc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3umbjewrz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qnelfeif.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wkrrytar.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mhqdvzlf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jnlimrvl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3klothqle.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxkplz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eknntjlh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3layrnfit.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kfrfmzhw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rqivkxwq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kspnuyzb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rfebqmml.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zvjkhuhe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3whnuqbhs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3svzibald.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3eamafxge.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pskxuwlj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3awxlbbzq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3awxlewiy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3waxvzddm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3dboaolgq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qxjuubvq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iiozjlfm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lsxzvvfr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ykrvlqnx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqszngrk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bqqgkpnm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ckmsbkwc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eecpdljf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wkbhjshr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zqyjtlis.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ttrklmpe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hikbgsqg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbnrpal.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mymcjcsf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3feopxiew.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ayxordmt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3skkmgecf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aahgitne.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3emqkewxy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3swwthfph.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3suneaxks.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vjiujboj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ntbadrxh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tofallqm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cmgwkbji.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3wcyzccwo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kfhlyukb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lvkzrubw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kyicrabu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3drlgaqlv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ovhuqmwt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wctmclyf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zrfphiwl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bwdmrhzs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzhsdgg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3blmcgkye.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bfpvutda.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3yyptjeii.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dgkowbru.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jjtdywxk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vciisesb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jbshxtal.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zginruah.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zvjwkuwr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3clpgudmf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jsjsuofa.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uajhejtw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3grriixvc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3groauhhg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3viczfxmb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hdsehfnf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jkgwscbt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lkuezufp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bmkwpmsw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jkjptxaz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3urgohvgf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ocdtaegv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ebrsruqh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fvrkdztd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hkqcrqcf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3djlsckfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjbuoufk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rgigffmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3veqopncg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dychcuve.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kpyawfys.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pblbiuvp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3medsxdkr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jgrvjene.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3obconmav.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3paqihxwb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dwkrvnte.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xnpubavf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sbqgzelc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gflibihc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3igvlazqa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mxmqmdfp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pujoqtio.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3oxfqnuou.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jbxzpymr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zlwuukst.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bqznqcax.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jubivxdr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ksushert.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hxunirzu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rzcimpsu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fgdakkic.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nhhlyyzt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uxggsubr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yixprgfz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3iswnzqyy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bdtooens.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kxvwzytw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xwgqriul.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uiqxhusr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wvftkjvt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wsiaelzi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3haimsiiu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gbkqiqab.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3snndazbs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3utkwdssa.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fcbwiejl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3iponmlcn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hjpyrwtm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bqzedvto.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hhqsvsxj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ixrzmivd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3hrpgghxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3risttkus.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zxlhodcc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3haijehcj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xgtpupjv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rxjedixu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kaqnbiib.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3khhzbobt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ywmiqrhm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3lsfnafbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smtnsypv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3icspsdro.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3egcgjeuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyxfhinv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ndjxcwhp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3tgfyspde.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dcaztvqc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgexya.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rtkcsnml.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wggtzpnr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3sjxxftjy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3cuzxkngw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3voyamica.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3vsimvalr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qzakntix.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uqacmijk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xlccsdmq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3teiwuqvu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3rmcoxykh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ecnjjjqu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tllotreq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dkkwezid.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ggwnwucy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3nmrxeojl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hvfgnruz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kxpekzez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cxspseqn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jlpqzdfv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xvcudkrt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rltbdmeq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tstxcxie.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xcabuhtl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rinfwrsl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3btjvqqgw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mmikvboy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ftznkdvg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgsmxgzx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pqncpwjq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aapwdxdr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ihktrgyv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fthbdrav.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rtlgohpl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hzebmbuz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fqyifafh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vxbnzvff.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ilrwwzkc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pqywygtc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3muexnxmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysakztpl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nbrwpwlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxadsxje.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3yuznmick.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ezpvhpyr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ynbrcnmc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jgrilcgv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zdpnrgpf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3umutjouu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ddikzoic.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qxwfjhql.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3prkntyto.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lfkcbiqu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbaebh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3huqskwsi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgnjgjx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gslqhtrb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3skyahvyn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3cwkpxrge.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xhkicnef.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzuugia.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3dyfsdazu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ekyfkzwk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3byvigjws.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lufgzpnc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgjmyhhl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwenbvbq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mawgtope.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wcaoimtb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kvtjmvza.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rwtupxdo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwlzfdn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfbmbbre.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3unprqfwf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ywiptylj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3tazctuew.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ohxldqxp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3oqrmvhja.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wsgfggvg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3idhddynw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rdzuwoxi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fnsjkgah.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhxvzzxc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3voyisgci.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eihjibfg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3khugicxc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tdqrnqvd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qrkrvlsa.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vxwbaagp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sysfping.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3znidrril.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3aouarrrw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vzzkljfy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qubiiplv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ggclybuh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cbzfczva.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cldwwyjp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smgknrtu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fckxofzd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lijyjbun.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3aelwldoi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nedyatul.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nxmzqusn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zguvecfd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wvjgrpgo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmnqkoag.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3jhhmvpqo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xvdfubvo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cmjomvdp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3klqglriy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ofautexa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gjfuivtg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3veyeqydg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3enpfadki.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3quryqhod.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kxvmwkcy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oprpadrc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzggwgfk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3abumcrib.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mrzizuhn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uliwjmhq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ujexjpbj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3yjesddlr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhrgaiyy.html


<!-- 参考信息 -->