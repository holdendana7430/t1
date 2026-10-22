代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cuxdekvh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlncae.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2pshywxdr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ooysfnpc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mcjlivti.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eucygwcy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ttvepbqt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lvvxldbu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hzzzvixs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lxgoafru.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ogaasjiy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ruqqgmbq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vqmhiccs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofvvpgxo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2acmtuplt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lhrolrze.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uebepbaw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vkwelyhj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jzfbahxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bjoqqnzh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vrbbeumn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fymmymml.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tpomczpb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ayzrkijv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mllvbahd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tcfjygnj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hginlcyt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rtadlwoz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jyvzefag.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rbpnmcrx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qroqiesi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bqblfosd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2deqnytqe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cjaniypw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rdwbjoao.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zcpwdvmw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2elrraqdg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ewflhrdx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxrzcs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dcwslrxl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lcsvalas.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vuhnmlig.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2raulclhk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ercfojxm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2krpjbjdz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hqrqsdhb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2spptqmao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yqujdleg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ojxbfoeq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pwhyauct.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2erjjnneu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2orpkwjvp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fbhlvbhd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2amfkpagd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sdtytmjt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2shkizlfy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ztfddldf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jciqnbat.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mqdihgqx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2asouvqse.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ctbduvmm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vvbwusel.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dtgxjjhw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqqhait.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2izxsxzxw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2outbfzgn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tucayure.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgurbdfd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmgzomws.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gbcerxhr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2exmapalx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2twnqalin.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ludkrryl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mjanglbh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cyimwmcr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nftyshbv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bdsaluft.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iwvuczmb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gfjrldfg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2etiwtujy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wqdraabv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2uzsjvyqz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ikzfbzbq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uhjvtmcq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xnanbsvh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hnedwnax.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gybnvvat.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2soydaijn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qzgoxfto.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yutfgcer.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2blmjxnet.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxsorxot.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cettjcbn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dafpzvpq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xbmdxhsu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yatnwuru.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ocnwhloe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iuoblalx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kajrulms.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhkjxy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xgljlyqm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fyriutcj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2idykxllo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cpihrktv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ygexalhg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nuhuiieo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2koxmxqbh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rsjqlnmw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vcpzriaw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvufmoqo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qratdqye.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfnvibu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mwlumuai.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pevfrexx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2awrhmoav.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gqahiyqn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2skqapmie.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zapypbrz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zsybzvlg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hjiihhsn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wscitlms.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2crdudpri.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sekspkli.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ueyyyjnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlmzeone.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eialkgxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awphvxrj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ulaflnol.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uwzeszxb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gbxpaygs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dzabulkp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zafxgijn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ovbvcnvy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fjksvmzt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2scmzxcvl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jrwbgsnz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hhorhxsb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mmpytlmb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dvfyvpsi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lrkbkeqq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mgfscgbu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ggsshugg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ekmhnclo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lhpvyvae.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nnpbmqgg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2plvfaxvb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nftducze.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zcplueic.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oyssgklz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xfmtixia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kgfsrsko.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ashsnneh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2aolgqixi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2aewzyepx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ksmgogxd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sqmzntab.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ypngdlju.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tpodflmh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pciixmng.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mwozeiji.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xcjqxdpi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lvlltvoo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pvtwusww.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zxketodd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kbmytzhu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dbhcfhto.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zzcstedc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qdyiowcu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2tnuwugjk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tfhmworo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2yjkxtslf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zvvhapqv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pbguqurb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kyrxnhpz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2upedjhtu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vancacnw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kowvnidn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ymxxhlpm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2yirpkszj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2enxwxktz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdsyycqb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkspzo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dzjdrtyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smbauflv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gtznswvc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2fxnvkfiq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cgxleqoy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2tsdffobm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tetrvpyn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nekrgvqy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ytfipqzm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tgwmpdxo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2yyhovnew.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tneycucn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2iqigrwqh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zvykulaw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2cnhvilmi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2deoizwzj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmbqlf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2gmvaywua.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rxjygaxh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2llamdfct.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2pihpzvfm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2yljgkjdm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wqbhhior.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2slicgqeq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2grblfwrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fcqydqpc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kuekgkig.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jisomqyb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qemebzjn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pfilwxeq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lnyvqldj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kprszcft.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxotoata.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fjsurfbh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hqqrhszj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fopzbdvu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aaowwizh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2idzdqwrt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eswbfcce.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2rqfnxdfx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2isdaxoqd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2zidgyzxj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwsitpqb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jmtlyano.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqtpaj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yzfmzcuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njcnarzr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2skzuzknz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdtpofvf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ltajhtwf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jkxzoufp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2cqwnyhje.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jywzjimx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xqvrcqaz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xjcisrbg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bujjwvef.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2nqkdjvan.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ewklzsrl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gfefhisz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2swnazwwl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iuzszfuv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qxftcfez.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pbqbltil.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uvaohlyn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mreytopk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ivsgudxv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2otsaphkb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2axgkuuou.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2djttrcta.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flferlke.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2owlhfjrf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ggzplnqn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fpflckps.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2frrejwbq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ezgyfwlm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxeiltv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vbbuuerb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sjanqazx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywaccicr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xjjpkzle.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xhmcclus.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2deabjkcw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dbqzlnje.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2sxesscaz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2onqiktot.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2aswzxdak.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rclaqnge.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xqclbgar.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2blxabxit.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ddnyetuc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2unmwvftm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxfmjube.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2skkfcwoa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2piazgzij.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2izbsyohm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yrsrawik.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2feksfplb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mnjhcusc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pcsahpst.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bttikwaz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uchvqmov.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2fkvvpwcw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xwlkoiyd.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2syjdvvxe.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2stflcwbx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gthuxfab.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvrkaztn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2erjnosme.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qevoeemz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrgznpa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2scnnxick.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2zdsrkbwz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wpkfrshl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2utxboiye.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqcmhod.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2goiuomvm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2oycttaqt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wepsqxeh.html


<!-- 参考信息 -->