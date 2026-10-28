代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.hongshengwenyu.top/gtgpalkngy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gogol.net.cn/gtuwemfdfs.html

[U68] PHP：PDO 连接
来源：http://hz.zhaomingkeji.xyz/gtdycowxro.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.mhx1999.top/gtggzwrkhf.html

[U69] PHP：PDO 预处理
来源：http://hz.kuanghao11.cn/gtiqahzioo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtqyqrofyr.html

[U70] PHP：PDO 事务
来源：http://hz.yueranfly.top/gtsyytmgqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.9152youxi.cn/gtrxxqggnf.html

[U71] PHP：抛出异常
来源：http://hz.sweek.top/gtwldevgzo.html

throw new RuntimeException("失败", 500);
来源：http://hz.cheryme.top/gtxphfwxsk.html

[U72] PHP：写错误日志
来源：http://hz.aizwys.cn/gtybvkjsux.html

error_log("失败: " . $e->getMessage());
来源：http://hz.redwolf501.top/gtipetmqfy.html

[U73] PHP：读取 ini 配置
来源：http://hz.pengpengdd.cyou/gtjnylnqmo.html

parse_ini_file("config.ini", true)
来源：http://hz.yonumen.top/gticgbhuis.html

[U74] PHP：读取环境变量
来源：http://hz.chenlongwang.top/gtkrocjwap.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gtvepjuqos.html

[U75] PHP：依赖注入
来源：http://hz.quarkkingdee.top/gtpvojdnnl.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtndchitwv.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtzacbltag.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sxryk.cn/gtneifpzev.html

[U77] PHP：模板渲染
来源：http://hz.tianlin.xyz/gtjahczocm.html

composer require twig/twig
来源：http://hz.smart0.xyz/gtqpywriif.html

[U78] PHP：单元测试
来源：http://hz.vqdsnc.cn/gtrszitjqx.html

composer require --dev phpunit/phpunit
来源：http://hz.fengsongda.top/gtspasrdpr.html

[U79] PHP：静态分析
来源：http://hz.hnqzz.top/gtdyqvkidg.html

composer require --dev phpstan/phpstan
来源：http://hz.ydjk.org.cn/gtggwnzstk.html

[U80] PHP：代码规范修复
来源：http://hz.cqqwz.cn/gtkfofdywu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtthwzcopm.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtmvndreiz.html

npm init -y;  npm i express
来源：http://hz.gogol.net.cn/gtzvbmapvt.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtntjsfepk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jiagoushi.top/gttliuwivu.html

[U83] JS：ES Module 导入导出
来源：http://hz.zdqjudy.top/gtxwonfzjs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtitedfqpz.html

[U84] JS：CommonJS 写法
来源：http://hz.zycfv.cn/gtanxohnrx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydzc1.top/gtygzqvvpb.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtvlzzczzk.html

a?.b?.c
来源：http://hz.svipenyu.cn/gtxemoslyp.html

[U86] JS：空值合并
来源：http://hz.hammf.cn/gtnpfoxrdc.html

a ?? b
来源：http://hz.yueranfly.top/gtljzulbmr.html

[U87] JS：解构默认值
来源：http://hz.ywan-chungtsiang.top/gtlhtrutwd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cheryme.top/gtzjpkblkw.html

[U88] JS：对象展开合并
来源：http://hz.xuetiantiany.cn/gtfbmzltqs.html

{ ...a, ...b }
来源：http://hz.tanke756.top/gtvmkzroyb.html

[U89] JS：数组去重
来源：http://hz.bjfxy.top/gtwahlyoti.html

[...new Set(arr)]
来源：http://hz.yuanzhike.top/gtwqvjsfes.html

[U90] JS：数字数组排序
来源：http://hz.zhengqikj.top/gttppphxlb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtflxyguve.html

[U91] JS：对象键值遍历
来源：http://hz.birdmap.top/gtxndimjew.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.fzhhl.top/gtjhtflmfi.html

[U92] JS：深拷贝
来源：http://hz.daxiang520.top/gtvouofmgu.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtpwmjhwcz.html

[U93] JS：模板字符串
来源：http://hz.zhijiandao.cn/gtegrcgpci.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtayjsoetf.html

[U94] JS：箭头函数
来源：http://hz.havefunace.top/gtakirbcst.html

const double = x => x * 2;
来源：http://hz.sxryk.cn/gtrpxskulq.html

[U95] JS：Promise 包装
来源：http://hz.chenjidiqi.icu/gtvhfmotqo.html

new Promise((resolve, reject) => {})
来源：http://hz.cashguo.top/gtvvnqpibp.html

[U96] JS：async/await 与异常
来源：http://hz.yj202588.top/gtnfytyitr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtluwijdfn.html

[U97] JS：并发请求
来源：http://hz.cucudq.cn/gtsmbakijf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtlyomclur.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhiwuduotai.top/gtoluxkohh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daria6918.cn/gtzvigvoha.html

[U99] JS：事件监听
来源：http://hz.c1oappe.top/gtlyftrbpd.html

el.addEventListener("click", e => {})
来源：http://hz.cashguo.top/gtkikiylhu.html

[U100] JS：DOM 查询
来源：http://hz.bjfxy.top/gtbzykcbnr.html

document.querySelector(".item")
来源：http://hz.jyoumei.cn/gtotbtkcra.html

[U101] JS：classList 操作
来源：http://hz.chenzaomai.com/gtecxkghtg.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtovuzxhea.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtygrazuuc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fzhhl.top/gtslpgxivz.html

[U103] JS：定时器
来源：http://hz.yangfankeji.com/gtrekcrdkv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ivvv.top/gteewbhguh.html

[U104] JS：防抖
来源：http://hz.shzxlz.cn/gtqzpyiplh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtrvewfxhk.html

[U105] JS：节流
来源：http://hz.hnxiangtu.top/gtdepzdvbw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.svipenyu.cn/gtdpdhmarb.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtrtwxkfxe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhengqikj.top/gtyeglrhpl.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtitoivgxg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jiagoushi.top/gtanrmyvmz.html

[U108] JS：随机整数
来源：http://hz.birdmap.top/gtpvlcwrdf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shuidangran.top/gtnqupbqhc.html

[U109] JS：数组分组
来源：http://hz.zycfv.cn/gtklizxrwq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtovswtulp.html

[U110] JS：数组分块
来源：http://hz.sweek.top/gtobkxxtfv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fzhhl.top/gthpymipuy.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtgmgrrils.html

new Map(Object.entries(obj))
来源：http://hz.xuanzx.com/gtvrifuqvu.html

[U112] JS：字符串补位
来源：http://hz.zhoulong.xyz/gtpfazclpq.html

"7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtuowhqqms.html

[U113] JS：正则替换全部
来源：http://hz.tian-w.cn/gtuwgczqng.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtinnjasep.html

[U114] JS：JSON 深比较
来源：http://hz.yuxming.cn/gtvcmwpdcr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtrovcnkna.html

[U115] JS：生成 UUID
来源：http://hz.shuidangran.top/gtmbbapbau.html

crypto.randomUUID()
来源：http://hz.ydzc1.top/gtoyyrlgis.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zdqjudy.top/gtzcqdaqdv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.wangdashe.top/gtnifwrxbj.html

[U117] JS：单元测试
来源：http://hz.jinghuilouyu.cn/gtodnmgyrs.html

npm i -D vitest;  npx vitest
来源：http://hz.jianghu66.top/gtmrnloljs.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtfbrxqslv.html

npm i -D vite;  npx vite
来源：http://hz.zhijiandao.cn/gthmktjoen.html

[U119] JS：生产构建
来源：http://hz.xuanzx.com/gtwcckelyv.html

npx vite build
来源：http://hz.ywan-chungtsiang.top/gtulsnxmsv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.vqdsnc.cn/gtfbrwmrlr.html

import.meta.env.VITE_API_URL
来源：http://hz.jinghuilouyu.cn/gtlmqjgcbh.html

================================================================================
来源：http://hz.zycfv.cn/gtcwhsydnp.html

统计汇总
来源：http://hz.yvedp.cn/gthsqbtwau.html

================================================================================
来源：http://hz.316326.xyz/gtwybbhudd.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtdpascpeh.html

Python ......... 252
来源：http://hz.fzhhl.top/gtaodmjlxh.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtnqyvrsed.html

JavaScript ..... 252
来源：http://hz.cqqwz.cn/gtekplcdhb.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gturejhdfr.html

Java ........... 212
来源：http://hz.svipenyu.cn/gticrglxcd.html

Go ............. 212
来源：http://hz.gaohongyu789.top/gtxdypttvs.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtsxgrcmkz.html

C# ............. 212
来源：http://hz.gotoacloud.top/gtglfatcdo.html

C .............. 30
来源：http://hz.52xcode.cn/gtyfrnrjqg.html

C++ ............ 30
来源：http://hz.snrcjt.cn/gtmehhlpvj.html

SQL ............ 90
来源：http://hz.jinghuilouyu.cn/gtvcrbgdnc.html

Bash ........... 80
来源：http://hz.tanke756.top/gtjkernuyg.html

Kotlin ......... 15
来源：http://hz.cucudq.cn/gtydrqduxs.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtfbjvdpah.html

Lua ............ 10
来源：http://hz.c1oappe.top/gtgyubuvdy.html

Perl ........... 10
来源：http://hz.zhixingplan.top/gtkdzdcqwm.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gtgfsxdxlx.html

------------------------------------
来源：http://hz.aizwys.cn/gtirlaqnhk.html

合计 ........... 2106 条
来源：http://hz.cheryme.top/gtibgtcnal.html

按章节统计：
来源：http://hz.jinqigfzy.top/gtwaeghwlh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtougtnlqs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtjsqfnovx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtwqpofkqj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yj20258888.top/gtecctrtbb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtlodppdxs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtpqvuzfeq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gthpaocktm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtruumvgno.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtdpnpdaxq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daxiang520.top/gtobzxizgg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtgadcyvnq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gthebmdtlb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtdzvbebwr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gtmqljoucy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuetiantiany.cn/gtewgfcjge.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtalrcrlyr.html

Q SQL 专题                              90
来源：http://hz.yj20258.top/gtirwvoukd.html

R Bash 专题                             80
来源：http://hz.jlsjyb.cn/gtrkncfuwi.html

S C / C++ 专题                          60
来源：http://hz.wangshuangyany.cn/gtuoniplsx.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gticnblbla.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtxltpdvtc.html

------------------------------------
来源：http://hz.0kj1m.cn/gtmzomojsr.html

合计                                  2106 条
来源：http://hz.ybcxt.top/gtqapozstu.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtbxhypges.html

使用提醒
来源：http://hz.xinyue.icu/gthamziuvo.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtwjpkwhqp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxinkj.top/gtwlegsmpd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydzc1.top/gtzronvlcx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuanzx.com/gtchbvftcq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ivvv.top/gtlwwvhpvf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtshmxofqz.html

—— 文件结束 ——
来源：http://hz.shangyingyoupin.top/gtzrejqoeo.html

================================================================================
来源：http://hz.guannengcc.top/gtlbtqozxn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shanyushiyangkeji.top/gtnwukezzj.html

Common Programming Examples Cheat Book
来源：http://hz.havefunace.top/gtzdjufsbr.html

================================================================================
来源：http://hz.zhengqikj.top/gtqkrsjhup.html

【收录内容】
来源：http://hz.bjfxy.top/gtcwahjaoj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhongyouzk.top/gtmlxzzcxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangkeji.top/gtwwolvjeh.html

SQL · Bash · C · C++
来源：http://hz.cqqwz.cn/gtacdxnzlj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nanxinkj.top/gtcxxrygdk.html

【使用说明】
来源：http://hz.sxryk.cn/gtbmehzcaj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.mhx1999.top/gtzdpbzmnz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtzsbutlsm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinyuanbaomall.cn/gtzmchngcc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zdqjudy.top/gthtruvkct.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtjcidtwad.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yvedp.cn/gtxhqbdpon.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangtech.top/gtpdycqktd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigufen.top/gtekevyaog.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtzzaxfivk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangdashe.top/gtklbpqftg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.redwolf501.top/gtxyuisayl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yonumen.top/gtpzzfpbur.html

【文件统计】
来源：http://hz.hammf.cn/gtqwffcarg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.fengsongda.top/gtdpeusgbz.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gtzkdyvpid.html

目  录
来源：http://hz.ybcxt.top/gtuvxfdvvv.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtxmzemttm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.9152youxi.cn/gtictrtaca.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yuxming.cn/gtrbpkxzvd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtgzljoiea.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hnxiangtu.top/gtqvavymdo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guannengcc.top/gtuvsbbekp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xingfuxueyuan.xyz/gtacxljdwh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtqnhfbgvg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.iojbl.cn/gtbywytpwx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtnqztnjcj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yonumen.top/gtsnhuwrgv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtzalezenq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtnclqiwta.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtxknbesxf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtzizkavtd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.kuanghao11.cn/gtfuzjfcsx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtzbqgbtnr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuanzx.com/gttajqzbpo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shangyingyoupin.top/gtlpcmjukh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.wangdashe.top/gtzgsmaebv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtxijxmfxf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.haohaochexian.top/gtnvqyyxmw.html

================================================================================
来源：http://hz.cdnleiting.top/gtvhocnrtw.html

A. 基础语法与类型
来源：http://hz.vqdsnc.cn/gtbpwqotai.html

================================================================================
来源：http://hz.gotoacloud.top/gtebwddsfm.html

[A01] Hello World
来源：http://hz.zycfv.cn/gtijunqgvn.html

Py:   print("Hello, World!")
来源：http://hz.9152youxi.cn/gtxpcfoqri.html

PHP:  echo "Hello, World!";
来源：http://hz.cucudq.cn/gtyvpeezlp.html

JS:   console.log("Hello, World!");
来源：http://hz.c1oappe.top/gtfrxzdies.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zycfv.cn/gttruvemhh.html

Java: System.out.println("Hello, World!");
来源：http://hz.birdmap.top/gtwqgvsxoj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.guannengcc.top/gttchajwzl.html

Ruby: puts "Hello, World!"
来源：http://hz.jinqigfzy.top/gttmxsutey.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258.top/gttwajaful.html

[A02] 变量声明与赋值
来源：http://hz.zhengqikj.top/gtzsjhqyig.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shangyingyoupin.top/gtwdrjfzei.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.haohaochexian.top/gtoikospub.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.haohaochexian.top/gtgqzjybfe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zdqjudy.top/gtbxuvdrbt.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtrhmbjceg.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinghuilouyu.cn/gteluqimwt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.316326.xyz/gtascadifw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gtatnperjm.html

[A03] 常量定义
来源：http://hz.guannengcc.top/gtibhkzldz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jlsjyb.cn/gtnzxsmjrr.html

PHP:  const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtqswifxvg.html

JS:   const PI = 3.14159;
来源：http://hz.aibaodan.cn/gteqnbnnaj.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtvvpsshsj.html

Java: static final double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtlnkpftjb.html

Go:   const PI = 3.14159
来源：http://hz.9152youxi.cn/gtaljyuzie.html

Ruby: PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtlemjdkca.html

C#:   const double PI = 3.14159;
来源：http://hz.ydzc1.top/gthwqzncbm.html

[A04] 判断变量类型
来源：http://hz.jinghuilouyu.cn/gtrbsstjxf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gtgfuijlwl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.cdnleiting.top/gtfthdqjvo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.52xcode.cn/gtonyeekgl.html

TS:   typeof x; x instanceof Date
来源：http://hz.zycfv.cn/gtjrpgocav.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinqigfzy.top/gtvfaktwgh.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinghuilouyu.cn/gtjcvomyyg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhaomingkeji.xyz/gtkyzrpyin.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinqigufen.top/gtxogsredn.html

[A05] 整数除法与取模
来源：http://hz.jianghu66.top/gtyygrbxxi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.wangdashe.top/gtifqhoymi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jlsjyb.cn/gtooodksen.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pycfn.com/gtagzihcsx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.iojbl.cn/gtmfxqeoml.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gthybnjnbg.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtapstmyjt.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtkyogniet.html

C#:   7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtvdipkqom.html

[A06] 字符串转数字
来源：http://hz.wangshuangyany.cn/gtdravmmay.html

Py:   int("42"); float("3.14")
来源：http://hz.aibaodan.cn/gthsimkono.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.wangshuangyany.cn/gtptkzjasb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtbkjplyfh.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guowangkeji.top/gtgqsxkvgr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhengqikj.top/gtrtzciipb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ehwqpu.com/gtxanuxsfs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.havefunace.top/gtirgxiwux.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jyoumei.cn/gtjtiajbfj.html

[A07] 数字转字符串
来源：http://hz.yvedp.cn/gtgbpdjhrg.html

Py:   str(42)
来源：http://hz.kuanghao11.cn/gtrnjryasp.html

PHP:  (string) 42; strval(42)
来源：http://hz.hnxiangtu.top/gtaruaxpzu.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangkeji.top/gtgqbyafda.html

TS:   String(42)
来源：http://hz.jyoumei.cn/gtdflmqcxb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zdqjudy.top/gtoycykyyw.html

Go:   strconv.Itoa(42)
来源：http://hz.pycfn.com/gtaqdncqig.html

Ruby: 42.to_s
来源：http://hz.jlsjyb.cn/gtrxgyabrr.html

C#:   42.ToString()
来源：http://hz.sufxvd.cn/gtqsikvumm.html

[A08] 取整与四舍五入
来源：http://hz.xingfuxueyuan.xyz/gtqtlxwlad.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.fengsongda.top/gtipsugikx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xinyue.icu/gtryxlcxek.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sweek.top/gtxwtbrmin.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigfzy.top/gtpmrxpoxk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gtshczmkqg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.9152youxi.cn/gtefntwkst.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.fengsongda.top/gtvaavpndx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.andypj.xyz/gthrwxdlil.html

[A09] 绝对值与最大最小值
来源：http://hz.jinqigufen.top/gtupuuwqif.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gzhubu.top/gthljfxcko.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yueranfly.top/gtthkcffiq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhiwuduotai.top/gtzhpvmued.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigufen.top/gtsszzguqb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhongyouzk.top/gtdnlkdzvg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhaomingkeji.xyz/gtukxfewni.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.wangdashe.top/gthizxzoww.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.9152youxi.cn/gtrflqnacd.html

[A10] 生成随机数
来源：http://hz.zhiwuduotai.top/gtgjklnklm.html

Py:   import random; random.randint(1, 100)
来源：http://hz.9152youxi.cn/gtqitibybz.html

PHP:  random_int(1, 100);
来源：http://hz.meibo888.top/gtfyektzkn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.iojbl.cn/gtemxuqkqj.html


<!-- 参考信息 -->