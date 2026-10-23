代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmnqak.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tjprquse.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ajoolwfk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kgvwffer.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fxahnlsb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3upnndifc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3voflqcux.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3unmezxlw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dkgcfyng.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gqaqhztp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ldtdccwp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dejflvfi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bpsdkomp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yfwtcyez.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wsgxzfcp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cybcukyg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pamjnebl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3eiedjzis.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3eyrnbnsf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsonjga.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eysuplno.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fjdicgss.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pkqbaaos.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uvvglzfc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vikwampx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tirwnkco.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jujduuiv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yfaacmps.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pwjieeyl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3nathejfl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3gppeazla.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vcdyngov.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nzdvdkzs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3loringib.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lgncibvb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tmpmrxvh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zekyuuir.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3sanvsijb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jupgwnkv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwstusny.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kecfmhem.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bngiuhwq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rujhzyuc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hkqbuyrc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pgudokxt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3apabrzxc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qleghkko.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktkonxwf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aierumcl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bufcruqu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rljcmmjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rqhhddxy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ctdfxwrw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vwoszmob.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nttzzsfd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hrhrpnwn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hnirzsjd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wvkqpylj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bsvxhfhw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3paomzmeq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dmwyvkqa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wyorujvw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xsauxwbo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehtmkwrj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cjcuzywk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qrlnswyb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lisrqlku.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jkgatkea.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3byftibyn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hbsukamc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3szemzaon.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3drmsrglx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3munqceke.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zhotmftd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3dqudokdi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wgbpnehc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rbscuvcg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3chodrrfe.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3klopgvqw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pyoabtsl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hetdzprq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jnvuesel.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3uorbnzcq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nchbaeuo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3agoyfmyk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pzmmfaxo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vdhplbxn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqolvrcs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pvyjeybq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rcoomgjq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yfqgbpfd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xcyjgpyw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3joxvidga.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ohuqtqmj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iexibrdd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ltthltqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iikrwlyv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wuzunmbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyawyngr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3htkbajak.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ggkgelyt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3guidaewi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tpfipwdt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zwstaein.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lmsdoutv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nvofziqw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hcisznyo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ggmgcbqf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xpfhvxdr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dgzrfjbj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3apvdkxfo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qcukzvvy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kyaunora.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3isqrhfcc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lpfkizsi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xahfofyq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wbyvayon.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mlxbizhs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rnyhlgza.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3trdciies.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lcfkpgkx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xtssaidh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xikegimw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qmddpbjk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3hafipomr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3aluhkgxi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lhghjfmb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3osfpfrfz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3osiiuiba.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hqicogun.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uiiebnzg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vftfkiiz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cpnksofe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3addagfyu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3igmvsjjq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqjqry.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3syfkgwvc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yylngcqb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gcpwxkze.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rnbraxcq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dcyyjksu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3saivbmty.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vjqydilk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tmsdsvlt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hdsnxuam.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aeeajcry.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dcmqckms.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3muepjeap.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ldwzjzsc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fnenkawd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uhxkijnk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kdtrcyho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifeagylv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mbcrezan.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhkini.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqgekpwh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3bhuqitnd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3kdvtrmxe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3euyiptyt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3urbrrrlu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fyobojje.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3slpcvcro.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3rxvpcjij.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pjsxwxzd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3djhlwpmq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jtgoobng.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qukkxdxy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ukixrncw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rhngybvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3onknbzgq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ngmfcmzc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3bsxoxwkl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3dqmgfiel.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3iikurncp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3boewmtxe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vuuafnph.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dudyhxbt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3gzlumwcf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3czgxngjg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymhbwpxg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfnbzeht.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xuercjit.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3iqdxitsm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ddgkcxme.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qkkiswuk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjmnvchs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzfirzuo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3clzrcleu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3penquhti.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmrumbnu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3alagrffg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uayscdmk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3odsaezgv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3gpjgsmpp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzpolnbp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bmehblul.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rtazwsff.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vyfnjajm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3veuipzeo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gjskwjkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyunxxmv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kwkqylxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biosgayx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kjgiakuz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3timkrunq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wiovchoh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mjnndudy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3arhaaorm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rfusyskd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tpyohcsb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nrovihzb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3grntjwnn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3xqivjcdi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3alsppwsm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cmyzbghm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xvkwbyis.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qxvcgqtc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nwdmvopn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wkgcpuqa.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cgvxojai.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nferqkfw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3plpdyzzd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tvvifviu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3blyryslp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qlclgyly.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vikfykwv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oogspagl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nspjauaz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cumoyybs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3diuxryli.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3oznymmij.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3szvdhlay.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mqksuyfs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3omiwzzkd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lxcnrqva.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3usqjizne.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3emexzobl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3sdifadlm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hnnubtim.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3almtjjzf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jecxnaof.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3faodmemo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwzrgxda.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hpugzbhk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zmxehfus.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3anuyvgnk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3koqzsbkh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3erxnsels.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hrzprkzd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3extizajy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3cmhyqund.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3icwlhsgx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ntgyugbg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3akxdpnls.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3llvtcsnz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zptbkrmt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3exebbkvs.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3grhpkpvi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3omvjmxyv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ohebnfjm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dtilclip.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ouhmjkpf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3orcbiqav.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nrubarpo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kstvzxgy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dtblmlbr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dgtiqpfe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lnkyysox.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrsbseh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hsljxrye.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tpolawli.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zxscaors.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zhssrpmx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zjuaickz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vrgjuhje.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cdxxjula.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wactebct.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwdbozg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lzsumitc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ornwhjoy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzjoqmg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3uylyzinl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3csoemazd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jxqtdmut.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oxgfxcdk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3chxqupip.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3apjfratc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xidjhnbl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrzrfaeh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cngjtadd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ciriidhr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bpdlumvx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ezswglnc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfhvwo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3prlmrmqu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ghbyjbpe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hcjxzmir.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rhawdpal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gkfkaixb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3uhztqdsd.html


<!-- 参考信息 -->