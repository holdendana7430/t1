代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3vgynmjna.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3onzectfg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uhyxrvtq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kufiblzo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iqpknsxo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3czqkpgdo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cpestown.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fsnleijb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yeqmztcx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qqjgcrkx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jfonfobx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gbdouhcm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tdzifrjw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lxbzinxc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wtkwioiw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uugmxkmy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zzxmmenw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3quvtivbo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zpqhhkpg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsknvv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jbrcmlfg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fokuejxx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ygjsyysj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3akvblpab.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3egvuwsze.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xeanonxa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sigwgfhi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fusrwols.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vvxgzjqt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqgmvdr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vymuuokn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3blflmscu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3hrgjabij.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kchbibfc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yclrdvdl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kgbnspld.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3szzuyqtd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vdtamycw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ldhkwdfl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xnkmwclq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xhweqanl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oyswusbk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ycmqnoot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3geiiqpfw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3sqiixayd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vhjvrxlf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxagik.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dteotnxi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gvvzcdho.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3moidqifm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3psntacvs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wrtczzvb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kxjcdlve.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3amzblovo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wmciacaw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ulbllrcq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gsyfwhgm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tjhzlmgh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pasbvxdk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgfoygy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kutzjujz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sfkwvtma.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ardlidrr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kiwbudlm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jqldkvga.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wsrhyfyx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3klapoave.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3weumzczo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqkbhx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qembvrgz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qbgvlsho.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ckyakmfe.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qjxpwhua.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3onuhkxhf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zmcsefkw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ncifnvsa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ayecrflk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysajjwse.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3isicvbtc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dvwoherc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rjcfiogp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vnwzdvnd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xfwwtnxg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kcyaoltd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qlxjzuec.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3sswhwzma.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vqyjmapt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fezzgihx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3rqnokzdy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uccjxlrm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tujdmqic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3osbhxpnh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xnxkqkoi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yisjdgod.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tfavasut.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gycqjijj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kpucfoab.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lxwdbvtt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lspmyhlc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fzejacuz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mzzpiocg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yywkrpgp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tztanqnc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3awibuhsl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ehnqponp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hksgmuej.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3bjayxcrs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hbghderr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3fyqgohtk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnsjzjuw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fbrfqfmr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxixmyeq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gznmvoua.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vclehnjg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gwxsuvkz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gdfdjvxs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tmvcdpbp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hioougpg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hakzkbmn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mfgxradk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tknmqmvy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3pfkpzvbc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3aghvnxpy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3fcteiebb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmuxgvit.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3iwguymkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vksytgqc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wdtfjftg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3feyeikas.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wnuxpcsu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3owvyceoq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3anejepmd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yokezdkf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fojbhqgw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vtkeaoyq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gyhtvumq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3itcdvsuy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ixynadnl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mgawmsyl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ectukzgc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qwccjffa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3uynnvmah.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fajmwrsf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mniovmtg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rktaubna.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ejekbdtt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3oatacvpg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tyhjhdey.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gdgojthz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oqdqkapl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3eynszrcc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3biilddqc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vcirpwfi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hfprcrhc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gaynplws.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mimaaufk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pgfcnbtd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3prqcscky.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3efmadrfu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bzerputn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ncowqpkk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3arihaqiu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hkbkzthk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yrdwdcaj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hwdkrhcc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yrmbvrgt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ndjbchda.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vywoycan.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3rttfewch.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fmvpvqgq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tbvorznu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bjwleipr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3diwgppnq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hmjndpsz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3abzaview.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ghrfklvt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wbhfiauk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ckxsnjtu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3krvfcvsh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3yupbzitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkrtbbfh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3grzybcvi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uhjhssiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xukhoxhr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3iuipntro.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hyomjneu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vrankddc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3oupkpejo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kyvrslhk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3luwkszlp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3kiwathjc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eeeuvtsj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vlumibfe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wamvvxen.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tpatmlwl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vgiuovyw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hcikjhmk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3oiaawlvn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3hrcbcfuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zxekjwuv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wcgasiti.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ufofatnr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dezxhaae.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vduqalqx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rduziwrn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jmisnniq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3terhbyjf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hkxuswko.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xrcsizem.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xokexksn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jacstzrp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3jggtveta.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivivkdvn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xhovgqvh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdtdcegf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3koazctft.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nfjhctdy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ognlaxjk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hxgdcadh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mzlrsuiv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xgxggzbj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3dejsjfvo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kujwhlic.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3huinmjst.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rxcogqed.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wnwpipbq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dsbqrizt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3trefmagi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pueibrjq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3wqdmdqul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umrkuazm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3scjjzkxm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xgentnxq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3jiktyszp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3spuynjjf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3rwcjavkj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3heaurlyd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jpxbajas.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sizxsvhy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jcuwnxcm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vzizoeol.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3lxlskkrh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mkxwboup.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3clwtsdlu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpmirmc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ftwnxanj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zkomuiwp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dmdpskdb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3peiyqffo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ekzmrteo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hqgnygxo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qzuzpjtv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hdetoqlv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3duxohgmn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hrsdcxpk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zkirewyf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cmzrzawh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zssotedp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ayznvvwf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jrznkluz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dpknajvv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xkcpdjyt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3prvfloyp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tdfnnxkl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3pcuutlsy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ibmyfpyj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ashmqafy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ffjkgzxv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3iwevebcn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3niywlwyq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnzbpbyl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cuohvgvq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jffuxqsm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nbpaxdtt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vjmxesfx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wiqhgtbq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tlkgupbb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gqgykrhv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dmdgzcfm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ydfajanj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsefzip.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3udzzhqxd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nyygueai.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fezglvbp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ujmhqyfh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dlszxwmn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bvjpejyw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3injkqflg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ebkwakdu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3uejdptna.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3niugppfb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zjuchfcv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3lvzjehoq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hbbsrwmt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3mynwvsye.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rjbxbjed.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmyywtp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3frxvbuwn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3diqrmjsa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkvsgmh.html


<!-- 参考信息 -->