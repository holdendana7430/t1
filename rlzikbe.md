代发 wailian999

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwousnbz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/guqmzdzkn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqmzysxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlpeqbxk.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzvvtsxqn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzyvdmfoj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkggaluiw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrlzzpig.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyhpaeio.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslhkhhew.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzitsujlt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gwzgrmbxq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjajebk.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdsperoq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypomlzv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gxhpdfpam.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplnuuga.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvawgqdr.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmytumum.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gpfoyxrhp.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gjirkfxii.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomzhylef.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfroqrsd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxalppmr.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjhvlmtk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlkzhasx.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gloskvlge.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgzkifsr.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gbotnzsey.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsttlxce.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/glgjletxc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqqfephxr.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gqydrequx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxpljge.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gcndimpxa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gymgpeczp.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gebbgwsxc.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gpbfonpyv.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjvmgbqq.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gafcwfpfk.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwobotlsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gghmglcfd.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauuorbni.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvfpwxeet.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhdydko.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/guspktsdy.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gutduvmcp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gthisajxq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdbdulnv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefavhbfi.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmbhqsby.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gellrtjhq.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gztopbewh.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhyuaifr.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpwkxmnrj.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbleqpbe.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gtbviuirg.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/glwczqboq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gkgfgbjpg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gngxnsmte.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcmhqswv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gqodfamic.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gthzlwfyi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/godjkubkr.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gozqpbilz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gbxvptpjy.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyarkcdpc.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gkinweeyv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrlgijai.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gmcywtwox.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/grskonwwd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdranpqwn.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoanrsxw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/guafvmnkq.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gmmevpisg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpblrhjaw.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/ggfgohbzk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gymelwrny.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbuxnjeay.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljnpdhg.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvglusxid.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffzpfkud.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gfwjfzpna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzoqxqx.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gppuycwsb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzyjbutv.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/govlyuzsm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmvmxpbh.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujcsutpl.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxsjhqg.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjbsjfv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdgbeuvh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gapfibome.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdchftfgh.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifoifxvk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhpgsqev.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfucqxhq.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnxuwvze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjsnoqzo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgfiutp.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gryuzrpgq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkzkmrdp.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gpsmlrxak.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gbertdsnm.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gowfxlaje.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/grunohlqa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gntsiobaj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdgimgjj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdflysqzn.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gsdesmfta.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giipvvkcj.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/ghcgniwzw.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gtxgvvsui.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/geuajkxnp.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/ghhdcauyb.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gurzzwrcb.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhqkfhpv.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqulxalc.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelnalwgm.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyqdapgt.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqwrdokt.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gtmlfaxdf.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gixqxxfra.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gnqrxlbyk.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gslbzrwod.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrrqlzd.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gysuiixjr.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gysxfxehy.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzyryoad.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzrnclea.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaueqelz.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gakumultt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpevfyak.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gyibxpwbg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzgxxzyr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnntbivdf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgyutwdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwrvkhya.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebjepuq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpsehnuh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwgbagdks.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfceeesj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkebvtjc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtaszmvh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gyqblaqqp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gdewjhtxy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtptrxqn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gifbegpry.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gwhbokpaj.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gsvoheiuq.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgdexwxf.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gljbmacxu.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvetattd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbezshbqz.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvyfoea.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gglibdjvs.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpncwaih.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwyupdfg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmwhrcg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gllegahlb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxyhklt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gbrrenwkq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gogykdaby.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gulgovgol.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gctofhmbi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxofcgovu.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gufdepkvx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghiplyodg.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gnuckqjhn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxbfovvg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdyhypqw.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gldkccyjg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzusbsy.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gkydhdcss.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmwvryji.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gpwioqvmy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/guctnmgln.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gucaqmoav.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gscgrdjex.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gfldhzdbm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdilzmjub.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/gdxuurngp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gimdwojcm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gkoogvnny.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gemctlctx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gwxujnkmt.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpxlsaen.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/grjyynvtn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/grkxbqock.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtwyqzkv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgwhgtte.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpnxihho.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjynqbr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaulryim.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gltwhpwnd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/graqkloxg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqdpjhw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeqrnabg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfavfcgew.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyurwttcx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/goggjtijy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/geexwbbtz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrlofcqy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpqzryjt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkguuyljn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmdqdujqz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzohcrcm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnprsyfjt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhcccfpd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsroqucg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhhnntfm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdytcvyqm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoseudh.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gygqlhkuu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjfkcmxz.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaehxmjj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytluvdxu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjxnrcdt.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gybdwodmi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtkltdah.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gfsvinapg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/goywkllfi.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcletuumf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gmlvxzuhm.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/gedpjzgrt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfmfvmdm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gviazqtmy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfszridu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/glcowetif.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfudbngjc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozucsscz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gszelsvqn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gthgujsjr.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbcbuabg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzhturj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gdzahvtue.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvjytepj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/giijdnvxj.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiesqhey.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gaczeadts.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrbrpzz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjshzuzdj.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqqrlydzk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gflfietpd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelkzgtwd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gufhvccyp.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjolktfc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gtnqxwdch.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdbgxmyd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/goadndekw.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfqloxb.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnwhlzha.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbktegtea.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gisrgjanv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpodcrugm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glfuazxhv.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gikdfuiit.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gebisgtyp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcqaukbha.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gesumjpbp.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfqrapkt.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gebopdgwl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtjgltye.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedcvkom.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gvphtfmmc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggouuazoy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvfqcrij.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzaexqfh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/geeqxcxyo.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grogpumho.sHtML

Py:   str(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexucwogm.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxnmoxoi.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gwhrhpepo.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzxlltox.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gamrrbeaa.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdntxekj.sHtML

Ruby: 42.to_s
来源：http://blog.fanxiaobao.xyz/Article/details/gtepzqqqx.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grpafkvvf.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/guolkcrec.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmcigpae.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccvwnpge.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtwxramc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoibppuq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdtmkpui.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnkxfyyd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnqumla.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptxtkeo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqpsqxoe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvsmujxb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrbhxbqe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhjwfpnj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gssqcpnia.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqlhcfz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehttsehp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gvuknexbj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gfyhvblgl.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gdellhegz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gujmfanqf.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxybsseb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gyzkszjrj.sHtML


<!-- 参考信息 -->