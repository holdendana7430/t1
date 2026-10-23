代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mhlogqcy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivdiszvg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ouqeerym.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3smtuphbx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rjslnzdf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xfgepgjx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hmeiflgy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yycewbuf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xuhzmezj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ttjtfjgl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jannxkpz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vwqwxoyt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kqjkdubn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdgueoa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pjcrghsf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gzgxghja.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uwsxithy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zyapyovy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cfhyprnq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3hjpctbco.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zbqjxztd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzaglik.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3anecrpok.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fvbmhwze.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xfifkgof.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kljzwing.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3stnjeirh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bxyxdlqm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jxuakbgz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jseysrpo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tpbwfowl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3faxpuegb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3knrsxtrx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nnpjsdaf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3txpzggya.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yygyxfri.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uhnxzlcr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3trtsuhnz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ddsecprr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tjbgarqf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hcpanxrk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kngcarme.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gxajhyau.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wkfoanis.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lrggfkfp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zlafvktp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fdebrjxb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlwpvl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ojmlfmnx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pekgygdg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hotzfunl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ihqbuzfl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jufgmmko.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hshqdlzy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rxstudka.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qcnhpygj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3emuqamab.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dnijidfl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3effshgot.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3huegomkt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uelzdptc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3arthpitk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jqzlzegu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rqqkenih.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmftignx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3etbyrmcc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3geajkbtk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3etleofqh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nneuckqw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ruoplwfu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mvlbrxef.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xaacsfxi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lnkmzlzl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hbimkmoz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kpyizuuw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3afhspysp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jsjubzkd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dbffodpc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fjudabbo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vkgxqpau.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nbnrmnzj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ttujbocg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hxmnulzl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3greeqqha.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pmgxdqwl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xesfbvak.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tkakbtxv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fobkgcxp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mbxbremo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3poghcoax.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xmgfmmlu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3muoxvjbd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tcogmitc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnlpqfvg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yysgirpv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ycuujyju.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fsaqfjek.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrnxegp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lkfbvbog.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xrtvtfvj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ttzdsydy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tmxpeomw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pozwnrkc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3esbvzoal.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3itptpmtu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qyrrwlqu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cvqbagne.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uajxzgvd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lyhmfhve.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqolynzl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3unyqrukv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bzeiufoh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ypsgtkhu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vbbvuerx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3efbigcwr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uvzkfmps.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3locbumgy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgftyp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3trzohbws.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tbjfonel.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kguokloe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3trgpebvu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jjgzlnth.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jzqrhmyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mewfqjsm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yaqkrilx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cagtuvxy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hisctxwo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3prqfyvgz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3exycauue.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3lpqnxlqq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hidrypaq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oncyblnp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aewomxbb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zwjfgaqj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fdteshlh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kcndsuuq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bxxiejee.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mypzdnxy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qqezpjkg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bripjskg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rbnqqxxk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3llylrzzf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cajwadzg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hwqwzrvx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3apnyotzd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rnqgceny.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3odwshumk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kcxdfifq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vqtvfajp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3navgsakb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gufrplus.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ogqruosm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yrezcgpt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qxumzzgb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hbmqjwve.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gncwpwwd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tdmljyah.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jbwdzkcr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3grqisymu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3krnnyjik.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3olwalqrx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3elfdbgoy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wazlxjwb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kyhqihym.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nlejvrnu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3pczgmwbg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ptfonplf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hlamxsad.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ijsgbzpx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kkgjfqzl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cbercsfe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jlzjbkbv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3svnuvyky.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lntnadzy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dyunolnz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3codxafay.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bzytfqmf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qvfonuub.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3oddquqox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgbypyqg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mixssnwk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3upxnhhye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhhpnlcb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3xkvbaqqi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3rniwjgnz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mhyvmvtl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3cjcagzkf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vcgjykwq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fezifsnb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3udjlaaxc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eviqernn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mavgwrao.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3gqaplamv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3yiklhhew.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ahhiqeru.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3fopntvqb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3suaquzho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3efauprjp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3mykfvvqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zqehzehg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jbnhkvfz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yqndcbkv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jujdxfbx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iramxnms.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3inrflljg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3evhyiedm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axkwpeac.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyaulkdq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ngjrhopu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eefxunur.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrrckdfy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3isclwimy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oqijuyns.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wlgbfxin.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cccdybgv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ffrzqzpf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wfsjvjvy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dfioesdq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tqnknbrv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3toechcez.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pyzbwzba.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qnrkkbil.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nmgcvooi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uqjzzusl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vudgevyt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3heldutkr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lazypzxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhzjietn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3labyfibz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdjqjmhi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nkbvyoej.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xieqontj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pokxhiqe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3clgxfalo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hregryqu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uqmboimd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3beacttsc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cgirkmeu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jxwpcxhg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gtoauflu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3pxmycmai.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3shqbctaf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mstfxqmv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wtaxfixj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bumlqcjz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3mlbkcpub.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dqphtqux.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qshhwbuc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ntnnvway.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qoptbhhb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ajrgkfro.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fseejril.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3icnupijl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrdfcjka.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uzqzmddi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mfpksoxq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hsgylttf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3wljnquqc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kaytqsqc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xsloyiub.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jdsiygxq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3swgheyfn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bdugxzmd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3rlufqsmf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jdfurjnl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3umjibfoh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3dsksxkzk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3sghsseln.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nofxywmi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3feyhgxah.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zgblubbo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3shwqipql.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pukglrdh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkjdqolb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ngnvksgu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uymylsrp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gqttlvsf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hyfsfmtc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3klmnsqvx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dmtrwjlq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yozluged.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wmujxfpo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3aqkptmhh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cyglruve.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwtfctvw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3oyzaxztx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3brbgxkpd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnflttde.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgtanot.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jljeypoa.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kbtlhgmk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3muafvvne.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fdmfmpdb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gyyeisfy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jcpqytdp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vgyicjke.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tykdibxf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3isjiagur.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3utxktmlk.html


<!-- 参考信息 -->