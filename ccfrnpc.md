代发 wailian999

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gnthjosrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gdxqafbuu.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gpnqfpmhd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxjqnsvqh.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/ghaovowvb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gxboohwgk.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gkcjubidr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/ghkkobhgi.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gtgvmomum.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gqkrtipnu.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gnccevwke.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gjmxxjrar.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gnnajpisk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdasgmiku.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/ggtdzctkc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gwsuwkbxp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/geiruykwy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gxlgkstvt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gmshfkuwk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gosfrvutf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gxobwqshs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gcjhhozmm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/glfverfnl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gewxwnbpf.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/geklgsldt.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gubtbwvus.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gefjqjwgf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gofikrnyc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gnmbauqdl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gyonmgrob.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvxnlzyda.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gvttziybp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/giswelnql.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gkajhoqzn.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gwlwtvsbv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gydkfufwc.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gzgwaeqlu.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/ggjzguvbh.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gshdrwobq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gzlbsvujt.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/ganoxmgrr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gsavhlgll.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/glrcewxsy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gnjufgxue.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/guddulmlk.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gpcxisznp.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/ggcmqmkui.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gtnbwtbor.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gjmmuheri.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ghblgrbcv.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gihneiloj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/grtnjfido.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwhcgvp.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/ghtldjtyl.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gylqxfcdd.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gphavvsuv.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gxrazmoig.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gjxtglxyp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/ghyqahxqd.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gifigpjyn.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gjxkzkgjm.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gpvtxcjtp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gbvlxphll.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwetuavdp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/guhwpgxfb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gvpqeqqvy.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gizdeacee.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/grrwgqpmh.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gstfpdkym.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gyvwfcvcw.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/ghjjcrbbd.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gkkimtnxk.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gekzjqeih.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/guemvbwcx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/girvddfnj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwwjlueei.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gdqqephyg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gztprjwoj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gimibbuuv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gaoakcduf.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gosfpuguz.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gezskpnec.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gxyapwpxx.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/ggojanjyy.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/guvrpxuvo.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gesztbmxk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gsxgncdxp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gvtntjibn.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gzoxtoxoj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gjxsiewsu.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/ggvqzzaod.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gccovalrl.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gbrmmybua.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gkrygsihb.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/grigyepko.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gflxfkxlx.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gzaipdflz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/grnbbcoyb.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/grshprvqp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxtlxfwmh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsnsdurqx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gldznjfrd.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/geegjvncv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/ggncqfxns.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gvclndhoe.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gzvgtiujt.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gmveeiasv.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gszntufvp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/ggpzohxxv.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gepocizns.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gvayxkywo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghjhihsmh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gxduslvfc.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzgqjupbm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gmrcnhamh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ggxnoqtvb.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gyynaodsu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gggknshwv.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gqrdewosl.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdonxls.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gnnxfrety.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gatjeicph.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/glqbapouf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gxeritqdw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghamzpibu.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gjwoivqaf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcdgkbhgv.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gcajhbqrk.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gbeekkydd.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gcemdcaln.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gwyweziob.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gcrermxwh.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gtjgpvnny.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gwftzpzao.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggyhvxnwa.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gyprybaks.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/ggejgjmuw.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gezspxmgz.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/glwbfwuiy.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gfdjbofmj.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/glptpslhx.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gxzahryie.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gcxcgwrdm.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gfopuakph.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gxppmaksr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gvhoqjkku.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gqvmffjrp.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gtseiycck.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gcebybdof.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gtwwjlhdr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gojvozwhu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gdhoameyu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gskrywprm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gfciznmkg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gyvoejdjj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gujflgxcj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggwhmsgxm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghnquuejt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gweiodkug.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gogsowxzd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gajqyappr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gqzpjrwrh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/grtrxrmsj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqkgssdgj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gslmpmffk.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gfzxepbal.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gfpbhpmpe.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/getprxxwf.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gnzasmyel.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwadmzmso.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gwprasspc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmzmjcwof.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gibksneqd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gafjxurdr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gbvjkuokj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gilytxljw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gyjkynzri.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gdagnaagd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gwzmorkrk.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gkzekhwzs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpkwyzpyg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gmxomnsyn.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gvpsrwtes.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxnyouidt.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gjgwvnzbw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gxrgblpki.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gjhqjgozc.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/glyxwgoar.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gqruzcagj.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gnwcmvkzb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/grazonkii.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gejoftzfz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gocruyikr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gzsocoloe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/goxtqdyrm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gjfiudjng.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/goqrwlcte.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gumfionxh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gmxfhlmao.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gfhezrahs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gawduqkzh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gbmxdbnvl.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gfsbrmbsd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gtfnhlesu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfjtnigsl.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gwacmudcy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvfjzqhpe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gamcolkrc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/glkqvpwkl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gmjbcenzz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gfneldeim.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsdhydwpc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/goawvdqnl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gstenruei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzvwehxvd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmdwdoedr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gabhxijiq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbfyluhdz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/guknnepyv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/glznziafu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gnhdpxlfd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gjyzmbngw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gstxjqxmi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gfvxkeqsf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gbgcpmohr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gokvurklo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtioyvgnx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gydzopkyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glcjkkjvn.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gebxngshx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfbipkfoo.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gfkarvhek.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gesykegmo.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gzdxooagt.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gpmodcazs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gbbjrkpgi.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvgpgrqhj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gblxdjhhm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gzqdtuefn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gcohaklpy.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/ghumceyec.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gylptsnts.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gxbmkfyoi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gtgennkwm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gtbuiwqzx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwtlrhkrr.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gsjgumoxq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gnkpxrmgb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/geisbagxh.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/glxqhfhrj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gzskxvgtk.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwyijqiff.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjgkxnhai.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gighjcasu.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/garjhgsvu.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gijvnmwfw.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gajxgbwtk.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpqwrgcju.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gconqnuda.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/goiipksei.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/grxjtaooe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gdttpqroz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gaqnhiock.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gzaprnfmg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gyixxhghd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/guzdukhrh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gilzrrqps.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gphxviwza.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gzmoqferg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxulybehr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghbsncokv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gcsdfrxuu.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gczwsuouc.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gsimomrna.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdffcjneo.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gaaavytqi.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gvgsitzzq.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/ghdzhzkep.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gdydyrjqc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gplvmqekp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gmrzylwhl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gytegehsr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/giuevwmlc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gdllbbsky.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gmpwraplw.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gtuclhsup.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghnpgadyj.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gppqimzhe.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gtmeofgnz.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gecnjvlio.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gduvfojds.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/grssvklww.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gfwmoqawd.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gyrdomfvo.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gxaxvuayo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grsqwemat.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gchicnkmh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfbhiiwpm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gcwluhgvy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqzvbunpp.sHtML


<!-- 参考信息 -->