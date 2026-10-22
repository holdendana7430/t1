代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2artfdaag.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qyocwogu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bgtxxorc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tjfqymmu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tehdmqga.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfaojrlb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2svggzqbw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kasebfyw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2uwutsomp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gzzwhzdx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djnhrzlv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tukysvdc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cfcflctu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2krvkwrri.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ennksaut.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gxiuyjun.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mgcpfyhk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xdvrcrmf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lrvexfff.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pfdxkijb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2okbvyxhd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2spjrzqhn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hosfnwjx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2symmnjjb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2esvvewow.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zvjvmglz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kexiusfh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xcnnmsat.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qnjsnqoj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2guuqgtvp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wafgijhj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nlqizxco.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gpegefpl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rsmxepke.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mxsfkini.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zyldsiwo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ybpzyobv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rslrcunl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rwfpfkmx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bfkwrbfk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hzyyqfxt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ijjxyveu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xsgjxnif.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zzhrwgxw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2psgmatvd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vmoxdoyp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pyykkqtw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jedjkmrf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2egvnjmss.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2crclhmlx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tqouvtfh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wbwuqakw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mrrlyntb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rbfnwqba.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qxymqmbz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2udpepiup.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vkbyolxj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2tgbiheps.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oaflagem.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2doluuweq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zxfgzlpg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfhmmjsy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pliayaoo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2owqvkwyj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xffdobvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pytdpzrp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vuwzbfrt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhokylek.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocnylqgu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wzzoymhr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aampehsj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jvthuecb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2sdwadsmp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dzqytzbo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2saweudww.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgnkpbll.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2euvxyfdm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pnbckzxx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sqjvnklj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2elsduvym.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zglhscgk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xhuuoris.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixianalg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bxccwrqx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vjlskegk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tvtwxewi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uytmhyrf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2epwshmmb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zuvtrsre.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jrjtcgfi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tcijazct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2syghbgne.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zizaotzq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iozjbfqs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qmgupcib.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hqtzjltm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hpcrxykk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoohdqb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2epqunwxj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2moozyetk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2qkxwtgne.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nzohhvsw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rqrlavgs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zhzjtwtf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rlpgjegm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wtbrhimz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ehdekmkm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mcwrilze.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kxgcfpxu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nxwzzapb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfmmdmts.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcahiwy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vyicxhgm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vicorepr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2iigheece.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ugjcmhvn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2toloincb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rgyosruw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ravbilxs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wirzyjra.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gtlwnvvd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ahjhqbqs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2bucrsbgi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2aahyxeyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alhqroys.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kemlogvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epxuvjte.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2oredesea.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gojpmmjd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jkjzgncd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xevwfpql.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hzbsfsmx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sdtqmnlt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ycpqmzrj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iehymimc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2duuzjhim.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2iikcepjv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2znrnribm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rtdpxaaj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ygilpdfr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xecalgai.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2imddijhp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vhhocaxl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qpjknowe.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jrhddgbn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2noepvkgc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2knwqinvk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2fouytxdz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pvalzsam.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iwhifdmj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ycyueinr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ldvuhima.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2pcbcbqok.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dpkzgesi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vqnodlej.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pxlbgord.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tyvdtnmi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rdmnlwhl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afqueubk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sarpajmq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tjksmpkk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xlnvlcod.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cssisyct.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vlcetgxg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2oopnhhqb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2canoghll.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ehxfqbng.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pamvpawm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ajrilxzu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xaetnohs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sdwfrlyv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lgjmrpry.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2avltnapl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zkosutjp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uvmcngin.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wzapefuh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2czeqsiyy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2goxoabrm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2bzvaybtz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rmljivaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmjrvruh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2eojrrnxm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xlnjqmct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uprdibcb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rdnonwhb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jertcqia.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dmwdcrof.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bphgluqx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qdrdlngi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zeqryaba.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dhjtcihz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2pqymlvye.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2csmvzxea.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2llnbxqof.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rnybpymr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2efldzzta.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2fkzeilbw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2luxzwgwu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2excyygkg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nnvmvptb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2wkxkzwrw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2tyreirni.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nauobrod.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xpafizcx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wzlybtpg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2pspxehdc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uwwyustx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igzbqhmj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jizmuxzr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2suybvcca.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vhuykoss.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cohwzrrr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sjwvvacs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ccipugjw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oawnxbwl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uyqxrpvp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2urtrspeo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2caxcbeff.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2flngsckv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdbicvkr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crqcosrz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhnqxrbi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qpibldwm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzrikfau.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhlnyfir.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zpscbaby.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2absksogr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzvlqsyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpwgxeqd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxnhbiuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dykwhjtp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rieaojim.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2asshpcfl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rqidylco.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zvggjute.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2tdcdrkbi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rwkeawae.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gofkehgr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2riouahzv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hitdxlna.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2fydalvqj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ynmbrinq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hzqcegoy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xmrunzrp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2arlgjmqk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nnzyfttj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gjksyxmd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xxqehlwv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jysmbdai.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mqcgzftu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2inouymsh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zaowsnxx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wrntqypo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kztoxrcx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yrbynfra.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kvgvxevo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tsoelgwn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lqwwsykm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2leelmobs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nzapirup.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2sikudsvg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2clqqdiuf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2icsczgqu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2sddsyhpb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mozfqkev.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2expolirt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2dpguhljx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2slpnxpgl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mxqwcmij.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zqlenllv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vbtqqvwe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2krirvqpe.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fwhxiunn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hgtfhpnn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vqteylwp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghvvnfar.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ixokimdv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2okcypssk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvphaub.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wqwstjrz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qiinirmp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2noolgrzn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2aibwscor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2oytlxjse.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ginlhaad.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ycgwimaf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zppokpcr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sskakzeg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2exyamtrq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwuobly.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dqvwnaqp.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfzbryp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dselfnmz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2znpbqrwu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ctjtbobs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbprbxz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kvqzrbym.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hxlnvxul.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtcyekf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgnaela.html


<!-- 参考信息 -->