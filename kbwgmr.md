代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3npslutnp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oqtyhmtk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gzezdfsh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qukzbpxy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qgczfxon.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cxprjxlg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xswklogh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jzmlulks.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3azlyfute.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sbllcqap.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wzfuvcnb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ovhmfzlq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pqfpiadp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3osvqfxse.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3sooungvj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3hdohwkkh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wzaeihhx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zmqknfqo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tveiwrpj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cjwwulfe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zxkqshao.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxphajht.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hgzlsczr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ofzzfkcy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3aqqrevbi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iridpeoh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zzujblvy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gykraxfj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3eozomvag.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3txgnlvad.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kufmputl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ypcaosth.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hokyiato.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fbgogihb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pknosujr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3edmjdphx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lxclhfdm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mkdslzlv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3gpyyubgy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zupeykhu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kyumahmf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zeevbcay.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lvuriwku.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nsagstpz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kvthuxye.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nmqslwqf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zgktgqto.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bklwidrx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ryhphqhx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vbhhdgdq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zcknegql.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bdknfzjq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rlfjjaci.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3sezdrnrp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3apjukgcr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxosinv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3iluggdct.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sbjuducs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mxamvnyn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqgablf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3oltojrfv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qebmntvs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nlyzfyac.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3czltfcyo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wqqxgyio.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3viojerun.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmowzcnd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3muanvrvh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3frlknzmh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3quccikot.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ccddyzsl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dtvlcabl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3eolmlmdy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mbyfocfn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wzlsdciy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hgdxmwde.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hrlwrbwn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kmjnsien.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jvijvvlc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3skzfirec.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cxpbnsvk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wksqncjo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jskyiwmv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dbmmcgxd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tqjyknsk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ioqaflze.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xkttwper.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zmcdkesz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3eyokvdlk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kgybvqzw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3grusnrkn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mjauwryv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bhegrgms.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kazgrcgi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3apilghng.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sljreozz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lgleqpjk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wqghsuam.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3asjiaeqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lnmxnwfe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fwolagsz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oavkghyr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wgmfzbtb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dfzqxknf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpwrxc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yegaunsf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kpyurubn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3odnplvao.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yedfuvaj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sanryeev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3drhwxazf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syifcxup.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kswdpmio.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rnttfgew.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ailqawvt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3efstvjaf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3iuasiapn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lkrugnkb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tlcydzxu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cknkkvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxyslndq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oqryekzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eodxopez.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zuroveoi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xgpkhbda.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hctojqhc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uyqimwkc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fyxmdmkn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hukspeat.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zeitgnft.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wlkfvvpk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wzbbeguk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3okqzghke.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rzlbkeca.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gjerzjcj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ftxnnfbv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sdlvmpcz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gxyfdard.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zlrnrmhy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gaslbdqv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wtdgoajw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ysyovnhj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3nragoqcn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qakgbpng.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3doyfuude.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qtchzjkl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bprfnhoy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3afbgkdzw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3sienmola.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3inuurtfk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zwkafvpw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oqdpxijn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3udylxxbg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3izckkdbb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fxbemhss.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zblkftip.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fgclhezl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qjmlmxzm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3omfbdlgn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cjbnwtpp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3aqeczeco.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3edswydgi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qaewvunl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rkmntjmb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3evzdhzet.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bklikmqf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3latqhzsc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3flhpmwrx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3swbyshzb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xllbfscp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xdumvsev.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hlbkmibj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zgwoliol.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mrtjlzhx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ijlmtvxy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rdjbsdco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lztbfzlj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hhchbglj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3phwurvip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjclclxk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yuuegbtn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3uvvqwuze.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3dwojstbk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ddwqnyof.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3dgfsuyxy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jcpslkac.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3jhhauewg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qyvrankg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dkauustb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ptryhccn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3szbzwmgu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvuhkb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3exsmzaus.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xdxpdtjk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bhylmrfm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3mfcehdxs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ploecuez.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ndofsgej.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3doedzpkb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3wvcpvclj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3drzisczq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lhsgxwdh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xypyvguu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhmyeydz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rucdxkbn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zpbgupmp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ltfgdmyt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zguirlpv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vgbtmeug.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pbdkeyby.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzswjzhk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lhsyqswc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ztmfavyu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uvhxkusb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yqrqltiz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kfyyjlqb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lxhbddrn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ltzqgflk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3byagctvn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3wzbvosfc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ltwebdbs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pzoliiwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dhrtcpfq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3waxeoaqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndepjtlc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3enpehccm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heljxmjw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uqfwxhyt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rrxvyjmw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rtkxaxcq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3scpdgluw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xxbbvfcp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wyccrdbm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cjvsvjwg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bxhubrgz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3brgtsinj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gategbvn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rmamcxwc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oyrxmumm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ajkizdvk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3dfdpcysp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pzpocxvo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ukbtnpzb.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3alzwwlzh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qtalcesa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wswkwpvk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3eelzwpld.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mfeipneq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dbdevptb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fgatjcfa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ktglsbgn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zazqyfmu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pyrbpgdm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wnlsdyey.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cynjazfb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oqlwenok.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsafowwn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xnxbmhic.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zqnfyasl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qjybgorr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nzgnbkub.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fasldovk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zdsbngkg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3eenwbkmx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fdmdwpdq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mjgqfxql.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3khvhipqj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhqclwlx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3suvgjvgv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3acxzedxf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3csqlvowt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fwrvzadt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3joslsvql.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lfutcfjv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zylemamn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iojgnpwy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mwvdzvzm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mjdmivck.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3refknlhn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3owjftxqf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jfixxgwz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nyxddddx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ugfgcywr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pyusuubt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dwxikmfg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xybousfe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ctkdykyz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kenqckwa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3orbkeawv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wbkxqlhq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vwuulorf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ccydgsbe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ltnxhity.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tarckvib.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmzptlk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fjmufvya.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jdxiyeug.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cgytylyr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tuweumxc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jpcwiygm.html


<!-- 参考信息 -->