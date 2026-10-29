代发 wailian999

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gcsfhqwhb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/glwnbpawz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/glqyubrfc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gttrvyvrj.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gcjstamoz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gjjuosrca.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gempalhvh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/glmxhvrit.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gtrnzevnc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gyibycnbw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gbtzjdemv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gawrbbzia.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gaqgtjehe.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gvaymhbht.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gjbagfnhn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gffpexxdn.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/grcrlunzc.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gtmjxnbil.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpycvqqdp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gldthrimf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gvvwprzyg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gyezpawtc.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gixpdgihe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gysniroef.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gelrjnggx.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gsidgygzj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gunonyarq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gkcwwqoxw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gwawpfnmt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/ganxarduh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gxlupzoix.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/goykjisry.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gqklrrgiz.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gysxsvayz.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/guowusgfo.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gdbuhesrm.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/geyhalvfv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/guxmmipqo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gmtqryvty.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gvgrzneth.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gqmtzjaxs.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqtjcrpzg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gshkxbwyd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzteckvnb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/grwxpjiob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gdngakqdk.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gwlbysiiq.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/grcwowqyj.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gtdfmfuzr.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gqjwrmhhz.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/ggibxeuah.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gjhimbtzy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gedvmadqy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/goejcldpl.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/ghetvsoxy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnkhyveta.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gxnykrqxn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gneuucnvg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gkquylmxc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gfgwftfom.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gjmcdlsha.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gkshhnsjc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gsrosjxkp.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gxlsgllas.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gqljncfqp.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gkjflzlpo.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/grqctwcer.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gtsaqxfdq.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gqdaiyfkp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gpyyqeivc.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gczzudjix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gllyapvsi.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhuqhvl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gvucczqhf.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gwgjoewdu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gajkfwifa.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gngaqznxg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gqxjczsoq.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/ghxjtufrp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/ghybsfbbp.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gnrahrubg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/guflcqxpi.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/ghpwbxwyx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gdueitxzo.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gevdgcpjv.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gbblxmrdx.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gcczofsdo.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpwqqdmqp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gcgeazdvd.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdjweeaeu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/grsumqkdo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gafpdqvhz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gbkxjratd.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grhkvsgib.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gfmrwqsbv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/giyqvszih.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gmtdmcibj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gtncxvxuw.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/glngwkacz.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gfyuxnlvn.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gdxcnzvzx.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gvozknmgo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/giryoemek.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gkeekqlgv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gptnhhpkh.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gfqurvbtm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhbfyfib.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gmjfeqbrx.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gtkpqxjiq.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gvusrghnp.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gqquzqnhf.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gjzhofsxj.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gdihefbfo.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/grnrfnbyc.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gtxqmznyf.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gtnyhscnd.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gxftuyall.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gakknwlng.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gijtxxrsh.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gtwfnrlgv.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/glrvrpnut.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gnwhzlbzc.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/ganavrzev.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gogcthmtl.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gyxirhpqd.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghxjrdozl.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/ghhjptoyp.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gmpepnilv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gwaewngps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gegawetja.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gskkdplfc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gzucjiiyj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gzupvudkm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gldvwnvkv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdknmyxob.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gpznxcpkx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghtkvmjsw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggnjswbzo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpiyszwnz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfvbiqany.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxeuexwnw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gjscpsnxt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gkhhfcjdw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gkoxgzoqq.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/goodjxblk.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gpkgaktxo.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gooyuyjzh.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gfbasmkob.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/giydivvrz.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gskuicyum.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gmjlukmbk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqnzbdwdz.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gefirjcbo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/glysjfvol.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gjqlnvylp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gnnlqeula.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gmoblowcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gdabzmbin.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gkbvqsjpi.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gutdxeixg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtqixjmfz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gdjhzyrck.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gqkwxcnbj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gllsubjeb.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gjrnyndcg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gczkouwst.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gptqcogil.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gmcrlkihl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/garijoghd.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gwlxekgyt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gxjhagnia.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gtwyiiury.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gfinrikro.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gwyoxuljw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gkihnedvd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gwhkfynka.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gobawzmvl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gzqnzkrlq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gvqvltlqf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gwffkvrfm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gwdqwqfez.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gmnjnbtcs.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gowxsqiwa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gvcfvmbnz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gaurdpsfg.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/goirbselj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gqujqheqa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/girskfokv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gpurkfnoj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/grsflzcxy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvqhvykjj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gzkzatwai.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gqqskrxbr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ggkxglkyf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goeyjbjom.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpumzalsy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gnspmnlpj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/grorqlfzw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gpoqwcevd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gtdzedkot.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/guffbipit.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gmcalmhcv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/glbzflvvt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gdhkwgrbq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gxrriewcp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gncrjload.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gonopyvny.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gfflpotqx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnufzuqta.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gchwhpkjx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbagukesp.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gwxtsbjkk.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gixmbamrf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gszwqiezp.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gzgcmtprs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gcfwnoeoq.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gpudckcfw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gqpoetjvr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gqsmcgipo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/ghfniuism.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gtooqfdzp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gbdcxckgz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gsidwixcg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gqzvghbya.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gyoyaxxvb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gcvziknee.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/grhzesvtw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/glleadzng.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gjnyepmzk.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gwjverhat.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/giqvrbwst.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/goubhmsmf.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grhuxmavq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnsazscib.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glbeoziwl.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gagwmonuy.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gkoouzckm.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gohfjettx.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gnjkfkswn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gdwrsbncm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/ggkyqziqp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gyigmhgrz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gpbmjzlqs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gvdtccmbt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gzzgolpaz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gpjbxwlhy.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gldqtvwzs.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gypippkoe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gnsxhwsmd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkbhzyamx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gdabmmiyh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gluqzqiiv.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdmcangvz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gucnsggfg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfipvytse.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gihxcglvv.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gahpmealq.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gizvhhiio.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gtiwacxnv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnoxemxb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gccpjzqke.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gkcngwfjg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gyvjefbhr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gfmaotcam.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/goxcommkf.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcyhezrop.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gfryrflgh.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/guzbwsllb.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gfvmcyecu.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gzsidprtg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/givyemuqw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gfhsezsji.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gtshuxeim.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/ghcpzsylm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gifaphllz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gjwwzcjrr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gkbvsrivm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gbumlmhph.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gmxotaelr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gjnkvrapl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gdmrzbtnj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/glavaffqa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gpeyrbwry.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gmexdevjq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gakeapbeu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwmatbcsi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/glrpdtixs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gprrjnyyu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gyivwociz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gdtspfplr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gldhzddqr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gsovniatj.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gihgelyuf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/ggqawdcty.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gqjsmkyrg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gnlasejqe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/grkacojik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gcsbqsxqi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gecneajmb.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gzsgboeky.sHtML


<!-- 参考信息 -->