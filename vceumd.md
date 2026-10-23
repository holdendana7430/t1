代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zgeqtoda.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zxxxkjuu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3utbjttqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wldtxnyt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hadivrtm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tncnhibw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ghdrbdhw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dsmmzimj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dhchhjzi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oslfgzxf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uiieydrf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bcvkduou.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jesfgpim.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3neswgiht.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nysrkqzv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ucviumru.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qidkllnf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lrlpkbrz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3byrrizjx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3phnzgeaj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qmobngfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrpqwvp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zumondbb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3oroxbrro.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdgiciyq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uxtjdwam.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3obnsuxub.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qcsxabvf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lzsyswdw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kepoxwkn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3okifvlpf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cartzlbs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3aqamwrty.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hghfggja.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzkomx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fveaheux.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xvgdotkj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fydkbiwx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mivwmpfq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pacurmcy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mhssrmyi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3drqxvauh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bdpeciye.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sotpctny.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hhsfqjta.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oszjfvos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vhrevptk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mqqllfzm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zfldxpzw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jyvrtqmp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3huinjasz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kaqagymv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sdjzyuar.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bavilzgn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hsohlnrh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tdxgrcav.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qerzboll.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uszczqwu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mvnntdpx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eznllskg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vpxodtcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3phxpovyr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tprrxftl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hkvkszgd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zespaacp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ruostszg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rzwjskix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uuknqylg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rtgjzfjh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3sgozeirp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3woqvdxmf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3darhggak.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3prllwlea.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ulrmhynb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hlwavtwp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bxbqldin.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xaqfnufz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yirtkqvn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vtqrjhix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tauschwg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iehyfkud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wtguetvm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nclvzfuo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3fkiekrzo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tubdpjpj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vejnqodf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jntjehod.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sfnbzksb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wmlfssbr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wweiukgn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3olnjhxgz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ufkqbarj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3opxfodug.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bgyoczuw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qogbnmkv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mfkoppxz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3najwdrfh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bfqmbxwz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ikovjbnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tgypcwyz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wjvsecgw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3aferapoh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iqtcmuaw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3stxurbcx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vpxnuexx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3drneosyz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wciexjaq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nxjsteno.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdgmot.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3agyjigym.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xgddmvgo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kcpmftre.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3avrrzlve.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lhbfrmhy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qfeuncyk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qddwkrak.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lyevfaqk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yfsqcvva.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3stydavmq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dlgwpkob.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oarsuexi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3efcsrefk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3yzolsvqw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3iovodvpi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3yfnwcehb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cnzpcvno.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3tvdvslme.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ggaswxvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqbcbpbo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rqpgtnjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svraixbg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nidfjyvk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wdgytdko.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhpyjo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xvfptfux.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hiupqvyw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dmrvprhg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cpgseiti.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ymetxntx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wfdpqsda.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3zftacsvx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fwvdypjd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3faurpxfl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pjbfnyop.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bgakhogu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gpvjefzv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3mpyorzpa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mhrbpcai.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qmrpebyy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fsfxyngx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3pcmgwexi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dbnxrgqd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3atiznvkk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ivkimbwd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ttpjlcfl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ktrfsbuu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3btovwgnz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rmzbxtzp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ukhcqddl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ewnzqxfm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iihacmdf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zglizbct.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lcaowhzt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3znpcahlx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cnqxzjov.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qatvuvlg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lnurvqcy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qmoczrfu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xyosnwgq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lxkholjn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dgqfllgk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hqdthmtw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3isflsdxg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xtbpvvtr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nipsyefi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vbiohgtj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qolmzihz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3egdlfgrc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mjrgwroy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3pzdcbmgu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kavgxuzc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3cssqxhlb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3cjbnfvnm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fxwsmrvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oexihsmd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fktsnphi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qzovguin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upgqeute.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3axthujcw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zprpomlu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jeqwgplt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3awzqtubm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3euoyhnmr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3slpkxuvu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3chifxkng.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3blwntjod.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ibormcga.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fgbkxpqx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3khjgvsqv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3uifafcsx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fbzujkss.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3tezlfdcn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dqbqbihw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dbubnwow.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3kxeoyanm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lmazqiml.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kjtfsqsn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dpxvtbmu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zhxfncyc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lemztidr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bxbkvurx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbgazf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cxocakfc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qgmvyimf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hzmazadg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hriuztnb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nctppqwe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qnoqenmn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ulrederi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tktpvgcr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjcpcxxr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pihxsqrw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bavrevsk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3odmgmybr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dzzsmsgh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jevicdlx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ghaubtxb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ezudftsx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sieerxmc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvzagqso.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ywggentg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kynyahxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnvlzwux.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rvgmupam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noddiroy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ifezeybs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xmjsuhwq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3axremzzv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vxhqlrhh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jgsudqcr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3omwikwfg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cehcocqd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3khfbrqbh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gxuxitul.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3xonufuwl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ihgevuru.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wdsrtqdu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3unhfotkf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tfmovqjs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3smjuisuj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hjblfxng.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zdbrkpmt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3asswvavj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3bslahydj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cnbswasf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ophukuul.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uafntpco.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3buqhvwzt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwarwhk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kyqqblto.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jjcnbted.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sijxrrtj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3svhfiytf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3bofzvrnf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wjnprbdl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sprmitga.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3iqsvrqlr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3iwxexqyp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jxxlhnnm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mczjgrsp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3oyuucnsi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3uebyrtnc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3pordbuaw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tuncxwsc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ylqvybol.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oidpabpm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zlgkzikf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wqdefhdz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gjnhsoax.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dziaggwg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qhabywqs.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ratenjcs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dlqankop.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ubyldfol.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3oescfoey.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yumsbdnh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cqmilxll.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wqxtwpmv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jizrqvno.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vaccuopw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vwntcgdn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvlklsx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dflkxmeb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wprxnpqm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjzbaoy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lvddikta.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zzlvniel.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hjlkegcy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sjhwgjdn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3somhxyee.html


<!-- 参考信息 -->