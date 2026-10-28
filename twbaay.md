代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.redwolf501.top/gtttmdqfua.html

throw new RuntimeException("失败", 500);
来源：http://hz.meibo888.top/gtxtawamiv.html

[U72] PHP：写错误日志
来源：http://hz.wangshuangyany.cn/gtpkenaqel.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtbtvdjiyb.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhiwuduotai.top/gtbylflrms.html

parse_ini_file("config.ini", true)
来源：http://hz.zhijiandao.cn/gthtubycuh.html

[U74] PHP：读取环境变量
来源：http://hz.hnxiangtu.top/gtgzapnxph.html

getenv("APP_ENV") ?: "production"
来源：http://hz.wangdashe.top/gtdkkmmfis.html

[U75] PHP：依赖注入
来源：http://hz.yanxiufei.cn/gtstexqrgo.html

composer require psr/container
来源：http://hz.sysykeji.top/gthwgsuuxk.html

[U76] PHP：简单路由
来源：http://hz.jyoumei.cn/gtfotqzyon.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.guowangkeji.top/gtuutczhep.html

[U77] PHP：模板渲染
来源：http://hz.zhongyouzk.top/gtsryliwhh.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtvuhgiqws.html

[U78] PHP：单元测试
来源：http://hz.xuanzx.com/gtzdglxlqq.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gtictctuui.html

[U79] PHP：静态分析
来源：http://hz.tanke756.top/gtuzyvzqbi.html

composer require --dev phpstan/phpstan
来源：http://hz.yj20258888.top/gtlvemseqk.html

[U80] PHP：代码规范修复
来源：http://hz.feifeiyinyue.top/gtpadobkbd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shzxlz.cn/gtbqlwwsrr.html

[U81] JS：初始化项目
来源：http://hz.mhx1999.top/gtusydrnfm.html

npm init -y;  npm i express
来源：http://hz.nwbrower.top/gtswiovwsv.html

[U82] JS：package.json 脚本
来源：http://hz.yuanzhike.top/gtfrocsccc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guowangkeji.top/gtykmrennn.html

[U83] JS：ES Module 导入导出
来源：http://hz.jqgufenzy.top/gttrzocxgy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenzaomai.com/gtafkbblmr.html

[U84] JS：CommonJS 写法
来源：http://hz.sxryk.cn/gtguyvpgum.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aizwys.cn/gtqggktpem.html

[U85] JS：可选链
来源：http://hz.birdmap.top/gtvyrzksfg.html

a?.b?.c
来源：http://hz.zhaomingkeji.xyz/gtykksufgv.html

[U86] JS：空值合并
来源：http://hz.c1oappe.top/gtnrpwfdhn.html

a ?? b
来源：http://hz.ydzc1.top/gtmbmkqmme.html

[U87] JS：解构默认值
来源：http://hz.yueranfly.top/gtagruivcn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hfpthk.cn/gtupckcqvl.html

[U88] JS：对象展开合并
来源：http://hz.sxryk.cn/gtnvosfkwf.html

{ ...a, ...b }
来源：http://hz.hongshengwenyu.top/gtqwjnxmxd.html

[U89] JS：数组去重
来源：http://hz.jyoumei.cn/gtgmtvqiij.html

[...new Set(arr)]
来源：http://hz.cucudq.cn/gtedzopvla.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gthqgpjaup.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtvntuggpy.html

[U91] JS：对象键值遍历
来源：http://hz.jlsjyb.cn/gtbhsiohdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gotoacloud.top/gtaaejyjns.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gtzpnlhfbb.html

structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtlgtwsuke.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtoxpuujgx.html

`共 ${n} 条`
来源：http://hz.gogol.net.cn/gtpidhzmlx.html

[U94] JS：箭头函数
来源：http://hz.sysykeji.top/gtaifxlzby.html

const double = x => x * 2;
来源：http://hz.gotoacloud.top/gtcxdevykd.html

[U95] JS：Promise 包装
来源：http://hz.nwbrower.top/gtkxfrgrjq.html

new Promise((resolve, reject) => {})
来源：http://hz.dianchejie.cn/gtewdiilar.html

[U96] JS：async/await 与异常
来源：http://hz.chenlongwang.top/gtpswekusj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtxltgcsyv.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtpokmpttq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtcvebaoue.html

[U98] JS：fetch 带 JSON
来源：http://hz.aizwys.cn/gtweeqsjnm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtnfxcwlcm.html

[U99] JS：事件监听
来源：http://hz.kuanghao11.cn/gtlsgagigk.html

el.addEventListener("click", e => {})
来源：http://hz.feifeiyinyue.top/gtxbnepfdz.html

[U100] JS：DOM 查询
来源：http://hz.zhixingplan.top/gtvvbmawta.html

document.querySelector(".item")
来源：http://hz.cqqwz.cn/gtcirjekjd.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtdgvjpydp.html

el.classList.toggle("active")
来源：http://hz.hongshengwenyu.top/gtmgdlgdop.html

[U102] JS：本地存储
来源：http://hz.tian-w.cn/gtyrcgytao.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.aibaodan.cn/gtydirdrzp.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtdszgzbcn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuetiantiany.cn/gtrgarxvfb.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtfhiaoqgw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtwmkqbeux.html

[U105] JS：节流
来源：http://hz.c1oappe.top/gttzorrpui.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gotoacloud.top/gtemqnrjlu.html

[U106] JS：日期格式化
来源：http://hz.hnqzz.top/gtwesubamp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yvedp.cn/gtetiprwnr.html

[U107] JS：数字千分位
来源：http://hz.gotoacloud.top/gtnjhbgxez.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guannengcc.top/gtlcxlmxtb.html

[U108] JS：随机整数
来源：http://hz.sweek.top/gttgefjbpz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yangfankeji.com/gtkdmnqqwk.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtbfkbhyly.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtfbzjyren.html

[U110] JS：数组分块
来源：http://hz.aibaodan.cn/gtosvolzxw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gtfxkvyyil.html

[U111] JS：对象转 Map
来源：http://hz.dianchejie.cn/gtgrgnwvrb.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtzdhqdgwd.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gtjjvvhhgk.html

"7".padStart(3, "0")
来源：http://hz.zycfv.cn/gthnvqazzu.html

[U113] JS：正则替换全部
来源：http://hz.316326.xyz/gtxuodjimo.html

s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtbviarnrd.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258.top/gtrkezgyid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtsvhildtu.html

[U115] JS：生成 UUID
来源：http://hz.wangdashe.top/gtlmvsknly.html

crypto.randomUUID()
来源：http://hz.gzhubu.top/gtbkhjijma.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jiagoushi.top/gtjyticzkf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gttxahcruy.html

[U117] JS：单元测试
来源：http://hz.ydzc1.top/gtyejjrdih.html

npm i -D vitest;  npx vitest
来源：http://hz.yuanzhike.top/gtmicofegl.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtezwvupzd.html

npm i -D vite;  npx vite
来源：http://hz.chenjidiqi.icu/gtnnumuuqg.html

[U119] JS：生产构建
来源：http://hz.zhijiandao.cn/gtxzzfstnh.html

npx vite build
来源：http://hz.ppjwa.cn/gthluqtmou.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.0kj1m.cn/gthorcdobh.html

import.meta.env.VITE_API_URL
来源：http://hz.chenlongwang.top/gtbugweyjc.html

================================================================================
来源：http://hz.fengsongda.top/gtwprkzavd.html

统计汇总
来源：http://hz.hywenlv.cn/gtphklrnbc.html

================================================================================
来源：http://hz.cqqwz.cn/gtfznrrhcd.html

按语言统计（条）：
来源：http://hz.shangyingyoupin.top/gttnttstaj.html

Python ......... 252
来源：http://hz.sweek.top/gtppfmkmwt.html

PHP ............ 252
来源：http://hz.0kj1m.cn/gtqyvideni.html

JavaScript ..... 252
来源：http://hz.ivvv.top/gtexucjbqi.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtlrwqlzsg.html

Java ........... 212
来源：http://hz.jianghu66.top/gthmjzrhlf.html

Go ............. 212
来源：http://hz.gogol.net.cn/gtijfjtkvd.html

Ruby ........... 212
来源：http://hz.cucudq.cn/gtueibjruu.html

C# ............. 212
来源：http://hz.jyoumei.cn/gtagfyafmo.html

C .............. 30
来源：http://hz.pengpengdd.cyou/gtpjeimbpg.html

C++ ............ 30
来源：http://hz.yongpay.top/gtstjpaami.html

SQL ............ 90
来源：http://hz.zycfv.cn/gtkvoonhux.html

Bash ........... 80
来源：http://hz.jyoumei.cn/gtjvyhzjwi.html

Kotlin ......... 15
来源：http://hz.feifeiyinyue.top/gtiphkesmg.html

Swift .......... 15
来源：http://hz.sweek.top/gtdpzmqwgn.html

Lua ............ 10
来源：http://hz.zhongyouzk.top/gtqpmypzle.html

Perl ........... 10
来源：http://hz.tianlin.xyz/gtkujtlovm.html

Scala .......... 10
来源：http://hz.sxryk.cn/gtfrgsdeya.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtnbykhfxm.html

合计 ........... 2106 条
来源：http://hz.yj202588.top/gtgwbwxogz.html

按章节统计：
来源：http://hz.yueranfly.top/gtwqgghxgs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cashguo.top/gtguqcnxer.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtwflruuzg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtsbzuxvhb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hywenlv.cn/gtuelxfthq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtwhpllqgo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtmunayvkb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gteoktzaqd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtqnvugxly.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gttprddqcz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hongshengwenyu.top/gtwdnaqlgp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtmwcnxajg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtyqookmxh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtqtmxommt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtgxxvdbhp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.bjfxy.top/gtkkboytts.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtowecydeu.html

Q SQL 专题                              90
来源：http://hz.shzxlz.cn/gtycvalwpu.html

R Bash 专题                             80
来源：http://hz.hnqzz.top/gtnyinxejn.html

S C / C++ 专题                          60
来源：http://hz.hnqzz.top/gthmfknkky.html

T 其他语言补充                          60
来源：http://hz.zhiwuduotai.top/gtfriytcpf.html

U 高频实用片段                         120
来源：http://hz.mhx1999.top/gtvbxahmpz.html

------------------------------------
来源：http://hz.chenzaomai.com/gtexnvdryh.html

合计                                  2106 条
来源：http://hz.zdqjudy.top/gtzjblponr.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtughgjfay.html

使用提醒
来源：http://hz.c1oappe.top/gtsdhbakkh.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtpyfymept.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258.top/gthifbsmnk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guowangkeji.top/gtzmjgcrhg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tanke756.top/gtuycwcgzd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.0kj1m.cn/gtlfdgcvhf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtjnktbado.html

—— 文件结束 ——
来源：http://hz.c1oappe.top/gtbyuxszvv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpfjeohge.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258888.top/gtuvzbmiru.html

Common Programming Examples Cheat Book
来源：http://hz.nanxuanxn.top/gtvvklcokj.html

================================================================================
来源：http://hz.nanxinkj.top/gtmfeszwug.html

【收录内容】
来源：http://hz.wangdashe.top/gtvqquajym.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hammf.cn/gtniflyqfx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.daria6918.cn/gtdefmnzjq.html

SQL · Bash · C · C++
来源：http://hz.vqdsnc.cn/gtcsguivfp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guannengcc.top/gtqeffhsmj.html

【使用说明】
来源：http://hz.jyoumei.cn/gtxevyvvmo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xziqi.cn/gtsqnvzosc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cqqwz.cn/gthvbwhcus.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shzxlz.cn/gtasoljmoh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenzaomai.com/gtoaevnhti.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtqbtflyui.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhaomingkeji.xyz/gtmvbgjmyg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dianchejie.cn/gtqbwiflne.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yueranfly.top/gtuuzftcse.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj202588.top/gtwmqzfase.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.316326.xyz/gtccvempgb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yanxiufei.cn/gtfpjhhhhr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tian-w.cn/gtgddaylxy.html

【文件统计】
来源：http://hz.sysykeji.top/gtqwbvbvyy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.wangdashe.top/gtvhkjttnr.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtjkmxzwxx.html

目  录
来源：http://hz.9152youxi.cn/gtwinoqtgm.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtdakxatei.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.feifeiyinyue.top/gtfibtpigg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gtertdggqi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtmbuprjhc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gtomeqzdne.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj20258.top/gtpyqxtxwf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zdqjudy.top/gtqdxegdlm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gttautlmhl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtdogxouda.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtjpmwpxxs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtvxrjqtoy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtydrmgvyk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtwkpclbah.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtiswjfaxl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtsjicrfym.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.c1oappe.top/gtfebcqjei.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtwrwadzfk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jinghuilouyu.cn/gtmciabylr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yj20258.top/gtzfcfexui.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jlsjyb.cn/gtkbkemboa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtvlwgzbwo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtqgakvwls.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmbqxqltd.html

A. 基础语法与类型
来源：http://hz.jinqigufen.top/gtmqkeddgl.html

================================================================================
来源：http://hz.sweek.top/gtyobrajdc.html

[A01] Hello World
来源：http://hz.zhaomingkeji.xyz/gtwqguesvh.html

Py:   print("Hello, World!")
来源：http://hz.shuidangran.top/gtvsslrhkw.html

PHP:  echo "Hello, World!";
来源：http://hz.wangdashe.top/gtoqukyynw.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258.top/gtqejhgkmd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.daxiang520.top/gtwkkedmdl.html

Java: System.out.println("Hello, World!");
来源：http://hz.316326.xyz/gtrxxnmssq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.tanke756.top/gttxcinqey.html

Ruby: puts "Hello, World!"
来源：http://hz.iojbl.cn/gtjtesfiua.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.52xcode.cn/gtmkfteksc.html

[A02] 变量声明与赋值
来源：http://hz.ywan-chungtsiang.top/gtmtpruxab.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gtujfrqiut.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ywan-chungtsiang.top/gtnxnlypuc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.redwolf501.top/gtvdzgbuwm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hnqzz.top/gtndrvamnq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtpvmuakmd.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gttpoozfpq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ydzc1.top/gtfwkjbpfo.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtngmyfqhk.html

[A03] 常量定义
来源：http://hz.zhongyouzk.top/gtbzhwnzlu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pengpengdd.cyou/gtrcsblkqv.html

PHP:  const PI = 3.14159;
来源：http://hz.dianchejie.cn/gtbiawnvry.html

JS:   const PI = 3.14159;
来源：http://hz.ppjwa.cn/gtfthonwur.html

TS:   const PI: number = 3.14159;
来源：http://hz.jianghu66.top/gtllvellkm.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gttksfcqyb.html

Go:   const PI = 3.14159
来源：http://hz.yj202588.top/gtooblepzk.html

Ruby: PI = 3.14159
来源：http://hz.gotoacloud.top/gtufcezztx.html

C#:   const double PI = 3.14159;
来源：http://hz.ivvv.top/gtbsnekher.html

[A04] 判断变量类型
来源：http://hz.haohaochexian.top/gtaczffyyt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxinkj.top/gtfillhmsy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gaohongyu789.top/gtuqvatxbm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xuanzx.com/gtdtviuaks.html

TS:   typeof x; x instanceof Date
来源：http://hz.haohaochexian.top/gterltchzx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.nanxinkj.top/gtdkhtdkrw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hysaishi.cn/gtzifmumqk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jlsjyb.cn/gtzavmgltp.html

C#:   x.GetType().Name; x is int
来源：http://hz.shanyushiyangkeji.top/gtnimyhuuo.html

[A05] 整数除法与取模
来源：http://hz.vqdsnc.cn/gtlkkziuez.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.snrcjt.cn/gtigyjgscu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.dashuyun.cn/gtuznwnnrw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtrptajztt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sweek.top/gtqadpcmro.html

Java: 7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtgbwrbirt.html

Go:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtnybuvmcn.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtgyxghslf.html

C#:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtnqymlusz.html

[A06] 字符串转数字
来源：http://hz.svipenyu.cn/gtxmodeqfo.html

Py:   int("42"); float("3.14")
来源：http://hz.ywan-chungtsiang.top/gtwghxkqgi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.feifeiyinyue.top/gtslxeqpxx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinghuilouyu.cn/gtgiootlvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydzc1.top/gtxupyjgpu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.andypj.xyz/gtcpzidzje.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj20258888.top/gtfdkyzbek.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.snrcjt.cn/gtypveyxvh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtheeyrrsz.html

[A07] 数字转字符串
来源：http://hz.tanke756.top/gtdbrgrhyr.html

Py:   str(42)
来源：http://hz.nanxuanxn.top/gtsvtnwgli.html

PHP:  (string) 42; strval(42)
来源：http://hz.yonumen.top/gtvekpkfji.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258888.top/gtuhfwvbrf.html

TS:   String(42)
来源：http://hz.hongshengwenyu.top/gtmkzmydjk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhongyouzk.top/gtuuytnwux.html

Go:   strconv.Itoa(42)
来源：http://hz.birdmap.top/gtrpydygqz.html

Ruby: 42.to_s
来源：http://hz.xuetiantiany.cn/gtuwnsrlhk.html

C#:   42.ToString()
来源：http://hz.yuanzhike.top/gtjtnlreux.html

[A08] 取整与四舍五入
来源：http://hz.jiagoushi.top/gtowygklap.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.redwolf501.top/gtvowvfbcm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.aibaodan.cn/gtupgpkkgg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258.top/gtpjjgfuqn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.svipenyu.cn/gtzqslhvii.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yvedp.cn/gtwzgiaawi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jqgufenzy.top/gtufgctkkg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.nwbrower.top/gtvifzjals.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xuanzx.com/gtcwokiuxo.html

[A09] 绝对值与最大最小值
来源：http://hz.aizwys.cn/gtyocitzgm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sysykeji.top/gtxmxpxfqj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gogol.net.cn/gtoruczdwd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jlsjyb.cn/gtlgnszfrn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gtzfzlqebh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtroluqrrd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.bjfxy.top/gtcznjpjun.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zycfv.cn/gtjuxrkyfh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinqigfzy.top/gtgjzriuhf.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtktxqfblt.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhengqikj.top/gtpfumgaun.html

PHP:  random_int(1, 100);
来源：http://hz.yuxming.cn/gtfnqdfxih.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hnqzz.top/gtykcgqtve.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangdashe.top/gtdjpnigie.html

Java: new Random().nextInt(100) + 1
来源：http://hz.feifeiyinyue.top/gtpvnyrils.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sysykeji.top/gtauspuzmv.html

Ruby: rand(1..100)
来源：http://hz.guannengcc.top/gtzrqquvyq.html

C#:   new Random().Next(1, 101)
来源：http://hz.tanke756.top/gtjxkngkwz.html

[A11] 条件表达式（三元）
来源：http://hz.jinghuilouyu.cn/gtyjvjewqy.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhijiandao.cn/gtlfcdeqty.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtmtqvhqjg.html


<!-- 参考信息 -->