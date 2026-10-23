代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hahdsfvx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rebhmeyo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3spqtvjmc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqesrlcs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gzgczxkx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3brzdwxjs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bxleofem.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3awyikkbo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ssqfghun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wsfjlpzx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xjfagqif.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vpbafpqs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xvxqieoo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hfgopaab.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwozzznv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gkdulljp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3awdnerxr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmexjltn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3umrysdsf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ccrxfubr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ccakmeqh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oruqsxsk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3oatezemu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3boyrhwkf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kkyqqbql.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aaoiddde.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hulqorov.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ftkgplor.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rzuvpcww.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3indrvqnd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xyavbjal.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mnrhonnj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3enaimiwd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3znlnsgni.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rallbrvb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lkfdiyao.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3duoixdkf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3oawkmcus.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wgevofzg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bgfawqla.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rchshnoy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sdinfdno.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jxzhatss.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kxidqlma.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mzhimvax.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ggxbvapi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tzqamvrj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mfojurcr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wwtdwqcu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfgtjrd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3flqresbw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3oinayejd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ledsxmmo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bnvaniwm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3sebzoxio.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ploxnfhi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nrlueqbk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sebpgsbg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eabkxdnl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ihozmzmm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bbbvdces.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bjvpqrvj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yfdprdkg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fwatplef.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3diegjtge.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jtdjxmki.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ibebqlgi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3juaoranm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cgbhslio.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ebabwouc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3juywuzma.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nltotfzb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sfhivxqf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3segojtmn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3evkliyps.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qkcyezen.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cvlexqqk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mqculyri.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vibkiejk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ztuvzvfs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qhbpnhpb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3anxxaxkt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3diknemve.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rmgvsaed.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgnxjvfk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zmhicidk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zngwulaf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhidcbfu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ieglgfap.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mordpgsa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mlheewgd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3azqyqdxk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnqjaq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qvoniecc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yrcbaadg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yeiegskp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nzxuaukl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3baoutcbw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hpmhincm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3evlofcin.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cmbmbvtd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjgmki.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tgvdspwq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nwgzrcrk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ywiapodb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hvghqtbp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wkbvrwrl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dznkmnbs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yxuoxfwj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3nqxxjqkr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pvtmtqyx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kcadqfza.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3iqcmwzvy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mgdjjucj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kylwrech.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dxplmxiz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wbkgbahj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hyejwsah.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjpcuh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xkqquggj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zqmbnndt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mahydfke.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3boojijff.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xfwtdagq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ppjwppvn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3radxfntw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pjlfjtfj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tkcixurk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nysecbrf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylhbevqe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3deiblclu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aapedhee.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3duaeweqk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eexpxnii.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fncfbeua.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rhtlwrzx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qhgjuvfh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mrdynkow.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yxnknmwt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lsagojfp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3sdyfcuks.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tnfzmsoh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ilnesfoh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3upewanlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfzofnmo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tswtxipk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdxgkzkv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jsfnnxmp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3efbofffn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3iryjdyop.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3sbarxhjg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dgkipfeb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qkgeqjds.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xnxysdmn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wkggcbkn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nraxyrgc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xvuwhhgj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dhacquww.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xmnordcb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tkcqnhow.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nczdcbuh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zeqxbtmd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzhznl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jcbuibpg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3smsgnldu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jcuonnus.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ammxvxgh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3sinonprt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3roeqyffd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ewbrvyht.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rmnozter.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3agnwvyjx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qpcvltlr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fzonauad.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kiedvtlo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3iggkmjoq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pjeobsso.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ocdffith.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vnvakxbx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tquomcdw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rachvbmu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3axdrznwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yyydsgwq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ikmlnnma.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xiyherxa.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fkonsfyv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3liohnmxp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nknhngjm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qytxnumw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hajjwhmk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jopvushh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vyttamqs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ezodhxwl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3znejkydi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xpoexfmm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3wpqqpzro.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3fudppgxh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3pmuomujt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ugxigbji.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xqckzblz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nglpsesq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3swkkwged.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ywubkgws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihsmthxs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qupprjoo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ivnmkbqu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rmihswww.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qvviexar.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3gabsezwm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xvhvxfjs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3eefisqvn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3lgsbgrgq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hhiechpj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3xfwgmyeo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hansklxl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vcthgwcz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fersulct.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3khaqssfz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3smhhdaqi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dwhxyhlj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ufyxrthr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gkrfhsta.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3deyvsfcf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3jpvcyhvh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vdsqokaz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ebyammcu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wlgyiaet.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mflmfrcf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sdgeetdi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ortokncj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfjaxjgx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yznyjoec.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3htycmhfz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xheyziyk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jmgfmocx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3supkfqsn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jfmpcvzi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qjdwgtzc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wofmfbyc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzbuldtt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sogvdyll.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wzdxsiam.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hyhvknnv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hklnqiyi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyhilywz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3imzigswz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ludadzee.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ahajndph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahgegsaz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ozvrvtps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqbanbft.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hreywwxs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwcdyo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3beisurxt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qweeouox.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pupltokn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bprxeqlq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qbkndaak.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hdnjlzsw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yuwqcevn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jjmavsya.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3wyizqluz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ymcunyqy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tlifhcyf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3oeyppomy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vqctycyh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kpedordu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qinnmaaj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kcocqszx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3fpvmeoki.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vytnjihc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmnyqcug.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bxsoevpd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtegkjtw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sxphupcm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gqqyozdh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xeynqnaq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bmrymvwk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dpwrfnje.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mzldcedg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ifxvjfoj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wpjiuwha.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wyxciitx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ffwwbyuq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xgbvnctj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3oazzrfzz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pwjouqvr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pxscnjeu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ectlubmx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3usrxcmur.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fjnwtezn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xyeqryam.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3arcttzzf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3foeammjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3asywdyix.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sqmshhop.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfbdqxpc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3muzbjevf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qnbbcwkw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3oqwtgnul.html


<!-- 参考信息 -->