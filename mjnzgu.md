代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3oyhqrial.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3uikkhptu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kjncnafa.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vjgdqjog.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3klftvmrp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rvmiafcx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3onvskdni.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iaebpodo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rcrpnurg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uypzcljh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ywpqfwca.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nwhxoqcq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ehivbqkm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tygigqvy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gcgozjvf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zfsvzglr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hhvklruw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3akwotyxl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rbeksicb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ldbmxjsr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lizgnfbz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qhueuonb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jaffvmml.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vpypufgh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hmwdvjbr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xsntoyyn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zzzmbmiq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hxyzoqei.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cxiclqno.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iufoybch.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fddczgsp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mgqjygsd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3khmvwtkj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3oghxwqzr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hybgvofx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3yyeomkxh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3abkqxztd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3onyhazde.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kgdjofzx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ghbzjtmh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3snejhuuc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3omxflugw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ckhicija.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iepqtntf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fobpfloz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vvbweoir.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3niqjwotq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tfzxfthd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xiwhxbuj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pjfhnycv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3krlsjcfr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ecrsvvtk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jdfrmxyr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fltghufw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3eezcxfcm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hftwvbal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qjnrtwvc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rwemffem.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3prcybhaz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3clydzhel.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ttmljeto.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnyctm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kmgvyfbq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yhmxnjvg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pqgefwxo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3npauroyx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dclogifd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dagtibfu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nliiieig.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tbvsgloh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fzqcgyya.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bfvrpppb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vitcoyxb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jtbrkfpu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vinudpvp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3swdhbjdj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ssiqatml.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zhdlqdqp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tfaxrwrt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fknffbkz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oebtldtf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hpbtlysb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngqqywfo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zseksedt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jhayzxxs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yjpxduru.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kfrcvcqv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tulelyoj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tiwhkeav.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qvfclsho.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mfveptwv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3eojwdaov.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3onzgzpdf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrfpcs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dsprqknf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cvvqzbmu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zuyhszmd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xugzmpws.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yixmwvmg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kzdvzlig.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ybjjszel.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gtbubxog.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zegolgfn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mciesiwl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xymqyphg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cujfdaiz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ilvwzvfd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ibnoqhcd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qhtvlnll.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlttqmb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jmclgpuq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ypzpztsh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ozkgxnnc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3icbtqqzm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ptvddcln.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cpbkqens.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3naxqtelk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jlronuws.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3avucoelq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzxkidv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qrumtdyj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acsjtjks.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kxqxapuv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jtzrxgis.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3omgndglj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wbtezrhz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qspkxmpk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihegdmcq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rjuedugp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gkajihfq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lqyrwntr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fhfdaydy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mbvedoqu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3otmamkpn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sxrylurd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3elmoghpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vevznwec.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3aqamntfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukzojnsz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3opsijtmk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hfcoytzh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dyodsxfg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3apgkevdm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nxhzdwzv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bacldwqq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3tyghkwfv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ghkgosdg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qikghyoi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ikgeeixh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3indezkfq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zwqcwscj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tmldtknf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3padnkzzi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hmrwzojr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lucwltkf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ikmlvbmd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3arsibool.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ybqcikfb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fsbvjxft.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zltflzis.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ivjdkfbw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3csvxhscp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vbcrfuky.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lcjjhlhc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nfrwknkw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sjilleio.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kqgtdybt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kslsyrhd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dovvqfre.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mvbywrqp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3taivrege.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rbumjygy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jdsdurss.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3evpehimn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qfxxpeiz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sndivamj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3twpwevxg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3stkngnvx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ubntdgfq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3unxfmewm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3plzjymax.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wsrltprf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gmqydwqb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3julnfpjg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hbzrodhu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3psvnlzbi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ehzdptvv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xhikbnos.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qcpxeqyz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ylubfytl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yxuatvwt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qtdyammz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtsowcen.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vwuxehpo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dpcrocge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psguqkdp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nnwuyupg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3csjfsjvz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3joegadwq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3krwwcfvv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jrupwrkh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hkhakreu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vuafjxgd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3rbogqsgh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3htcmchew.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kxhlvbgs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3coxxnexa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ncqqhmom.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dwxzbwkq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vvjegaxk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3flrouzhe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3stvwhtqk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3bhawnoik.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jjdmojie.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jaajbhrr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3siezrelt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqxemnyi.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jkvfjdii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bxwetfoo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gsmbxxux.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cxxrymke.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3opovvbqq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mbltvigv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3iawohhos.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnobveun.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncbsxior.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyirlugd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3atpjnjaj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xgljwqtq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etizogkb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzmaetib.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcnodqlf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dpjtower.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ropkjfnd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oslbjoxu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3qwfohpeh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xgmdsfil.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3smnvtzwi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ganktnnv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cughnlpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxjrbebg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3cifojwyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhkioizi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpskbbox.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yzomxrbv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gyozzuei.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3eianlhhl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3obvacugm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eaxaiful.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xmjskxrw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nkybdzqw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eapdaued.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3eghlbchl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ibjaurts.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ussgvqzg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rvpbmnbe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bdwgvlyw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qbtltjgz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3aevqepiv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mdladxsd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dtrjhdzg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ppvehxes.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3akeakkhy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vjdfcijp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qxkqjzcl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vpsoiqcx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pseqiydg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hpkxxgfw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zmwxmaaf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vqdxnyvj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqympvah.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cecqppww.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3pcrddkui.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fhjjlacm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kfyfbrpe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zjyatlrv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mgvzctmt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nfzgusux.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3alovmuhu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3syvedpdq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jftkrvaq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3seujtowo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3efayrbdv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iujnzarg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3afxhpekt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3scmwufcg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svwcrfyi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qivmcigk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bwdofugd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hahsndga.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jakbdftt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dttsrelb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3buveofls.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xmkarxdw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnmzxob.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3egvpyoom.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3btjjhqbz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soajfwrb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrtcofi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qtjzqxwc.html


<!-- 参考信息 -->