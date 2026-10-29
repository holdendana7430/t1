代发 wailian999

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gwnfjdaqy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gyyquclhp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gtfnljvej.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gvrpdynov.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzdlxhwkv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gfddbbkeb.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gwbcgtrrc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gfymizvpy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/grqpyitis.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gxfpwvore.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gldmdzhyv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/ggutsvvae.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/grdyiytqf.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/ghydbcdbd.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/govkbpgtb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gxosvpcgx.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/giifiblik.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gplproini.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gcshyafys.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gadlhnpzn.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gcpirmnew.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gbydbmgho.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/ghqkfunrn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gdaeoytsf.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gdfushnxc.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gybnkmanl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gpfhdmisn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdynivpy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/glwfioifh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/ggcxxvctr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gyghrhxjw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/ghzbymjru.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gwscrxhld.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gvqtckxch.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gdwxvztzs.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gjllbwmoc.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gdjfqwjhe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gwwpmlkxt.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gvdegqcfz.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gubebxueo.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gcwllisvb.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjlxsrpqg.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gqjqovlgd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/govaopdfz.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gpiilgbsh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gzbgdmkdu.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gzekvcezd.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gpgfvnzmc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gycqglkln.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gqzlntgew.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gtcjzmczv.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gwgkdgijz.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gmcgcirzo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gocdsnuwe.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gkgunxxhd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/glzhfwtmi.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gzpwitmfj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gfwhawwew.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gwziynpqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gbslzuwsm.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gfxermrnb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gjkqefsnr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gegvrbtnp.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/garxqlabq.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gppduwfrt.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gsxpdfnhc.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/grihvvvmn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gbuthdxel.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gkmxsivqf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gyodvofmk.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gvsdibunx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghvqijhmy.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gjnkmosgb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gdslooled.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gpdsklhjp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gpptcxesp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/ggclxmfjk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gxaisdors.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gzadosqub.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gvqgrfmjk.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gzcmcjhih.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gqyrpprlk.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gsjjnefvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/ghfagxxdi.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gyqlbwcrq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gojdbpqkf.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gqyytzthn.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfdeesbyq.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/goyguwlqd.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjqbgtmga.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gedaksath.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glbiiwcdl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gtxavgqgf.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzyqukbld.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gfdwmsjns.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gjfufzayy.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gapqitcmo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gwjsnwhjm.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gvbmqcrmg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gjvvfaeer.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gfxeeusux.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/ghzqgcnsq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/ggxvrfsnw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gajsfidgz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnipwuirm.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/ghbpmivxe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giuxtgsst.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gfhjavpxr.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gtfxqaeqm.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gudvlsriq.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/grvbthhuy.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gzlzkgmxo.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gxxpwpmax.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gscmabmqu.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gggcsrjih.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/geydqaxxf.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gommbsgrp.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gilgfxpzc.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gikwabddh.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gzgftvzkl.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ghtaivoyd.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/ghzdiquwj.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gosfzflxn.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/ghwsgffwu.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gxzpfbaou.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqlukhltj.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gtntseklb.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/ghnlwfpeq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/grdfvdlqv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gzbjlogal.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gtltpcacx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gfkwfpxyp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gfhqisyjj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gastxfnxi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gtmavuckv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gtuhqqxby.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gjdaxrrfu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkhmnhtmc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gsugamzcv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcnoirqpd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghfncknlw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gzjvpfbov.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/guycfyrxf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gywtqsaip.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/grganvwyf.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/glsaxjhgg.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gafxsjwri.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gsnthjhdz.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gqiwiabwe.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/grgrleowj.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gnsqwfavx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ggcvheyys.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gbbplztoa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnswprdtz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gphurrapa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gkjnhzegl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gxzfxsaow.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gnlgrxlnb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gbhudcsud.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/ggalknsve.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxryddztc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gqspidahp.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/ghmytrekq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdcsraocm.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gvbarcrtj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gbpecnckf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gngzcsejs.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/guewaabcq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gdtsiajjq.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gzfytsmqb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gjigjtoaa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gflpqmovl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gflmbcjdu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gjzsxcwfy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gfyhnquwe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gohwxsaci.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/giqmshwve.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gkzwbvbfi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gmzdsazml.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gawwqebyg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/germbbfpc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gyqvqwjkw.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gfkcswkqe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/ggivmqvtx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goitbpmpb.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gqxzpmvmn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/geffshmzu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gcgdyarnk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gpdwrzvzt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfjyrunxy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gyfzzwpgz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/geebplfwt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gunnrznvd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gdeczstoh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gmkgtngqc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ggfyqlxus.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gwrzdcnms.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/garykonvd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gngfkprmb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gilqnjywz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjebmbzry.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gnocxeypx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdoxvyaem.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gdwxmzbsm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gcbwlhwvw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gogouuwaa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gjrunbftm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghnplfolt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqapzdjqt.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gopswoxcg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdpatydnm.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gqvxhidkr.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gwmlvlwin.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gbszbpqzs.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/guhnajkgy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gdothmlat.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gskdxxuai.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gtyrmtgny.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gjthcwjik.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gomqlecby.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gclwhhbsl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gobilrmgx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gmwuttrrx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/ghgbuprgo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gplykdfsg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gtwvtfppu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/ggzghpqiq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gsorxjmsa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gfdutcbes.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gqtyiqgja.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gfvokagdl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gltdgrskw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfouhnsxr.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpemelsvt.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfclebcwx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/grvwuyuea.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gtrbajppj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grkepserq.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gmhjppgva.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gghdsvrrz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gblgzznxv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gcphlmwqx.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gdjxomkyw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/ggrgvjoka.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gstpppafw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gboqnllfx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gdwqicquj.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gqvtamtkn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gadsluqcm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlrvjgo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvquhbroa.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gcvqeowxr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/goqnuxzly.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gvivzqvqx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnwbwfwft.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvkkrlmgm.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/glkgtrcvx.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/guyxqisjx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gnmnkveqf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gervuxjwz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gfwzckafi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/glfvxdvyx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gemcoedxe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gdlhkazzx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gpzyvtogq.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmcwjrwoe.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gejbscjak.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/godujiqua.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/ghqilhzpn.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/ggyqgnfgp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gujhedbem.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gmvounapw.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gezlwpubc.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gquochaim.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gptbstzrx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/grgsfervr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gnqcspsbr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gaodijdwm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/ggpzbkedi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/glpfspvhk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gfxlodhdn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gqgbprfbe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ggldpnnix.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gfskvcooe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/giobbxdgh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gzomjbhvv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gbpgetksh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/glkmrmwlt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gckospadb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gpcefhaxg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gajndbrom.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gwzymlwtg.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gcfovhlgm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gimamycra.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gikxfries.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/ggczhchlx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gqpiznnau.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/grnpzwvki.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gxkqmdisx.sHtML

Ruby: rand(1..100)
来源：http://wap.fehbvm.com/Article/details/grcczugxt.sHtML


<!-- 参考信息 -->