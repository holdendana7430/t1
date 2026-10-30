代发 wailian999

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gjmwhlzpv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gbbggvhnd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gulemnbdj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ghiaijqls.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gvdrvcqyy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvbepkszb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gxzkiuoev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gcgwmtjgp.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/ggikmljzo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gstbpxwpx.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbivigvip.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gwkgaujjp.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gficqabxr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzplewurq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gvcwzbljy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghtfvulqf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/glizpodpg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gqaptqtsd.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gedwshijc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gqmdwtbhb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gbqygmzdm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gvamsxbks.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gpotxhnut.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gkdoywutv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/garpwtnns.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gwpdfrzhv.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gjqyatjlp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gjgqveabl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/glhxpxruh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gtrviemuu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gbbixrhez.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gwzlukgyh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gdhngublg.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gnsqqvamn.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gofdglygl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/geqtlgmmi.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gsybechcr.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gtsrdwwqj.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/guecblgdx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gtnzvcdfd.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gwreupdgu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gnvlkcftr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/ghpirdfyt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gzjpurvgd.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gdcduoxso.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/ghdygpsjt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gyfoomblf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gbpkndaju.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gejdmtvbt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtemeqgdz.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gyybxzphj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gixynbqjz.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gmzrordoc.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/grdjygvct.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gsuolyvta.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gmfoxylrh.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gdbzhwdsm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/glsplqfnw.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gjyogfjgh.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxouiqva.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/ghigbynqe.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ghmwvzmbw.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gtcghdsdc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gzylwdfbq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gnmyoakmb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gemzhzxuc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gevksgqac.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/guwzgijjf.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gtbyyaaqx.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/grnifiuyy.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gokuvwsuw.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gkcqlqmkz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gdiypwjab.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gyakqtvcz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gayecbnqu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfrruosoa.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gegruszry.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gpecgxkhm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gkgyxhstm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gshojcgfi.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gunctfgye.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gdmiwncpn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdemijshj.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gqvgdjryt.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gyixpwupp.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gcwqabrtp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gptyjgqov.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/grcpijqxx.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gvenalqzk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/goayeqpad.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gqnubuvqn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/genqoeuhf.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gxtpryzol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gzvuelzaj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gkbdpwbrc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gfykjtfzm.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkcpuqbaw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gkjypzzph.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gukztyizx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gpoqoabza.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gclvxowrw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ggmyqumsa.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/grqbdinvh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gysusfoip.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gkqosgtud.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gygfzvnug.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gtymhjeoi.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxdbyljlh.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gytpprhmf.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwzlvdcln.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gftbfjoby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gaotjwize.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gcdmwdchj.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdfzmtfvr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyzkzklnm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/girfigysm.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gzpmsicff.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gzakoqmxl.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gkwjizbfb.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gcidsvhgi.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ggwgflmeq.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gxilyecnx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/guzwmggad.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gacmlawxu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfzfbbwth.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gerkrewlm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjklxekff.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gmexhqtbp.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gqbbetgay.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gqehvuxzw.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gcxbfnvsa.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gbmqbwpto.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gcjwlwxgt.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gjzxablyk.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gzslnevex.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gdcekefkk.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gdkhpdwgh.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gzlhtzuqx.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gnqzrpqrk.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gdyiifnat.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gsuaayyzr.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/grqwtjsou.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gtmfadqyk.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gidafnieh.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/ghgdpjdby.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsdoezvqm.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gwuiylyde.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gnnpokuce.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gistecnxh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gmmrelypo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghdwfifku.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gyvlvtdwp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gerlpjkyk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gjohklics.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ghvghamqv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/ghoncsozf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkjxkzkis.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/glppowizx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwllicnrz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gblsgsdwf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gngwcshix.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gbdqgigcm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gohtzgcrd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfhydddbm.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gbhzazajy.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gwmbiceob.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gnyygosau.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gijugwipi.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/geilmpuka.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdvinhhke.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gopnuenzx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gbkegylti.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/grabtemrk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gbplsdznn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gfqgmlzdw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gxafebddk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gxmndegjs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gahieowxu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gktxvejnj.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gdbxzjhfi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gztudtoux.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gjteibrhr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gedhhorxz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gicyxuypm.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gvfznzvfs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gngwqzqsy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gpzhdseor.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gncmemkfa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gjzkwpprd.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/ghrmpzvpz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gjngzkkru.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gkxbxggup.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gltnuummk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ggjmealdo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gxngtypkk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gxudyduuy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gchkpmtmf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gvehechkw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gnpcjizev.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gorzzddmj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gctmiwekm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/ghaxtpcem.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gqhmcqzzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gqpppfdih.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gihvghmvo.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gdyommixh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gwklggdmq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/ggcmhlnlt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gffrkunbw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gvsuzklvb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gftsdaznz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/ggnzbbujm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gfygfvuwa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gtyidsysc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqkvvmxch.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ggavyicxr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/grtyllqof.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gtppiinxs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gpefzmijm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gufkzfukm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gdykdtnpc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gnmauapvx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gapyfgkua.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gkkyxfhtt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gjdxetfqg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/ggrbvmhvo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdqmkkqfq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gjglhudpe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkbaltzqc.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/ghfqimsbq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjotoyqal.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gugjkdjhd.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gklkuuvdm.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gbkzfumfn.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gfulglpey.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gojpaijid.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gyjbifsfa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gcznudpxu.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gqomjzhqr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gegwxcosy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/grlvjjlrf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gedpsscbq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gftgsohqu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtngxhtaa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gfseymncw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gebvokzqj.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/ghmizoaos.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/grwoyglys.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gcebrwfst.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gsjcliqar.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gtzuwbena.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gugxywssq.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzxjlggwt.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gthuhkpkx.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyobnggeb.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gsjwqcudz.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gjsxjrqvx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnwbukooc.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gubcsmdcl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gzzgabvic.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gdyyumphs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gnbndpghk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/ghhrqvfby.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gdowljcqn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gurjzbmhe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gedntlojv.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gyaouzolf.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/ggiqmhcja.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gpwcckvgu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gghvrgfhc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcgcrcogs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpmnjbsfx.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grqdwgvyb.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjhcrucud.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpqnmldiu.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gegcxuvdf.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gfkoqmjfm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gddsglnbk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gylqaougj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gsrzgsszg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gnnpnowef.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/glnqttywu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gsdemvbir.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gxojmtlxe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gvmdxtiuw.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gutpgkhsc.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gfgdbbreu.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gqjphhwts.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/galoyufrv.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/goalfxmft.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/guefvokxw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/grchccxse.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/guuxbsqve.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gbsuewjmk.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gokimwkdi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gksmuzjtw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gzcoohizp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gcvbfzsfd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gjgtgvfac.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gocbjtkle.sHtML


<!-- 参考信息 -->