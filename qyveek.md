代发 wailian999

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xdtukjry.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxrzjbij.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wwusyrgh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvljohwn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bbopgvfm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ljwtghgb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bzcukslu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xmyhmmai.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tdvvnjyh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rvlixapl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hlrcwzxg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2khmnhtni.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2saanjvic.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fmuyblfg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hwyjvbqh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yxduqrhu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oczbtyer.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cwipzfiy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cacpuick.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bsthwaqo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2slohizcy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2plkwcjeg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2knfnohxw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ldyzuzcq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ttzrdsah.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qqcedvla.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2cmltskih.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2exvbwbob.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xvdwdszp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zrnmjhhc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tjfdjwfl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nqorahjo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iiuqkgbd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2aemoklkt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vkbbqjos.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2izyurayv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2esgykyph.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dfgdtvxw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ccchymdl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ryehlfiw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ktyqceeu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bipyuahy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tofaocqu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nrvuihbn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nfuiqqcd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2aarrorbn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2iupsecbe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ysmscrqx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ayvrwjsz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xownfder.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ncvmhzph.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlfswoxz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ticnigae.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sxqffrfv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dbhnuzbx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2brtmkwtd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nurjuntf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2akcqvutd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nlzuqgks.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jomxzzdc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cppzlkoo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xlmbuvze.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zioaajvm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhwrqhp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tbktotcd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bruvxrxt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dzeembsh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mzluxgml.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gsferjzi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xabvsgdm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nvspiqxm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gufootts.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xleoojfi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2delotbzv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zajayoyp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ezuawhaf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2oscccjav.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wsgbkxhm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2gxfywquj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2movproaz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tlnjqnqu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tasieunv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tofdppma.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ejiryzer.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zuejgszr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2etiwclfa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dupfvodc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ychpkvkt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2imkprjxi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhkiyjv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yzgmcmzk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2avlpzmfa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2admcwvvl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gffbukfi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ekihvywe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbkxavsl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wjinnlxj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zngmghzx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hzrxmzfa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ttnpubcw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2idxqzuam.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhkfblm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wvagyvdy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2rasubjis.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2nbglspyh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ouhlonqu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pimruzuy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2weoikolw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yyinqyix.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tnnkaxtv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fhfflmen.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qprrfvtd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kvlwmdzi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzswxkug.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ldqzwuap.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqpzsuy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ugaqmktn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqtkal.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xktytpxe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmmhpezo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ehlhxeja.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bhhbevna.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zrkqdnxn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bvpleanr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bozcigrs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hzujmkyp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qyvukdmm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2peewrpux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pepycsvd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pvcvocbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhvwrq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2akpmqjju.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2htncrcws.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2orqxbhhq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mqubpymp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ushcvytr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qpowjzpl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nvjpyakp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vncxffka.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eixmltpn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xmkjufwd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hugptsdd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zceosqmg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ayrbavtn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zeschffo.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zvnffngl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fosyorad.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aibqbvxr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lvmgrerj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qsikbhyl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2funtsbyd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dgyrxkeh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bkmjgybt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fbvfhqit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mqmcdurr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2faszwtgb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2kdcelpok.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rxczscvn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zcijsrcm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zdywwpeh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2guuabbrv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2obmbrysn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vtcbvjdd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fijlhkzu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cqnametc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cfwmykju.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hsafdlqp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2potpnvuf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kpufxvoc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2olcucxff.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qdctgctk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mcbyackq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sdjkwhzq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qgtmhdbj.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cimvyepu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tduullkv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lbsxbcqr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vksnqbgq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2znulpwxx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2crhtmdvd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nfvbvosm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zolcqghs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2owrjodep.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jhdgteag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdeehhlk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2rwsgjbbn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dzewapab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfdhgzgt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ztpcwbly.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2yyvhencj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gyfrypsg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tbyxsbzw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pxpgmxzn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lhmbmdxm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2nejlsomq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hufdjxzn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ngepebio.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2goffgbdm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nposdsid.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qrchsbmh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qzzmmwex.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ogfhktce.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2czuynmlg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xooqalqe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2yfmgjoza.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2crdzmmks.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2kazwdauc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ipukjpmz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sjozerun.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kazwfsli.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lepmasfn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2apfbyltb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydysjafk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugcyiicn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzrnajni.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ielltgtm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmkqemyt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2iwcllejp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjlapduy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pbgezrur.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejxdqthj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxdrefmd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2obnxajko.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2stswrmfz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rsnztquf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwwywzuz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqduhrhn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zoaclsam.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2olozsixn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2avaudpml.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ekufuxrq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gqgbfdqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnwmfxak.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2glszqcbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvpzpzbc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2orgrznnj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zktkolwc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zgkxbacz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uhzkwrsn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dqkojfvk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hekowxsh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ghiiejrh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bhmchrxh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tfwdtloh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jxsnpljt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cvdunxwv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2igwdmdcn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ckfgilxs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2nwsnlufk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vawzeysl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uwnouqfw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2tmsdbtll.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sxgfdhjh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2iexuyeqv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xuwhgeov.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2umgdwqto.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2klfeehaw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2keipwrqe.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ekykiiuh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cmwawiwi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2eshhsaxi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2crvfywjo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2otmzbyxg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2bwfxdoqd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pihxfbzg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jpynpoux.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fvurxzef.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2noiyulgy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sjhfhibj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2uwsfavbo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hegfemzq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jpqhiqgi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zyudcjhb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ipsszpet.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tsvntdtp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yvkvptxo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ltxnapjl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2slsonnfu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2foxfzxlr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wycbvhsa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ylyyjdvg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kvwuodjo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2alswffjq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2coinmkpt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dczbaoct.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jynjzwyw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2axznqzkl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qbefxdsk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uuxcdqun.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2onlppeap.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2utoxhxmn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jfnesulp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vswwvrre.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2syxsmrui.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zzecfnwi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqoicbp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2biuywthd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2uzfixzca.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jmtngnyl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qorrtgea.html


<!-- 参考信息 -->