代发 wailian999

[U63] PHP：文件读写
来源：http://hz.jinqigfzy.top/gtcyoesdhm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258.top/gtokodampp.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gtwsnnenkr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jyoumei.cn/gtetaegkkb.html

[U65] PHP：会话
来源：http://hz.smart0.xyz/gtvlssdrcc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtpzsqezfh.html

[U66] PHP：设置 Cookie
来源：http://hz.shangyingyoupin.top/gtqpxdznlt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258888.top/gtlowbbzne.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtcnqyceag.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.smart0.xyz/gtybtyeiks.html

[U68] PHP：PDO 连接
来源：http://hz.yongpay.top/gttqydqczq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtecfiyfed.html

[U69] PHP：PDO 预处理
来源：http://hz.dashuyun.cn/gtsxqnjgvx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.iojbl.cn/gtjmxbnmjz.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtmlfzpafq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.andypj.xyz/gtgsczpjhk.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangtech.top/gtdxwjknld.html

throw new RuntimeException("失败", 500);
来源：http://hz.sysykeji.top/gtuquznnyk.html

[U72] PHP：写错误日志
来源：http://hz.9152youxi.cn/gtsrzlvezw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinqigfzy.top/gtmohoiwkh.html

[U73] PHP：读取 ini 配置
来源：http://hz.aibaodan.cn/gtlimhfzsk.html

parse_ini_file("config.ini", true)
来源：http://hz.guannengcc.top/gtvtdrgmrd.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtyayvjpjy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daxiang520.top/gtmyedsufl.html

[U75] PHP：依赖注入
来源：http://hz.havefunace.top/gtsbcereem.html

composer require psr/container
来源：http://hz.zdqjudy.top/gtmoxszjol.html

[U76] PHP：简单路由
来源：http://hz.guannengcc.top/gthwaropuh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sxryk.cn/gtuyeejeal.html

[U77] PHP：模板渲染
来源：http://hz.zhaomingkeji.xyz/gtltwolxxm.html

composer require twig/twig
来源：http://hz.zhiwuduotai.top/gtqpmewath.html

[U78] PHP：单元测试
来源：http://hz.jqgufenzy.top/gtlgzhqzqq.html

composer require --dev phpunit/phpunit
来源：http://hz.guowangkeji.top/gtrlsexyoy.html

[U79] PHP：静态分析
来源：http://hz.jinqigufen.top/gthdnpcbhc.html

composer require --dev phpstan/phpstan
来源：http://hz.zdqjudy.top/gtcdtvwysl.html

[U80] PHP：代码规范修复
来源：http://hz.shzxlz.cn/gtegjjwrze.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.vqdsnc.cn/gtwaoufhqy.html

[U81] JS：初始化项目
来源：http://hz.yj20258888.top/gttgzjbvxu.html

npm init -y;  npm i express
来源：http://hz.pengpengdd.cyou/gtvzlzvjgi.html

[U82] JS：package.json 脚本
来源：http://hz.yuxming.cn/gtzmiwchqt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.quarkkingdee.top/gttpcbeekt.html

[U83] JS：ES Module 导入导出
来源：http://hz.tian-w.cn/gtizuyyttp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gogol.net.cn/gthkhxvffz.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtfozdhhav.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinghuilouyu.cn/gtqtppllxn.html

[U85] JS：可选链
来源：http://hz.hongshengwenyu.top/gtayhtggwi.html

a?.b?.c
来源：http://hz.shangyingyoupin.top/gtyvdzltua.html

[U86] JS：空值合并
来源：http://hz.chenzaomai.com/gteuodbcuv.html

a ?? b
来源：http://hz.dianchejie.cn/gtpehedxxt.html

[U87] JS：解构默认值
来源：http://hz.gaohongyu789.top/gtsftsqjud.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yvedp.cn/gtdanwrlwv.html

[U88] JS：对象展开合并
来源：http://hz.tanke756.top/gtbfoeblix.html

{ ...a, ...b }
来源：http://hz.chenjidiqi.icu/gtnodputbg.html

[U89] JS：数组去重
来源：http://hz.dianchejie.cn/gtzslyrbct.html

[...new Set(arr)]
来源：http://hz.andypj.xyz/gtgjpvhotw.html

[U90] JS：数字数组排序
来源：http://hz.jinghuilouyu.cn/gtfitnixbb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtggdtjbib.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258.top/gtzlnyhctt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gtwketvjuw.html

[U92] JS：深拷贝
来源：http://hz.gotoacloud.top/gtrjnfopzb.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtsiqijbmz.html

[U93] JS：模板字符串
来源：http://hz.jyoumei.cn/gtkqhdcyhf.html

`共 ${n} 条`
来源：http://hz.daxiang520.top/gtyyqwcryp.html

[U94] JS：箭头函数
来源：http://hz.yj202588.top/gtbbexbivt.html

const double = x => x * 2;
来源：http://hz.hfpthk.cn/gtukwywxxb.html

[U95] JS：Promise 包装
来源：http://hz.smart0.xyz/gtkikhzsla.html

new Promise((resolve, reject) => {})
来源：http://hz.xziqi.cn/gtwvtmmike.html

[U96] JS：async/await 与异常
来源：http://hz.aizwys.cn/gtidslolgi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtcwbtknrr.html

[U97] JS：并发请求
来源：http://hz.sysykeji.top/gtfdgodwjm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gttvybzekh.html

[U98] JS：fetch 带 JSON
来源：http://hz.yueranfly.top/gtxnitpdyt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gtpnhcased.html

[U99] JS：事件监听
来源：http://hz.xinyue.icu/gtpydngqdp.html

el.addEventListener("click", e => {})
来源：http://hz.quarkkingdee.top/gtmfusaucm.html

[U100] JS：DOM 查询
来源：http://hz.zhixingplan.top/gtxreewbtj.html

document.querySelector(".item")
来源：http://hz.yueranfly.top/gtouqvvgmo.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtyaapeeyh.html

el.classList.toggle("active")
来源：http://hz.yvedp.cn/gtrfwzbzuk.html

[U102] JS：本地存储
来源：http://hz.havefunace.top/gtbemyyfll.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xziqi.cn/gteaypuzsv.html

[U103] JS：定时器
来源：http://hz.zycfv.cn/gttfjmydqc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dashuyun.cn/gtymyhcqml.html

[U104] JS：防抖
来源：http://hz.dianchejie.cn/gtethnfclt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtzidssyma.html

[U105] JS：节流
来源：http://hz.daria6918.cn/gtmolrursa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.9152youxi.cn/gtsvilzyyg.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtxrqtlnnd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.0kj1m.cn/gtwrfmecks.html

[U107] JS：数字千分位
来源：http://hz.zhaomingkeji.xyz/gtobqkewpt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pycfn.com/gtpizkahag.html

[U108] JS：随机整数
来源：http://hz.jiagoushi.top/gtulctnbam.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cqqwz.cn/gtalfmgmji.html

[U109] JS：数组分组
来源：http://hz.tianlin.xyz/gthtsoysyd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtjjejskoy.html

[U110] JS：数组分块
来源：http://hz.havefunace.top/gtibljphpe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhijiandao.cn/gtdzriptqt.html

[U111] JS：对象转 Map
来源：http://hz.gzhubu.top/gtbdkwzshx.html

new Map(Object.entries(obj))
来源：http://hz.zycfv.cn/gtzcgoqdht.html

[U112] JS：字符串补位
来源：http://hz.yueranfly.top/gtdkwoduvt.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtcmlaxlrh.html

[U113] JS：正则替换全部
来源：http://hz.wangdashe.top/gtwhtnnxko.html

s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtvjqgjzhz.html

[U114] JS：JSON 深比较
来源：http://hz.pengpengdd.cyou/gtvsvcfgui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtdriuvhok.html

[U115] JS：生成 UUID
来源：http://hz.tian-w.cn/gtmdmaxmvd.html

crypto.randomUUID()
来源：http://hz.tanke756.top/gthitdwxiu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shzxlz.cn/gtzhqoxrtg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.feifeiyinyue.top/gthzgjetis.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtoovfkgrh.html

npm i -D vitest;  npx vitest
来源：http://hz.hfpthk.cn/gteukehwjm.html

[U118] JS：开发服务器
来源：http://hz.gogol.net.cn/gtoonvkary.html

npm i -D vite;  npx vite
来源：http://hz.xuanzx.com/gttyjpbnxa.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtruekgwgx.html

npx vite build
来源：http://hz.hfpthk.cn/gtqbcnfgsh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hysaishi.cn/gtoejvcgwz.html

import.meta.env.VITE_API_URL
来源：http://hz.iojbl.cn/gthruuswxm.html

================================================================================
来源：http://hz.jqgfzy.top/gtfojjywrc.html

统计汇总
来源：http://hz.wangdashe.top/gtaqdpjfii.html

================================================================================
来源：http://hz.9152youxi.cn/gtjqrgueva.html

按语言统计（条）：
来源：http://hz.sysykeji.top/gtwuhfjfcr.html

Python ......... 252
来源：http://hz.ydjk.org.cn/gtbkapymea.html

PHP ............ 252
来源：http://hz.tianlin.xyz/gtyeodqdan.html

JavaScript ..... 252
来源：http://hz.cdnleiting.top/gttpkqbetg.html

TypeScript ..... 212
来源：http://hz.quarkkingdee.top/gtejroyicb.html

Java ........... 212
来源：http://hz.52xcode.cn/gtmhadwbvo.html

Go ............. 212
来源：http://hz.xinyue.icu/gttltezudr.html

Ruby ........... 212
来源：http://hz.ydzc1.top/gtqbyqovqz.html

C# ............. 212
来源：http://hz.yongpay.top/gtsrecshkz.html

C .............. 30
来源：http://hz.nanxinkj.top/gtcxlhlotd.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtisxasmqz.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gtsbiyfwxd.html

Bash ........... 80
来源：http://hz.jinyuanbaomall.cn/gtsrgcdonr.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gtzramzifc.html

Swift .......... 15
来源：http://hz.daria6918.cn/gtoydtgiub.html

Lua ............ 10
来源：http://hz.pycfn.com/gtpxmjzula.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtzzyikhxo.html

Scala .......... 10
来源：http://hz.aizwys.cn/gtfqvhwiel.html

------------------------------------
来源：http://hz.yuxming.cn/gtaijyoebz.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gtgvvmibhf.html

按章节统计：
来源：http://hz.chenlongwang.top/gtmzcikhjk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtiittcsio.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gteiqablij.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtuudjnhud.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gthqwulbhq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.52xcode.cn/gtylymxadd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ydjk.org.cn/gtopwkowpw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtcxaatkor.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shzxlz.cn/gtzgekqeuh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtqkeixybc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtkzjffvrs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtrarcabar.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtqrsohrop.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtvrekhspp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gtdefsfpfz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.quarkkingdee.top/gtpccanoxv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtknkyifko.html

Q SQL 专题                              90
来源：http://hz.andypj.xyz/gtjkasfhkz.html

R Bash 专题                             80
来源：http://hz.ywan-chungtsiang.top/gtbkhkfppw.html

S C / C++ 专题                          60
来源：http://hz.9152youxi.cn/gtnygoukzb.html

T 其他语言补充                          60
来源：http://hz.sxryk.cn/gtzfbaokli.html

U 高频实用片段                         120
来源：http://hz.hnxiangtu.top/gtegbkxhlx.html

------------------------------------
来源：http://hz.shangyingyoupin.top/gtygtijxef.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtistbknsg.html

--------------------------------------------------------------------------------
来源：http://hz.xuetiantiany.cn/gtoocqdofd.html

使用提醒
来源：http://hz.xinyue.icu/gtdbcuxudr.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtpfbzgwmm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gtiulnizug.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhongyouzk.top/gtprhncser.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.daxiang520.top/gtyfaiuzmw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yanxiufei.cn/gtlaxebjqd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.feifeiyinyue.top/gtvvsdykiv.html

—— 文件结束 ——
来源：http://hz.52xcode.cn/gtbpeamnur.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdouvlrlq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hywenlv.cn/gtpanbnned.html

Common Programming Examples Cheat Book
来源：http://hz.meibo888.top/gttmqntqwo.html

================================================================================
来源：http://hz.jinqigufen.top/gtulvgwdcb.html

【收录内容】
来源：http://hz.sweek.top/gtgqnsrbcn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cqqwz.cn/gtkclflvga.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtkbzxegow.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtezvlmtba.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuetiantiany.cn/gtcucngfwi.html

【使用说明】
来源：http://hz.zycfv.cn/gtbraqyvfv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhoulong.xyz/gteozpbcsq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sysykeji.top/gtmezvzybr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yvedp.cn/gtccyromxz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yvedp.cn/gtrkzjxtgo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.andypj.xyz/gtdblwnmbf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shanyushiyangtech.top/gtjskbghsa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.snrcjt.cn/gtdwxsitls.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinyuanbaomall.cn/gtkhouaazp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxuanxn.top/gtdwzkjowl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tianlin.xyz/gtcmraopvd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nanxuanxn.top/gtrzcqguwr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuanzx.com/gtbxxgpkyu.html

【文件统计】
来源：http://hz.iojbl.cn/gtfflerdug.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yangfankeji.com/gtnmeiodyv.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtddkbuxij.html

目  录
来源：http://hz.tianlin.xyz/gttlcaludz.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtzyeknbqn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.mhx1999.top/gtngmfwsyo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtgnlaxexe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtgiwbjqml.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.redwolf501.top/gtndwvlylg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhongyouzk.top/gtqhbweuwf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.snrcjt.cn/gtxnrtqzfx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gttpznzsig.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cheryme.top/gtozfyjxmk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtkqqbepvr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.redwolf501.top/gtwsuzaqqt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtidfmsjkd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtokscejzn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtkgxadkew.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nanxinkj.top/gthwljajcr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daria6918.cn/gtqlybcaxq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtmblmawqi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtmqbfmjke.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.smart0.xyz/gttpwkosuq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhaomingkeji.xyz/gtwusbyceg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gthhciowqv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtgzelsncf.html

================================================================================
来源：http://hz.shzxlz.cn/gtsclmwlob.html

A. 基础语法与类型
来源：http://hz.shanyushiyangkeji.top/gtbabrwiye.html

================================================================================
来源：http://hz.jyoumei.cn/gtstnxfddb.html

[A01] Hello World
来源：http://hz.zycfv.cn/gtoescmklf.html

Py:   print("Hello, World!")
来源：http://hz.gogol.net.cn/gtrulqzgwm.html

PHP:  echo "Hello, World!";
来源：http://hz.xingfuxueyuan.xyz/gtlpquydon.html

JS:   console.log("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtfqajgwhl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258888.top/gtwmsviuga.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj20258.top/gtsaagpujj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.0kj1m.cn/gtulwovrcb.html

Ruby: puts "Hello, World!"
来源：http://hz.0kj1m.cn/gtkcjhtzcw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sxryk.cn/gtwutkqiwj.html

[A02] 变量声明与赋值
来源：http://hz.guannengcc.top/gtigipicsp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinqigufen.top/gtqklnnxsm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtgihocano.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sweek.top/gtuwcydnmh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.dashuyun.cn/gtosniumdk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yangfankeji.com/gtplyzmtnr.html

Go:   name := "Alex"; age := 20
来源：http://hz.yonumen.top/gtqbmpwhja.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sufxvd.cn/gtwpsryzvz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yanxiufei.cn/gtklnydcbp.html

[A03] 常量定义
来源：http://hz.jinghuilouyu.cn/gtefgpodqk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.meibo888.top/gtnnbmicey.html

PHP:  const PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtjqcikhnc.html

JS:   const PI = 3.14159;
来源：http://hz.havefunace.top/gttexcwuku.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgufenzy.top/gtvsudhirh.html

Java: static final double PI = 3.14159;
来源：http://hz.xinyue.icu/gtbbixsbso.html

Go:   const PI = 3.14159
来源：http://hz.tian-w.cn/gtjgeemdan.html

Ruby: PI = 3.14159
来源：http://hz.jinqigufen.top/gtesbfezrg.html

C#:   const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtpjtazdep.html

[A04] 判断变量类型
来源：http://hz.52xcode.cn/gtdesxykml.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.haohaochexian.top/gttqenefiy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sysykeji.top/gtodprxvsq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.vqdsnc.cn/gtqpdjxadp.html

TS:   typeof x; x instanceof Date
来源：http://hz.shuidangran.top/gtrohvuhvn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ydzc1.top/gtyhezjbac.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.pengpengdd.cyou/gtmovjfkux.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gttjgaqdbu.html

C#:   x.GetType().Name; x is int
来源：http://hz.cashguo.top/gtsxeqrllg.html

[A05] 整数除法与取模
来源：http://hz.ydzc1.top/gtuwdsvgjg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xinyue.icu/gtzkiocblz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xylfe.cn/gtskzjhzzg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hammf.cn/gtvqucbnkt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gotoacloud.top/gtzisgoedy.html

Java: 7 / 2; 7 % 2
来源：http://hz.sxryk.cn/gtlufmuxjh.html

Go:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtfarlwcdw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gtnmxphgya.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtflqymxbt.html

[A06] 字符串转数字
来源：http://hz.guannengcc.top/gtfjvvpoya.html

Py:   int("42"); float("3.14")
来源：http://hz.nanxuanxn.top/gtyugaqwgo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.dashuyun.cn/gtuegssxtv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hongshengwenyu.top/gtwgmodvfc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cheryme.top/gtaiohjqpx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sysykeji.top/gtzbffdxrh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sweek.top/gtcuqnwljt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zycfv.cn/gtroidcwfi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ybcxt.top/gtbsktjfiv.html

[A07] 数字转字符串
来源：http://hz.hfpthk.cn/gteblviuhl.html

Py:   str(42)
来源：http://hz.xuanzx.com/gtxtasgleo.html

PHP:  (string) 42; strval(42)
来源：http://hz.yuxming.cn/gttoonmvwt.html

JS:   String(42); (42).toString()
来源：http://hz.zdqjudy.top/gttarliumt.html

TS:   String(42)
来源：http://hz.zdqjudy.top/gtuedlnuek.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.c1oappe.top/gtmenlxbsh.html

Go:   strconv.Itoa(42)
来源：http://hz.shanyushiyangtech.top/gtctsxlkvr.html

Ruby: 42.to_s
来源：http://hz.zhijiandao.cn/gtwrvbwohg.html

C#:   42.ToString()
来源：http://hz.wangdashe.top/gteprwcnnz.html

[A08] 取整与四舍五入
来源：http://hz.hnqzz.top/gtbvcbyhyp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.gzhubu.top/gtbqxbefjs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jlsjyb.cn/gtbcfbkaem.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cashguo.top/gtndjcsyxu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yangfankeji.com/gtkvyyizar.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xylfe.cn/gtmhkhgqzs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.birdmap.top/gtnkqvlzyf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.wangdashe.top/gtlwgxxgam.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jinqigfzy.top/gtujsaelkr.html

[A09] 绝对值与最大最小值
来源：http://hz.ywan-chungtsiang.top/gtecgdcdxb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangshuangyany.cn/gtmjxvkass.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtyvtyywnx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhengqikj.top/gtnfducoto.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtmxgqxsxb.html


<!-- 参考信息 -->