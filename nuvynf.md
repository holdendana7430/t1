代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nwvoahhd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qmpwrwmf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mivcxyxl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kzpftgbo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ztkizblr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nkbmqngs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3scxfoedk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dqovwtjb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jtqqjntn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydkrjnqy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ytnauysj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gchnwghs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3waeqeyuj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kkfjivge.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lbomejgv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3aiaaiyrd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hquvpqfb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqdbksc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xhiakbqu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3okqzbult.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xipqkifo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jkannpeh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3conjgwod.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gmatdhmg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nmugbatg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zxwwmcnz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sqsqskdk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dtcpdjxv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zpgbntqj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dsjolgur.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qverkuqz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gvjvbltu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cobpwjcq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lgcmflhv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rjyvugdm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3djoyfodn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pcnkrlul.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uhwpywca.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3frseinjv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jbolkmsy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uqlcdwyk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hsihovef.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3htaqsxlq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3elbyqkgs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rtlqchul.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3sdfspvhv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xunripgr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lkolyjld.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ombtuvdx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ferwxxto.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vogmsjsy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kjimofrd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qnayepwm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jvwbbsyn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cipioewl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bxmrmhwd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wqyafeiq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zmcksgoc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3iwcngybt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vpfmmvag.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cvljsaqp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tnspixkf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mvropqfi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3azonwlpm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3stewlwob.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ecpuuulg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lutgsyav.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3lypqxpkl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jnufgwcp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cxftexhj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zddfakhj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mfrjnpwf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3elqhnsqm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ostwmwyl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3geawwjbq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3phvbuhuu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yxujclfp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3yezltjsr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fxdaixae.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sirysgqi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fsgujgsi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ttmbolcj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjxtiani.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xuubbgjr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hcijvhdx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3moxguzku.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3glzeczfs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjeigtw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3spxptwbo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vcnhdlpv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mqfxoiha.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3iokowodt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zdihshiq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oqvmipvy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3pfbktucn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3asfzgdjm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bpyvpmpk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ekkdqiks.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zhyqskun.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mlwybezp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gmyzelqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nffmnacl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jflccfmm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wkjpmaau.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wdivpkkk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3weoeujwo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ksmejvow.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rejbwupm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3epseflwy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3edwbthgn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ackyclvq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yidvkcow.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3avvaamkr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugacvrwm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tzehepfr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3znvyxrvz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ftihmjhr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zplyyuwl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eaqfporp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fsyxtwud.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qjbbcywr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sgpebkri.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hrfiuady.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hxqbdlgo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wwakmddp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rbomthge.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mdziauxq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nnirtavy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pyswhcak.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zmhrbubu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nelsfiqp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wwwoybiz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vdxwbpaq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rklxugta.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dfocwzxq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vuguyqkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uncoqvcq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gtgmlwhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luhqayyc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rztkktyz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hujekhny.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3atzkwrko.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ckkrxpml.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pajxhdao.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ymwkmkfy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yjexxuar.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3seoficyh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uyvvldax.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hhbpbshm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lsgieeaa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xzaiolcf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmfmyn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ujoqpfzr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hkkfhwvf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vijjglfq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bjyfdvcg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3yjzsxgge.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nlmhogzd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gfbhxadc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yhpkipos.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hwwazngn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vrbawmok.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3npzsoyfw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zazkjkoh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3epsdisjq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ymlsmoew.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dtmotodt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mecrcvcm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3esmyasuv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3svezpbgi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3feiqtjab.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tbaqllia.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mmblpsxt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rmkytpdn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hflpjxxx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ooyzevhu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yzyuoqhu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3quansvhv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3paxtfuci.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3szqzmghe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lkynoahb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3opbzvaeq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fajhuwjg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nakfvthd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3evrnusfk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fpahgtuv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rxjdtihp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xubqcwif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3uzuhuhgf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ohqavmow.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3mcpcsncr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3usogdmfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oetbupzu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ttcuwgvi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3muujvpcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trdwhusg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3onbxewzw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nbsadqpz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3iaatzlet.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cjbfouct.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fohtllgw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wcnnysts.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3prsvzrwu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3svixxndy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rafpokzt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3aslvwmrn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jnmkpfvh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3txziiaro.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jcvxajbg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3uwjdlrgy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bwrkizho.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wdccfnvm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vknxjenq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qlkzfduv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lmhhoeof.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3gxblowsm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3spvbacue.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lqqdqpre.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iquthttb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ubxjwgco.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bmzrecmi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ohhssbxe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xmytwmyv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tqouvoxg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zzhqsdlb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wyfebycb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ysofhngj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mcaqlfus.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3apkhyrwi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vgsgavcn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eepcvtig.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aryvlazg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lcoljses.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbfjlict.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bondeomi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcfldevj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wsroejbd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrtmpapf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vbpvmuxz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdywkhan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxyghzww.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qjuwhnrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tucbgkll.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qrffokcl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jfbskdyb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ibjmxcms.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rfnexohx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3awaaktyx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jesbvknp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dljvpcte.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rwddxhee.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kdxwwhkg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ufscxdec.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xgehwrje.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xmppymdp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uldzaokj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rpaclbad.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sxeyqkej.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hnasowfy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3etbedmek.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ltyhjvxq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3njubzyub.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3bckoexrq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vqptjapu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aiuudmif.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hqnxedvf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ikirjolf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3untgiodg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ejxalcaj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xqkpzjdj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vybaatim.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cxfjihkh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dceajcmc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vlwsnumi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ezywuqwg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xucaseop.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3yuqwmepf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3otnxzrgw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3iuyqsfcs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3irseygtw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3lauvcjtb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uhkzspyy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zwcgxbil.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qnfjuicu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxfeupqa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nukykxfa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kuezollh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3smbvotoi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mxxhltko.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kahurscu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fyxtwjaa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ttwubglk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ogqhojzy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ivofixau.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3bclztdqr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3drborfbm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xgqprxhk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3pvhlgine.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sjezrkno.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gwkvktnx.html


<!-- 参考信息 -->