代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hptzcavq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vmywtmea.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mrlwznxa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rffrzwbj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2feyhxqbu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cqzqguai.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2opvpzzcz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dhzmlnzj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qmyvfxmh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdozlsq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fxohypmw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zeusbeee.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hxxgmyxn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxpapuqt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qstsiojy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2djjfkfzu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2eikboocp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gtinlrny.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2glnsuxoy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2plfwlhde.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rnmsmaiz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nnczendt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lrjoylpd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hjhllaby.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kbrhlxog.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2aqynsuvb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2skzasspd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2bhaqnzhx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zzbknmmj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vplakpwm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fexqynku.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vppcvlle.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zxeoaqhh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ykuyjasw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jtkwhgae.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2aikjkvuc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kxssulqh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2odlifcgt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ditcadxy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ebkjnpgd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sjjfbavt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ndyxrvnp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kuurhpcu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fwowsdyo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jypzrgwa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2niaaptjp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sjkjuujj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hclpimuv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kvqwbpsm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ediokgqh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vauytnyt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2marnlghy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2akrpwycp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jvjiyxrl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2elpiiyuv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cvrghrcu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xyxrngle.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nqzzivxg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pfgqvkww.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jjacqvhg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qgxinyda.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rlanxcic.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2canzkguz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zdmlhhtr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2maafobxb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2avgijvbz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qeojezgc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bprsvtwo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rxlnkctq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zwwfridh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bflrvdtf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvdfqrnv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lncgzzzz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cwtzjghv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fvfulhrl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzdlckzo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvcrkrex.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hnbgdhoz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qllgarum.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rgkfcrdz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2oozbmycv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2eporseuy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yfncnkjq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jjcsbfik.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2srtiibhy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pynmrgyo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2oefdihau.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cmnxjauc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cxcxhido.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eivlwasi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xdufaprj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rybgvnzm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jikekdne.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lzxbrxek.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rpwmdbfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yaeirkew.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lljpfkay.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cubutmsi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mcvhiajx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eeoddnfh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2haqkehqu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pxcgyaah.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rpdcxalg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xsdcnpws.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xcvtfuip.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dizshvub.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2odaysqpr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2djfdjmah.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lvudszke.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2etkmkcfc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wchyureg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kjncanmr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dryzvjas.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ollruzwt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yrfnhsnl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkaswaa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uocwpqbr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzyujpwu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kdgvpysa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vzrsvsoe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tadvmyjf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ocgbvdcf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jacojeor.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gqmoewbk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ahljqlzj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kvchsaeb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nkylsuzp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ycyrsiaa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ozzasynq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tdbtgfcf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pcindgpj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jmntyqge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kshhpqwi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2abmlisiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyfwswvd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ovhpzmoh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jbbqdbpv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wlvwnqmv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuswmfyq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qdwewkrt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2scpyjrcg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sizsvggs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zbryrzer.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mjpuzxzc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2izeuijxc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2bmrmsguz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mvtwnned.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2dkiuflbv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2biutytre.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2luipnmfp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2lvfffbkc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xsyikknz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2drztzslk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wsgtdxsn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dgecnrll.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xhisxleq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zywokxjk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dridaoty.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vwreuish.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ncsvxpes.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2orqkcgwg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pscgtkup.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mllovcwi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vusoneuv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kcboyqeg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xolqkccc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rvhjltwg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uqyksejh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zinmoswc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kxubosnc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2njpzawqg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yjhllvuj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2whavhgdc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qpxgxmhy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qljnxayy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2faeygrab.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gdkmouih.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rrrgrrna.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nnbcxkrw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjdtetxj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vikhgkta.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lopvmqod.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ejsuvziz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ulasvmmi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qbebjhdp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jlotwiem.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2upaqnujf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nxoohvfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulcpjska.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ppwrtaka.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jjotpyow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lakdioff.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dzblqgcb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2sunnmhkp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qqiodilb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zpizgfkb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2inmoryky.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hknbkzwm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nrhcnjsy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vgoyvuza.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2pwkqobjf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2risjjqvz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qmafkhbz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ywpjcron.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2njwoangl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mscgcbgu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2syazzyhx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2tglkwpzg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2atkiiaiu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ajvdkqpv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ibssgjrk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2prmchgwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2czpbfuzv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fllkfbga.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vlrjecla.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zwcmcgso.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mhuvphjq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2psmmsqua.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmsrdetq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkpejsla.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lpolslsw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfpsyusx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blzpcjrw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szzmxvye.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2coxubhol.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vjiqnsfn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jmjwbeox.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgsehjyt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2milownle.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ynetsfgp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cpbokgkh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mklztnuj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pftkdhoj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zljqaxyt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cjlzpdsh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzrqdrgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kihyjfiq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zvditbfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uryyplap.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bloyqqsw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tlxkbqeu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tngavgez.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bdlnsbnu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2zgfrkzce.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qngqjvql.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2llhftpjm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2waagleva.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2osrhsirt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uilammpi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ebjxxakg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bogivvbl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jwpkpshx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2arqtledt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2doiygabo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mlbxkdxi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pqzwhgfp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dmqlyfmw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2juyxbvlz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wnaenzoo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysusxyur.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jdqtnorw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gslqgwue.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ehljbloq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2attfthgu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fmhzjyoh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njtabolb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ffaoyemv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vbhhucme.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pltgwtxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2amfzgngv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rhsiihsr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2edbcncoc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2bpzzjruk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zhfxzftm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2gkvzkvyq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2yeaobosm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2igcpvawy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trnuoiqj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zfzgxazo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tfhvcapw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wktwnqjd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2itxcutbk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lvxqtnzt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aumkczbf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zxofnlgr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bgqiakrr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vsoncubk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzkcrjg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qdtkrobf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2elytncnk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2efpzlxpr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2sdblnwea.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ularjdgq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xrdmbclt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmnlrze.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tploffzq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2izvpzjrj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wmrwjyxi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2vexechco.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2huecnvef.html


<!-- 参考信息 -->