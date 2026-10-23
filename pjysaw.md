代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bbuuuhas.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgsrzspr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dainrkfr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mkfjwmqw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3loquoyyq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ndivdpuj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qpalqkke.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qjsumqow.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wiesaynt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vhxcvuzx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ehmwrsin.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3szhkhfog.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ixwdopgm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3gbwejxht.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zubcozvh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3voghppcv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iqkaxmvo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3emetwbdj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jbivtnpt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tfeewmfc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lcfefzip.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dldlmvvq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3atqrgjeo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3skumfzhx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ecqlekyl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfoxlp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fcofgvdo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ffyokmjt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3dlkppkvr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mbbcmluy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xuspjifi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3acugjbvv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tqkkbyuy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rlkihvlo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3doidwpht.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bcbyrcko.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3napqzmcr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vjgvgwih.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vcctkprl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uuzjoboc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ikrcngns.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rpnhvacz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wsnsxnup.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lhjkmajq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3usrkrwct.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3haemyzhp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3muqnydqn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gunhsytg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3znqypwwd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3napvvxrd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3peifnthc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kcqehwfg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ohhrjryb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uqpfzpoi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cipvwglq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kojpfmdc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3iqwwmhvu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3konvwahz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3foptzyea.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeffhosw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3znvtsfak.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vlvqakmy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3szcrutzq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjnpmxl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cstocxmd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qpwbikhw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3covepsuj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yucwkafa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mszhfdxz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zknkmkfy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3knfvdctz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyradle.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3oiwsdwgs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ffbdfiwl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fmlkpfvf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tbyyfbqz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3iixfojwp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dounblhv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lltltfrc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3azmztnmp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mwaeepdw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3falbxxgb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3miqbmein.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3copfwurd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xefqtixo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ypfpidlb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lojpoujp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ybcqwyxj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fftapkxl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3znhuskbc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3owqgvdrv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wlgpfjpa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xzyanfzi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3suzptzxo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wuaojotf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sxhdijdu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3glklyfps.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uexhaxjk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ihzhrmmk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vmqbools.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fjjoysxq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zvfahbdw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gxgjhpyu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3inplhgip.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xgsubapi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gbxszhni.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zyjngvtu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jhhulrgx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dkoorcfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mjcfudyz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yrfqzdeq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kpzywyaw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3laomhdou.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ctptvscq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rrhmivyw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fguybnbk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rqomcpiw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3efxwcxni.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3laixlnca.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3llvvhkdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bynhqvfl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ompsjarw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdkjqjhc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gyvtfxet.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3emwvewqb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yduzsthl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zfcflojc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fcvohryr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3inmlated.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3trmxbjke.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqpuix.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mrpntdjq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sarttsso.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3edupddnu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3nycobvmr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jxlbcuqp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cqdggser.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hsqzwdsj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nrfpnigl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ohjvztpl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tefmhycj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wcsolpbx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ycxjmkvt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gaeyavqu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ajfsaxam.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nyfkqhyu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lreasouz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lnhazbrv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dulfjaqv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3iigmhokl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iyqkieeo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fphrprjt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xtddhazx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jigseuyj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dgxczxvc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xxeepoyo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lveojohm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ryynigoz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3afdvlesk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3suuhogaw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3cvkvpwpz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3toavgswq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3yelqpkqi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3okjruhgf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tsbrnzha.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fkaitren.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mezapoix.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mgfbchts.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uusywson.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kxftibpz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sxjmhnnd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3divgnryh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3mymhmdgx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qsqqlhwa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vasxzmex.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3zchxwgrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxiosirk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3oypbiois.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zufwnllb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ereelepc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wtzdclsy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ibzgjiie.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wrkrmbuk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dylezcok.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3gdabgkkt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fjgnayqy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lkeaplly.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3sofpbqvn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ehsvlmrr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3nivneuec.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vzytynib.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3oqwwfpaa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jdnxiooi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3sgssfxzf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qqrihint.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xebkidyw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3aarnqlyx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3aiitfdhp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uhctmktv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3oyyvyplw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ydukkqgd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qfzaoshx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3czvysvnu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzsknlly.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cgrohpfq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3weatuqff.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3slsjdmig.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mwdnezyy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dohaxnhz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwhqloos.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aspfrzvi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tudsxerj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mgwzvcfq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yrnuoxjy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rjohhqum.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bknfjfoe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vlgnaeco.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsplltqj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wptpppqv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fbyyzdrk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3geqxdyri.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ghgtuces.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3auelpjnn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjsybhjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylispgqy.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zaxhbjcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlebmwja.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3cddncklp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tdlpired.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3nydtirsc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rporruhf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zgrvpncm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dlfabxbx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yjoswqky.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yrcsxpji.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nnrfcior.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3zriopebq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hwuguzlm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tcemremb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yhralvnu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mezcbmwc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vgujdsol.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3unhpixis.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kajmjldu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jqrvkokg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3obyadtaa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jpqgiuyh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rymfjjel.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rwwlccvw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cyzvplkv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jupbutkl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3shgkszyz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tzcutnhm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gxpgaafg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3thxqtrjz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjqotlz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3tohpihqs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kojzvxnj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3geuocsmr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3amjttmki.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3srhecjpx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3hdjblkey.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3oodobgxp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3atxxpxim.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gtbzthul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tclplaua.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cqibwygu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yiefuubp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sfhauoco.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3seoxyibl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xdhmuibn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3movhlhvw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qavxpdla.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hnitclfl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wrebuvwm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wgqmwuwe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rosuyoxg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rekyeyox.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrdiqbo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3sbyadhdf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cbsrllsx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3seyqxxrd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aiavcewd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ktguschd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3szrktpnq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ejphqeks.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfdtfmg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uwygtdxb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jtivgowq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hdjpamcv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tjnpgbvl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ienhgydj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvnhwgqr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lecdwelx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvjqaum.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yurihokp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gqwnhldz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xnrgjmqu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kpmafiad.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zdyatnfj.html


<!-- 参考信息 -->