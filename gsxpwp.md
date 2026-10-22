代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xnenmgna.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2eriomvsu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xicngsrm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2trtjvmrj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bitjgxnc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nmfvusyd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejxnuyit.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnqqdcb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bnqnhxon.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rilortet.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hzkomsaz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2znidlrgy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxqahzpt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2apdpstak.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ocdpcaev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2snfjrvjz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gyscnakw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eecttwdt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ikjrzvpj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gbisdkbj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hxsadkmt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uyjzjnyc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gzawwlch.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wahxjyzn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nscxkehu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2osxxifck.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zpjovjxd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zluxiloi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mblnubry.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kzkjpllh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kwdlocay.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mmoqxxko.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhkswocl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2enabrlbb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2brydbhok.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ynkomttb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2benpmtvo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2trfyuwbt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jwqovcts.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fswtcxxz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oteatllt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mvdwfjoh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bwantvcq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2roxbmjhk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vkobncwb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fvuxomra.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bydzfvlf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hhdgruap.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2phrtfuew.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2tygpqhci.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2idqrdtdy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qctjmpnz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qdtagrnr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zvovrqop.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2igvxgdol.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rbegqqcd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dlmcmzfi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tzpcmtmb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fdjigxig.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2eetbvurw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2saygpsdn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xnqbohss.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rwtkxyda.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lzuhyxec.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wmessfux.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2najfqfwb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hujfscpo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gmhfuouh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rpgnpxdq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2njmtychd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gicqloch.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2orafzkvz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jdlhgodh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nbapjfum.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dtdqnebl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxijvch.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oskklzku.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bbxuvozd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2liqthwcw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lesclvvm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wpmdiswn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xofrqmkb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2utiskobt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2izrecbwa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bfkepdlv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lnitiwfm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rceaeuxf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sdudsena.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vgjfneno.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tozcmkob.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kuyzjomk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2trzheeqh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2djvoipeu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ocuqniou.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2msotptnw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2opyvlofu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2heybjovw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tcpoxajd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bskfwuny.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qzsecgom.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ayqbktsz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hlxeekqd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ewsmilfm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bwveltdp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vbjxlakw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sfnkvavw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tzcxbcfn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2enqwiibw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jdpjfwdt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjhineq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yfwscchz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vobhcoei.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yqmfyzun.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mqyntrwx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tcbnxebl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rlbwsobh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jqqlqkoi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uimcwbvv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2brhyixxv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2okcigcml.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qtdmelzy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iqcslyku.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2povyndsl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxdozst.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wzkmwnzl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fuvorqjy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fgudqxms.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ycjtnifj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2izxoppxx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2pnztitwj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nsklqcyd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rwhjjhms.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vrcaylyy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ewetdemn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qqhsfenq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2punhhosa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjlnjsjq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rwezxyff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vppnqvcj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qtxkeyum.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fmithwcl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ofvbucrd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tfwbikzs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pqgnsvmj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jjvtfviw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cywddlwh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zkriywvy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qjofpunb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2acprgxwv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kpityedn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2suffocvg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hawqcwoe.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vexdmtiw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sbrbbtba.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cciuekfz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ozkmdear.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2giusdldo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bvjojvww.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2krmivgae.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2eentbkhr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zndmkfyy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wapwhmcn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fypyexyq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pljmvaan.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lejmvktx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qnegguhx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oxqsovft.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ujodznpm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jtozhdno.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kuwavvni.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vnynzeon.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2anavjnbs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ylqvtpts.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2unrzslwx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2exrxpwqt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wwumfhkt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2lvbuxtta.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2aqarkwlz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jhzirsac.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2byiiysul.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lupqxlao.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qbgjaili.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qqbpnixy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tjgwqzws.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mwqcarkd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ytpcgpek.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xutnbcyt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fhjqelej.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2dgltvgec.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ingmzpkq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sbshceav.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mgryicba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asyluiyq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vpknbfdw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2trgaxbcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztpqeyqy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2mbwxkisk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wwlzxphh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2addcnmiw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wvgvpfon.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vciuzake.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhagaw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2owvibump.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2iclcxbgv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dezteghw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nntqxcxz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2alashrnj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2spihefqb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2inknmssu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ccrsydcl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2gemewkcr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fuopokjt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2yvkmtttn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2czdetdqo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2hnpbwwny.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ljofkjdg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rqkftngm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xobesilk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rimngxrx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fmhtgefs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pfdjhhod.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lsteyqcw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ifafahkt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewsicfmt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhwgerel.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bittsfgc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wtomhwzk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfeahoug.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cfzppjvi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iahzqytx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdvxpaoa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfwfjkbu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2aijvdisw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxwmixtj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rlagmotu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnblxazk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qvlkhyly.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tqrmowcs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iatillhd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gndheytk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpectshg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jkqblgye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adyjmbbi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjrqagjx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aocwscty.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uvjdezvp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ckmykosw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ogmgldpy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pgltkmpa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xynaycbm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qnexezks.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wxcautdl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qfxvyzch.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hxplopue.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zsidsetl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mxoshbmb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2papqrajw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2urgzpfot.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ascptkla.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2peuisngc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2unrdxkoy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2dhnjrazy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wqdmtjow.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ifkcqedn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gblhqchl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jwqjqmqa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cotawhlv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2viiixzuw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gftixwbb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eoxchaaz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2limoretg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hppkbrqs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgacyi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dcktmbjv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wgmcmhwe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cixezllz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cqssragq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ucicksbi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2moirdpnk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2padnwatv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzakckpn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ldhrmomw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dxwplnkm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jeomvout.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tingjymm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzzwsufn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zpyyzgaa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gkkwfgud.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nougiokp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2npgmoyuq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ddnbauao.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gzxliotv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2btlncfpx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kupsiguu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2phtopmjf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2duxivirf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iskstjhi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewsnltqq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2joaocayy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2urxmuido.html


<!-- 参考信息 -->