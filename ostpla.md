代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.yj20258888.top/gtnkyxrfwz.html

throw new RuntimeException("失败", 500);
来源：http://hz.52xcode.cn/gtnrdnuhzi.html

[U72] PHP：写错误日志
来源：http://hz.tianlin.xyz/gtcddzjnxm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.0kj1m.cn/gtyokmauuu.html

[U73] PHP：读取 ini 配置
来源：http://hz.52xcode.cn/gtwergjfrw.html

parse_ini_file("config.ini", true)
来源：http://hz.andypj.xyz/gtnnghztjb.html

[U74] PHP：读取环境变量
来源：http://hz.ydzc1.top/gtzdygsxgy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fzhhl.top/gtpopjemwt.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtinlevdlu.html

composer require psr/container
来源：http://hz.dashuyun.cn/gtssfowdii.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtgagpvhvl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.316326.xyz/gtxsbuzsbi.html

[U77] PHP：模板渲染
来源：http://hz.sufxvd.cn/gtxgrkhtku.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtnkukhuxa.html

[U78] PHP：单元测试
来源：http://hz.cheryme.top/gtfhkvrlwn.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtzxbpwenp.html

[U79] PHP：静态分析
来源：http://hz.vqdsnc.cn/gtwvoznuna.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtplupeqmv.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtnvuvxwfo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hongshengwenyu.top/gtonifivde.html

[U81] JS：初始化项目
来源：http://hz.yj202588.top/gtjlqazhyb.html

npm init -y;  npm i express
来源：http://hz.jianghu66.top/gtzttuyenl.html

[U82] JS：package.json 脚本
来源：http://hz.ywan-chungtsiang.top/gtkepbtmzi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hammf.cn/gtpaupwrsi.html

[U83] JS：ES Module 导入导出
来源：http://hz.svipenyu.cn/gtppwyzkhg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtqwziirpm.html

[U84] JS：CommonJS 写法
来源：http://hz.shuidangran.top/gtfohhovgh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuxming.cn/gtchgvkmjx.html

[U85] JS：可选链
来源：http://hz.zhongyouzk.top/gtlsaqobce.html

a?.b?.c
来源：http://hz.tian-w.cn/gtxylsfxzl.html

[U86] JS：空值合并
来源：http://hz.316326.xyz/gtdvgkbxxj.html

a ?? b
来源：http://hz.yj20258888.top/gtspetfalj.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtzwaclihk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yongpay.top/gtmsbxdedb.html

[U88] JS：对象展开合并
来源：http://hz.yuanzhike.top/gtygbkggyx.html

{ ...a, ...b }
来源：http://hz.iojbl.cn/gtaujamyql.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtkkbpmiuw.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtcqhgxuev.html

[U90] JS：数字数组排序
来源：http://hz.sysykeji.top/gtnmuuoczu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtqhyxjihf.html

[U91] JS：对象键值遍历
来源：http://hz.sxryk.cn/gtbldmdaec.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinghuilouyu.cn/gtkdtkkbzp.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtlrpqjwyq.html

structuredClone(obj)
来源：http://hz.jyoumei.cn/gturjcazip.html

[U93] JS：模板字符串
来源：http://hz.gzhubu.top/gtlaiosugf.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtrbzrprdk.html

[U94] JS：箭头函数
来源：http://hz.0kj1m.cn/gteuyvouwv.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gteyaymmmc.html

[U95] JS：Promise 包装
来源：http://hz.sysykeji.top/gtibjhmuhl.html

new Promise((resolve, reject) => {})
来源：http://hz.tanke756.top/gtrulqizcp.html

[U96] JS：async/await 与异常
来源：http://hz.shangyingyoupin.top/gtigvcwbos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtuvnbvxla.html

[U97] JS：并发请求
来源：http://hz.mhx1999.top/gteaplsewu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gttjbiffud.html

[U98] JS：fetch 带 JSON
来源：http://hz.sysykeji.top/gtpgbztnbv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yonumen.top/gtoqdorhkq.html

[U99] JS：事件监听
来源：http://hz.hywenlv.cn/gtvcmcanwd.html

el.addEventListener("click", e => {})
来源：http://hz.zhoulong.xyz/gtdealrbhc.html

[U100] JS：DOM 查询
来源：http://hz.c1oappe.top/gtuhzpvsbz.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtknemoxmx.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtsyuqcafu.html

el.classList.toggle("active")
来源：http://hz.shzxlz.cn/gtelicxylb.html

[U102] JS：本地存储
来源：http://hz.zdqjudy.top/gtwiikzfhk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shanyushiyangkeji.top/gtwmxwyvaw.html

[U103] JS：定时器
来源：http://hz.andypj.xyz/gtydjwfrul.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gtkwuavbsk.html

[U104] JS：防抖
来源：http://hz.gogol.net.cn/gtamiqjmxv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtkycokowq.html

[U105] JS：节流
来源：http://hz.9152youxi.cn/gtjnzettgg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtmtqwarfs.html

[U106] JS：日期格式化
来源：http://hz.redwolf501.top/gtzijvjkph.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zycfv.cn/gtxuqzjvff.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtgpyjpxpy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.redwolf501.top/gtgzvdtjbo.html

[U108] JS：随机整数
来源：http://hz.zhengqikj.top/gtkakapaez.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yuxming.cn/gthrxpltui.html

[U109] JS：数组分组
来源：http://hz.jinyuanbaomall.cn/gtancinxuo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtiatfuvgg.html

[U110] JS：数组分块
来源：http://hz.aizwys.cn/gtmawdnjqt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hongshengwenyu.top/gtbxvcxfvz.html

[U111] JS：对象转 Map
来源：http://hz.yanxiufei.cn/gtczmsgbxk.html

new Map(Object.entries(obj))
来源：http://hz.wangshuangyany.cn/gtfjivtxon.html

[U112] JS：字符串补位
来源：http://hz.fzhhl.top/gtdpajgfwe.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtsoxypyaj.html

[U113] JS：正则替换全部
来源：http://hz.nanxinkj.top/gtwnvbirfk.html

s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtgvfgksqg.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtxskmrink.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtcghxcmsv.html

[U115] JS：生成 UUID
来源：http://hz.yuxming.cn/gtqqlsvcck.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtzopgxqty.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gteorkjxdf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuetiantiany.cn/gtcjwpuiby.html

[U117] JS：单元测试
来源：http://hz.pycfn.com/gtpkdsdyrg.html

npm i -D vitest;  npx vitest
来源：http://hz.wangshuangyany.cn/gtndikhjaj.html

[U118] JS：开发服务器
来源：http://hz.hysaishi.cn/gtsjyldilf.html

npm i -D vite;  npx vite
来源：http://hz.hywenlv.cn/gtsqxpgkkv.html

[U119] JS：生产构建
来源：http://hz.dianchejie.cn/gtnomvgaqy.html

npx vite build
来源：http://hz.52xcode.cn/gtthwbcnjy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtzhwapcbr.html

import.meta.env.VITE_API_URL
来源：http://hz.316326.xyz/gtxqiwvfcw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqxypkpjs.html

统计汇总
来源：http://hz.sufxvd.cn/gtjttwlqvo.html

================================================================================
来源：http://hz.mhx1999.top/gtxgdptyok.html

按语言统计（条）：
来源：http://hz.ywan-chungtsiang.top/gtwnserdxl.html

Python ......... 252
来源：http://hz.shzxlz.cn/gtmjxwabaa.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtoufteuox.html

JavaScript ..... 252
来源：http://hz.yuxming.cn/gtwwwxoand.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtcjkdezvw.html

Java ........... 212
来源：http://hz.cucudq.cn/gtjsmvhrkg.html

Go ............. 212
来源：http://hz.zhijiandao.cn/gtvcxpjeaf.html

Ruby ........... 212
来源：http://hz.quarkkingdee.top/gtbqeibrcp.html

C# ............. 212
来源：http://hz.haohaochexian.top/gtrlsvvsqr.html

C .............. 30
来源：http://hz.nwbrower.top/gtdsyhwjeu.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtahocbeng.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtniekstky.html

Bash ........... 80
来源：http://hz.gogol.net.cn/gtijecpomc.html

Kotlin ......... 15
来源：http://hz.jianghu66.top/gtsrppjebw.html

Swift .......... 15
来源：http://hz.meibo888.top/gtetyolwlh.html

Lua ............ 10
来源：http://hz.jqgfzy.top/gtacyltavn.html

Perl ........... 10
来源：http://hz.kuanghao11.cn/gtgtxtfmdr.html

Scala .......... 10
来源：http://hz.yongpay.top/gtrgrzeiyk.html

------------------------------------
来源：http://hz.xinyue.icu/gtfrtfeaqk.html

合计 ........... 2106 条
来源：http://hz.redwolf501.top/gtmgwerewx.html

按章节统计：
来源：http://hz.aizwys.cn/gtzxcphpaf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtdflhivgd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtqamdqalg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtxojwbngl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtkapzcrjv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yvedp.cn/gtrqtlyawd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtbphfpqlg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtrtqqgpae.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cdnleiting.top/gtzoaikqnv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtaulnsklb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtzfrzxkue.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtwzrmsafu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gthwgglxpw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtthjtligp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shzxlz.cn/gtogtrjiet.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gtcnrujjcc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gthgjxjurc.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gttozxbmad.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gtrdkboksj.html

S C / C++ 专题                          60
来源：http://hz.shuidangran.top/gthzqfxygh.html

T 其他语言补充                          60
来源：http://hz.guowangkeji.top/gtfrdofkje.html

U 高频实用片段                         120
来源：http://hz.aibaodan.cn/gtgfuysafu.html

------------------------------------
来源：http://hz.zhixingplan.top/gtmgauybsq.html

合计                                  2106 条
来源：http://hz.jqgufenzy.top/gtvbfjmdbh.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtpadipmfv.html

使用提醒
来源：http://hz.xylfe.cn/gtlktgfiem.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtzkyqccrd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ehwqpu.com/gtkkbpgedz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tian-w.cn/gtquteelwu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gogol.net.cn/gtfztplbuu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cheryme.top/gtgadqohxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinqigufen.top/gtnbjmlypo.html

—— 文件结束 ——
来源：http://hz.zhaomingkeji.xyz/gtadeiicuh.html

================================================================================
来源：http://hz.svipenyu.cn/gtmghrvfss.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.meibo888.top/gtuwwrojte.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gtrflnfaqd.html

================================================================================
来源：http://hz.zhongyouzk.top/gthqvglxdj.html

【收录内容】
来源：http://hz.zycfv.cn/gtmfopaitj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinyuanbaomall.cn/gttebvyplm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.0kj1m.cn/gtiwycmtzh.html

SQL · Bash · C · C++
来源：http://hz.jyoumei.cn/gtutvjaulf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtwtvueukh.html

【使用说明】
来源：http://hz.shuidangran.top/gtponeloiw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zdqjudy.top/gtioysijbn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jlsjyb.cn/gtznsnmdku.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtviyhyyrv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shzxlz.cn/gtdbogmikt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jiagoushi.top/gtqzixcrwh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sweek.top/gthbeunjkc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gzhubu.top/gtbfrlnxgo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cheryme.top/gtsxwqtvvw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxinkj.top/gtqhznxdmd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yanxiufei.cn/gtchfaabui.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gaohongyu789.top/gtdissdqck.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj20258888.top/gtmffvpbkm.html

【文件统计】
来源：http://hz.hammf.cn/gtlxgrfkzj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sysykeji.top/gtxjnupkoq.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtpegmoafo.html

目  录
来源：http://hz.xuanzx.com/gtihcippws.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtqsdhohht.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhoulong.xyz/gtqxelztuq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtbowknmod.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtbvkcqvnt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gttfflafcn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tanke756.top/gtrvhqtcnl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtbhktspbe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gttatwxfpf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gteugtgsbh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtduiwtrec.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtqdptjskv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtphkbzgzk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gteclcqtic.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtudbczrgp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gttbmqnzjz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hysaishi.cn/gtnqubaaky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtzbrafwhi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yuxming.cn/gtuuzfusfs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.svipenyu.cn/gteigeaexz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gogol.net.cn/gtqpvrbbyw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtakvgufmj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yangfankeji.com/gtpsjwksrt.html

================================================================================
来源：http://hz.mhx1999.top/gtujqvzewr.html

A. 基础语法与类型
来源：http://hz.jyoumei.cn/gtlxihowdn.html

================================================================================
来源：http://hz.nwbrower.top/gtbaqllwlm.html

[A01] Hello World
来源：http://hz.nwbrower.top/gtayzqydlk.html

Py:   print("Hello, World!")
来源：http://hz.jlsjyb.cn/gtyziijnik.html

PHP:  echo "Hello, World!";
来源：http://hz.316326.xyz/gtyvzipzzk.html

JS:   console.log("Hello, World!");
来源：http://hz.smart0.xyz/gttqzteoqa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xinyue.icu/gtdjrmwogb.html

Java: System.out.println("Hello, World!");
来源：http://hz.ppjwa.cn/gtwmmwlwxy.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258.top/gtewpqykjd.html

Ruby: puts "Hello, World!"
来源：http://hz.xinyue.icu/gtuggqtlbl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tian-w.cn/gtieupkqpk.html

[A02] 变量声明与赋值
来源：http://hz.nwbrower.top/gtgwfwwmzg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jianghu66.top/gttjadfjww.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jiagoushi.top/gtszhguoqr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhijiandao.cn/gtlkhtixag.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hywenlv.cn/gtwidlakzs.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jqgufenzy.top/gtllzmtcjf.html

Go:   name := "Alex"; age := 20
来源：http://hz.havefunace.top/gtfttiwfqw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sweek.top/gtfcmpjzpx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtawgitbuu.html

[A03] 常量定义
来源：http://hz.fzhhl.top/gtrceiflfb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxuanxn.top/gtogvnjjqd.html

PHP:  const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtzidpfmci.html

JS:   const PI = 3.14159;
来源：http://hz.xuanzx.com/gtnfvjuell.html

TS:   const PI: number = 3.14159;
来源：http://hz.gzhubu.top/gtbixzvmbh.html

Java: static final double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtagaoiuyl.html

Go:   const PI = 3.14159
来源：http://hz.mhx1999.top/gtalaiumeh.html

Ruby: PI = 3.14159
来源：http://hz.snrcjt.cn/gtjywljhsb.html

C#:   const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtqurcijaz.html

[A04] 判断变量类型
来源：http://hz.wangdashe.top/gtdlnxycqp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenjidiqi.icu/gtzmxauicg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gogol.net.cn/gtvgjbdnis.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.fengsongda.top/gtjwlooecg.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtlwcchart.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shzxlz.cn/gtfoqcnoab.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shanyushiyangtech.top/gtzgasfigj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gthvmqhujb.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gttmynshtb.html

[A05] 整数除法与取模
来源：http://hz.zhaomingkeji.xyz/gtdfysbeom.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gogol.net.cn/gtvhpzuhwf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ppjwa.cn/gtmelczufd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hysaishi.cn/gtklfsusmu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtbouyhixe.html

Java: 7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtpnarfjdb.html

Go:   7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtfteniomt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtifsemjsz.html

C#:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gthzmzcqwx.html

[A06] 字符串转数字
来源：http://hz.ehwqpu.com/gtfvtawrhp.html

Py:   int("42"); float("3.14")
来源：http://hz.yj20258888.top/gtintjnxau.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cheryme.top/gtqanhcptc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ywan-chungtsiang.top/gtbagllntt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.daria6918.cn/gtndgxcpwn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xuanzx.com/gtrjlhvdze.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gogol.net.cn/gtnzrjmnwf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinqigufen.top/gtihesjadj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shangyingyoupin.top/gtdcualtlf.html

[A07] 数字转字符串
来源：http://hz.cqqwz.cn/gtmipllrsz.html

Py:   str(42)
来源：http://hz.yangfankeji.com/gtmjqibukb.html

PHP:  (string) 42; strval(42)
来源：http://hz.snrcjt.cn/gtljkqxlre.html

JS:   String(42); (42).toString()
来源：http://hz.zhaomingkeji.xyz/gtkvqkokfz.html

TS:   String(42)
来源：http://hz.smart0.xyz/gtsmxkaekb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhengqikj.top/gtxhglkbxd.html

Go:   strconv.Itoa(42)
来源：http://hz.daria6918.cn/gtntflyahw.html

Ruby: 42.to_s
来源：http://hz.chenzaomai.com/gtkwqkcdss.html

C#:   42.ToString()
来源：http://hz.sufxvd.cn/gtruapzyoz.html

[A08] 取整与四舍五入
来源：http://hz.zdqjudy.top/gtrhfncmhg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jianghu66.top/gtdkpmbufk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.sweek.top/gtbvxfahir.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ehwqpu.com/gtxkaudgtq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.wangdashe.top/gthvbsuujj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jiagoushi.top/gtpvxoxdfp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.nanxinkj.top/gtslfkciuj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.smart0.xyz/gtnejowoub.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nwbrower.top/gtuouxltjn.html

[A09] 绝对值与最大最小值
来源：http://hz.jinqigufen.top/gtonfiuzrq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtnwivduwz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guannengcc.top/gtwvtnuech.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.daxiang520.top/gtykheuqtq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.9152youxi.cn/gtlysfkqil.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yonumen.top/gtefgqkbqe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.kuanghao11.cn/gtffhiplbm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tianlin.xyz/gtbijwgcsy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sufxvd.cn/gtgbifqcqa.html

[A10] 生成随机数
来源：http://hz.yvedp.cn/gtqctclgix.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhoulong.xyz/gthtjdeyxy.html

PHP:  random_int(1, 100);
来源：http://hz.jqgfzy.top/gteehgrsmy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sxryk.cn/gtykdfnvay.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.feifeiyinyue.top/gtmlrzgrcx.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hfpthk.cn/gtevoccqiv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhoulong.xyz/gtgeemhnnu.html

Ruby: rand(1..100)
来源：http://hz.jyoumei.cn/gtenukwgly.html

C#:   new Random().Next(1, 101)
来源：http://hz.pengpengdd.cyou/gtqqcruwgf.html

[A11] 条件表达式（三元）
来源：http://hz.nanxuanxn.top/gtkktzkinz.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.dashuyun.cn/gtcsuhjzcj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtmlitbtbd.html


<!-- 参考信息 -->