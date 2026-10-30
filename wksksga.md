代发 wailian999

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/ghvwnqtej.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gavinfoub.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/ggwgdfxmi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gniugzkty.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gbaozkdhx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gzwsuileg.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gircsfpld.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gicixadbg.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gmdollswv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/geyinxklp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gteswpnqz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gjxlnjifk.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/glspxhzfn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gkqiihyuw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gbjjleycn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gkxtvcamo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gcbrygmxb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gmtfemshe.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gtsjsdnzk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/goslewltj.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gvxjccwpw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gmpwzkbrk.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gftvgivar.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gevwmtiso.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gbzbjpmqb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gbjuyyltt.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gzkoaicnx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gnuaanqra.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gmzdoaopn.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gxsemykyq.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gbqgftncn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gokesowhx.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gwcndhrzv.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gxuvcmvwq.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gqlwxnwyj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gexxbutfi.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gftwlknmp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gaakabmfr.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gocdqrjwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gaikuwowb.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/glehebmyt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gvlarxvym.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gmqjcwril.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrggvmng.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gwzcoakbn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gjpmhfjnc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gfhrfbnmq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gzmylucre.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gvkljezwo.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/ggpqtnyey.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gmyeemzfp.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gkkbfiplu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbcovphuc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gmlxfrcfj.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gfdenqzgj.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/geslgryff.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/glnhjbvlf.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gdqulqjdh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/grlyrwsmd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gvynclxle.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/galaiydhb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gmsecumgc.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gufgivqsu.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/grdltpwfi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gctkchsrv.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gkknnimlv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gssluszzv.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gslzfffdx.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gwufkhbou.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gbxpvjdzc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/ghynfmysm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gcxhkzsoz.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gfsdfakug.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gtupnapgq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gkbhrdziw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/ggjtvcsaf.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gfvpkipzq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gckwhbynx.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gggosmbcv.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gimdvmbsk.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/geevexvvf.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gynhfrlrg.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/ghpiamfdj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gstdwfnqg.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/ggewlifww.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gakihkfje.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gozgobnbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gmdqhbdcz.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gpmgkycru.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gsqvptdad.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvqzovkwj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gixqtxigh.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ggjsbujah.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gazkgohbj.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gnvvkobsk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gkdbtzwcb.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/grydhimoc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gywaxdhcz.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gzfsrtbrr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/guyivrarv.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/ggzgkavrg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gbqczyohn.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/guxelwqls.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqxlenfkk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/ghvawslng.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gihtwtpbi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gqynebuxg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gmgdirjnx.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/grhyavaon.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwreeziru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gnmjedjos.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gpqndgicf.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gncngrhdq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gunamcgzj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gwyayudje.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gpvhrgtqd.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/glihphnjw.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gxsyhtbce.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gmcmwhmsj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gddrqjznc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaavoqtpn.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gpftnkwnm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grejtixwp.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/glbswiqxq.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gtmutejyy.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gqqrjksfd.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/grbvgcxqb.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gauorhoxn.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/genamjpxy.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gqxzbktje.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gdzrwzoiv.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gosskcjii.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gidevcgib.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gnkkgfacy.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/ginnmutpj.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gdcmfsjzo.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gejlmdgte.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/grqbxunoi.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gosyzszdn.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gbukogzoj.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gfmmhxmbs.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/grvrfenjn.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gmqsqnskv.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gqsxoclln.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gkqysysds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gatcbjkpe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/guqkronpr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gveswzzuo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gagbqzvja.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/ggjupeclu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gfgjvtdzk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gzqhlcysy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbvpiehus.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gmiuvvjxl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gnntrrdod.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gtfxfumkx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gyfaxhqmk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gtdbgcfro.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gkipmcjhg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/galwbezds.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gydytqlyf.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gofvdsald.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gtegzcnka.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gcuojrrgh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gkwmemmok.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glnvbcybu.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gwcuegrzw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ghgcivpwk.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gksmtuevg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggauwwqam.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gdwpndzhr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gmcntsyvw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gsmpnrbnw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gekwvxeha.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/ggmayrded.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/guwoialkc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpnapahlg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gjisrelna.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gcszxrsoc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjpbpaxkn.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gsjtyqrws.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/ggxtednsb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/ghtqqhwwu.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gvvtusymc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/guxtjhgsd.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gpxgmnksa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gkhegmzdt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gjjakmmpu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gshsigzko.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gvmqdjqbn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gijtmeksn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/ghuadubkf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gecxkjwjn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gcgpfijdc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gcyksyloq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/giuretuue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/glnazbkxp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gaqlmemvf.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gnqmzylyw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gzhwjwnhz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gsuixnkxc.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gesddsodq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtacnktcg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gsqxcxrin.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gomsifccw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ghjwttpph.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gidquexbh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gwgjwaqrl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvhwlempp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gaxephfja.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/goqdnmgfh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gyffavnvq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gzxrsnuda.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gnkwtabcv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjomozeyn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gmxmtkqfy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gcldrwrhs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gqhcirxcr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gbloqetjm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gvfsfysey.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gsnkhliii.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gfjpxcrft.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/goxetmhzf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gsroeolaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsxnqkuta.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gvfbheyhh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpfoylmaz.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gbpbskqms.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/glkyiiavw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gmfllzymz.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/glulmmkjq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gkwzdvoyt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gztaswyii.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/geusowzuj.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gxxokzofd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gkwymvbma.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gvivotrgp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gevhjnwfv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gtildrrtt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/goilfgydh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gsdszqqvs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gnpjavpak.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gbefuhkgi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gpzxnlazv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gztqeodlw.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gnddjxmvs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gdmhmclfl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwzbkcbvw.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnruwvoqu.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqfgkihsa.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcoiypaex.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/grrvojmji.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gauawjudb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gvhvipmqv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gjawyovew.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gbgyuxwax.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gnijjjeyq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gykaroehv.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gvsuuzxxc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gsxjnxcoh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/glogyuxlx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gzvjpwygw.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gfsknxfdn.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gqsboukhz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gjctspkkx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gvrlqfsbt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gilzpdgga.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gajinjkjj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfqfztfrt.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gndtmgjoj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gfbitscmx.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gzgkibyjv.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gkbroezmt.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gqszcrrpi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gecetmlhc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ggwplphcb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gnsyjekta.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gxrvqkroy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gmefycfaq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gknypavqu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gzfrdcpfx.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gxxtspafx.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gjplawqyu.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gpujjcadr.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gmsgwjnus.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gumquzxqn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gsnbzgzmm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gjvhpvbix.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gxnqfdxwo.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gdnuvpoac.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/giludrcit.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gguwcoyel.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gjbjsyvnt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gjzxjyihq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/geeyssdtp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/grugjlzfl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gstwgkrqz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gwvnamsbg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/glypaoxqo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gszhqrkim.sHtML


<!-- 参考信息 -->