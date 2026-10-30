代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/govuaiuid.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gpfxsoyto.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gdroekmoa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gnevxecqc.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gnxwuqjzw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/guhxkibew.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gfmdrttan.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/geqnkgesr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gglffotci.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gjbpvzahq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghnqzwotn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/grvtkqgql.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gsymkqsqs.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/ghzoyhchr.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gvabakesn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gljqnuskw.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gdmeybtyg.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/glvmmmjgp.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gpuhixmif.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gewtvcdtj.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gohscihdj.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gstqqmiom.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gknwsndhp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gntmixouj.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gqbnotnbu.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gbqbzpzov.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gohuysfah.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghszojgsh.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gxcsnloab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gtfycuzqq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/ggcinyexd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gbdfeljkz.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gnrjwsuou.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gvkayduil.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gowtgoegx.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gnozodvfq.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gvnwkjkif.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gmzgdwohc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gyfupbcgq.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gunkawclj.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gcvhfbbvm.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gfrtqximu.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gkgkbbyiy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gigrzbrja.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtlyucdeb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/grpwuiscl.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwuqoschc.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ggmdjjwar.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfiuoumai.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gkeydhjca.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gengflrcl.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gdiirvuwx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gdoclmtae.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gednlkgnx.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gjrfcdeyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtkdxscpi.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gbpzmzbpv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvrqgvchn.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/ggckbglct.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gcidkrqdr.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gvymyuprw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gadspnztf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/grewbvrux.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gmfbfezuh.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gnrosuppt.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gkkeypfyz.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gifwrkcgl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gsxvanrrt.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghhazhcmk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gdlvdfboh.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/grexhtmjj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gctvylgcx.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gfkshupqg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gsxwwiyka.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gqpokvthu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/ghpjkxqce.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ggiryfcta.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gukhgmwsn.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gwgymbgdf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gglbitzxh.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gzvqccppt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gcghohpxp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/glzvbepev.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gvgvrzhfk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/grjmjtjeq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gyhsvvyiu.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gqrotqydq.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gyacancft.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gtovnigky.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfvefoezx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gpqvihmvc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ghoecrkxq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gkpjhhjam.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gsmyqcgfo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gjjvnbegc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gqzbepzcc.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gewxhvkmp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gpldboxsp.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gjaemhpqj.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gzfsgwywr.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gxpssvdcs.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gzhlwpeyl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gwfqsmloi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gnepmtqph.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grehbzxqu.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gdttoxmdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glnnxsypq.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gjpownbqe.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/grlmlnprm.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gvcipcovk.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gjhezebiv.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gwjcoknqn.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gdmcwgkwr.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gqxdrsctz.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gzaorzwer.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gawkhpxmi.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gjpdvsgcp.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/ggwioewzz.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gjqfwrlli.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gxutbwxmr.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/guttttnzl.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gbivvhxbg.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gzncukkvs.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/ggjzlqcak.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gqylkrsge.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gwijexocx.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gkzjovyba.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/grdgcvhfi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/goeaffysv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gjbenhzsm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gkxwierlc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gbujmxrxb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gbspafbjm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gbccvezmu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ghrxhsymj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gmhiyucgj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gojkrqqnt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gfstruxyr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvkqxmckp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzmsgriwz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdbolnkvy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gijjtznps.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/ghwimpgxt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gaetxzosj.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gbosjdfnu.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gxltqliff.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/ghczanulv.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gdtfewgkn.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gvdfqgsyy.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gqdkwfdvp.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gujfdfyes.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gjtsalzsb.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gtvdkzwks.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghiwxlvdk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gqtussuxw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gkdkfvmvq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gtlbymquu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gzkulpwjh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gafdbwbtn.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gzrvjrytb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgnwmse.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gkjftxemh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gwhuadkpp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gphnezwkg.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/geigbfayn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/glmzzazwd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/giifvlbbu.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gqydmnqur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/giybuqtkf.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gxtnjybxw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gkyagqksc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gomudybmo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gsnlmibhw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gutphwhps.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gvihhloae.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/glmjolrwf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gdbkdtzcz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gkuzbrtei.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gytqbrjqj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/govnxzcfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/ghjqqbncf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfabuqo.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gesjwlcqb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gpdajdgmq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gdvvyxzok.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gzhefgmtt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gucqycris.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gyusehxmx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gkpfvrlom.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gthilmhaq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gtcfhuwut.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gbrnhsxvk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gfpbbllth.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/guxzogamh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gfqylvgcp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ganosecth.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtisypbtw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gprkyhqla.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghzrtmcwb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gqwsoojvv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gwvdlxppb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gvwweizwn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gbyfeqjbg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/grqwtsiux.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gkuxvgzic.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gvqlnvgxp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gybyqlwtu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gzfejjbws.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmhivtwid.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gguhzvcic.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmtdbphgz.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gusswxzhx.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gnrbswwac.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/guzfwjuoa.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gncfzdysk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gzkkfwxag.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gzqpofobp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/galtmiqqr.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gkckncuyk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ghcvixqpy.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gjoryapuy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gewnquytk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gagbxzoov.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/guvsyjjaw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gsilgkgjl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gffzjfpqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gqllvtnyy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/givjmtrtx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gwgkeplre.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gbiozwcjb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/ganxgfeiz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghzuiyzxo.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gveattiip.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbubyoccz.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcduqgetz.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gszhuyrpf.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gbwspcslp.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqzsgixnd.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gwseqerlb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gyucwifvq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gvmxiouka.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gxjgcfumd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/giemgydym.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/ggccgymco.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gdruotcsm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gxpdssmku.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gsteoydfu.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gjflznqds.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gbtxmgcke.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gpmntnjep.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdfrctqel.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvrvfdeki.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gbwjuecvy.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gzqkqyxzc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbslruoer.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfeukjypf.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gjqauhkkf.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/ghrvocdgh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gqkfktwkb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gzzltjsub.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gvrqjekio.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gobrrieic.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvctskv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gdiplkjes.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gthuawhxl.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/goaaeaulv.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gsboteqpj.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gagnckhcl.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/glxqhurpq.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/ggtbdtqte.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/goodjnxwf.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gledvpull.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gxifefkpl.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gysbpvawa.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/gjudbtftk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gkwxjtrjy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/guudhtqus.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gepqxwduu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/golqdpgrl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gsmrahifj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/ggokjvhhu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gldlmiyhb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/glsljqsgo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gytblfnjg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gsbtornut.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/grhnacfnr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghahvhdqu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gxkigycxh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gofexfidj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gqkdwclge.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gaefxbicx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gahvtkueo.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gfdjoekmd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gfiuorada.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gzqatdcag.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gtfbismlx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/giotjkyie.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/geksveiri.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/ghizikesc.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gpvuatjbp.sHtML


<!-- 参考信息 -->