代发 wailian999

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gyymilzkb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gwkejwjzw.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gbqyznlim.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gcrripotp.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/glafwvyji.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdqppyquf.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gvqzyjqsg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gaseyvhmm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gxpatvqim.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/grccmbvrq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gwtyihwym.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gfypclzmy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/geniszugi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/grccluunb.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gkgdbctwf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gfmebkgkb.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/ggodxrfyj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gcfnjeldl.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gvmbwxkhl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/grgpsmeim.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gwahlwvoq.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/goaosqmaz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gepaeyhpb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gkuhfeplb.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gjgczlxda.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gfmawdmfv.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gvjhtdekv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gddquvjqm.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gmuikvqnr.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gbdvaouhb.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gwgbvhayg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gowemuqxq.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gjcfeghgb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/ggaztcvri.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/golnhhgef.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/ghblzpjdj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gulknxqne.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gdcfuvplk.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gvmzithjy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gyhtwjkwj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gpytrlpfc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gaebznlii.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gdhjgemby.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gvtkohvcd.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gzzqcphcd.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gqfheoozf.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gjljwkqbf.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gfglavqgg.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gwujgthbx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/grmnvgcns.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gepfognjm.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gjzwhxvjp.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gnobhvwuj.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gzkeohnra.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gzbxdiudz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfslhcaln.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gllbkbqri.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gtntujsqx.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gdtsrwdnn.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gzcskwnxs.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gwkvwkvyo.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gzbsxilwh.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqokkfuar.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gmamvrkrg.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gfgfthjsf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gqvpluslo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gkgszgifn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzktfimkv.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gfwgydwey.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpbtemyvp.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gsookwoda.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gulzwfqzk.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gcdxbhiym.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gymqdznuw.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/grwaxpdvh.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gytxwwarw.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/ggbnakefa.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdltxuk.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gftjqmmlx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gbrxdsaul.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gomtnunng.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gsqvcutfi.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gplcuhgak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gadpvcvrf.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gvrayurdv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gciwrmhjm.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/guyccvxsk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/goytwbstc.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/grtpxglcb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gctdukbca.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gyswrohga.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gyhtjxtki.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gbseorypu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gsryqptew.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/giurmbyms.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gowxzfgse.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gqnpernue.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gmzcciknh.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/ghuqiulaz.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gsacrethi.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gfzffuyxb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gypexssqa.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/grhvfsbtt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gswbmuswu.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gyzfxqwjk.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmuoevvbb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gbfhnqczr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsscbzbnk.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/ghzsnpsto.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gynbetdqw.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/ghqpjntvz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/grljarzzi.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gdwolvvnn.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gendfmnrg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gdyowkfqg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gfindkbez.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggrnkundk.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gqyvubtyo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpydzfzhj.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/ganncfqxd.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gfmcxjfcq.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gxtotxcxw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/glczyaski.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gmrhyaivg.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gsjsatodq.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/glgfztzrc.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gxjdmzdzk.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gwsmedsxx.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gmchbvdkg.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gydewbefj.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gnwidnrmv.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gvjtytied.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gdxodgpqz.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gtvbxxfxn.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/ggaohiduq.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gwkzhzahg.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbdzviz.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gucjukyll.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gcdepkffh.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/goplneyqo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gevetiuto.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/glaveoajk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gigrapqwx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/grbthpjrs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gogdccsjo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gdgwfalre.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gooctjyro.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gccgqneys.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gbnmsyacg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/giotkwtzi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnomzudgx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdwohhwem.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gaevrular.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gomnvwrxx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/ghdxzzoaa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxvleeaei.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gxqakeyyo.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gcknhuydr.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gvjfnlrxq.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gwsekufmi.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gjbsxhitr.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrwlvqw.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gibrsdmyg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gcardrxnu.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gzubfrsgy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gttpipidk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gnoifkzuz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/goeivmqpz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gsergbxjk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gwrbvpgkz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gyvasumlk.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gxafowqwd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghnoeevfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gugvvgewd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/glpcgnqwe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbpluwlhz.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gfobteuhd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/ggizgpyhq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gulpjbruo.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gkkyxlvug.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gmbgttoth.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gvwtlqynb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gmhiajnbb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gdqevmanb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gekawnflr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gumckhkjc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gccsynbnf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gghevbkxo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gpluuxdak.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gzsusvzqg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gendqwmke.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gbzkjjiik.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gxqeqpogz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/ggtluupfz.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gwufopstl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gjbafcnha.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjolwtnvx.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gzazemdyr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqsdefgid.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/glhfdrphf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gsbqghbsj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gcaixqvmp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gbnanacwz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gfcsqbsbe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gpbjyjuqw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gtcgivazp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggywqezoc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gtpjwfzxl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/goerdzueb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gmrrfhdhe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gappvukni.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gxkfvztpw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gqhoawjvp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gyjuqqgar.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/glukmrnqj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gfuhhtown.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gkmelqusg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gymcjwizo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbzrokyzh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwgpjrayx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwxaxlxoc.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/ghgimqhov.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gylpunggi.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzdvkdjtg.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gikqzfinb.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/ghwdmtmpl.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gggzxauwv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/ghotgnnnx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gckykkppz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gfarajsjq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/grufuifnz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gewqktsmq.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/grinmoiwg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gprdarbuf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gsipmcrkx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gmlpntgei.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gvvitsvsv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gfrytvxte.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gvbrrduxc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gddmeqlhn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtuspwvmb.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gwpjdsgyg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/ghpqldasz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpcumgkyy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gunorsats.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gukndtkgc.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwcqialbj.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gssfksplv.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/groczfptu.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggdobvtay.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gszkkshzc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gceufrmdz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gvezjtwad.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/geusiklcv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gpypahikj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gatvmqivj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gysncqfuz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gxnylpwdj.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gadcmttgu.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gvtitjuiv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gdxksupoy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gabigaxjp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfylbkoce.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghharvush.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqitwuokx.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkomevith.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbymyjfwg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/goskgtzdv.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/goitxepfw.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gkublkqvg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/grcopvfpv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gjrmaatdg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gjehhrmzs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gorxfvstw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gcqqsxflm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/ghjcbbnrj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gqmqajiwx.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gdohxekbu.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gpjsfqzbp.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gvmhwthqp.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/grlibqeyt.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/ggfckdqib.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/ghvvmynmj.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/grmmdulcu.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gagzoiayh.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gtqvwfrrk.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/ggjxenzvz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gmwaullri.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gkqfonaxa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmiesyemc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gnjsbjkkr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtfjjtedt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/giednylft.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gyoibelmr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gbqsumomd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ghftwbosg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfqdhzhyd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjtgmvmoo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gxovdwfeq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gudcrikwx.sHtML


<!-- 参考信息 -->