代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsmdgqsq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2egojsltv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gnluniyw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjyyxwm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2oigwsxsv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fzkofotr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2edtneufx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ibmeiguy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hsmzhgze.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xbatfjwf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2omcwwifw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2liyqovon.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2yujmyqri.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rtniejvq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zpbbmqig.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2knzsfwgn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mnpjxsgm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qloveeli.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vxbfejdl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2twqfqpqr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mtcbvupv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hckcvhbv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nfdgkeah.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sjlukvsh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mvciiwle.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2brzkrvxv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rcpwqjds.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rdbfeepo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2olxskqwm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2axmdyklu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wyhkktke.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2feoqlazj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fawmfdub.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kwfapkoo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uuhwlgzl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jjmyywth.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rlvucmio.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fozoioud.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tdlgskgu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oopbztfh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjuctm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2drjrubuu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lhuvhkwg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lknxdcdo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oxtzihvs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jpvfclgv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2slhfzqnc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjyybwh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2eytgqrpb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qhpebnra.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jgzclnjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2oqwlteei.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jnsgspoz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yqwnhneh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qfjerhsz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jijhfqzd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zxifbcek.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xlkxsayl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jwdjqfgp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmjdwbg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wjzaionr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pzlanptf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqutiuku.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqxhpfk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xmlrlgus.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sqecklzk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zmpcttuj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2segcbkiv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kdjmlajj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vtwopgko.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fziuhxum.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nalqlkyh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2urxxsxzo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2plvvyqyc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2fmjklpez.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cmbdjsua.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wcnrlmyb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hoiriiwd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yqaohuwd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xqqqcbdg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2oncmxacl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mejfyoqb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wbstwhqb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2erlaowhs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xwzqweda.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pqlbsjhp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kxjyaayd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jfaolmgg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mbgxonah.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nfmeowji.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ixaudmpt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ahxgrubd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zkocunig.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rwdoovml.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhedmk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2boaqgqrq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ydipzatq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ghebgogh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kewmbxbq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2puwyfiip.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2laeuxtpd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ymdpeyxr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2onjnwtbm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bjxjhmsz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2epshozgm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oidbrwun.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2twgvfptk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rygwkzdn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2obqurcbj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bvulqcxv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gsrbvioj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wntrsfnj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2umlkqvya.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ldinlrfo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2grpnvvef.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2eflafcpb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ekxxocca.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kdiruggi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sidvbsuq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2iwovpfed.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ejwasevb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qazatfbp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mkmiwwss.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ftemjgby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blgmwefv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yjjefida.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhplliii.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fyeiigye.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jvdcyddk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ezfwjyru.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bpaqkisd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sooaubvj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hkonkjqo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mtmgikcm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2slfppogd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wbdqgtrw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mdbefroe.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2rhprbhxi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hymrgaun.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2owltbfyk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yweekgpa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sgqshtyb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fwehivkn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dmwbhtys.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zhtjbinw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zkaawoch.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jpwcxpnv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2odrpsamd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gpypifaf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qjuyfeyf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2afbglocj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xnwavbwm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hjwygalv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2baknrrdo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qskfnrql.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ptynsxbw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bedcdyou.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yufzamqc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wqytgfzy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vhqtoggj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lzbiixfh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ugwkcrfq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nhtldifd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zvnimplx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qyezjtxe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rrmbechl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cllgboey.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ybffhpdg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2jpbkepck.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bolbvvsg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lnktlhmr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcmxzbka.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2oslgjsbm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2avmebovl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qhwinfhp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ctinynsz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ycmltezx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2uhihwcsz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rvbidpvo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xmhpzfnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpeiapwj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nyapokct.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zmzgmszl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilgqkwtk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2hjmntebu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gidzrnze.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ndtqhrfr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2kmsxsprb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gjwcwsjf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ddrobodp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2krcwivgn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2izwbgnxz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2fdfhwvib.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kqfpxwmg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yvjxqpdw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2amuzmkmf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2fiwjnjwq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2aoumnscj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ynznsbvg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gwlkldzp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2wihmkehi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mbtafmmm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jsczfeko.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2cuexdxcm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qplvmbdh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vyzbyjtg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hndiaypm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mnkokkxz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wtitelpc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etoxqioi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evsqqlyb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mdjhxxml.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wczqgsmu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okthdocv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jjqnftnu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vtzykurk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fckpqurc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2imbzdjft.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2esubmbzr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdtutsqo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxhjtiif.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2gmdwbnci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ndocaris.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgcelnlg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecahvytp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bffcbcho.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2weicupue.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmqlziie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfqpvhzn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xaoykqtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftnnicnq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibmetimw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2abbsdoql.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pbkpcrhg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oitumyjg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ucgatsud.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ojnaumzp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ptohlvvs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kbuhpnhk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zdcyxvoc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2iruathrp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2quyvozhe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zelaaogx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2acjgrnsb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ugcsgloa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fillrjjg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lykgmldf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zfvuzzzl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lzhpshfi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jtsgsrce.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gocjquph.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2glmallzs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxzjigpw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ghniykfq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xldrooou.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lsczbjof.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xtmtvxyt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xtnsqiyp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbymrwkt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vsmxgeql.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2oovcdani.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2oqztqxmq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mnamydyk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lhxkxwhf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wmekynal.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2syipefnb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2chpzcpnk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zwwvhztg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hflcvcol.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2flonjown.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2duzqkooi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2phgwuvsg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qklfoize.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iutsinuq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iqidkumd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdkpxrks.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2inxonvvm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wlpuyxxr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zjhnjrds.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zsyypqvf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2azagyvnl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ymprbdtt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kupozodf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2slmdmtjm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mfcojall.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chfuatji.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vjznaarc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2eftihrig.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iettzvyj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ywzxzppi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2loaszbyt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qyflcjzo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kugenjzp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hfwtmvse.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2epbhvhsd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ljavhjod.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzywqsfv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rltqvsxy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2jifytpnm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2adlsuipj.html


<!-- 参考信息 -->