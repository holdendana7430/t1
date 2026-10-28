代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.yj20258.top/gttpqyrhyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhijiandao.cn/gtxonkojta.html

[U68] PHP：PDO 连接
来源：http://hz.xziqi.cn/gtnrjugoso.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.svipenyu.cn/gtlizfaavg.html

[U69] PHP：PDO 预处理
来源：http://hz.redwolf501.top/gtqlsqxbaw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xuetiantiany.cn/gtdyleoajk.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtyilzalro.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258.top/gtnzaruuhv.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gttnyqybdn.html

throw new RuntimeException("失败", 500);
来源：http://hz.andypj.xyz/gtgjsfbjqu.html

[U72] PHP：写错误日志
来源：http://hz.hywenlv.cn/gtzuqozijt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ywan-chungtsiang.top/gtgkhxuiso.html

[U73] PHP：读取 ini 配置
来源：http://hz.fengsongda.top/gtimxydwbm.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gtpgkizuwc.html

[U74] PHP：读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtbaeylqtx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.havefunace.top/gttzjuvmtl.html

[U75] PHP：依赖注入
来源：http://hz.zdqjudy.top/gteyztjrzu.html

composer require psr/container
来源：http://hz.yonumen.top/gtmjzhhhcd.html

[U76] PHP：简单路由
来源：http://hz.yanxiufei.cn/gtlncmqwjm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hongshengwenyu.top/gtsbadryzi.html

[U77] PHP：模板渲染
来源：http://hz.smart0.xyz/gtimnndexx.html

composer require twig/twig
来源：http://hz.haohaochexian.top/gtxzoqdzvm.html

[U78] PHP：单元测试
来源：http://hz.nanxinkj.top/gtelidcivh.html

composer require --dev phpunit/phpunit
来源：http://hz.svipenyu.cn/gtescwprjy.html

[U79] PHP：静态分析
来源：http://hz.redwolf501.top/gtkjscbgus.html

composer require --dev phpstan/phpstan
来源：http://hz.cdnleiting.top/gtarynnpay.html

[U80] PHP：代码规范修复
来源：http://hz.tianlin.xyz/gtubeymutn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cucudq.cn/gtcushhzgd.html

[U81] JS：初始化项目
来源：http://hz.9152youxi.cn/gtgmvcgrlj.html

npm init -y;  npm i express
来源：http://hz.ivvv.top/gtpglvisni.html

[U82] JS：package.json 脚本
来源：http://hz.haohaochexian.top/gtmrzblzfz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj20258888.top/gtwezzhfaf.html

[U83] JS：ES Module 导入导出
来源：http://hz.cheryme.top/gthrcrjovr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.snrcjt.cn/gtpsaiyonl.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gthcimaphn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydzc1.top/gtkgdnqrcz.html

[U85] JS：可选链
来源：http://hz.yonumen.top/gtvssokocd.html

a?.b?.c
来源：http://hz.daxiang520.top/gtodlkirsf.html

[U86] JS：空值合并
来源：http://hz.hongshengwenyu.top/gtqndqgayk.html

a ?? b
来源：http://hz.svipenyu.cn/gtdmoeytai.html

[U87] JS：解构默认值
来源：http://hz.pengpengdd.cyou/gtgluxqtqe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.52xcode.cn/gthcayjivc.html

[U88] JS：对象展开合并
来源：http://hz.tanke756.top/gtozmyisro.html

{ ...a, ...b }
来源：http://hz.cdnleiting.top/gtzzbvhmpj.html

[U89] JS：数组去重
来源：http://hz.nwbrower.top/gtpiojzeje.html

[...new Set(arr)]
来源：http://hz.jyoumei.cn/gtjdhxeiej.html

[U90] JS：数字数组排序
来源：http://hz.kuanghao11.cn/gtyevtmvnc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtrmyrbdzd.html

[U91] JS：对象键值遍历
来源：http://hz.jyoumei.cn/gtdroogwqt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jianghu66.top/gtckwenwzv.html

[U92] JS：深拷贝
来源：http://hz.aibaodan.cn/gtuhcjswvy.html

structuredClone(obj)
来源：http://hz.smart0.xyz/gtsvkanmpx.html

[U93] JS：模板字符串
来源：http://hz.jinqigfzy.top/gtqsbsnsdz.html

`共 ${n} 条`
来源：http://hz.hongshengwenyu.top/gtcgeomiic.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtehgpazlp.html

const double = x => x * 2;
来源：http://hz.hnqzz.top/gtetrqngiu.html

[U95] JS：Promise 包装
来源：http://hz.ppjwa.cn/gtfydvtwnv.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtmddapuvg.html

[U96] JS：async/await 与异常
来源：http://hz.haohaochexian.top/gtclsntbfz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtkxwfjldt.html

[U97] JS：并发请求
来源：http://hz.c1oappe.top/gtiidzsxag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtikmbnpcp.html

[U98] JS：fetch 带 JSON
来源：http://hz.aizwys.cn/gtwoancqat.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.smart0.xyz/gtmsudqybt.html

[U99] JS：事件监听
来源：http://hz.dianchejie.cn/gtpfsewnwq.html

el.addEventListener("click", e => {})
来源：http://hz.jinqigfzy.top/gtujkeyqzn.html

[U100] JS：DOM 查询
来源：http://hz.xuanzx.com/gtyaooyonk.html

document.querySelector(".item")
来源：http://hz.hammf.cn/gtopradruy.html

[U101] JS：classList 操作
来源：http://hz.dianchejie.cn/gtcpelyyvf.html

el.classList.toggle("active")
来源：http://hz.gogol.net.cn/gtinohinlx.html

[U102] JS：本地存储
来源：http://hz.jinqigufen.top/gttdllxxeq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhengqikj.top/gtnkvqeoob.html

[U103] JS：定时器
来源：http://hz.daxiang520.top/gtbcxmwrxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zycfv.cn/gtkkfwlxnf.html

[U104] JS：防抖
来源：http://hz.zhoulong.xyz/gtbwuhxwjk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gthyfhbcjb.html

[U105] JS：节流
来源：http://hz.tianlin.xyz/gttgejbtlj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.havefunace.top/gtcjwbtgkw.html

[U106] JS：日期格式化
来源：http://hz.snrcjt.cn/gtqigubqeq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.mhx1999.top/gtatyogywu.html

[U107] JS：数字千分位
来源：http://hz.sufxvd.cn/gtweopyecv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhoulong.xyz/gtoiuaowfw.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtynemhgmr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtpqktqlox.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtfsrslklr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yvedp.cn/gtwvlrqcat.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtecpxnwzy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.haohaochexian.top/gtxxbdniue.html

[U111] JS：对象转 Map
来源：http://hz.nanxinkj.top/gtfwaczlpq.html

new Map(Object.entries(obj))
来源：http://hz.zhengqikj.top/gtnfgrbmpx.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gtfjhmblix.html

"7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtlxpgmoiw.html

[U113] JS：正则替换全部
来源：http://hz.sxryk.cn/gtiwjlguae.html

s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtkefvmbol.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtplzjtbwe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtvetfbbmi.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtsxfjnkqr.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtcclojine.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cashguo.top/gtkyqfdkhp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgufenzy.top/gtbvgilxoa.html

[U117] JS：单元测试
来源：http://hz.cqqwz.cn/gtkfwkxdkl.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtjyimjvtj.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtxxiqwdwd.html

npm i -D vite;  npx vite
来源：http://hz.kuanghao11.cn/gtnvffsxzo.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtetmgpmfe.html

npx vite build
来源：http://hz.tian-w.cn/gtqvbxgyio.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tanke756.top/gtaqyvlntn.html

import.meta.env.VITE_API_URL
来源：http://hz.havefunace.top/gtgoevslnj.html

================================================================================
来源：http://hz.nanxinkj.top/gtfmhxwrez.html

统计汇总
来源：http://hz.tianlin.xyz/gtgxbsvgde.html

================================================================================
来源：http://hz.sufxvd.cn/gtzdhetdqw.html

按语言统计（条）：
来源：http://hz.cheryme.top/gtmlgnkjmk.html

Python ......... 252
来源：http://hz.yanxiufei.cn/gtxgzcnfyl.html

PHP ............ 252
来源：http://hz.0kj1m.cn/gtoqrhoqtx.html

JavaScript ..... 252
来源：http://hz.hnxiangtu.top/gtcjmcuywo.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtzzcuyfru.html

Java ........... 212
来源：http://hz.ywan-chungtsiang.top/gtcdzwkgbs.html

Go ............. 212
来源：http://hz.jqgfzy.top/gtrihqqtbj.html

Ruby ........... 212
来源：http://hz.tianlin.xyz/gtjxwowbmq.html

C# ............. 212
来源：http://hz.cdnleiting.top/gtmceozrwo.html

C .............. 30
来源：http://hz.chenlongwang.top/gttinkxcbx.html

C++ ............ 30
来源：http://hz.ivvv.top/gtsfenoxre.html

SQL ............ 90
来源：http://hz.smart0.xyz/gtzyvkjkuk.html

Bash ........... 80
来源：http://hz.ehwqpu.com/gtreexzixa.html

Kotlin ......... 15
来源：http://hz.yangfankeji.com/gtwsozssnw.html

Swift .......... 15
来源：http://hz.shuidangran.top/gtfyzsghla.html

Lua ............ 10
来源：http://hz.jiagoushi.top/gtsukkfqep.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtkygmisva.html

Scala .......... 10
来源：http://hz.pengpengdd.cyou/gtflinawpr.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtqjsmlnsy.html

合计 ........... 2106 条
来源：http://hz.0kj1m.cn/gtvzeawzal.html

按章节统计：
来源：http://hz.yanxiufei.cn/gttpzsuhvy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtfrmykiwc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtintffrau.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtqrmillry.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gthxbsvodf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cdnleiting.top/gticocpjde.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.andypj.xyz/gtzaokwxtr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtllajylpx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtgxllmhot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtruyhgqjf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhoulong.xyz/gtulexazaa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtmbmmwitz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtecwgyryw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtgcgqnfdi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangkeji.top/gtjhsycfnf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tanke756.top/gthpaawikk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gthdjwvyny.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangkeji.top/gtbhlmhntp.html

R Bash 专题                             80
来源：http://hz.gogol.net.cn/gtkvdafgbr.html

S C / C++ 专题                          60
来源：http://hz.gotoacloud.top/gtgxqzmwja.html

T 其他语言补充                          60
来源：http://hz.sysykeji.top/gtiaquxohk.html

U 高频实用片段                         120
来源：http://hz.birdmap.top/gtbgaqzfxg.html

------------------------------------
来源：http://hz.tanke756.top/gtutgrxkey.html

合计                                  2106 条
来源：http://hz.0kj1m.cn/gtrqghyzco.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtdxfdtqmv.html

使用提醒
来源：http://hz.wangdashe.top/gtdofezoby.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtjdcietgq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxuanxn.top/gtylvxvimk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cheryme.top/gtzzdkyxiq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shuidangran.top/gtqsqfaitp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xingfuxueyuan.xyz/gthivfxyrx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.daxiang520.top/gtevhsogec.html

—— 文件结束 ——
来源：http://hz.feifeiyinyue.top/gtumipubkj.html

================================================================================
来源：http://hz.meibo888.top/gtmxnmzlrt.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aizwys.cn/gtlmlfvqst.html

Common Programming Examples Cheat Book
来源：http://hz.cheryme.top/gtrizpcmyl.html

================================================================================
来源：http://hz.meibo888.top/gtstfrvcmw.html

【收录内容】
来源：http://hz.hysaishi.cn/gtmtlmfvns.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenjidiqi.icu/gtsyleoqdz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xinyue.icu/gtuajblzry.html

SQL · Bash · C · C++
来源：http://hz.yj20258888.top/gtrgwklpaa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigfzy.top/gtimzfqamd.html

【使用说明】
来源：http://hz.hnxiangtu.top/gtfdeuypzd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenzaomai.com/gtvgtlsagw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nwbrower.top/gtnvtygwrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtebipunbn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jqgufenzy.top/gtfpgtvisj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ppjwa.cn/gtgoaqvsdo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hammf.cn/gtoudendvr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.bjfxy.top/gthrpwqowp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yvedp.cn/gtrbuedrle.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gtixafeuqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jlsjyb.cn/gtozqaxabq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.birdmap.top/gtmlarafov.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shzxlz.cn/gtxozjbwla.html

【文件统计】
来源：http://hz.hongshengwenyu.top/gtklscwvtl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jinqigfzy.top/gteibpcjjo.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtqirzmopd.html

目  录
来源：http://hz.zhoulong.xyz/gtdgskugju.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtlezetgxn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtgpbganxb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigufen.top/gtewwxxdfv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gthdpmybni.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gttcjhwisr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinyuanbaomall.cn/gtagyerhnt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gtxvulkygr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtxwfacdyq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.9152youxi.cn/gtweizfnuu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtlclscizd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhiwuduotai.top/gtdpdzhgfi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtymuwbqmc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtqmctaxqk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gttzlsdxod.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtdppitoej.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangtech.top/gtrrimamhj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtxyobsjuw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xziqi.cn/gttlcjeenc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtgxngqpsz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.svipenyu.cn/gtinbtvzbf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtbuzyqswb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtujcuhvew.html

================================================================================
来源：http://hz.ybcxt.top/gtbukztxjy.html

A. 基础语法与类型
来源：http://hz.yanxiufei.cn/gtdbvdpege.html

================================================================================
来源：http://hz.iojbl.cn/gtgypadrxl.html

[A01] Hello World
来源：http://hz.zycfv.cn/gtsurddkzl.html

Py:   print("Hello, World!")
来源：http://hz.guowangkeji.top/gthjqhfffr.html

PHP:  echo "Hello, World!";
来源：http://hz.dashuyun.cn/gtvqfdarjx.html

JS:   console.log("Hello, World!");
来源：http://hz.iojbl.cn/gtvnfbozto.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yueranfly.top/gtcmxbqwsd.html

Java: System.out.println("Hello, World!");
来源：http://hz.shzxlz.cn/gtcatremji.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.iojbl.cn/gtlyoqnzxt.html

Ruby: puts "Hello, World!"
来源：http://hz.9152youxi.cn/gtvphdwhrc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tian-w.cn/gtqxnkumio.html

[A02] 变量声明与赋值
来源：http://hz.chenzaomai.com/gtyrznfuke.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.redwolf501.top/gtzrrcljaj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.havefunace.top/gtatbdpvdd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gotoacloud.top/gtarbzbkbc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yvedp.cn/gtxwpazwdy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtbeasljnc.html

Go:   name := "Alex"; age := 20
来源：http://hz.nanxuanxn.top/gtpofppawn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sweek.top/gtqtvtwumi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gttozxdhuz.html

[A03] 常量定义
来源：http://hz.jinqigufen.top/gtxqetdngg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gogol.net.cn/gtmdzewwwd.html

PHP:  const PI = 3.14159;
来源：http://hz.meibo888.top/gtwkgbgteh.html

JS:   const PI = 3.14159;
来源：http://hz.hnqzz.top/gtthaypxdl.html

TS:   const PI: number = 3.14159;
来源：http://hz.feifeiyinyue.top/gtmwkqaixa.html

Java: static final double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtcorqednh.html

Go:   const PI = 3.14159
来源：http://hz.xingfuxueyuan.xyz/gtvbazhccx.html

Ruby: PI = 3.14159
来源：http://hz.yvedp.cn/gtrbutzlpv.html

C#:   const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtzelgygpf.html

[A04] 判断变量类型
来源：http://hz.9152youxi.cn/gthjnxwrmw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shanyushiyangkeji.top/gtkokqiocm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hfpthk.cn/gtlkrfrseb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.fengsongda.top/gtldyxpyqf.html

TS:   typeof x; x instanceof Date
来源：http://hz.smart0.xyz/gtxnpusvzk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.dashuyun.cn/gtuiovfmye.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhaomingkeji.xyz/gtbpeixdpo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhijiandao.cn/gtolzkuecz.html

C#:   x.GetType().Name; x is int
来源：http://hz.gogol.net.cn/gtufktjphl.html

[A05] 整数除法与取模
来源：http://hz.jlsjyb.cn/gtisqmezjh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xylfe.cn/gtaomdzdku.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sxryk.cn/gtlargfizo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gteghzczlx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cqqwz.cn/gtddrameym.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtifibtpxh.html

Go:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtlwhivucx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtwarprdrn.html

C#:   7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtomvrhyqf.html

[A06] 字符串转数字
来源：http://hz.daria6918.cn/gtzraxtbto.html

Py:   int("42"); float("3.14")
来源：http://hz.bjfxy.top/gttywaprgk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ehwqpu.com/gtmgyknfha.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.dashuyun.cn/gtjwymtenr.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jiagoushi.top/gtgdglmomq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hnqzz.top/gtqgohbqdi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ivvv.top/gtqtmwmred.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.redwolf501.top/gtywywwrfu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.andypj.xyz/gtydflvokp.html

[A07] 数字转字符串
来源：http://hz.chenlongwang.top/gtwtsuqxny.html

Py:   str(42)
来源：http://hz.wangdashe.top/gtrxqutbkr.html

PHP:  (string) 42; strval(42)
来源：http://hz.hammf.cn/gtfabfuqoi.html

JS:   String(42); (42).toString()
来源：http://hz.c1oappe.top/gthmvlnslq.html

TS:   String(42)
来源：http://hz.guannengcc.top/gtalqymxgh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.c1oappe.top/gtdcxrwcsc.html

Go:   strconv.Itoa(42)
来源：http://hz.nanxinkj.top/gthxodozpq.html

Ruby: 42.to_s
来源：http://hz.yuanzhike.top/gtwnpfgoov.html

C#:   42.ToString()
来源：http://hz.cheryme.top/gtiphqnewd.html

[A08] 取整与四舍五入
来源：http://hz.tian-w.cn/gtylsffymg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.sweek.top/gtjktvysii.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhiwuduotai.top/gtxeicslzl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gtfpulqkgx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hysaishi.cn/gtpndlviqx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.52xcode.cn/gtquaujfhv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cdnleiting.top/gtwchcqbfh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.bjfxy.top/gtqzkekjyl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gaohongyu789.top/gtouhbdyhc.html

[A09] 绝对值与最大最小值
来源：http://hz.svipenyu.cn/gtqmxuyfhw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenjidiqi.icu/gtpkpkitpq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hongshengwenyu.top/gtivpcubut.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.0kj1m.cn/gtemirgqdv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yj20258888.top/gtrwkqcvxs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.havefunace.top/gtfgzwcjen.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.ivvv.top/gthchbyqwg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.dianchejie.cn/gtdbimsdyf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hysaishi.cn/gtnmsppfmt.html

[A10] 生成随机数
来源：http://hz.redwolf501.top/gtfjefbdag.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xziqi.cn/gtlusvtpbr.html

PHP:  random_int(1, 100);
来源：http://hz.hywenlv.cn/gtksmqilos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigfzy.top/gtzfdjrlqh.html


<!-- 参考信息 -->