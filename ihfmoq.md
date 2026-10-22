代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xosznorx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uuvhjlgt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qnyfskcm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jagqxtkr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2yhfzppuh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nlwdxgol.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tpmzbxxi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2atuymbzy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oyichfyq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vwybypkm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zapefutr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhkztlbb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hueiytqw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bcqmjbgw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xacqeomp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wkjxqyoo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpfitkkj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sjkarxkf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jahcumlh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2emuppibt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tladpamf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pnrdhxob.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lfcjfevj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hggkxqba.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lyjfppdn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jjzzbrqu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tfoaxawf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bxybzbgm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sokxvfrj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ecguyaxm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hhvgyfqu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2goqfesjc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ghjpxste.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yxrnoybq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2axjvdzik.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tqucsnce.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qpvqdkvl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfhsktdz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bfefyayc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pnrlopoz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kzmgymyi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zqqrkfoq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jalrepmi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ccihamox.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dwypvted.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yvscumsu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tjkkjttx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xdubsxhv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zzyukllx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qcmxgrfy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2trdietmw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wollubew.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cchsialk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2czvpokaf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tzsavshq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tvsxpfin.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wcweqfhi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ryhhomna.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wigpwdik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wtintist.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jcijwecq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uzrdugjc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2pcogskrs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nmasixtw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qdhyqwvt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2whxtsvdo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2brzobidn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lllvoaaa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2emvasuvd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gviapneg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gvybpgay.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xeykhcsy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ccirvulh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eillorem.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xciovoas.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2mkbsehce.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2toagoedu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fzoxlnrz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2giwuqczm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jecjwtyv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mpuqlwzb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jaqgopkb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lfezsioe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gnuujpxl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxykcvhc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cbvrcohy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2smvlulea.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2shvpfzhe.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2pstkhucm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ebomnhyh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2aqwyddoc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tlblpcud.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rtcwdrjn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2loimhnni.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ibopdkes.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2emldjwis.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wmbotsye.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sqvshzpy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2obfembno.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2uczlzcuh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fqszdrek.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wivczkol.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2gprhzbzi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pzbgplnx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hvxhjwua.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xfyrheud.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kewrzwys.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nyvrnqxs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2omuyomyn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2szqteemr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fjdlvxme.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2orzmwskd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rayvtpli.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2adzxcgmh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2idniissl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2oxgxjfwy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2etgezqjp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dohzwvaq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sniqvuat.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cmvajasu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pfbqtpra.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qwvgqjds.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bltzbyxd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xjgwnhki.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2apwijoka.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ykvkjlxb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dnnjhfgm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyqpjnv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jcvdbkzn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fasuueyh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qckukkht.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmbtqqcf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qusyhgbi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nctzrchw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mbisfstp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2poyzsgwr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2psupzikg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vqeaoanw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vezuuapb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yqwwfpkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofmrgbqj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yvggdwvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtllenju.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ffcczdaf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ibwftyqv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kbpwqeyf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gppyxwut.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ikuoqjit.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2anjasuow.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hqwyglcl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2grnkuhrc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mafdfwan.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tdjsxhdd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xcmctyxx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ogzakrcd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ggzcwyjf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2azukdylf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qcyikcnw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2txrjhlqe.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qgjzqvly.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nljivbmb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mzucistx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ooagmnuw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wzowwjrb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jegsdtqx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2egodiyyq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2btxxqesz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xyxtbixv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ovwvxkhb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qcagsaoa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mewfjnhv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nnutlrrf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oxnpfvna.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dqntxhfc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kndvgnqm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2izedvdes.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kiwklxmm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2valsphrg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bgfxzddm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jnedbdef.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2watynnwx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gkomutdx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ikzmlrnp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pugqiukm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lkzwzmug.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lmdbmdgt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yyjyvxqu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2npiquego.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pakxsrzm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lrvapbfl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ywxdcvpj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zcahkmab.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2apimlczr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ctshffmn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xvmnjrer.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2mhpbozvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eecznkoe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qqumzsbp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2kreoesdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jazzdlag.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wdpncyrb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hicjxyio.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jxnrkqcz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mhbnbgbn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2snqwwyad.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lneytrrs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vtrscqhc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2npjpxgrf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ygiapvoh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2usajigsi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2edlfewnh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2klmmguut.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mzhrdctk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cmdrjtye.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jejeouku.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2sfjrffiw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uwdkxqca.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2woekxrxl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2eevtsdcj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2fpsvpenu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2awoukyvz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2awhejrgm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qqugjmrb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzlejlfi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enzvtsip.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxjmcavq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2prpwbjto.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2smccvohz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tvwddwwc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jeagxynp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygrayxeo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2utvlkfun.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ghiagnqh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xhswxsiz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tffhujrc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bpmgrznm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oigsvuak.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zewlibve.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bbybfeso.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tjowlofe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jydmsebt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lmilzftc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hhaibjhf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ldframks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aivzvzti.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sskbpwqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chvxceqd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tqrmmaol.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cowexmsf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pmjwkhuo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wvsfueok.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ulkrkwwe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ncpudccc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yhoyelxj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qafvkzoa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ifirfsnw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2anzzebej.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lspibwfp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gkuzqdgq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nwmszdsq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2anxvanqp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zzntfatv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ebnalsvt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2bsenkorn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ziglngyv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vyhuluck.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2cvmcmgej.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zxxqjzcw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kcnqavvm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ooufxwlr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxflzohg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bdtqbted.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2naedkfii.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tievnvbk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zagsbrbn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqqfedj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrseujcs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wjgacvqj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gxlzrzhc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2qgdpppgt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ikiecpnn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ggnbjrsu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2oycxddow.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dhojgovx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2blnxltqn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2utzjlssf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xwwsajbc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bjsvvtpw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wjxvjqul.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wszudsox.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svebmgwe.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxbfeomr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nbfqtrkb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xjzbtvop.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yvbmkrwe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wvrwnetf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wicstvlc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2orvtiijy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lcifdhnn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2uxfczhiq.html


<!-- 参考信息 -->