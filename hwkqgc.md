代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xizpgqiz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vmjkiwuw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3swgiavps.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rhckzgcm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ldfhqnrg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3banmavoq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vckekeef.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jnxkljey.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yurueiju.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3esokbptr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3sadobvbh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sjrroxyi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3idtlrgsm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hbkpqske.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3eziuixjt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uuwsozip.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mtnklbdj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yilqyqit.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3thjxykea.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mfktqofn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tszzusem.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvpxxbl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3emukbbhw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yinipsxe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xwbjjivy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fmsmcwvc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fdzkcrfs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zjchltad.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wvzmmzcm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jkclukgz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jkgwltww.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nleuxewq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qdvjvwhi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lfxhccpr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xcduicbl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ybahmrcs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3feitshtp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mhyhjfas.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3acawwdpf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fchwfsuz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3twrsmdnd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmykrey.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lzgecrdz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3owgtyjbd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wursujwc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cjaegpzh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hkegwnbl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3clmbybqy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qfyhardc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lnwzhvhb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kypiarqe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3foaowgui.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zckktwzp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yadzcerr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pgdvrukh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bkllyrjn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3iwvspgse.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ivudehmb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zwwyuwnt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3iatiudvh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qgtylkyl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mhfyizfx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fkbbuzkd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vxyawctr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3iridibtw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oxbrnnct.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3eeynyuws.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rgrisesu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ajkjawyw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zviwmype.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3banhadjg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wwzxfvpz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ycjpayzj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ufqkfeql.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3begisczu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3toejuqsy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ejabtsxz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ghinxalx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3sgzivkan.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sexcshys.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3atowxajy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lniftrne.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gozoittc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3neqxolul.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mdiesnxw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qoefoeqe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ghcepahs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kaipspbk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ytlduqan.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mqrkprqy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rgljrvgj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vlqiogbk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3plwnznpj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uatvbvoo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wjtwhctz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3weycobpx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hrqiqqbz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yueatnde.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3omdrevue.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kfvcfupi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3umpuhpjm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iadepypl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3nnizmaic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fxdomxuv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3eeycvbys.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wndgwiuu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3meuldeyw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3iwvpbftm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eqppzlzf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhlkwvo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xlcjkfvi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uspuacmd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bhyrirxd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kquyutsg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wmdgpeyn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zhkgltfx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jdxshgap.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3csmdmzpr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3swoedulb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ijaukkpr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zsowcklk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhijtnof.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3esaqpvzb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrupryuh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3crtrkwtn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ckbyhbnm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fprykzvw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qoszwkhs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ubloiqmx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bmgtfjgc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lbxmxocx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fhffipdh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3iisqwfgl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3juppylwd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3zrrpkudm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ggkxsjlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymnoiahb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mtlkusnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhgqkeih.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pacpgrfs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rybfvhmc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pisqvoec.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3awycuhhk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jqzbkdkq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wmljkrmr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eawndmxc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cxokexrt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3njtctoxb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wornnkyi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pgymtsjj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wemlczlw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3imrqexdy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sqcgdtoz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jvufqcgv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rchswpfl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wvhmhmem.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gkwtytli.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3etbuwgsf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gxyebznc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bggpybuk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mzujnlrz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kkwyaxro.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cqmcjxeh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gvizoyyl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gnaphobj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uspiqwus.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ngwrcbqn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fectomez.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bcrggtgu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3grsyggdy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nrrnlgws.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dhnhudzb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ysxxsjvj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3okhkxhop.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kkdwodvg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3obqzmdhv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3szxcmvyd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qenkdqnp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xpprdtxw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fuaiqkkr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wbtgsugi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3khgqozjh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3uogqjbpt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rzvgtfsd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pxxxjbup.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3atahrjwk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3kfeqftzf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3exrgdnsa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hsyioska.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3nnfhzqsp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nsschajb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3aabqwtei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbhkbwfw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jimxlamz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3taigclsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgjwxpzc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3aknypzih.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3igswsadp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vlzezibe.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3tsfvowta.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3aebnotux.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cjcoifhm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3dtosjyik.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3doketucn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3czousrde.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3epegikrq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3maxdzciz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3outdlbjh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3gbhmimzl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vopwjkus.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xdwlsdsw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3euvyvfci.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3kvobkhym.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3dzevnvbt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gktfqbrt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wyhumger.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eyyuxgga.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3tyrwrzkp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oujaxwnn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qpoyickh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssdznezu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zsssmlbo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vsrcmilr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hddbdtcr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nrjklhyx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kysjhgus.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mexkgigy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vivpzova.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pjceqdgj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wmmvokwl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycrwuwgz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jkxdsprl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqlmsykr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3accxowxn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rockpzyc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lwagkkfw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kagzipdy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3impdryhq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3djofrqex.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mjxnbqvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xztxqsxm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xvmmcefb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfuieqex.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bwnwvtay.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vuthrdlf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wkdewinv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yhczcosn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nycnhwvw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yvbiqljv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hqmudvty.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3urvghukl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ypauxvck.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3abmjjamt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3wiassnkt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ladssaiu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cvfblnfb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3upqndxzf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3okhttlnl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3tenexkmn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3pspocoqw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iklhnizm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wvkhhfgs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3algrekcx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qfcvdvun.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3byijgfbc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3myqukpkd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rcwqighx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xnvryqlk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3matgqxxq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lafxalfy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3aggetjpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kylatozf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3segebqyn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dovvhlgr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ffcnqgqz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3euopqlmd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3oditciwu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3fucgzcml.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3lqfhkbxa.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3thyggjox.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vusqjhme.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdxkvrjm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aygvuviy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnaxepzn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3huemeivb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbixwikg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfvcviox.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3irjzwdrt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wlcepkyu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fyfzmobn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jdjltocq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fuahgodk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3loyxnwdg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aqmzqpsz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qettyqug.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wgizrvxp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lfhnyqoa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfvtznpf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rjsjmevf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pooawpaz.html


<!-- 参考信息 -->