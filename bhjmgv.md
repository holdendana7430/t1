代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.shangyingyoupin.top/gtslavmphv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.9152youxi.cn/gtvabvbhry.html

[U68] PHP：PDO 连接
来源：http://hz.cheryme.top/gtodgelsrx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.smart0.xyz/gtedksjqev.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtfvzgljsn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuxming.cn/gtmeggbbiw.html

[U70] PHP：PDO 事务
来源：http://hz.zhengqikj.top/gtjbnhsupg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tanke756.top/gtgiwghied.html

[U71] PHP：抛出异常
来源：http://hz.kuanghao11.cn/gtjqevdvyh.html

throw new RuntimeException("失败", 500);
来源：http://hz.yuanzhike.top/gtuaedtznm.html

[U72] PHP：写错误日志
来源：http://hz.dashuyun.cn/gtdtywxraj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xylfe.cn/gtbqnuyiit.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuxming.cn/gthimzmtem.html

parse_ini_file("config.ini", true)
来源：http://hz.hysaishi.cn/gtwnmbmqnv.html

[U74] PHP：读取环境变量
来源：http://hz.ehwqpu.com/gtnpiccfxw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.bjfxy.top/gtetvvuesc.html

[U75] PHP：依赖注入
来源：http://hz.zhoulong.xyz/gtxwxhfraa.html

composer require psr/container
来源：http://hz.hfpthk.cn/gtbiyddnzr.html

[U76] PHP：简单路由
来源：http://hz.sysykeji.top/gtwwgvddra.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhaomingkeji.xyz/gtnofhuswv.html

[U77] PHP：模板渲染
来源：http://hz.guannengcc.top/gtbbdbginq.html

composer require twig/twig
来源：http://hz.shanyushiyangkeji.top/gtldnqwsbf.html

[U78] PHP：单元测试
来源：http://hz.xuetiantiany.cn/gtqhyaujen.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtytqfnnbv.html

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gtsatlwkwm.html

composer require --dev phpstan/phpstan
来源：http://hz.meibo888.top/gtrwrdladb.html

[U80] PHP：代码规范修复
来源：http://hz.mhx1999.top/gtschroene.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cashguo.top/gtucufdqoc.html

[U81] JS：初始化项目
来源：http://hz.yuanzhike.top/gtpwtplygq.html

npm init -y;  npm i express
来源：http://hz.wangshuangyany.cn/gtihmubnza.html

[U82] JS：package.json 脚本
来源：http://hz.cqqwz.cn/gtcjhkabvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xinyue.icu/gtwpqpdazz.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gtxsjboywm.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yvedp.cn/gtjdxzlnit.html

[U84] JS：CommonJS 写法
来源：http://hz.zhixingplan.top/gtozhyldpi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinyuanbaomall.cn/gtuxcddegb.html

[U85] JS：可选链
来源：http://hz.jqgufenzy.top/gtooazzqxu.html

a?.b?.c
来源：http://hz.zhoulong.xyz/gtcibkvivf.html

[U86] JS：空值合并
来源：http://hz.chenzaomai.com/gtwetsvdeh.html

a ?? b
来源：http://hz.hongshengwenyu.top/gtjdgxzxia.html

[U87] JS：解构默认值
来源：http://hz.ybcxt.top/gtsnqwfvom.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gtbneokuyu.html

[U88] JS：对象展开合并
来源：http://hz.ivvv.top/gtoefuggrk.html

{ ...a, ...b }
来源：http://hz.hammf.cn/gtppkhcwny.html

[U89] JS：数组去重
来源：http://hz.cucudq.cn/gtqijpkndt.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtyvslgtib.html

[U90] JS：数字数组排序
来源：http://hz.aizwys.cn/gtxwfvfrqy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtageygdhd.html

[U91] JS：对象键值遍历
来源：http://hz.sweek.top/gtchanhswz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sweek.top/gtnuaubwow.html

[U92] JS：深拷贝
来源：http://hz.dianchejie.cn/gtcepsxxnx.html

structuredClone(obj)
来源：http://hz.9152youxi.cn/gtugpyjqjg.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtxpjytlju.html

`共 ${n} 条`
来源：http://hz.gogol.net.cn/gtelsmeskf.html

[U94] JS：箭头函数
来源：http://hz.jinqigfzy.top/gtelxbjvfd.html

const double = x => x * 2;
来源：http://hz.sufxvd.cn/gtmzrjpykb.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtngoojfcq.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtzebtzwsk.html

[U96] JS：async/await 与异常
来源：http://hz.ppjwa.cn/gtnjsythvq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtuxysfwos.html

[U97] JS：并发请求
来源：http://hz.pycfn.com/gtmcdxryav.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gttmrhwdhh.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhaomingkeji.xyz/gtnpqtvupp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnqzz.top/gtvqrvvqul.html

[U99] JS：事件监听
来源：http://hz.chenjidiqi.icu/gtjjgdwgys.html

el.addEventListener("click", e => {})
来源：http://hz.bjfxy.top/gtqamkvnrd.html

[U100] JS：DOM 查询
来源：http://hz.vqdsnc.cn/gttomcqglu.html

document.querySelector(".item")
来源：http://hz.havefunace.top/gtsqfxksbr.html

[U101] JS：classList 操作
来源：http://hz.havefunace.top/gtfbtamxdr.html

el.classList.toggle("active")
来源：http://hz.yongpay.top/gtdrljrxdr.html

[U102] JS：本地存储
来源：http://hz.hnqzz.top/gtdggbgwbc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtrxswgtql.html

[U103] JS：定时器
来源：http://hz.snrcjt.cn/gtwreseapk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuanzhike.top/gtxxgaurhs.html

[U104] JS：防抖
来源：http://hz.sweek.top/gtmtmbubpg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtnyiqdknc.html

[U105] JS：节流
来源：http://hz.ppjwa.cn/gtnzdphlnd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xinyue.icu/gtpqeqldvr.html

[U106] JS：日期格式化
来源：http://hz.mhx1999.top/gtoepayyvp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnxiangtu.top/gtmdqxyotd.html

[U107] JS：数字千分位
来源：http://hz.gotoacloud.top/gtnbrnjqal.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jianghu66.top/gtmvbkbmcc.html

[U108] JS：随机整数
来源：http://hz.yonumen.top/gtohivkawo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cdnleiting.top/gtjgaepfxj.html

[U109] JS：数组分组
来源：http://hz.tanke756.top/gtahppanja.html

Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtlnuseatz.html

[U110] JS：数组分块
来源：http://hz.haohaochexian.top/gtfhnkmgch.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.vqdsnc.cn/gtpajjsbir.html

[U111] JS：对象转 Map
来源：http://hz.gogol.net.cn/gtrtpzbzkf.html

new Map(Object.entries(obj))
来源：http://hz.316326.xyz/gtvluhklkv.html

[U112] JS：字符串补位
来源：http://hz.ydjk.org.cn/gtbcevbenz.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtgptixrhz.html

[U113] JS：正则替换全部
来源：http://hz.xinyue.icu/gtpkbtzpif.html

s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtwkstnozm.html

[U114] JS：JSON 深比较
来源：http://hz.xuanzx.com/gtrabkwwks.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxinkj.top/gtogksmsdo.html

[U115] JS：生成 UUID
来源：http://hz.chenzaomai.com/gtzybyigdo.html

crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtqfyjlvux.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gtddaygdro.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnxiangtu.top/gtuiembbyx.html

[U117] JS：单元测试
来源：http://hz.xuetiantiany.cn/gtecxeusyo.html

npm i -D vitest;  npx vitest
来源：http://hz.ywan-chungtsiang.top/gtrojgsrxe.html

[U118] JS：开发服务器
来源：http://hz.haohaochexian.top/gtaqmdxort.html

npm i -D vite;  npx vite
来源：http://hz.xuanzx.com/gtztwmbknl.html

[U119] JS：生产构建
来源：http://hz.pycfn.com/gtzokeruip.html

npx vite build
来源：http://hz.haohaochexian.top/gtachnbogk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tianlin.xyz/gtrkdqboei.html

import.meta.env.VITE_API_URL
来源：http://hz.zycfv.cn/gtelthqmgc.html

================================================================================
来源：http://hz.ydzc1.top/gttenanjko.html

统计汇总
来源：http://hz.zhengqikj.top/gtfpwfyxld.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtntdopqpy.html

按语言统计（条）：
来源：http://hz.birdmap.top/gtvmejibkj.html

Python ......... 252
来源：http://hz.yuanzhike.top/gtufkennfe.html

PHP ............ 252
来源：http://hz.jianghu66.top/gthdonuqbc.html

JavaScript ..... 252
来源：http://hz.chenlongwang.top/gtzwvnphig.html

TypeScript ..... 212
来源：http://hz.c1oappe.top/gtkosohxmu.html

Java ........... 212
来源：http://hz.cdnleiting.top/gtackpqbyj.html

Go ............. 212
来源：http://hz.tian-w.cn/gtkmvfgsuv.html

Ruby ........... 212
来源：http://hz.shangyingyoupin.top/gtmpdmvxnd.html

C# ............. 212
来源：http://hz.52xcode.cn/gtrivmlxeh.html

C .............. 30
来源：http://hz.sufxvd.cn/gtwbmcljhv.html

C++ ............ 30
来源：http://hz.gzhubu.top/gtmvitqarw.html

SQL ............ 90
来源：http://hz.chenlongwang.top/gtqqqkqtqs.html

Bash ........... 80
来源：http://hz.zhixingplan.top/gttrwgyvxm.html

Kotlin ......... 15
来源：http://hz.hysaishi.cn/gtifdndwgg.html

Swift .......... 15
来源：http://hz.chenlongwang.top/gteuwhndwv.html

Lua ............ 10
来源：http://hz.sweek.top/gthjkuynkh.html

Perl ........... 10
来源：http://hz.yj202588.top/gtjxavxmem.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtdqudqtiy.html

------------------------------------
来源：http://hz.gotoacloud.top/gtouzdlcul.html

合计 ........... 2106 条
来源：http://hz.jinqigfzy.top/gtmqivsvkr.html

按章节统计：
来源：http://hz.shanyushiyangkeji.top/gtqwfmdkub.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gtcwrzzzbw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtnrpbewme.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gthuthabuh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtjrkkiqzy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtrijzejai.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.iojbl.cn/gtfcvsydem.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtmttbnddc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtuqxicmsu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtsdkqjujl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtyfgsislq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtakzesgge.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtvornjcyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtqpxbqvfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtharvcxbd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.feifeiyinyue.top/gtccmbftsa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtyrwqsfcn.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtqxtnmvsr.html

R Bash 专题                             80
来源：http://hz.mhx1999.top/gtwtsacqdq.html

S C / C++ 专题                          60
来源：http://hz.cashguo.top/gthehbotso.html

T 其他语言补充                          60
来源：http://hz.zycfv.cn/gtyustawxv.html

U 高频实用片段                         120
来源：http://hz.xylfe.cn/gtltzydbcj.html

------------------------------------
来源：http://hz.iojbl.cn/gtasbpiiiv.html

合计                                  2106 条
来源：http://hz.daria6918.cn/gtchiomnhk.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtczkarlhm.html

使用提醒
来源：http://hz.gotoacloud.top/gthcmxeysk.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtuzqlwpsg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cashguo.top/gtbbrhbvby.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cdnleiting.top/gtcvgtriqo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhijiandao.cn/gtwaboibml.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hfpthk.cn/gtpssnsbxy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.smart0.xyz/gtxdpkgfsy.html

—— 文件结束 ——
来源：http://hz.yuxming.cn/gtzdoqavrf.html

================================================================================
来源：http://hz.cashguo.top/gtnxpggowh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sysykeji.top/gtckaedanw.html

Common Programming Examples Cheat Book
来源：http://hz.gzhubu.top/gtupeqdsbq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbfszijmg.html

【收录内容】
来源：http://hz.feifeiyinyue.top/gthbqwjity.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zycfv.cn/gtvjjbttls.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.daria6918.cn/gtazjyfuta.html

SQL · Bash · C · C++
来源：http://hz.zdqjudy.top/gteiuvzdxk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtppraulzy.html

【使用说明】
来源：http://hz.daria6918.cn/gtbsrtrhax.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhongyouzk.top/gtvfiprxnm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xziqi.cn/gtpjshqkfk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenjidiqi.icu/gtfgkdxeet.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cucudq.cn/gtdqnrqryc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cucudq.cn/gtnalrwgha.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.mhx1999.top/gtrsskvrwh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gtiwpegpxq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yanxiufei.cn/gtfjgepemf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.316326.xyz/gtmmboluqb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinqigfzy.top/gtvmtgmdfj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.meibo888.top/gthzvicqeq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangdashe.top/gtaqslhxua.html

【文件统计】
来源：http://hz.zhaomingkeji.xyz/gtpdizjzlv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ybcxt.top/gtsyrgegtz.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtggfcfuwy.html

目  录
来源：http://hz.snrcjt.cn/gtbzyikgal.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtjkqwysab.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenjidiqi.icu/gtgjsamczy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtnbyhnmgu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtcoabtdbg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtuqmbpzfo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cashguo.top/gtunreesqc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtcjpkwxmg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtpyaldlyz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtqfduxlkq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtncuufhlz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xingfuxueyuan.xyz/gtxtafyvhq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtiemboyvi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gttdhwcrox.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtxzxarhqq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xziqi.cn/gthazloyjz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zycfv.cn/gtoivqeres.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtiyvyqwmd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydjk.org.cn/gtvpokhnyo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tanke756.top/gtsjlfwndq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinqigfzy.top/gtskugwxca.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtuzakblae.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtrdaiapsy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfasyptdq.html

A. 基础语法与类型
来源：http://hz.yongpay.top/gtklvigyix.html

================================================================================
来源：http://hz.9152youxi.cn/gtjnoctavs.html

[A01] Hello World
来源：http://hz.nanxuanxn.top/gtnkrqiwxc.html

Py:   print("Hello, World!")
来源：http://hz.smart0.xyz/gtzgeniwjw.html

PHP:  echo "Hello, World!";
来源：http://hz.cheryme.top/gtmazxocfg.html

JS:   console.log("Hello, World!");
来源：http://hz.tianlin.xyz/gtmcvevclg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.quarkkingdee.top/gtscfgfxau.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtnzyyhhef.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangdashe.top/gtaqurqluj.html

Ruby: puts "Hello, World!"
来源：http://hz.tianlin.xyz/gthjeyujsm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jqgfzy.top/gtewrhenws.html

[A02] 变量声明与赋值
来源：http://hz.aibaodan.cn/gtapcvdave.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gogol.net.cn/gtmpjtiutd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ywan-chungtsiang.top/gtzwqjbisl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.andypj.xyz/gtbjtdvegu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.snrcjt.cn/gteftqhdal.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aibaodan.cn/gtdfcozliw.html

Go:   name := "Alex"; age := 20
来源：http://hz.redwolf501.top/gtpjvjyqhf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.pengpengdd.cyou/gtjlhsyrvm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtjaeffcpl.html

[A03] 常量定义
来源：http://hz.haohaochexian.top/gtvtmuuamg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aibaodan.cn/gtcaabduuu.html

PHP:  const PI = 3.14159;
来源：http://hz.chenzaomai.com/gtrmrdsfiu.html

JS:   const PI = 3.14159;
来源：http://hz.bjfxy.top/gtozxvfhgt.html

TS:   const PI: number = 3.14159;
来源：http://hz.chenzaomai.com/gtapauvofa.html

Java: static final double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtqdjmogna.html

Go:   const PI = 3.14159
来源：http://hz.gogol.net.cn/gtjzjpczwc.html

Ruby: PI = 3.14159
来源：http://hz.gotoacloud.top/gtieyqqwry.html

C#:   const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtirqlyzvy.html

[A04] 判断变量类型
来源：http://hz.chenzaomai.com/gtdslwvict.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gaohongyu789.top/gtrmgqpell.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.kuanghao11.cn/gtmrgnfjqh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jqgufenzy.top/gtxthdnita.html

TS:   typeof x; x instanceof Date
来源：http://hz.redwolf501.top/gtzeqhizpu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yangfankeji.com/gtzcpongub.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.havefunace.top/gtscoqdalq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xziqi.cn/gtfzziklnb.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgufenzy.top/gtbxgfaobt.html

[A05] 整数除法与取模
来源：http://hz.redwolf501.top/gtpqlkymcf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxuanxn.top/gteavjdqci.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhixingplan.top/gtxrimecks.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shuidangran.top/gtedxynsob.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ehwqpu.com/gtmaocuugq.html

Java: 7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gtzjguikwf.html

Go:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtkjesxweg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtsagmfeyg.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtfonwckwo.html

[A06] 字符串转数字
来源：http://hz.yj20258888.top/gtuuntqfyd.html

Py:   int("42"); float("3.14")
来源：http://hz.dianchejie.cn/gtzjnrfcsr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cqqwz.cn/gtknvhbbnw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.quarkkingdee.top/gtzhtfnfox.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhengqikj.top/gtwvaqhzxw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuxming.cn/gtfrhqckra.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pycfn.com/gtpumptqxl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ywan-chungtsiang.top/gtfbyrynem.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.kuanghao11.cn/gtmyhpjvvg.html

[A07] 数字转字符串
来源：http://hz.guannengcc.top/gtonibriad.html

Py:   str(42)
来源：http://hz.jqgufenzy.top/gtouwvfbex.html

PHP:  (string) 42; strval(42)
来源：http://hz.fengsongda.top/gtmlkccsbi.html

JS:   String(42); (42).toString()
来源：http://hz.daria6918.cn/gtsxfsfhzq.html

TS:   String(42)
来源：http://hz.dianchejie.cn/gtupesrcpm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.daria6918.cn/gtgvlayjyt.html

Go:   strconv.Itoa(42)
来源：http://hz.xuanzx.com/gtlrtpnrjv.html

Ruby: 42.to_s
来源：http://hz.yonumen.top/gtljojjwkd.html

C#:   42.ToString()
来源：http://hz.nanxuanxn.top/gtgxlecjgv.html

[A08] 取整与四舍五入
来源：http://hz.sxryk.cn/gtmfzcvadd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.sxryk.cn/gtgqelqhrr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.iojbl.cn/gtiazaktby.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.wangshuangyany.cn/gtngcysmaj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yangfankeji.com/gtxrmkddae.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.pycfn.com/gtnvplntiv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.wangdashe.top/gtgrdfbtuk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.guowangkeji.top/gtrscsazxm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.0kj1m.cn/gthoyuxksx.html

[A09] 绝对值与最大最小值
来源：http://hz.xuetiantiany.cn/gtdrfhqnyr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.9152youxi.cn/gtlrjkjpcf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhoulong.xyz/gtkphsaers.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jinqigufen.top/gtqojocfbs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ydzc1.top/gtyjwcacha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenzaomai.com/gtwtljqysq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinghuilouyu.cn/gtipcevnzh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ehwqpu.com/gtmlxiybnd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yueranfly.top/gtzotomcza.html

[A10] 生成随机数
来源：http://hz.nanxinkj.top/gtxqwftkgy.html

Py:   import random; random.randint(1, 100)
来源：http://hz.chenzaomai.com/gtevopfwyr.html

PHP:  random_int(1, 100);
来源：http://hz.ppjwa.cn/gthvlssjxm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daxiang520.top/gtvgipzjxt.html


<!-- 参考信息 -->