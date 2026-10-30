代发 wailian999

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwglxsl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gijlfzfwn.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/givoxpyvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkcgkdvb.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexskuya.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnzofkdgi.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkfhrrkr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzsdrblpw.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gmddpkwgo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmclnfelt.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gttytdcon.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytnfslf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtoyvipc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/grnanumdj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepgplyo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/geuvvxhbk.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgxuzzqa.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gwycjkuzd.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmlzovcub.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnvutxsj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgugmtd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpskptxy.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqippcd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepgcgolr.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpegfym.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gkikmtmyz.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gkokfzbun.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gcctszaxq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhhhblt.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/guyftrtmj.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/grabwzcin.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gybycptwg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflfecair.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gdlywolvl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gthhwrezq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnyxxowh.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gybrsorkq.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzequujq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gjamoglsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkjjxauv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gzxfgdgyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gntdnzajc.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gryfvimpk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gasduakto.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gurkbixvu.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gkshtdcdm.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvhdtbxg.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/guqnfspsc.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/goggrisep.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmlvnmq.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gfdoqmfyy.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/ggamxkgsd.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweztlffl.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gvpshksrk.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoungkkn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvfchyg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/guhoepdqa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/grztyfxka.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwcoycl.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gougsujrp.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guqexbwlm.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gmldlxoia.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnplcotm.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnsadrbh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzgunswe.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/grdibzguw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiqgqqfd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgpeepby.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gacfsgnzn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrtjutnx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhayxiks.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnugtygqp.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/grulpzuep.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzdfopke.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gfseiidbj.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpchdxll.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gosszngzw.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuinjzvr.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdtiycar.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gytffppfv.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxikbye.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszktsiwh.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmcaovrq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmbvlmug.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gnyiwpqdf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfvnjozi.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvavbmcwz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gujhlihkf.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/glcokurpe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gtdjsfdms.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmigpywxs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gvebpdlhm.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gqgwmqjkb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gulkmbkag.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gdctmwqmr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gdomsjdyd.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gskvilbyf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/guajmfyme.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcerblfn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfmyonnk.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gomlnxhrk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdujzyrer.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbgqrohe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruygqhus.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbmhlxia.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfvwgbtr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gotxlngve.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhqwgjwa.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvdirlwa.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/guerfcsaa.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoqroupl.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gdpzlgpth.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/godemlkvo.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/glwogjddc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxznbjlr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcuqpveq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspoeboh.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonfxuzdb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhtjejtq.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gjmxqpsal.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/glgqxrkht.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorqcwxld.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gohdpbcgf.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gibvgrzbc.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzointrq.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxyasulc.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvhbblwl.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gumnsudjw.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gplcwjcif.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gmezrfyjn.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfejbpue.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/galkgidod.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkujqoyn.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gybppeppq.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/galmvudii.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqgipkq.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gynviwyjw.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivibdpm.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvydmeja.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gagxrhtou.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gjawpywpf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwsqwul.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/ggceyuwbl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gyudtullr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuowqvhl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvupujhgy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcvpwuwl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdixwvuqi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/giampxzhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjkykqk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhohpjt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmgheopu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrdlbftn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkdavzrb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzeamxtb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueybywup.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gybouowmp.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfizfdhbz.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbxctfo.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsvipwo.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gyrcjmomq.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawkcowye.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gdmjqfsih.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcasrile.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gpmcyyeto.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gumgstxtw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsvugwzb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqcbntu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdsuzlbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcilfzve.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgskbacm.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhxsgvb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gapjqpwgs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/glpyekawj.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gwkyjvztj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfiveiwl.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshlziii.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytcajaoz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gswotcxpp.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gruookodw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyguicig.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzhavov.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmugsowq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gneksqaxx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gvfvvzimm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gumsbjwoq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gfcjbvccn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/ggyyvzjvf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gddgmabua.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/geuzhjaca.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/grdtyndwc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gzkomoaeo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjciyfpes.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/garmcsafi.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gytzcuxtn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymusoczz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gujiivadw.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gghzdyfys.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdofdmszi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcfwadpe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gelzycdkd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrempkmz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdmjqcio.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/globecucc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbxosdcc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxjzatjy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdhhyxtty.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gslgqiawy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzqdpiiuc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gntusniaa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcrthfdvf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplczxctf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grxlvfmks.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gketgejlx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgqxzgov.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geircpgep.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gchfwritw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoqssntt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/glkkfjsxj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxufiajw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqkwfpov.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdmkobz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzkzptqg.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grifkevnm.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gqptkikos.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/gwxobumht.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gtooseayf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/giigevhau.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvzfbbdz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuticuxx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfybkfxha.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/ggnkrsytc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnkekyza.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljsaopgz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbshrnok.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymfffiq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiqjlvrw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhulaaly.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfqjtrzg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gucovcueg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjwccsh.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlbkbchi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpsvthd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhggbaau.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/giglrmfgj.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfhprxbo.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gpnlvtqeg.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/goorevidy.sHtML

Ruby: PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gimuppmir.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gcebxwprg.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzhwdlnfq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfomlvs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmeucyos.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzcidkgm.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/glgvkpixl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gsagryfho.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fanxiaobao.xyz/Article/details/gjqqxvyqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gekbykhxc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/gnelkqxua.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjaxicf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjligrzaw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwijnwhsv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnmgtvji.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlrombws.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/guflwlhhl.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giwbvscro.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goiqbfuii.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gguulosxx.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/glxefzzcn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofwhmlgi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcesgdkd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcposuxob.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbkuzrol.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxaghky.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizeallby.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fanxiaobao.xyz/Article/details/gmeahurta.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcidfpygs.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghibcnzlx.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjhnogyi.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gaeanyihq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/guwkyrlxh.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsvgvgpx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fanxiaobao.xyz/Article/details/glmusrynp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcztclpzm.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqqowzma.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejrxrpw.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmszsiokk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvgtqydb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhspaozu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gtatgksui.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvovygdqb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgmdxufh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gpaofzmvn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gmgcvjfww.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwaaatzv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxstluvco.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjlguddl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobvhhqhi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrhqlnji.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfzawkntm.sHtML


<!-- 参考信息 -->