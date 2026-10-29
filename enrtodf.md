代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gvzrcvpfl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gbvxxeaqx.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gfyrzdjwn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gjqjhztin.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gpwsokuhx.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gqpukypeh.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gkxkwsddl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gjrtannnw.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gerwxfhfz.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/ghkyiaple.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/ghrhnwxge.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gammibutt.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gzvckmald.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gwflrngpm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gmllyhtgd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/giqghonwp.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gktdpvavq.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/ghcserisu.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gfzonxdta.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gymbsnags.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/grpxnohwy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gawmwmkiv.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ghyxeuutt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gyrdgsstx.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gzkejmgho.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gchlpbzgn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/geryjjizd.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/ggjtsrjiv.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gbuqoesgw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gzbxfuvsi.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gthlhlyzo.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/grmbreuzu.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gaphuoyxe.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggvygtmpf.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ggbfdyggj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gouslqhjs.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gvaranbxd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gizcewlji.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/guwoyzimf.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gbonxiakq.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gcibymrkx.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gnezissdm.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gmvovgrrk.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gyopdszux.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gqlsfwqyf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gygruzlai.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/goyrqtqkh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gdcolwmvs.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/glpzgxpva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gezmfbsao.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gwsudpiwy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbqbesr.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gpfujpkbg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkmytzk.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gzvlczvrd.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gdpeqmlhd.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/ggkcapwzs.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/ggwaglley.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gtrvxeysu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/grdolqiyb.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/ghfwwwrop.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gyykesnpv.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gacesbzex.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gusvhulup.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gpfhzowja.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gjhueerah.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gyqifgkkf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gaazypeex.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/grrzoqxre.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/guvbhaktv.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gcbkcvzgi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gehlpiiql.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/ggwbawpgr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/grfvjaazo.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gyspojfsp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gqjiimxhg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gsnptctqb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gdfgmvcmd.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gtuezbprc.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbrpexdtr.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gnmgnqtrb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gglxrpbwn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gfuflsuzy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gkigataln.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcfpigyjy.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxgqdkgil.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gabejsfnt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/goxnauapo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gqrnozcse.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gjlpznuey.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gncndcbfg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gzsfyxivp.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gelcysdky.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gtdjekrzi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gbbncgehr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gwvuinhfp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxfdbnkzh.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gjcbvoctj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gumddtspv.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gbrhpgabz.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gdaeapqzp.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gxybfvqac.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gdmzkdjho.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gxzbdipnd.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gptitutdy.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gsaegofbx.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmdvkheke.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gbfzcnmtl.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gxauxqoet.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gnqknxyvr.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gogcibhal.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gltybldgl.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gubctwmeg.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gujhkazdd.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gfbklqpdf.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gzbkaoaav.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gxwjwbeod.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghtxvvfsa.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gllfvuzxj.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/grmzjahpj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gtuzrnxow.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdgcjqwsj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/glqcjyzme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gmukrdfxc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gpbhgztpu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gvoagfbac.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gdkgduybv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gvhjhzvbp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvzyocoof.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gaczqlyjm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gnbtuciar.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcotpuhpp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ggojjlmec.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gghufnoli.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/ghifzydrz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/garzjuiht.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gliddigpk.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gsfsfagsv.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gellpcqin.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gukdqmryc.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gbbpndtmj.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzeufvvga.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gtasejvwi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/goszaqoqz.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gdciwsjxn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghvjxbkkg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gauinpxum.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gyqcmdgwq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gcsqudmtf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gddsztpik.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gnvruurxk.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gpijltkep.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/garbhgkek.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gsukrnhxb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gxawrfivu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvgufgdvo.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gnefoipvs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gfidgulck.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/glzeqtvwa.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gwdpvetfo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/grheeuzwk.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gyzcaguxg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/glzgiczsb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gtuecfqqq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gwnqjyskr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/guwiqrmol.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/ghsufuucz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gkbxjqnru.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/ggbifuedj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gpznssmmf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gybzkkjyi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/grrgecwcf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gzsukmobo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gqlllmcxb.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/galsrmqpv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gnqeelxee.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvsezlast.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gdcbrzzdo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gljxioulr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/grgqnhggo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gxsdfaayy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gbjntpocr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gibvqkfhq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gdjdbywmb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gluwqezeh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gxmgmsitr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gjcvpwajl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gsnnxcdyq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/giqcstbxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbyqgqzcc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/geqsfnnqp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gcgexihpk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gjtnvkgrq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxceclcjn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guhzdcdeg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gwljnxdir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtdmmhxuw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/guykrmupy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gqhjbgqyb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/govyqdseh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzrmzewrd.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gxfnaofbr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gldkbhjfy.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gucxcdctc.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gixxawxkd.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gqfzfxfqg.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gshffmbkm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/grdusqgeh.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gdkavmmvw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/grsihcbcn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/giftyymqx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/grfyrgieb.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gffrijlpq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/giqdwvxrr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gddtccbfu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/ghvoasybo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/grohynddo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gktibvpbv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/glnppkpel.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gxizcdiyu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gownaouak.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/ginctzxgk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvyhdap.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpezsiwhf.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyajfjwjr.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdzadtdxr.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grmdrxbrc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gcjzmvklc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gcqqsquad.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/glhrvtkif.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gikqkwkln.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gsfmgaktt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/grnltxfml.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gdvvcntwz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gcqzyvqxf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gtxhydbtq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gmusjoukm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gmhmznvun.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gxglfjosa.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gfogwksqe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gbjzbfemw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ggthmkmff.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gmgtlzjjd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/grlretpvf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gjthpuqhk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/geufzvzia.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/giqrrfwiz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gcwlstmqf.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gtpevvaag.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/gxbwqparo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gzlkcbydx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/grktjataz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gbzdfwogu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gjflttqfn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gorgaykvz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gcdpnnmla.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gsutevchf.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gxdowtsyy.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gfaorituz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gphnrroeg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gpshdhmud.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gcnkjlcps.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gxpjgmghh.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gwoalypsy.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gdwxgeawl.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/ghqklzbjk.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gmjlndorj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gfpovqych.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gvnjxrjni.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gscseihtl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gmiomjrps.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gcwkoqsdu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gwhvlsdco.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gbdltcwyg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gfqtjkdql.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gtitweqgf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gowwkvyap.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxuikhsgn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsrftcqnr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gulvlnayh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gewrmvvfn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/grojsrapf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gthpfxdzv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gvhphrkco.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gnbbtctgw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gvdjaafmq.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gxjyrqdoh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gajimluwv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsuomttan.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gduqfvfem.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gtzfqcqhh.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/gzxylicbo.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gamdpkfxf.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/gplxhfyam.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/gigbwffvm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gebydjkuk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gldsxsfcz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gybgvklwk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ghtbwxhcx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gbraorqdi.sHtML


<!-- 参考信息 -->