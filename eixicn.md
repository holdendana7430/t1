代发 wailian999

[U63] PHP：文件读写
来源：http://hz.yj20258.top/gtipcffxvx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.52xcode.cn/gtzpsczoht.html

[U64] PHP：目录遍历
来源：http://hz.redwolf501.top/gtttecxdbv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.iojbl.cn/gtohsdrjta.html

[U65] PHP：会话
来源：http://hz.jianghu66.top/gtxovdfrmu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.snrcjt.cn/gtmfovfzrv.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gthircnraa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yvedp.cn/gtfemolwyu.html

[U67] PHP：处理文件上传
来源：http://hz.mhx1999.top/gtqceiroqk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgufenzy.top/gtdmcgxsyw.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtbcpzgnrt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yanxiufei.cn/gtopwzncrh.html

[U69] PHP：PDO 预处理
来源：http://hz.daxiang520.top/gtuiqifscs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtlvtbccfv.html

[U70] PHP：PDO 事务
来源：http://hz.9152youxi.cn/gtoinvrwje.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ywan-chungtsiang.top/gtzuodblvo.html

[U71] PHP：抛出异常
来源：http://hz.dashuyun.cn/gttyyjkdyb.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtimnuljmo.html

[U72] PHP：写错误日志
来源：http://hz.fengsongda.top/gtmgvwnhcm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtlnertnzq.html

[U73] PHP：读取 ini 配置
来源：http://hz.yvedp.cn/gtejwitzlh.html

parse_ini_file("config.ini", true)
来源：http://hz.0kj1m.cn/gtenapviie.html

[U74] PHP：读取环境变量
来源：http://hz.cheryme.top/gtpjcmsrdp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xingfuxueyuan.xyz/gtrqljgrcc.html

[U75] PHP：依赖注入
来源：http://hz.meibo888.top/gttzeasgxr.html

composer require psr/container
来源：http://hz.52xcode.cn/gtzbrywlow.html

[U76] PHP：简单路由
来源：http://hz.shzxlz.cn/gtoybkruhv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yonumen.top/gtuigbirne.html

[U77] PHP：模板渲染
来源：http://hz.wangshuangyany.cn/gthulehesj.html

composer require twig/twig
来源：http://hz.ybcxt.top/gthcgdcmbl.html

[U78] PHP：单元测试
来源：http://hz.snrcjt.cn/gtckpcnxba.html

composer require --dev phpunit/phpunit
来源：http://hz.jlsjyb.cn/gtdzvbogmx.html

[U79] PHP：静态分析
来源：http://hz.zhaomingkeji.xyz/gtzpvyjzfc.html

composer require --dev phpstan/phpstan
来源：http://hz.yvedp.cn/gtnlpsqdlh.html

[U80] PHP：代码规范修复
来源：http://hz.xinyue.icu/gtsnfkhljp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.52xcode.cn/gtxnjbbljb.html

[U81] JS：初始化项目
来源：http://hz.gzhubu.top/gtpxsmcbag.html

npm init -y;  npm i express
来源：http://hz.zycfv.cn/gtamvyrmas.html

[U82] JS：package.json 脚本
来源：http://hz.vqdsnc.cn/gthzwfuvvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtpwrumqcx.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtyikasxgv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtturovgny.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtiltifxnm.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hnxiangtu.top/gtzjeorqsu.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtnqqjtpwq.html

a?.b?.c
来源：http://hz.zycfv.cn/gtkjjuqkgm.html

[U86] JS：空值合并
来源：http://hz.zhengqikj.top/gtxwljtfjl.html

a ?? b
来源：http://hz.yj20258.top/gtjohehrdf.html

[U87] JS：解构默认值
来源：http://hz.zhoulong.xyz/gtafgiolps.html

const { a = 1, b = 2 } = obj;
来源：http://hz.0kj1m.cn/gtswdhtkmu.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtegbppeaa.html

{ ...a, ...b }
来源：http://hz.yongpay.top/gtcsdyjdmu.html

[U89] JS：数组去重
来源：http://hz.zhengqikj.top/gtxgqnfzvd.html

[...new Set(arr)]
来源：http://hz.guannengcc.top/gtlzhutdiw.html

[U90] JS：数字数组排序
来源：http://hz.xziqi.cn/gtbfnmenlo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtjsbvdkgb.html

[U91] JS：对象键值遍历
来源：http://hz.dianchejie.cn/gtkqsbrmun.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yuanzhike.top/gtthhdvfym.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtbynhjbdb.html

structuredClone(obj)
来源：http://hz.hnqzz.top/gtwrqzhhts.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtemkvfgew.html

`共 ${n} 条`
来源：http://hz.sufxvd.cn/gtolrntesh.html

[U94] JS：箭头函数
来源：http://hz.kuanghao11.cn/gtxupxtydl.html

const double = x => x * 2;
来源：http://hz.aibaodan.cn/gtlkowbqyn.html

[U95] JS：Promise 包装
来源：http://hz.havefunace.top/gtgmeodamy.html

new Promise((resolve, reject) => {})
来源：http://hz.c1oappe.top/gtcphalpwl.html

[U96] JS：async/await 与异常
来源：http://hz.havefunace.top/gtuebudnez.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtapvbhsrg.html

[U97] JS：并发请求
来源：http://hz.ydzc1.top/gtqjafkumq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtimlzjqmu.html

[U98] JS：fetch 带 JSON
来源：http://hz.pycfn.com/gttipmqmfg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtkjyyprot.html

[U99] JS：事件监听
来源：http://hz.aibaodan.cn/gtvjgpjylb.html

el.addEventListener("click", e => {})
来源：http://hz.zhiwuduotai.top/gtxevrdwxs.html

[U100] JS：DOM 查询
来源：http://hz.svipenyu.cn/gtdmgyhcbo.html

document.querySelector(".item")
来源：http://hz.gaohongyu789.top/gtlczsvpoa.html

[U101] JS：classList 操作
来源：http://hz.ppjwa.cn/gtmdlgtinr.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtwsjrcxck.html

[U102] JS：本地存储
来源：http://hz.ybcxt.top/gtjcspesub.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cucudq.cn/gtrwlryxeu.html

[U103] JS：定时器
来源：http://hz.yvedp.cn/gtyjogogan.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xziqi.cn/gttvyoumpt.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtgbxflwqi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtunyoersu.html

[U105] JS：节流
来源：http://hz.ydzc1.top/gtyswvqead.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangshuangyany.cn/gthppjmqgg.html

[U106] JS：日期格式化
来源：http://hz.yanxiufei.cn/gtbxypsygf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xingfuxueyuan.xyz/gtwygmzpwq.html

[U107] JS：数字千分位
来源：http://hz.ppjwa.cn/gtfpidiesi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtieazhtco.html

[U108] JS：随机整数
来源：http://hz.chenlongwang.top/gtilukmskz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hywenlv.cn/gtyxdjtrna.html

[U109] JS：数组分组
来源：http://hz.jqgufenzy.top/gtwgemvjuc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtzbfbskrp.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtewbhhmgn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sxryk.cn/gtunvhbyng.html

[U111] JS：对象转 Map
来源：http://hz.yanxiufei.cn/gtpihamaoa.html

new Map(Object.entries(obj))
来源：http://hz.jinqigufen.top/gtkjcxvimi.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gtlwtumytf.html

"7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtgfkvtlcw.html

[U113] JS：正则替换全部
来源：http://hz.hnqzz.top/gtxeknrbww.html

s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtrolhxord.html

[U114] JS：JSON 深比较
来源：http://hz.xuetiantiany.cn/gtypigavwl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtjtsciedj.html

[U115] JS：生成 UUID
来源：http://hz.yj20258.top/gtfhfvgbqw.html

crypto.randomUUID()
来源：http://hz.sxryk.cn/gtbcprrgsr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtfwqmrezr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtritklcmo.html

[U117] JS：单元测试
来源：http://hz.havefunace.top/gtsihdcysp.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gttngabida.html

[U118] JS：开发服务器
来源：http://hz.ywan-chungtsiang.top/gtdekldawo.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gtwljlhtyj.html

[U119] JS：生产构建
来源：http://hz.cheryme.top/gtohcwgnhe.html

npx vite build
来源：http://hz.cashguo.top/gtaoclgicb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.c1oappe.top/gtmzxkuylm.html

import.meta.env.VITE_API_URL
来源：http://hz.shuidangran.top/gtevrprevy.html

================================================================================
来源：http://hz.iojbl.cn/gtsulujkuq.html

统计汇总
来源：http://hz.zhongyouzk.top/gtfimliset.html

================================================================================
来源：http://hz.chenzaomai.com/gtdzqbmypt.html

按语言统计（条）：
来源：http://hz.redwolf501.top/gtmewwattw.html

Python ......... 252
来源：http://hz.hysaishi.cn/gtaxfpjkay.html

PHP ............ 252
来源：http://hz.jqgfzy.top/gtbmrppmlv.html

JavaScript ..... 252
来源：http://hz.yj202588.top/gtjuupsbeg.html

TypeScript ..... 212
来源：http://hz.cashguo.top/gturslzglo.html

Java ........... 212
来源：http://hz.fzhhl.top/gtudnomvhw.html

Go ............. 212
来源：http://hz.pycfn.com/gtfrgklyhb.html

Ruby ........... 212
来源：http://hz.cashguo.top/gtcysqlxxz.html

C# ............. 212
来源：http://hz.zhongyouzk.top/gtmrazfiub.html

C .............. 30
来源：http://hz.vqdsnc.cn/gtooiccabc.html

C++ ............ 30
来源：http://hz.nanxinkj.top/gtnqngewlj.html

SQL ............ 90
来源：http://hz.bjfxy.top/gtpeztnnuv.html

Bash ........... 80
来源：http://hz.aizwys.cn/gtthhkiirc.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtnlqtnajv.html

Swift .......... 15
来源：http://hz.shzxlz.cn/gtveupdhke.html

Lua ............ 10
来源：http://hz.svipenyu.cn/gthxxjfnah.html

Perl ........... 10
来源：http://hz.zdqjudy.top/gthjartvkc.html

Scala .......... 10
来源：http://hz.andypj.xyz/gtnyuonnue.html

------------------------------------
来源：http://hz.hywenlv.cn/gtrsgyxxan.html

合计 ........... 2106 条
来源：http://hz.c1oappe.top/gthuraqdsu.html

按章节统计：
来源：http://hz.yuxming.cn/gtljthsmue.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gteiarsfqu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtkdhhdjcv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtzrnmikrq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtayfahkcs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinghuilouyu.cn/gtdmjmnmah.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hnqzz.top/gtvqbcxrvi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtjiwupidk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtiwdelhlq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gttjetblni.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gtdsfrduim.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtwzwcaxtr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtetbkzpcs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtzefgwjjw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtsszsfroi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuetiantiany.cn/gtezcigprn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtnbjjuwis.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtngbmrndm.html

R Bash 专题                             80
来源：http://hz.gzhubu.top/gtcqcwoadf.html

S C / C++ 专题                          60
来源：http://hz.ehwqpu.com/gthtatxvev.html

T 其他语言补充                          60
来源：http://hz.ppjwa.cn/gtwgebndni.html

U 高频实用片段                         120
来源：http://hz.yj202588.top/gtkggspunm.html

------------------------------------
来源：http://hz.guowangkeji.top/gtwwuirwvo.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtjuryiyij.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gttofztaij.html

使用提醒
来源：http://hz.hammf.cn/gtdqglrgde.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtzyozzaxv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangshuangyany.cn/gtvrnrivir.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnqzz.top/gtplfpclue.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenjidiqi.icu/gthhsghmbl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yvedp.cn/gtcqtxkwqp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.svipenyu.cn/gtxermfphr.html

—— 文件结束 ——
来源：http://hz.yanxiufei.cn/gttncdsofx.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrarrjkoo.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.andypj.xyz/gtznlgkfbe.html

Common Programming Examples Cheat Book
来源：http://hz.hammf.cn/gtyyzcfihy.html

================================================================================
来源：http://hz.c1oappe.top/gtxxvaiagt.html

【收录内容】
来源：http://hz.52xcode.cn/gthzoggeok.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daxiang520.top/gtcqmzhgtb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cucudq.cn/gtttdobdid.html

SQL · Bash · C · C++
来源：http://hz.ivvv.top/gtgkseygqf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yonumen.top/gtcnhtnjou.html

【使用说明】
来源：http://hz.nanxuanxn.top/gtffqopcit.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zycfv.cn/gttbybrbqd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gzhubu.top/gtkrkpaeuv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhongyouzk.top/gtnoowwedu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.daria6918.cn/gtupwknlkz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtdojnfgte.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yvedp.cn/gtopcmznzz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hfpthk.cn/gtgqlhdedc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shanyushiyangtech.top/gtuwgijhxn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj20258888.top/gtzhasmliv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yangfankeji.com/gthnnjvirr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtdtqrafsb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.havefunace.top/gtqllgrokb.html

【文件统计】
来源：http://hz.316326.xyz/gtnbzroxii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sysykeji.top/gtuvzktjye.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtrfxfzhrc.html

目  录
来源：http://hz.chenlongwang.top/gtiisodwzp.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtboewvcmy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shuidangran.top/gtiyzhavta.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtsekgblxi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtpxwqmowv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtlfaqhbob.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.andypj.xyz/gtsbgstmxy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtvjmupdxj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yuxming.cn/gtybsexuls.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yvedp.cn/gthqxfkdqg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtogyfbvmp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jiagoushi.top/gtlncyttuy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtfvulytrh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gteexjnwwf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtwqsionya.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtkzgozlat.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pengpengdd.cyou/gtduehqncx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtsqzdyhbp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtievijlfl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenjidiqi.icu/gtevyxrnby.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtydplsmmj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtyyuvmvpp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtrvbtzhip.html

================================================================================
来源：http://hz.yj20258.top/gtofiwmflz.html

A. 基础语法与类型
来源：http://hz.yj20258888.top/gtpcsmcvyw.html

================================================================================
来源：http://hz.mhx1999.top/gtsfqhrjiw.html

[A01] Hello World
来源：http://hz.xuetiantiany.cn/gthnposogo.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtjcabqbos.html

PHP:  echo "Hello, World!";
来源：http://hz.cucudq.cn/gtjtuoqfae.html

JS:   console.log("Hello, World!");
来源：http://hz.jinqigfzy.top/gtrclkxgzl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gogol.net.cn/gtwhiebbxo.html

Java: System.out.println("Hello, World!");
来源：http://hz.gzhubu.top/gtyzgvfozu.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgufenzy.top/gtxgkmpguy.html

Ruby: puts "Hello, World!"
来源：http://hz.fengsongda.top/gtzctplbnn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tian-w.cn/gtqbgggshl.html

[A02] 变量声明与赋值
来源：http://hz.sxryk.cn/gtlfyyprrs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangtech.top/gtbpwuunwb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtrbzwrrmj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shangyingyoupin.top/gtjdiqxnnf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.snrcjt.cn/gtcmcwqzhz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangtech.top/gtprxbebzl.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhaomingkeji.xyz/gtsyzxxrpr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.9152youxi.cn/gtihzwxqdq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtwtnkyhlh.html

[A03] 常量定义
来源：http://hz.guannengcc.top/gthhlfnuud.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shuidangran.top/gtgvfmlwwe.html

PHP:  const PI = 3.14159;
来源：http://hz.haohaochexian.top/gthfsppdfl.html

JS:   const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtliggmpqg.html

TS:   const PI: number = 3.14159;
来源：http://hz.gaohongyu789.top/gtuxnkqpzv.html

Java: static final double PI = 3.14159;
来源：http://hz.xziqi.cn/gtphbceuyi.html

Go:   const PI = 3.14159
来源：http://hz.andypj.xyz/gtrjdyfnbm.html

Ruby: PI = 3.14159
来源：http://hz.zhengqikj.top/gtmyawligu.html

C#:   const double PI = 3.14159;
来源：http://hz.smart0.xyz/gteopugrkh.html

[A04] 判断变量类型
来源：http://hz.feifeiyinyue.top/gtpzdtqazc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnxiangtu.top/gtquswesep.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hywenlv.cn/gtphddnkfb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.snrcjt.cn/gtiqtaaqph.html

TS:   typeof x; x instanceof Date
来源：http://hz.guowangkeji.top/gttxheldes.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gtdeqtbffn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gaohongyu789.top/gtrpthcqnn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.birdmap.top/gtjnifrwcj.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinyuanbaomall.cn/gttqqjuxtv.html

[A05] 整数除法与取模
来源：http://hz.smart0.xyz/gtxscgntvy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shangyingyoupin.top/gtmynvrckr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.svipenyu.cn/gtxkssgddk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.iojbl.cn/gtcstnqncl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yangfankeji.com/gtprmocpwd.html

Java: 7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtaxlqmicn.html

Go:   7 / 2; 7 % 2
来源：http://hz.pengpengdd.cyou/gteczpcfuo.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtbnwqacan.html

C#:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gttimyyjuj.html

[A06] 字符串转数字
来源：http://hz.xinyue.icu/gtogftrcny.html

Py:   int("42"); float("3.14")
来源：http://hz.yonumen.top/gtflyhcyxg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.nanxuanxn.top/gtbjmrzopn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.tianlin.xyz/gtttpxxgae.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.gotoacloud.top/gtqhkcltvd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sysykeji.top/gtzhyilvaa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xingfuxueyuan.xyz/gtxcejffhu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.9152youxi.cn/gthisglrjj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtzpocvgcg.html

[A07] 数字转字符串
来源：http://hz.shzxlz.cn/gtwpoppdlu.html

Py:   str(42)
来源：http://hz.ehwqpu.com/gtmtunfdrf.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj20258.top/gtzyjipqmu.html

JS:   String(42); (42).toString()
来源：http://hz.hywenlv.cn/gtcjwkrkoh.html

TS:   String(42)
来源：http://hz.zhixingplan.top/gtyfabjtxy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sxryk.cn/gtzympkyfo.html

Go:   strconv.Itoa(42)
来源：http://hz.xingfuxueyuan.xyz/gtdtvfsxom.html

Ruby: 42.to_s
来源：http://hz.guowangkeji.top/gtbukyervr.html

C#:   42.ToString()
来源：http://hz.haohaochexian.top/gthqsgugtj.html

[A08] 取整与四舍五入
来源：http://hz.pycfn.com/gtaicbfjsr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.birdmap.top/gtjalaelyo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.guowangkeji.top/gtsidyjxpd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtyktspohc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zycfv.cn/gtlbtjyzne.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yanxiufei.cn/gtiigwjgsa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.gaohongyu789.top/gtdiaxtmzm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yueranfly.top/gtuyqhyrbc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sysykeji.top/gtkgedwenr.html

[A09] 绝对值与最大最小值
来源：http://hz.gogol.net.cn/gtkgzpvfgu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.snrcjt.cn/gtfirxthep.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhixingplan.top/gtgxubxoqp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xuetiantiany.cn/gtpyvxtptp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtglnurguv.html


<!-- 参考信息 -->