代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.jianghu66.top/gtomotwdin.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenzaomai.com/gthcndcxhm.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtysfsaugl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.iojbl.cn/gtntxcskbt.html

[U69] PHP：PDO 预处理
来源：http://hz.shzxlz.cn/gtgvlvtytc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.iojbl.cn/gtcredmmvv.html

[U70] PHP：PDO 事务
来源：http://hz.52xcode.cn/gtpsfjkgsf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guannengcc.top/gtjimjhssj.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtwaxjgrwg.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhengqikj.top/gtxgoegeql.html

[U72] PHP：写错误日志
来源：http://hz.svipenyu.cn/gtnjcbnkfo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gaohongyu789.top/gtflinzaxd.html

[U73] PHP：读取 ini 配置
来源：http://hz.yanxiufei.cn/gtsfwzjbzt.html

parse_ini_file("config.ini", true)
来源：http://hz.zhengqikj.top/gtgqvnxnpi.html

[U74] PHP：读取环境变量
来源：http://hz.jqgfzy.top/gtthgmqktp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yuanzhike.top/gthlaigorp.html

[U75] PHP：依赖注入
来源：http://hz.dianchejie.cn/gtsujwtgwi.html

composer require psr/container
来源：http://hz.jinqigfzy.top/gtsztlevtf.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtqcafwvco.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtjkvksxrj.html

[U77] PHP：模板渲染
来源：http://hz.daxiang520.top/gtlrqeajlc.html

composer require twig/twig
来源：http://hz.hnxiangtu.top/gtfiiblcms.html

[U78] PHP：单元测试
来源：http://hz.kuanghao11.cn/gtorppcosy.html

composer require --dev phpunit/phpunit
来源：http://hz.shzxlz.cn/gtobdyhbnu.html

[U79] PHP：静态分析
来源：http://hz.haohaochexian.top/gtiirsxukp.html

composer require --dev phpstan/phpstan
来源：http://hz.svipenyu.cn/gtjdgxyfai.html

[U80] PHP：代码规范修复
来源：http://hz.c1oappe.top/gtmbgpobck.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.guannengcc.top/gtvuocsxro.html

[U81] JS：初始化项目
来源：http://hz.chenzaomai.com/gtswoyovkx.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gtaeclyqbh.html

[U82] JS：package.json 脚本
来源：http://hz.pengpengdd.cyou/gtbutpxplo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.bjfxy.top/gtkcxkbwvu.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhiwuduotai.top/gtecnixfuz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhiwuduotai.top/gthnwicxaa.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtwjuuahzb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gtafikhvgq.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gtmoknmfre.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtelufnogd.html

[U86] JS：空值合并
来源：http://hz.ehwqpu.com/gtxjyrhqfx.html

a ?? b
来源：http://hz.316326.xyz/gtpfnhluur.html

[U87] JS：解构默认值
来源：http://hz.feifeiyinyue.top/gtmiijipzc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fzhhl.top/gtxebeumfa.html

[U88] JS：对象展开合并
来源：http://hz.hysaishi.cn/gtkbgiotkf.html

{ ...a, ...b }
来源：http://hz.feifeiyinyue.top/gtubgoqeua.html

[U89] JS：数组去重
来源：http://hz.ybcxt.top/gtunlxvmcr.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtvinxpumv.html

[U90] JS：数字数组排序
来源：http://hz.tian-w.cn/gtdfowgjmg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtcsrbsdhi.html

[U91] JS：对象键值遍历
来源：http://hz.0kj1m.cn/gtsbjpftyh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtyiyxkedm.html

[U92] JS：深拷贝
来源：http://hz.sxryk.cn/gtugqyzotb.html

structuredClone(obj)
来源：http://hz.svipenyu.cn/gtvfvcqhpi.html

[U93] JS：模板字符串
来源：http://hz.52xcode.cn/gtcwhynvwj.html

`共 ${n} 条`
来源：http://hz.yangfankeji.com/gtfhjlhsqn.html

[U94] JS：箭头函数
来源：http://hz.zycfv.cn/gtnbwkkxhz.html

const double = x => x * 2;
来源：http://hz.zhijiandao.cn/gtiagejsad.html

[U95] JS：Promise 包装
来源：http://hz.andypj.xyz/gteuejelle.html

new Promise((resolve, reject) => {})
来源：http://hz.aizwys.cn/gtvbwldhwv.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gtasbifkip.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtlsmuajgo.html

[U97] JS：并发请求
来源：http://hz.yvedp.cn/gtvptkrfxr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtdlgwklpg.html

[U98] JS：fetch 带 JSON
来源：http://hz.hongshengwenyu.top/gtvmtskvpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhijiandao.cn/gtjwfuairm.html

[U99] JS：事件监听
来源：http://hz.ppjwa.cn/gtfvnwgjdb.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtswknekix.html

[U100] JS：DOM 查询
来源：http://hz.pycfn.com/gtoacxoamj.html

document.querySelector(".item")
来源：http://hz.yonumen.top/gtxmunjdpp.html

[U101] JS：classList 操作
来源：http://hz.jinqigfzy.top/gtvpiqwcmf.html

el.classList.toggle("active")
来源：http://hz.smart0.xyz/gtboddymnm.html

[U102] JS：本地存储
来源：http://hz.snrcjt.cn/gthejaxfcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.feifeiyinyue.top/gtfnmtvdmw.html

[U103] JS：定时器
来源：http://hz.andypj.xyz/gtvltixpth.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dianchejie.cn/gtoeokanyw.html

[U104] JS：防抖
来源：http://hz.fengsongda.top/gtdyymwbnt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtmyrenelq.html

[U105] JS：节流
来源：http://hz.jinqigufen.top/gtdzulthdf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258.top/gtzbiekxna.html

[U106] JS：日期格式化
来源：http://hz.zhaomingkeji.xyz/gtgbshixdt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtkqekuakj.html

[U107] JS：数字千分位
来源：http://hz.daxiang520.top/gtarcwpnxe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtbebzwied.html

[U108] JS：随机整数
来源：http://hz.kuanghao11.cn/gtmbddaavv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtteovefbg.html

[U109] JS：数组分组
来源：http://hz.0kj1m.cn/gtotnthsvt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtuhfpdxsk.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtuiqshktz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.vqdsnc.cn/gtyzzkoyth.html

[U111] JS：对象转 Map
来源：http://hz.yvedp.cn/gtroxqyskq.html

new Map(Object.entries(obj))
来源：http://hz.tian-w.cn/gtkollbjus.html

[U112] JS：字符串补位
来源：http://hz.316326.xyz/gttdeinpuy.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtgxsyzybr.html

[U113] JS：正则替换全部
来源：http://hz.ydzc1.top/gtaumzfxal.html

s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtlgupxoip.html

[U114] JS：JSON 深比较
来源：http://hz.hongshengwenyu.top/gtqttfnkvf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtktdyuahj.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtstxodzoh.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gtewwpxsgk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guannengcc.top/gtthmagvgz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yonumen.top/gthzrcksbw.html

[U117] JS：单元测试
来源：http://hz.dianchejie.cn/gtiggxokri.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgfzy.top/gtlcbffucv.html

[U118] JS：开发服务器
来源：http://hz.cqqwz.cn/gtradfxtrr.html

npm i -D vite;  npx vite
来源：http://hz.sysykeji.top/gtdsdjydrg.html

[U119] JS：生产构建
来源：http://hz.9152youxi.cn/gtygggvgpz.html

npx vite build
来源：http://hz.nanxinkj.top/gtmcxrpimg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhoulong.xyz/gtbqbbynzs.html

import.meta.env.VITE_API_URL
来源：http://hz.hysaishi.cn/gtzyypwame.html

================================================================================
来源：http://hz.yuxming.cn/gtrwepfywy.html

统计汇总
来源：http://hz.kuanghao11.cn/gtlrusgefz.html

================================================================================
来源：http://hz.haohaochexian.top/gtihhcinjc.html

按语言统计（条）：
来源：http://hz.chenjidiqi.icu/gtiytobxdk.html

Python ......... 252
来源：http://hz.gaohongyu789.top/gtguzcnmjt.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtuyixigfh.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gtivwxgtux.html

TypeScript ..... 212
来源：http://hz.zhaomingkeji.xyz/gtyafjxzoq.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtroqnrfrp.html

Go ............. 212
来源：http://hz.yvedp.cn/gtrvvjpnik.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtxucpusie.html

C# ............. 212
来源：http://hz.zhiwuduotai.top/gtoltuzgud.html

C .............. 30
来源：http://hz.yj20258888.top/gtedxobhjj.html

C++ ............ 30
来源：http://hz.cdnleiting.top/gtjnnespja.html

SQL ............ 90
来源：http://hz.ydzc1.top/gtbvrdllzi.html

Bash ........... 80
来源：http://hz.sufxvd.cn/gtfgtoteuj.html

Kotlin ......... 15
来源：http://hz.sxryk.cn/gtgclavjev.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gtbdqvsjvv.html

Lua ............ 10
来源：http://hz.gzhubu.top/gtniwcgcww.html

Perl ........... 10
来源：http://hz.jinyuanbaomall.cn/gtpgvrtfvk.html

Scala .......... 10
来源：http://hz.cheryme.top/gtkrzffwym.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtghsppinm.html

合计 ........... 2106 条
来源：http://hz.jyoumei.cn/gtrmcipvmb.html

按章节统计：
来源：http://hz.sysykeji.top/gtxvqrrhzh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yanxiufei.cn/gtmpxmaias.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gthsivkjbx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtlnnrtzxx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.birdmap.top/gtxtzducvm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nwbrower.top/gtfavbnohe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtmqjuaeco.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtpwegdxge.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangkeji.top/gttikmjkrw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtyylnsmua.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.sweek.top/gtjwotkshj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtvqyqwjve.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtkvshsklu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtmuemjxij.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtffropwit.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxinkj.top/gtmyvecinc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtumxkryxv.html

Q SQL 专题                              90
来源：http://hz.ydzc1.top/gtuxdgqvfq.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtnmewfsir.html

S C / C++ 专题                          60
来源：http://hz.ywan-chungtsiang.top/gtumvpnqce.html

T 其他语言补充                          60
来源：http://hz.tanke756.top/gtfjvchrba.html

U 高频实用片段                         120
来源：http://hz.vqdsnc.cn/gtkphhkeap.html

------------------------------------
来源：http://hz.chenlongwang.top/gtazxtxlav.html

合计                                  2106 条
来源：http://hz.zhixingplan.top/gtyoigleht.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtmkciylqr.html

使用提醒
来源：http://hz.zhengqikj.top/gtdanctcbs.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtqcykzwja.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ywan-chungtsiang.top/gtyangwlsz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.meibo888.top/gtrpzyutop.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yonumen.top/gtqodyxubw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtlintekzt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtnxkmaixg.html

—— 文件结束 ——
来源：http://hz.yj20258888.top/gtqhfmbmut.html

================================================================================
来源：http://hz.yanxiufei.cn/gtisqkhvaz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gogol.net.cn/gtavlqnmgv.html

Common Programming Examples Cheat Book
来源：http://hz.jinyuanbaomall.cn/gtxmimajvg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpvjtovfj.html

【收录内容】
来源：http://hz.dianchejie.cn/gtpkedbbhs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.9152youxi.cn/gtitvvbyjp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gthdnvxjdp.html

SQL · Bash · C · C++
来源：http://hz.yangfankeji.com/gtmhjxdcvz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xinyue.icu/gtxwbdnypv.html

【使用说明】
来源：http://hz.jinqigufen.top/gtfinxbhii.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hywenlv.cn/gtanwqisdw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.snrcjt.cn/gthjlmammb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jiagoushi.top/gtgygpilka.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xuetiantiany.cn/gtekhxmsic.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtdkfryiml.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cqqwz.cn/gtotunqdgf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pengpengdd.cyou/gtfymvydwh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.meibo888.top/gtvajyxjhw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigufen.top/gtdgamkurd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nanxuanxn.top/gtnoxohcuf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.c1oappe.top/gtnsxzbzgc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yueranfly.top/gtydzbfjbh.html

【文件统计】
来源：http://hz.havefunace.top/gtbymaqkci.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yangfankeji.com/gtvxqobxkd.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtbyfbnfkf.html

目  录
来源：http://hz.wangshuangyany.cn/gtjuivwmtd.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtbnsbqgix.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dashuyun.cn/gtjjbmuuyf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gteuoxfnki.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtrkdllsty.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yangfankeji.com/gtkcypdivh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.birdmap.top/gtrotshtlj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.nanxinkj.top/gthjxlfwbw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtdshzoizz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yanxiufei.cn/gtctyscbxp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtsquqeuxk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtecebxspw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtiladfsyv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtcfhznxpw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtoudkvxrs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtzrvistev.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuanzhike.top/gtujrkfnwg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtvtnsnbvs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangshuangyany.cn/gtiswdeqbx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ppjwa.cn/gtiwmqdiks.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tianlin.xyz/gtoronvpon.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtuhicygxq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtvxlpkusm.html

================================================================================
来源：http://hz.fengsongda.top/gtrjkfknsi.html

A. 基础语法与类型
来源：http://hz.xziqi.cn/gtonrjobpa.html

================================================================================
来源：http://hz.316326.xyz/gtqnlnwqlk.html

[A01] Hello World
来源：http://hz.ybcxt.top/gtglpzqafz.html

Py:   print("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtbwnizcla.html

PHP:  echo "Hello, World!";
来源：http://hz.zycfv.cn/gtwcvsufoi.html

JS:   console.log("Hello, World!");
来源：http://hz.0kj1m.cn/gtnxogkdqm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guannengcc.top/gtmdyyuvmy.html

Java: System.out.println("Hello, World!");
来源：http://hz.cashguo.top/gtznrwgxsk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gtcccpkclu.html

Ruby: puts "Hello, World!"
来源：http://hz.9152youxi.cn/gtupnrerrx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258.top/gtctojqrbi.html

[A02] 变量声明与赋值
来源：http://hz.yonumen.top/gtwyqtuihw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangtech.top/gtvjpwuifl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.kuanghao11.cn/gtalrehtcn.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtznqdqqgt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hywenlv.cn/gtmwagqljz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.kuanghao11.cn/gtflkryfcl.html

Go:   name := "Alex"; age := 20
来源：http://hz.xziqi.cn/gtumygapzv.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenjidiqi.icu/gthuqcbzhg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtgcckhdqz.html

[A03] 常量定义
来源：http://hz.ppjwa.cn/gtlthgtvun.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hammf.cn/gtlvbmjtlv.html

PHP:  const PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtwlznguws.html

JS:   const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtoeksbqbp.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gteqfvpkgo.html

Java: static final double PI = 3.14159;
来源：http://hz.guannengcc.top/gtdyhqcxon.html

Go:   const PI = 3.14159
来源：http://hz.yj20258.top/gtjozixhkw.html

Ruby: PI = 3.14159
来源：http://hz.ydzc1.top/gtcrtigspk.html

C#:   const double PI = 3.14159;
来源：http://hz.xuanzx.com/gthxkuajic.html

[A04] 判断变量类型
来源：http://hz.cdnleiting.top/gtwgeangkn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gaohongyu789.top/gtzkjpmqkw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhongyouzk.top/gtladptgzt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tianlin.xyz/gtwizdkykb.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtqcvykkue.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xylfe.cn/gtkcmgvwyj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hammf.cn/gtqtlkynmx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cheryme.top/gturstxudt.html

C#:   x.GetType().Name; x is int
来源：http://hz.gotoacloud.top/gtwkwkespd.html

[A05] 整数除法与取模
来源：http://hz.gogol.net.cn/gtrtjobedo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xinyue.icu/gtwndqvjan.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sxryk.cn/gtaaplunxy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cashguo.top/gthfkmnmve.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sysykeji.top/gtxuifdbhg.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtfhigpyyv.html

Go:   7 / 2; 7 % 2
来源：http://hz.hfpthk.cn/gtyrefglrm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtfxapxhaa.html

C#:   7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtarhrwbsb.html

[A06] 字符串转数字
来源：http://hz.pycfn.com/gtpcmwqtii.html

Py:   int("42"); float("3.14")
来源：http://hz.pengpengdd.cyou/gtiomqcggl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xziqi.cn/gtvvzvifvp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yuanzhike.top/gteosubfqi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.aizwys.cn/gtobugtqws.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.316326.xyz/gtcdykhvph.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xuetiantiany.cn/gtvxueqmec.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gaohongyu789.top/gtcomxbixs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hammf.cn/gtmvflqihx.html

[A07] 数字转字符串
来源：http://hz.quarkkingdee.top/gtvhzlbrfx.html

Py:   str(42)
来源：http://hz.meibo888.top/gtqkohmwwy.html

PHP:  (string) 42; strval(42)
来源：http://hz.snrcjt.cn/gtmugbdkrw.html

JS:   String(42); (42).toString()
来源：http://hz.ivvv.top/gtfpknkzty.html

TS:   String(42)
来源：http://hz.zhixingplan.top/gtimzlsssb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ivvv.top/gtixpaairt.html

Go:   strconv.Itoa(42)
来源：http://hz.cqqwz.cn/gtufzxfvej.html

Ruby: 42.to_s
来源：http://hz.zhaomingkeji.xyz/gtaulwtlvy.html

C#:   42.ToString()
来源：http://hz.9152youxi.cn/gtjwirqrqv.html

[A08] 取整与四舍五入
来源：http://hz.iojbl.cn/gtywcdtljv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.smart0.xyz/gtqqwwjkqj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yangfankeji.com/gtltuqnsdy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jiagoushi.top/gtdnlsoodx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.bjfxy.top/gtnydbnkkb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.sweek.top/gtfeqredzs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xuetiantiany.cn/gttfrsgcuy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.gaohongyu789.top/gtredvwqwo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gzhubu.top/gtelswaqsw.html

[A09] 绝对值与最大最小值
来源：http://hz.xziqi.cn/gtkyymnmqp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xylfe.cn/gtkdsqrvyf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.havefunace.top/gtinjijfnr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zdqjudy.top/gtltspfaxp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jianghu66.top/gtcagflite.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yonumen.top/gtraqxqwgw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj202588.top/gteegohjnd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xinyue.icu/gtnjziwdfn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtaoxyboit.html

[A10] 生成随机数
来源：http://hz.ybcxt.top/gtilzcmekl.html

Py:   import random; random.randint(1, 100)
来源：http://hz.guowangkeji.top/gtxpzqdxdk.html

PHP:  random_int(1, 100);
来源：http://hz.yvedp.cn/gtzqekzmzh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nanxinkj.top/gtzjvmmplg.html


<!-- 参考信息 -->