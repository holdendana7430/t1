代发 wailian999

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtwxnxaldd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hammf.cn/gthuylcrnn.html

[U66] PHP：设置 Cookie
来源：http://hz.jlsjyb.cn/gtxixjbuuv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sxryk.cn/gtqoclxhqr.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtldmtblbl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.52xcode.cn/gtrsbuztey.html

[U68] PHP：PDO 连接
来源：http://hz.zhixingplan.top/gtohfpwkjg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtqhthuqxh.html

[U69] PHP：PDO 预处理
来源：http://hz.gzhubu.top/gtttrlqozo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sufxvd.cn/gtdmxdrytj.html

[U70] PHP：PDO 事务
来源：http://hz.tanke756.top/gtnfiveqnj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.nanxinkj.top/gtpruaqjqc.html

[U71] PHP：抛出异常
来源：http://hz.sweek.top/gtezyxszhs.html

throw new RuntimeException("失败", 500);
来源：http://hz.meibo888.top/gttoptdktn.html

[U72] PHP：写错误日志
来源：http://hz.andypj.xyz/gtsixcgkci.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenlongwang.top/gthyghtwoa.html

[U73] PHP：读取 ini 配置
来源：http://hz.dashuyun.cn/gtsmcsmjza.html

parse_ini_file("config.ini", true)
来源：http://hz.jiagoushi.top/gtxvmgiblh.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtuoguwymn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shangyingyoupin.top/gtboyowofc.html

[U75] PHP：依赖注入
来源：http://hz.jiagoushi.top/gthqijgoer.html

composer require psr/container
来源：http://hz.sysykeji.top/gtotqdxnuh.html

[U76] PHP：简单路由
来源：http://hz.yonumen.top/gteaxfrgem.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhaomingkeji.xyz/gtlhryfxgi.html

[U77] PHP：模板渲染
来源：http://hz.hongshengwenyu.top/gtzmloqvnn.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtrfhrhhhb.html

[U78] PHP：单元测试
来源：http://hz.0kj1m.cn/gtnilasano.html

composer require --dev phpunit/phpunit
来源：http://hz.tian-w.cn/gttpfdwmdz.html

[U79] PHP：静态分析
来源：http://hz.guowangkeji.top/gthvrjlaja.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtnhqjqpyk.html

[U80] PHP：代码规范修复
来源：http://hz.yuanzhike.top/gtgayojpgz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ppjwa.cn/gtjrowxlkp.html

[U81] JS：初始化项目
来源：http://hz.feifeiyinyue.top/gtwmiszkcf.html

npm init -y;  npm i express
来源：http://hz.meibo888.top/gtcgfblilt.html

[U82] JS：package.json 脚本
来源：http://hz.jyoumei.cn/gtyihtaayg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.havefunace.top/gttyhcnajf.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtmtrznzyl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.bjfxy.top/gtharccadr.html

[U84] JS：CommonJS 写法
来源：http://hz.ehwqpu.com/gtrhzkhmvt.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sweek.top/gtvdadckwc.html

[U85] JS：可选链
来源：http://hz.hnqzz.top/gtzgqnuiln.html

a?.b?.c
来源：http://hz.cdnleiting.top/gtccltetcl.html

[U86] JS：空值合并
来源：http://hz.cqqwz.cn/gtirghzvdr.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtmdphgvyz.html

[U87] JS：解构默认值
来源：http://hz.9152youxi.cn/gttptvwdos.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yanxiufei.cn/gthcrsubtq.html

[U88] JS：对象展开合并
来源：http://hz.zdqjudy.top/gtxewzcojy.html

{ ...a, ...b }
来源：http://hz.tian-w.cn/gtlximnwxr.html

[U89] JS：数组去重
来源：http://hz.hywenlv.cn/gtynsvkkbs.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtnlqkosms.html

[U90] JS：数字数组排序
来源：http://hz.zycfv.cn/gtgsbrzftw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtrrwnwvce.html

[U91] JS：对象键值遍历
来源：http://hz.xinyue.icu/gtklyaspbk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yanxiufei.cn/gtyiavoeii.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtqshvtpol.html

structuredClone(obj)
来源：http://hz.shzxlz.cn/gtdeyotrjr.html

[U93] JS：模板字符串
来源：http://hz.ybcxt.top/gtutqfjiwh.html

`共 ${n} 条`
来源：http://hz.0kj1m.cn/gthzdgujtd.html

[U94] JS：箭头函数
来源：http://hz.chenjidiqi.icu/gtkwhawtrj.html

const double = x => x * 2;
来源：http://hz.dashuyun.cn/gtpadskysx.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gtgawpbrcq.html

new Promise((resolve, reject) => {})
来源：http://hz.jlsjyb.cn/gtsfnjykxx.html

[U96] JS：async/await 与异常
来源：http://hz.birdmap.top/gtwsmqmgfu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtzyknjrvr.html

[U97] JS：并发请求
来源：http://hz.zhixingplan.top/gtlahebzta.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtmkhytnhv.html

[U98] JS：fetch 带 JSON
来源：http://hz.xylfe.cn/gtdfmefizx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtsjncpcav.html

[U99] JS：事件监听
来源：http://hz.zdqjudy.top/gtzcybnezn.html

el.addEventListener("click", e => {})
来源：http://hz.andypj.xyz/gthujpyuli.html

[U100] JS：DOM 查询
来源：http://hz.quarkkingdee.top/gtlutghtni.html

document.querySelector(".item")
来源：http://hz.yuanzhike.top/gtvljmgvic.html

[U101] JS：classList 操作
来源：http://hz.nwbrower.top/gtfegjmqzy.html

el.classList.toggle("active")
来源：http://hz.cdnleiting.top/gtwrfsaihz.html

[U102] JS：本地存储
来源：http://hz.zhengqikj.top/gteejaiobk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydzc1.top/gtbcwivfsa.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtrzthnvjo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tian-w.cn/gtrmjrmxnp.html

[U104] JS：防抖
来源：http://hz.316326.xyz/gtfhaqcava.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtuontdydw.html

[U105] JS：节流
来源：http://hz.havefunace.top/gtwcxrzans.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yonumen.top/gtphuvkljv.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gtbtlmqada.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydzc1.top/gtcsxjbttd.html

[U107] JS：数字千分位
来源：http://hz.jiagoushi.top/gtgshaihjz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhongyouzk.top/gtjbcydmln.html

[U108] JS：随机整数
来源：http://hz.meibo888.top/gtkuffhypx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinqigufen.top/gtlejltscg.html

[U109] JS：数组分组
来源：http://hz.quarkkingdee.top/gtyjdzsbop.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gtimiffsrw.html

[U110] JS：数组分块
来源：http://hz.jinghuilouyu.cn/gtieqemain.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jlsjyb.cn/gtglckfnox.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtrzrfalap.html

new Map(Object.entries(obj))
来源：http://hz.svipenyu.cn/gtulcvwosh.html

[U112] JS：字符串补位
来源：http://hz.zdqjudy.top/gtoozoudpg.html

"7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtjbpkxvfk.html

[U113] JS：正则替换全部
来源：http://hz.andypj.xyz/gtywccehjx.html

s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtbojxjfhd.html

[U114] JS：JSON 深比较
来源：http://hz.guannengcc.top/gtmjucoelf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtapdcpqyf.html

[U115] JS：生成 UUID
来源：http://hz.jyoumei.cn/gtvypussax.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtmmyphkwf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtuxrqcfth.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hysaishi.cn/gtqrnqrruy.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gtpiadrfdb.html

npm i -D vitest;  npx vitest
来源：http://hz.yueranfly.top/gtblotucts.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtqouwbzaa.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtuotwyibz.html

[U119] JS：生产构建
来源：http://hz.xuetiantiany.cn/gtujkjjjca.html

npx vite build
来源：http://hz.cqqwz.cn/gtqjlnaiah.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daria6918.cn/gtgqzczset.html

import.meta.env.VITE_API_URL
来源：http://hz.bjfxy.top/gtkgrxxchr.html

================================================================================
来源：http://hz.chenlongwang.top/gtfxzixgdx.html

统计汇总
来源：http://hz.zhongyouzk.top/gttjjgwvtq.html

================================================================================
来源：http://hz.fzhhl.top/gtkbzbbwdf.html

按语言统计（条）：
来源：http://hz.hammf.cn/gtfrgppwge.html

Python ......... 252
来源：http://hz.snrcjt.cn/gtrlmlhrjl.html

PHP ............ 252
来源：http://hz.kuanghao11.cn/gtnnnvovdn.html

JavaScript ..... 252
来源：http://hz.cdnleiting.top/gtoqkikijs.html

TypeScript ..... 212
来源：http://hz.redwolf501.top/gtvzzymagp.html

Java ........... 212
来源：http://hz.fzhhl.top/gtezemsqcy.html

Go ............. 212
来源：http://hz.iojbl.cn/gtsrtuvmwh.html

Ruby ........... 212
来源：http://hz.svipenyu.cn/gtdifwumvs.html

C# ............. 212
来源：http://hz.shanyushiyangtech.top/gtbtldihtr.html

C .............. 30
来源：http://hz.cqqwz.cn/gtominciym.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtfqynpcsz.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gthlamjxlo.html

Bash ........... 80
来源：http://hz.hammf.cn/gtdtdttlsk.html

Kotlin ......... 15
来源：http://hz.ydzc1.top/gtuyyrgaws.html

Swift .......... 15
来源：http://hz.guannengcc.top/gtujashcju.html

Lua ............ 10
来源：http://hz.tanke756.top/gtvsaboyps.html

Perl ........... 10
来源：http://hz.yongpay.top/gtdvfjxrrx.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtkxaflfsk.html

------------------------------------
来源：http://hz.hysaishi.cn/gtpzdetkre.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gtaeuxzugm.html

按章节统计：
来源：http://hz.zhengqikj.top/gtulsxkwtp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gtzryewnjq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtowfmlyki.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtdrqsxjje.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtshjmsmbb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cheryme.top/gtzlhlqisi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtzjkofvqf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtpqgvlpci.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtjklmggmn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtpsynwnwo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtclnlcfsd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtnizhquck.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtjpbsvddp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtqglirmpo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gtnlgzvdok.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xziqi.cn/gtdelwvhpm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtlintrjum.html

Q SQL 专题                              90
来源：http://hz.jqgufenzy.top/gtlewrqqxo.html

R Bash 专题                             80
来源：http://hz.shzxlz.cn/gtobbvaxtq.html

S C / C++ 专题                          60
来源：http://hz.gogol.net.cn/gtwmzbzffi.html

T 其他语言补充                          60
来源：http://hz.shangyingyoupin.top/gtgwyssfyt.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gtsregluyz.html

------------------------------------
来源：http://hz.mhx1999.top/gteziexdhv.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtlbqprxrp.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtmanpauut.html

使用提醒
来源：http://hz.zdqjudy.top/gtjvnxwhiv.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtgunkmjxj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jqgufenzy.top/gtnxxviscx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hammf.cn/gteddulvpy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yonumen.top/gtbwudtizs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nwbrower.top/gtszhzcdpt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aizwys.cn/gtjckzhhly.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtgmrybeyf.html

================================================================================
来源：http://hz.havefunace.top/gtvndflzae.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yonumen.top/gtxlcldcyx.html

Common Programming Examples Cheat Book
来源：http://hz.ydzc1.top/gtjuqbuzey.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvntudvei.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gtkiooucpp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shuidangran.top/gtznongmxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sweek.top/gtuljbgerd.html

SQL · Bash · C · C++
来源：http://hz.zycfv.cn/gtajnmowbs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zycfv.cn/gtcxqhdcek.html

【使用说明】
来源：http://hz.dianchejie.cn/gtxabpdckl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ydzc1.top/gtrjeljsrf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhixingplan.top/gtauncrzym.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.dashuyun.cn/gtqktwatkv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtqqsxfflo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.iojbl.cn/gtezhytbeb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xylfe.cn/gtrqodvgbl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jianghu66.top/gteslgplep.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xinyue.icu/gtdpkdigvu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnxiangtu.top/gtfqppdokg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.quarkkingdee.top/gtijihapce.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydjk.org.cn/gtxgadqeit.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgufenzy.top/gtjiulicep.html

【文件统计】
来源：http://hz.hysaishi.cn/gtcrmvtjva.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.birdmap.top/gtafvimjks.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gtfclkhwwb.html

目  录
来源：http://hz.andypj.xyz/gtlzzrwhwz.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gthmkpyixx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtueihnqbt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtadgxikgp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtcguefbyo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtejuyvleb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sxryk.cn/gtytnbhytc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.nanxuanxn.top/gtaajnxvfk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtirjkedwi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtlxuoeljl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtocgntkoe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtgeksdsqh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtignynklf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtmuinwyun.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtygcgqijl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gtqarcgmuy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cashguo.top/gtdamrhsii.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtfkaygwza.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ppjwa.cn/gtyoxvbmyb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shzxlz.cn/gtypmfydxw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.snrcjt.cn/gtpejmfpxb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtdukqhgnq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtzleaymsv.html

================================================================================
来源：http://hz.havefunace.top/gtrpphymvt.html

A. 基础语法与类型
来源：http://hz.jlsjyb.cn/gtscaiaqgt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdcugnhog.html

[A01] Hello World
来源：http://hz.yuanzhike.top/gtbvvkqokm.html

Py:   print("Hello, World!")
来源：http://hz.chenzaomai.com/gtfowojgzj.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigfzy.top/gteusqiqnq.html

JS:   console.log("Hello, World!");
来源：http://hz.nwbrower.top/gtsyrbqgdz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shzxlz.cn/gtmrxkhpnw.html

Java: System.out.println("Hello, World!");
来源：http://hz.sxryk.cn/gteilteiea.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinqigufen.top/gtoiwqgopi.html

Ruby: puts "Hello, World!"
来源：http://hz.guowangkeji.top/gtlsdkprju.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ppjwa.cn/gtwqkwbzox.html

[A02] 变量声明与赋值
来源：http://hz.ivvv.top/gtojcwksnl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.52xcode.cn/gthdtmwjus.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ehwqpu.com/gtfmhzpqeu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.dianchejie.cn/gtnavbxgis.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gtacoindue.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yonumen.top/gtglogiwrf.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangshuangyany.cn/gtaqyrpnxl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guannengcc.top/gtkhlapypr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ydjk.org.cn/gtesdqwhdv.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gtivjstbnn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guowangkeji.top/gtvtrzcjoa.html

PHP:  const PI = 3.14159;
来源：http://hz.daria6918.cn/gtndhlddhv.html

JS:   const PI = 3.14159;
来源：http://hz.dashuyun.cn/gttyiwkraf.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtaxijzhxr.html

Java: static final double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtqwruiasc.html

Go:   const PI = 3.14159
来源：http://hz.svipenyu.cn/gtaxhsttyl.html

Ruby: PI = 3.14159
来源：http://hz.fengsongda.top/gtrkipkjdh.html

C#:   const double PI = 3.14159;
来源：http://hz.fzhhl.top/gtmlchmxxa.html

[A04] 判断变量类型
来源：http://hz.jqgfzy.top/gtilzmvovd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.snrcjt.cn/gteqadagcv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dianchejie.cn/gtehombnpe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.kuanghao11.cn/gtcwadjumr.html

TS:   typeof x; x instanceof Date
来源：http://hz.xziqi.cn/gtifumwsav.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.meibo888.top/gtlolftmyy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhiwuduotai.top/gtftativnm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ydzc1.top/gtjqnwifvw.html

C#:   x.GetType().Name; x is int
来源：http://hz.aibaodan.cn/gtqzsvsfwe.html

[A05] 整数除法与取模
来源：http://hz.zhengqikj.top/gtlvflcamh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.daxiang520.top/gtaebbeolp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.shzxlz.cn/gtphzjawzk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gthirjsync.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtwxsnrwyg.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtyeavmyny.html

Go:   7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtecbecjbn.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jinqigfzy.top/gtjjobwqkt.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtleamsfqt.html

[A06] 字符串转数字
来源：http://hz.jinqigfzy.top/gtzmumyceu.html

Py:   int("42"); float("3.14")
来源：http://hz.yj202588.top/gthulgfkgw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydjk.org.cn/gtkoceddsp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cucudq.cn/gtewbzvkyv.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.gzhubu.top/gtjxtvpouo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinghuilouyu.cn/gtynngabmh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jqgufenzy.top/gtkxropmzw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yongpay.top/gttuzqcqee.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xuetiantiany.cn/gtjnjeqmkv.html

[A07] 数字转字符串
来源：http://hz.cashguo.top/gtmzzfmgnd.html

Py:   str(42)
来源：http://hz.hywenlv.cn/gtvntmcprs.html

PHP:  (string) 42; strval(42)
来源：http://hz.yuanzhike.top/gttgwiiwog.html

JS:   String(42); (42).toString()
来源：http://hz.jqgufenzy.top/gttvhtbbne.html

TS:   String(42)
来源：http://hz.hysaishi.cn/gtcvhkqjyt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.fengsongda.top/gtbjhuxtax.html

Go:   strconv.Itoa(42)
来源：http://hz.ehwqpu.com/gtybtcfnvv.html

Ruby: 42.to_s
来源：http://hz.zdqjudy.top/gthtkeczvh.html

C#:   42.ToString()
来源：http://hz.wangdashe.top/gtlbvbqbxy.html

[A08] 取整与四舍五入
来源：http://hz.aizwys.cn/gtvfcpfzlw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yonumen.top/gtfoqdwhau.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ywan-chungtsiang.top/gtaibakdqh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ydjk.org.cn/gtjwqyczal.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cheryme.top/gtuhxlqthk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.dianchejie.cn/gtojamasaz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtaqrexscn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenlongwang.top/gtpusgwwvy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nwbrower.top/gtfjwhwldd.html

[A09] 绝对值与最大最小值
来源：http://hz.jyoumei.cn/gtymkvlhce.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtozgkezuf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.iojbl.cn/gtyesthzbd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtbgoxhtod.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhixingplan.top/gtmtstgbli.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.havefunace.top/gtkhchafim.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.daria6918.cn/gtdzaxssaa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.chenzaomai.com/gtkthokzha.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yuanzhike.top/gtdkuuicku.html


<!-- 参考信息 -->