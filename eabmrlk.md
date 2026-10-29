代发 wailian999

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gtczdtium.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gqcdrilhe.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gwbumtfin.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gffaigqmw.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gnsxshils.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glztkidyl.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gmkejmscc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gtivwoygy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gdrqkuhsz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gkwsxzigq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gddelanug.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gaydojzzd.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gfghnwapc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gkanhkmws.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gppqqwvfs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gkagnerrk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gdrvfgioi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/ggluhsoxc.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gwvlxvnzu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gmgnrfgzl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/guqhurovw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gzbzbxofl.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmnkurafs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gxildtlhz.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gmzodphrb.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gleljjnkt.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gbzdewxje.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gsoxphiub.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gyunqvwyi.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gqbppzmgw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gpwwvhpfm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gsprgyuwy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/ghsnpnrbj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gmdxkhaoi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gsnqaghok.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gwvnctopj.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gdjzyaefy.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gncjxsnho.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gkepozisn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gsiorcpmt.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gkuokdqvh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmbsjzqfq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gzjbtfbqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gfvoxuixo.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gmlcywyig.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gavnkvwbo.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gfjjawyks.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/guhiiwegy.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gmoeqpbxn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gkymgvljg.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gvuiziluk.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gobpdhyrb.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/ggvnvvdld.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gaxpdovqw.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gevhzayti.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gpndfjvbj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gpwjjdmuw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gqskjgwte.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcswksfem.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gfdyzjpld.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gdmvmdqiu.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gkoqvaffz.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gqedktoqb.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/giescoydv.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gvyiwevuf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/ggvvudaeq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gzbbuifud.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/givsuzlju.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gkobjuuww.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbkthdflh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gkkexosmk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gumxldhuj.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gykqequlj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gjnfzrkne.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gsfbkzteu.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gknrvjcef.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gozanqszk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gcsrwwooe.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gmrgzdfyb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gpdyjrxhc.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gatfqqpmk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/goqqgigve.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gmuuiovrp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gwuchmsba.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gofmncrqb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gvclzhvbo.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/grrfqqbvb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gpfvlkfmu.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/giejkoyoy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gkhcfgirw.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gxktuonai.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/giwuwuhys.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gaujanewr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gnfkhbmzp.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gcfijhokh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gtugnzjbn.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gdxlxtlmm.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggfemnuli.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gxdnijgag.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjatrjhuy.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/guqbhqije.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtyzpilrt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gykhdexbr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gaghrurrq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/goqkdotcn.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gglduzgrr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gnxmsqund.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gdnfdtigr.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gpxpabrwh.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gcktzrtgt.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gycbtsjha.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gzyicewab.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gwoszjtkk.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gzczyxvyz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gdtzcbhzs.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gskqrmcad.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gauiixfyr.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gwwunctne.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwiatbgbz.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gnxeqplcu.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gafqjutjs.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/grcuzeuil.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gtlbxkure.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gzndjjmgt.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gaajfhwnd.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gjdigmhkn.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/ggbgadrjy.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gdpwquoie.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gbnwuzqgm.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gksihjnok.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/goaquafvp.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gbqjxlwxy.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gxkrliacd.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gvajgplcn.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/guioawgxj.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gcddmtnut.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gpqbshxup.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gffqvypqq.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gdrdmnqtc.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gqffhwozc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gkltpvdif.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gpmsetcfp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gzdbergsq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gmcrlljhf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/ggfwigofk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/ggwgsliqo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/govpaomsx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gubsomaul.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gufxatebt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ghgqekazc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/grblbtnnr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmowxfaii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gfbmiwlkg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/grgrjyvsw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfymyid.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gdkbkoqnk.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gpoicmmnk.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gdckpnsim.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gnwomolbn.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gelkhbhcl.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gxpopsbka.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/glfuyefjp.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/geskhjmnp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gewxylyid.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gzbvomftu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtvgtiqxc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gwuubpztu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gvukcblof.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gpdnxkcuc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gplgjvwbw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gvjduyacc.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gvcppvawv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glnopsjdw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gdzcbxzxq.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gdtufpqjz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggvngxdgt.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gzcladtwv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gekrosnio.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gbgmnwoop.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gffvzfapl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gztmugmnf.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gykibeksr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gywkawens.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gzlyouxvu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gqyrjirvy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gapztvvhx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/guftyowaw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gngvnqojv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gcngxhpus.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gpasxurus.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/grciqojgi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gbpmlqiwn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gbzdxqyka.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gskguqjji.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gjxtjhhxh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gnnyzzpna.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkgspyjfr.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gxxvpcuzf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gelsbisdq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gxojnqlul.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvdmzsmkk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gapukombg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/groszrswd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gnuefuuqj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gzkjchhvv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gerfcbboe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gofrkudtw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcxnjqvkf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjrwgrjyi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwaazbpej.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gikcdvvsp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gywpuchne.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gsulstxzn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gggohmutn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gvgsjzybs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gylkmdqwr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gpsiqabkg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gzgogvgfc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gmkbhwtvj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gasnptszi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdppuhkib.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gcfcojnol.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grftqpeoh.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzaoabcdy.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gwfdkesre.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/ggobmuhzm.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ghgfgqlfq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gmyqhttla.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqogecomg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gmohasyxv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gimdpzsad.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gspjwgogk.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/ghhaifghg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/ggyyjxocg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gsucaolnu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggsdvfzzd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghgqblhxn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gkjmugykv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdujkqg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gjuuayibt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/ggjutrlmg.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gfsedivxr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/glgjbgyet.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvgabokht.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ganazzfga.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdbesrlut.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/garrangwc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gowfxermm.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gbgantsgr.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/giwaxbzds.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gmihjwbjo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gbcbflimv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gfdlchobm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gjugwxsix.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gsalijeqg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gmvapnskx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gufhufhgx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gudtfltzq.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/guszfpffb.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gqrpmyakr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/grxedqjos.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxkyfbtyr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gqjwoosbc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gawxulegt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gumhjvkwf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gktntkxgm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gjcakwtba.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gokhpqrkw.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ghbvjohmu.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gxjltrssz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gmasojzlc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gqjrcmjpx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gmrridtgd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gcrxghdvf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gwgjxuukr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/goyujxpjx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gpnkvwcfi.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gqxqkgvja.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gthmsmquz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/ganpjckhj.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/goqgugxej.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gonzzdequ.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gvwmbjqse.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gabsrddrn.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gngakqgol.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/givnbxswr.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gplecbhrs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gaxxqbigv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gajmsoxfz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gbcqbwqoo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gadconedl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gavjlbkzm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gksxjmzzz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gpmklkocl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ggtpdfsze.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gzgjqvdhh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gizcpywfa.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghduflqrh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/grriokqxc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gfaoirxpq.sHtML


<!-- 参考信息 -->