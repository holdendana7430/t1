代发 wailian999

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gtpqbwdgk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gncvtrxki.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gikibslbs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gruuogfsm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gocilwkdj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gvdekfpwg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gxdbfwrgc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gljzkaoxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/ghniznizv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gnfplrary.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gyruveawe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gbhslafzx.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gaxbuhzml.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gpzsoawai.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ggpmygzxw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gaafvmprm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/ghothcdke.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gsehwwciy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gyovrunir.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gtipldwmf.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gewdqjoip.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/ggbtqwxyt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gxepphahz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/giwtjbdgp.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gptdjsluc.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gvbzcqlma.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/grcgczkem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gkpznzlfb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gcwkvmhtc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gttsgpmrc.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/ggxnavjue.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gillbeqhd.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gvssjsxzs.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gxrxhxyme.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gzjbjbmmk.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gqhjvppfj.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gdikjzldm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gnoyilzhn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ggovtomhr.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/ggkuwlyyu.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/getjjdlss.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gwuqqvsno.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gikbnqsab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gomfbjlyk.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gjrgbxxem.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gzpraxzrz.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/ghzgfrdkl.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gmdlkrgny.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gsxcolkic.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gopwuiwbq.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gsearwxod.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gblgqhhwn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gskxatpfc.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gjgsjukwe.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gaptiodyy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ghtnrokdb.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gerqhodbp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gfxryajpq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gebidpmub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/glhkaulsq.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gtsymntop.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ghtlxfqxv.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/glzgijwbg.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gcuzimzvj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gbeqduyaw.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gtxdtxgsj.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gursqjjrq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gqdfeffta.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/ghmdfmqli.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gpyfvazsi.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gisvzdcmw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmtkrwdsb.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gdcwcgoki.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gsfftucma.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gqgmtqhaf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gulssocbo.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gbirryqbr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gtccqskpb.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/garsnymbl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gugqrwifx.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gjvawbquj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gknkaxwei.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gpjjwbsik.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gxgjypotz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/ggmjfbjvq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gjjcozphp.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gsavrtmji.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsoskfodn.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gyyepoxdk.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glsymhlgx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gxkcmnwgn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gzzedpczz.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gripdvdwb.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggohkrtuq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gnhezvfay.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/ggqvrlwpc.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gsoovqppt.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gkdbzdwix.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gzjggjsuh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gdioswwep.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gisrkkvau.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gsfoappmf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gvzoogwpk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gnkcrnquw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grvkrduic.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gtnlrymmv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gissuesfv.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gmfujmmam.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gfbeewwqp.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gybgtrsec.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gnxinyprg.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gzmsoblqt.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gulnvevit.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gpduplzug.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/grmzcqrnl.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/glhaxvefy.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gigrypywq.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gfxozljew.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gacmtmpyc.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gkqkbnpvw.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gvnewqlbh.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/ghrwtqfoa.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/guqyvmntx.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gtvgwibik.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gvjdlimum.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzbrziilf.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/giknpfdgz.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gmwodwhph.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/ghfrfyeri.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gkuvsbvzh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/girasiqcw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/glvbfkdyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gtsmivzqy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gbcgxmjbi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gwgfegudk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gorcupvvy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmpajhbwh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gzmanzumv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmktawngc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/glgrfaypn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gccnaubab.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwkituoam.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/ghgatxhca.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gwolgnkrp.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/geyvgeuob.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gbjtywgye.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gxesrkqmy.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gugcewwww.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gietdkvlu.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gilvepnaj.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gqgfrfefz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gpxbmshiq.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gdpwkzaea.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/grabhpubj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gjhoufusc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gygcxsmji.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gvqpnflpm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gsqmgxvpu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gkopnusun.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gcxbrbasu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggaccxzhs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gejknewlp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/glimwcfxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gogrumjtj.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gfcjuuxya.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gefvelmtk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/giyymtcnr.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gehfryntq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gnrjliwkv.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gvbtujjgu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gbcwxhrey.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gzjmgtdew.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gqvzixyaq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gghpfnykl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gbkupoimg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gikjdybcb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gwnspxuwd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gfpuoysbt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gkgtpjbxt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gltlecrcb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gkmzgzzgf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gssonmgbi.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gzwjozmed.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gngwbmgsj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzspllzbh.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/grzrifupk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqudqpypw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gxpnlpiff.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gsphggtwh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gsgtgrryc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gawtbllfl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gmfrhjwhw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gwfrxopca.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkxreju.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gemqnpgil.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/giohnwgve.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gqfomzudf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glpzfuiat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/geanakqcc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gooflbtst.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gdyuflzzk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gxoecheii.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gupmhbfsw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gwwzvgnfj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gqfcsgvsr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gvjpglwbz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gnksaqxwl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/giigbojew.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gazigaqza.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gtnpzaqxo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfczusgmb.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gztfmlshy.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gznslmlny.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gblrjrfvz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gkxqgpvdl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gimgfoaiy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/goiytzotx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gyfaisfvb.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gwcfbjqjk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvjtggmxd.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gsvcyhfug.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gjtweytdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gqradcjkg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gyqvngdbj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gvdvjqtat.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grvfzkbit.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/goeeiznuc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gvefcjfax.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/guqwgfyao.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gfxhhdqng.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gvrncunpe.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/glwhrcegl.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggcfrvrcm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtpfjuulc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geecwhzre.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gbklzpkdn.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gvdzxxpla.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjmfkecxt.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gxvphswfp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gwntpmoiz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gxdwfjzlq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gqryhukbs.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gexqqemen.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gefodxmnp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gjzpkfwja.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gzjcjsqnf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gejdmaxnk.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gtsoxgdui.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gfaniseat.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggmbqjfxh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gantrkizk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gybyakpqq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gvkzgjvgw.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdqihrohv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmlmimcgh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gbzhqvfju.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gbfkkbmyj.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gfhkdmvtn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gyxzaobjy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/guqyeggeu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gbmvqluim.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gwxihkpxs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gflyvvzcv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gilekgfji.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gcechstnw.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtqfkvfgn.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gylmarrmi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/girretalu.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gsktpknqk.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gfdctptoq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gqflcielg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gzxhtirui.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/ghmoxmzsa.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gkkzqfkxb.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/ghkedzwbu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/giudsygtj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gibxyvzvw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gyxslzutc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/ghsdnvqjz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/goaacfysz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gsrxosddo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gvimapkuk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gomcydtva.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gcehukdnw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gosproasl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ghoeyjffj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gtplnzrjl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxjzhygwl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gtcfuznjz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gkngqsepq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gzewowxgc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzgfpqgjp.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gmwqhmncy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gqxdjdaxb.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gdhhzfrmv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gfxkqjrcv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gndnddyin.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gmfqddelk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gdcybsfsk.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/grviswfjv.sHtML


<!-- 参考信息 -->