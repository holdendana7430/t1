代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.jqgfzy.top/gtfvorfdeo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinghuilouyu.cn/gtcijdrobb.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gtiwkmicep.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aibaodan.cn/gtmcwzwhtu.html

[U69] PHP：PDO 预处理
来源：http://hz.andypj.xyz/gtgmoywdiv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gtzlrsnzbe.html

[U70] PHP：PDO 事务
来源：http://hz.dashuyun.cn/gthpzwxlrt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pycfn.com/gtvtyfoelx.html

[U71] PHP：抛出异常
来源：http://hz.sxryk.cn/gtkchoflzy.html

throw new RuntimeException("失败", 500);
来源：http://hz.sufxvd.cn/gtfkwqybgr.html

[U72] PHP：写错误日志
来源：http://hz.pycfn.com/gtttugnsod.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cheryme.top/gthwpijkjd.html

[U73] PHP：读取 ini 配置
来源：http://hz.xziqi.cn/gtdnhwhetp.html

parse_ini_file("config.ini", true)
来源：http://hz.hongshengwenyu.top/gtaqqpwusy.html

[U74] PHP：读取环境变量
来源：http://hz.xinyue.icu/gthmnifner.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sufxvd.cn/gtorvdkddf.html

[U75] PHP：依赖注入
来源：http://hz.c1oappe.top/gtdamypxga.html

composer require psr/container
来源：http://hz.cdnleiting.top/gtvaqdttuo.html

[U76] PHP：简单路由
来源：http://hz.wangshuangyany.cn/gtfvtprtnb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhoulong.xyz/gtsaotaegv.html

[U77] PHP：模板渲染
来源：http://hz.daria6918.cn/gtuexajunw.html

composer require twig/twig
来源：http://hz.vqdsnc.cn/gtvtoiqeuv.html

[U78] PHP：单元测试
来源：http://hz.c1oappe.top/gtthrzxihg.html

composer require --dev phpunit/phpunit
来源：http://hz.ehwqpu.com/gtvhwwibez.html

[U79] PHP：静态分析
来源：http://hz.xziqi.cn/gtovcraoas.html

composer require --dev phpstan/phpstan
来源：http://hz.xuanzx.com/gtjpuizcsk.html

[U80] PHP：代码规范修复
来源：http://hz.tanke756.top/gtvzdttckw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xinyue.icu/gtzshbqurr.html

[U81] JS：初始化项目
来源：http://hz.yueranfly.top/gtfipnfurh.html

npm init -y;  npm i express
来源：http://hz.fengsongda.top/gtqgshuwik.html

[U82] JS：package.json 脚本
来源：http://hz.hongshengwenyu.top/gtgtvbqjsq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tanke756.top/gtsvqwbueg.html

[U83] JS：ES Module 导入导出
来源：http://hz.pycfn.com/gtsvmddrpp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhijiandao.cn/gtlswtvqsm.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtjvuojxpx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shanyushiyangtech.top/gtuneqelor.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtshniasiu.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtecdfpbut.html

[U86] JS：空值合并
来源：http://hz.gzhubu.top/gtrfwkghkd.html

a ?? b
来源：http://hz.yj20258.top/gtrycoeqbu.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtdeqewmda.html

const { a = 1, b = 2 } = obj;
来源：http://hz.birdmap.top/gtqoyqmyjq.html

[U88] JS：对象展开合并
来源：http://hz.mhx1999.top/gtogjuxxaw.html

{ ...a, ...b }
来源：http://hz.yonumen.top/gtyfkzrker.html

[U89] JS：数组去重
来源：http://hz.tian-w.cn/gthhmfxsdr.html

[...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtcggnzsoi.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtvcqnocrp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtuzmskodw.html

[U91] JS：对象键值遍历
来源：http://hz.jyoumei.cn/gtgiqhaexz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yvedp.cn/gtglpxdqma.html

[U92] JS：深拷贝
来源：http://hz.aibaodan.cn/gtehbwozof.html

structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtmaffjngd.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangtech.top/gtjlugyrok.html

`共 ${n} 条`
来源：http://hz.birdmap.top/gtfzpqnqzf.html

[U94] JS：箭头函数
来源：http://hz.xingfuxueyuan.xyz/gtrbrynbbi.html

const double = x => x * 2;
来源：http://hz.yangfankeji.com/gtribadcae.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtiqeylxcc.html

new Promise((resolve, reject) => {})
来源：http://hz.hammf.cn/gtyaguemuu.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtpxdzqauv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtyjhcmjju.html

[U97] JS：并发请求
来源：http://hz.xinyue.icu/gterzkbykc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtbsoxvhht.html

[U98] JS：fetch 带 JSON
来源：http://hz.gogol.net.cn/gtnhwpesma.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xinyue.icu/gtzdbygyxl.html

[U99] JS：事件监听
来源：http://hz.ybcxt.top/gtfvrruqnd.html

el.addEventListener("click", e => {})
来源：http://hz.ybcxt.top/gtiyzdppwh.html

[U100] JS：DOM 查询
来源：http://hz.hongshengwenyu.top/gtqnhcvhxp.html

document.querySelector(".item")
来源：http://hz.zycfv.cn/gtdgdzoqcv.html

[U101] JS：classList 操作
来源：http://hz.jqgufenzy.top/gtwkdnufhl.html

el.classList.toggle("active")
来源：http://hz.vqdsnc.cn/gtjthxpchq.html

[U102] JS：本地存储
来源：http://hz.316326.xyz/gtxwuumcde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guannengcc.top/gtdoiheubq.html

[U103] JS：定时器
来源：http://hz.jinghuilouyu.cn/gtzkqdirqn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhijiandao.cn/gtzkrzhkhj.html

[U104] JS：防抖
来源：http://hz.xuetiantiany.cn/gtdmzkegiu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtrrfwblas.html

[U105] JS：节流
来源：http://hz.52xcode.cn/gtgvlmrskg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.mhx1999.top/gtczkmovzn.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtftywmjyy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigfzy.top/gtjcpkocgf.html

[U107] JS：数字千分位
来源：http://hz.fengsongda.top/gtvaldhlth.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.meibo888.top/gtsqmsvwbe.html

[U108] JS：随机整数
来源：http://hz.yuanzhike.top/gtxeijsfnm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.pycfn.com/gtgkpztmxi.html

[U109] JS：数组分组
来源：http://hz.yj202588.top/gtgtbnopdv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gtjwvzichp.html

[U110] JS：数组分块
来源：http://hz.jianghu66.top/gtdunhpsab.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gtzotckybi.html

[U111] JS：对象转 Map
来源：http://hz.sysykeji.top/gtjwihjbpx.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gtjmbsdiqo.html

[U112] JS：字符串补位
来源：http://hz.quarkkingdee.top/gtojshelyv.html

"7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gthpcfzvnt.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gtfbhbywdn.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtvpsghmbq.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258.top/gtbxfsqasd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtovjdjqyt.html

[U115] JS：生成 UUID
来源：http://hz.yangfankeji.com/gtgotdfkyu.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtwrlunxox.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ehwqpu.com/gtnmacwspj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhijiandao.cn/gtkuiwjjqs.html

[U117] JS：单元测试
来源：http://hz.wangdashe.top/gtwmjkumob.html

npm i -D vitest;  npx vitest
来源：http://hz.meibo888.top/gthylzhkam.html

[U118] JS：开发服务器
来源：http://hz.kuanghao11.cn/gtmcdreqdz.html

npm i -D vite;  npx vite
来源：http://hz.yanxiufei.cn/gtotjpizif.html

[U119] JS：生产构建
来源：http://hz.hammf.cn/gtoclsaoqr.html

npx vite build
来源：http://hz.hysaishi.cn/gtwqonyoha.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtupnzvvro.html

import.meta.env.VITE_API_URL
来源：http://hz.yonumen.top/gtjdgetvhk.html

================================================================================
来源：http://hz.daria6918.cn/gtzbauzhzm.html

统计汇总
来源：http://hz.hongshengwenyu.top/gtiejbwfep.html

================================================================================
来源：http://hz.cucudq.cn/gtkoyqatjn.html

按语言统计（条）：
来源：http://hz.zhaomingkeji.xyz/gttngzojpj.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gtzyegpegb.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gtfbdpntgh.html

JavaScript ..... 252
来源：http://hz.vqdsnc.cn/gtxdwkbdns.html

TypeScript ..... 212
来源：http://hz.shangyingyoupin.top/gtcyltysza.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtdzvsrcrp.html

Go ............. 212
来源：http://hz.cucudq.cn/gtlijapigs.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtvctzadpo.html

C# ............. 212
来源：http://hz.hammf.cn/gtmyuzhzue.html

C .............. 30
来源：http://hz.feifeiyinyue.top/gtwvxvkxgd.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtyoqywniw.html

SQL ............ 90
来源：http://hz.xingfuxueyuan.xyz/gtgnkzdcmk.html

Bash ........... 80
来源：http://hz.cheryme.top/gthmveutsq.html

Kotlin ......... 15
来源：http://hz.shanyushiyangkeji.top/gtybnjtaiq.html

Swift .......... 15
来源：http://hz.snrcjt.cn/gtzlftmlmz.html

Lua ............ 10
来源：http://hz.smart0.xyz/gtwqqzwchq.html

Perl ........... 10
来源：http://hz.yuxming.cn/gtfwhvwqaf.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtbxdayjnd.html

------------------------------------
来源：http://hz.gogol.net.cn/gtlbhdjggo.html

合计 ........... 2106 条
来源：http://hz.yangfankeji.com/gtkqfxkxvj.html

按章节统计：
来源：http://hz.shanyushiyangtech.top/gtaikemwnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tian-w.cn/gtqbkaojme.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtldgqlfqz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtedhbijhd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtnhimdfbk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.redwolf501.top/gtdcugvfcu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yangfankeji.com/gtmutlogfu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtamgiswfa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtcordyyzm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtcvkgaxnx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hongshengwenyu.top/gtgdvvrefp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtqqrojhcb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtzpmmxbnr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtwydpcyam.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtqexwapkv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sxryk.cn/gtfujdjtkd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtnwuqputs.html

Q SQL 专题                              90
来源：http://hz.fzhhl.top/gtxxouhqfo.html

R Bash 专题                             80
来源：http://hz.yj20258888.top/gtpdphnlau.html

S C / C++ 专题                          60
来源：http://hz.yonumen.top/gtzhgallog.html

T 其他语言补充                          60
来源：http://hz.daria6918.cn/gteklsetlz.html

U 高频实用片段                         120
来源：http://hz.ydjk.org.cn/gtehvjwbnj.html

------------------------------------
来源：http://hz.yanxiufei.cn/gtdqbijibb.html

合计                                  2106 条
来源：http://hz.yuxming.cn/gtwarirxjo.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtipvksqcr.html

使用提醒
来源：http://hz.aizwys.cn/gtuoddebnd.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtpihroegl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtnuqptyhq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yvedp.cn/gtxsebmjyp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhaomingkeji.xyz/gtyauyivzo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtgapeztdb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hfpthk.cn/gtnazxqqau.html

—— 文件结束 ——
来源：http://hz.yongpay.top/gtzvsmegjo.html

================================================================================
来源：http://hz.vqdsnc.cn/gteuahqkzg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yangfankeji.com/gtsosfezmw.html

Common Programming Examples Cheat Book
来源：http://hz.daria6918.cn/gtapkrjkfe.html

================================================================================
来源：http://hz.ybcxt.top/gtddbspcak.html

【收录内容】
来源：http://hz.pengpengdd.cyou/gtuacmitdq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.mhx1999.top/gtcodihbyg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.9152youxi.cn/gtshngikzh.html

SQL · Bash · C · C++
来源：http://hz.yanxiufei.cn/gtovvwtcim.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.andypj.xyz/gtyjdtqluk.html

【使用说明】
来源：http://hz.guowangkeji.top/gtmmfulrlx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jianghu66.top/gtmluhabpw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guowangkeji.top/gtpeperinf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yanxiufei.cn/gtppxtkzsc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.bjfxy.top/gtavsxbrmw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cashguo.top/gtmpguympp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gtcmoluyci.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.tanke756.top/gtdjdmhovb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xylfe.cn/gtidjmslct.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xingfuxueyuan.xyz/gtnxzfwfxr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenlongwang.top/gtwlyzpdqt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tian-w.cn/gtmlpbnezf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangshuangyany.cn/gtesnmzziw.html

【文件统计】
来源：http://hz.jlsjyb.cn/gtujyzqdpe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jianghu66.top/gtozllvvdb.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtkozvrgyn.html

目  录
来源：http://hz.zhixingplan.top/gtmjxrxusm.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtjvtsyvjv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yj20258888.top/gttzufkbhl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtjkekplmh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gtenbojjzw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtjuegzjwy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yangfankeji.com/gtfilyufit.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gtysdgjkls.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtwqeiewgb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtijbdcpcb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gteawuskjv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtbucwsedg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtzyqwoedh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtowqmefxv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtclvgzfuo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hysaishi.cn/gtuicbwvdi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shuidangran.top/gtjbbbisup.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtovqmjajj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shangyingyoupin.top/gtknbfdgjl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shangyingyoupin.top/gtdsyfzwbc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cashguo.top/gtiijtsajk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtjfcxuzbx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtbhmrubdm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbunpvdtm.html

A. 基础语法与类型
来源：http://hz.zhongyouzk.top/gtddbpratf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqlsctsqv.html

[A01] Hello World
来源：http://hz.zhixingplan.top/gtovepimqp.html

Py:   print("Hello, World!")
来源：http://hz.ydjk.org.cn/gtjxkijwnu.html

PHP:  echo "Hello, World!";
来源：http://hz.wangshuangyany.cn/gtzzfkkaum.html

JS:   console.log("Hello, World!");
来源：http://hz.havefunace.top/gtykitmdjs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ydzc1.top/gtrkxetnhg.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gtbtpkfqlt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.pengpengdd.cyou/gtptwibpzc.html

Ruby: puts "Hello, World!"
来源：http://hz.ivvv.top/gtjbwatbiw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenzaomai.com/gtekeelpom.html

[A02] 变量声明与赋值
来源：http://hz.ehwqpu.com/gtmncwecpt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.daria6918.cn/gtczrplbrv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.0kj1m.cn/gtthaqwlfx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yangfankeji.com/gtpczyxuvg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hammf.cn/gtjgereunk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtiqivrrfs.html

Go:   name := "Alex"; age := 20
来源：http://hz.tanke756.top/gtihvqwcwh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cqqwz.cn/gtgppyytsw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cashguo.top/gtrbaycnzk.html

[A03] 常量定义
来源：http://hz.sweek.top/gteewyqygk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hywenlv.cn/gtbbuifeod.html

PHP:  const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtlyzbvvlr.html

JS:   const PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtypkugpup.html

TS:   const PI: number = 3.14159;
来源：http://hz.sxryk.cn/gtkxiincqs.html

Java: static final double PI = 3.14159;
来源：http://hz.cdnleiting.top/gtlzegmjew.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangtech.top/gtakkqgqzu.html

Ruby: PI = 3.14159
来源：http://hz.jyoumei.cn/gtnkrkvlkg.html

C#:   const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtppqszxfi.html

[A04] 判断变量类型
来源：http://hz.zhixingplan.top/gtdzbngfmr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigufen.top/gtvqocomtj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gthlcygnxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.bjfxy.top/gteoliexym.html

TS:   typeof x; x instanceof Date
来源：http://hz.bjfxy.top/gthdoeshmm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daxiang520.top/gtnnhtlvcu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.aizwys.cn/gtjkkeimsb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.wangshuangyany.cn/gttaeabejm.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtctesgopv.html

[A05] 整数除法与取模
来源：http://hz.hysaishi.cn/gtoaylbubo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.dianchejie.cn/gtpkkcujhd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtbivzkaxx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daria6918.cn/gtqxctjrxu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jlsjyb.cn/gtszghgewz.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtkgoigjle.html

Go:   7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtqbznookn.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtobqzzndw.html

C#:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtmlnvkaav.html

[A06] 字符串转数字
来源：http://hz.zhijiandao.cn/gtkrekxrsp.html

Py:   int("42"); float("3.14")
来源：http://hz.ppjwa.cn/gtfpfllkkq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xingfuxueyuan.xyz/gtktpxxpsk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xuanzx.com/gtdlmtrtpq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yuxming.cn/gtnrjrazjz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuanzhike.top/gtfuxlkcbj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtgockflmx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hnxiangtu.top/gtqqkdzkrs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ivvv.top/gtesckumcc.html

[A07] 数字转字符串
来源：http://hz.hfpthk.cn/gtxmaceqng.html

Py:   str(42)
来源：http://hz.xuetiantiany.cn/gtlonkskxu.html

PHP:  (string) 42; strval(42)
来源：http://hz.dianchejie.cn/gtvfkfzmgr.html

JS:   String(42); (42).toString()
来源：http://hz.sxryk.cn/gtwalxsydi.html

TS:   String(42)
来源：http://hz.316326.xyz/gtrvgvczta.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hysaishi.cn/gtvasxineg.html

Go:   strconv.Itoa(42)
来源：http://hz.meibo888.top/gtufaoixfj.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gtgefpzbas.html

C#:   42.ToString()
来源：http://hz.sufxvd.cn/gtpvyzgixp.html

[A08] 取整与四舍五入
来源：http://hz.jiagoushi.top/gtogkjgpkp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.9152youxi.cn/gtkocjdkwz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.meibo888.top/gtiemtlzex.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ehwqpu.com/gtfnggsfbc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.mhx1999.top/gtjehhkgrg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cqqwz.cn/gtpryyotyi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.aibaodan.cn/gtynlqzeuj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.gotoacloud.top/gtufhkxfel.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.bjfxy.top/gtockzezvd.html

[A09] 绝对值与最大最小值
来源：http://hz.yj20258.top/gtnkmckttl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ydjk.org.cn/gtsbopubyq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.vqdsnc.cn/gtzikxioec.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yj20258.top/gtnzahcerz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ivvv.top/gtbufjkabd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtvijfgefi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj20258888.top/gtlxkcokka.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.meibo888.top/gthieodlsv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sweek.top/gtzdqyqucx.html

[A10] 生成随机数
来源：http://hz.ehwqpu.com/gtmtxgwsmr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jinqigfzy.top/gtuhxhescx.html

PHP:  random_int(1, 100);
来源：http://hz.zhaomingkeji.xyz/gtgqdcrvbw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangdashe.top/gtkvbiglwq.html


<!-- 参考信息 -->