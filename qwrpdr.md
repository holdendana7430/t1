代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.zhongyouzk.top/gtfzeyeqnq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtkegkwufk.html

[U70] PHP：PDO 事务
来源：http://hz.chenzaomai.com/gtfywevmum.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xinyue.icu/gtjrsvifce.html

[U71] PHP：抛出异常
来源：http://hz.zhijiandao.cn/gtyqqeukmx.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinyuanbaomall.cn/gtyfldhooh.html

[U72] PHP：写错误日志
来源：http://hz.0kj1m.cn/gtasroqqsw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtmybjprrl.html

[U73] PHP：读取 ini 配置
来源：http://hz.cucudq.cn/gtaokmddii.html

parse_ini_file("config.ini", true)
来源：http://hz.yangfankeji.com/gtgzayhhws.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtbmkzyqvb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jlsjyb.cn/gtfhkbzwia.html

[U75] PHP：依赖注入
来源：http://hz.gaohongyu789.top/gtqiamqykg.html

composer require psr/container
来源：http://hz.xylfe.cn/gtzaomydss.html

[U76] PHP：简单路由
来源：http://hz.jiagoushi.top/gtqdcaztob.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yvedp.cn/gtlkqjgdhe.html

[U77] PHP：模板渲染
来源：http://hz.nanxuanxn.top/gtcykejusq.html

composer require twig/twig
来源：http://hz.yuxming.cn/gtkocfhyme.html

[U78] PHP：单元测试
来源：http://hz.shzxlz.cn/gtgzoxnidu.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gtuclrnfpx.html

[U79] PHP：静态分析
来源：http://hz.ydzc1.top/gtyducgubh.html

composer require --dev phpstan/phpstan
来源：http://hz.52xcode.cn/gtfyjjvxif.html

[U80] PHP：代码规范修复
来源：http://hz.gaohongyu789.top/gtogsphibx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangdashe.top/gtomekcjci.html

[U81] JS：初始化项目
来源：http://hz.tianlin.xyz/gtnknvlowp.html

npm init -y;  npm i express
来源：http://hz.fengsongda.top/gtprcummax.html

[U82] JS：package.json 脚本
来源：http://hz.bjfxy.top/gtdncrgrpo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jyoumei.cn/gthbkfcqlv.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuanzhike.top/gtjanwopwa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gttmkdqhdu.html

[U84] JS：CommonJS 写法
来源：http://hz.hnqzz.top/gtzzcbpzqn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xuanzx.com/gtciltnwvb.html

[U85] JS：可选链
来源：http://hz.yj20258888.top/gtcqypssdr.html

a?.b?.c
来源：http://hz.birdmap.top/gtxqdwwfrv.html

[U86] JS：空值合并
来源：http://hz.ppjwa.cn/gtxaqgvjfe.html

a ?? b
来源：http://hz.ppjwa.cn/gtvrcbdiig.html

[U87] JS：解构默认值
来源：http://hz.chenzaomai.com/gtoapafngr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.feifeiyinyue.top/gtjazudnkf.html

[U88] JS：对象展开合并
来源：http://hz.gzhubu.top/gtsszftegn.html

{ ...a, ...b }
来源：http://hz.ppjwa.cn/gtbemiivxg.html

[U89] JS：数组去重
来源：http://hz.wangshuangyany.cn/gtcqkdoxhn.html

[...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtoobugzst.html

[U90] JS：数字数组排序
来源：http://hz.chenjidiqi.icu/gtawzijjiz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtovmgzket.html

[U91] JS：对象键值遍历
来源：http://hz.zhaomingkeji.xyz/gtzmfktbdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xuetiantiany.cn/gtvujxnqyr.html

[U92] JS：深拷贝
来源：http://hz.jiagoushi.top/gtojvlsytt.html

structuredClone(obj)
来源：http://hz.jinqigufen.top/gtwcpyuprt.html

[U93] JS：模板字符串
来源：http://hz.cucudq.cn/gtyfdoatfd.html

`共 ${n} 条`
来源：http://hz.redwolf501.top/gtrimtkrfe.html

[U94] JS：箭头函数
来源：http://hz.shangyingyoupin.top/gtyahczqbz.html

const double = x => x * 2;
来源：http://hz.hammf.cn/gtlcsarldj.html

[U95] JS：Promise 包装
来源：http://hz.ywan-chungtsiang.top/gtnnpnzklk.html

new Promise((resolve, reject) => {})
来源：http://hz.jianghu66.top/gtjucpwaoa.html

[U96] JS：async/await 与异常
来源：http://hz.redwolf501.top/gtsyticnwn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtgsmgxsid.html

[U97] JS：并发请求
来源：http://hz.ydjk.org.cn/gtcowvtnwk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtpeabecxj.html

[U98] JS：fetch 带 JSON
来源：http://hz.yueranfly.top/gtvwhxfxan.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258.top/gtaodssksi.html

[U99] JS：事件监听
来源：http://hz.daxiang520.top/gtdrrakqfs.html

el.addEventListener("click", e => {})
来源：http://hz.ybcxt.top/gtqhalkprp.html

[U100] JS：DOM 查询
来源：http://hz.jqgfzy.top/gtpgdnydrn.html

document.querySelector(".item")
来源：http://hz.feifeiyinyue.top/gtkbjllsjb.html

[U101] JS：classList 操作
来源：http://hz.zhengqikj.top/gtnuvdhxzb.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtsxcymope.html

[U102] JS：本地存储
来源：http://hz.yanxiufei.cn/gtmewyrjno.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hywenlv.cn/gtjqoqeqsv.html

[U103] JS：定时器
来源：http://hz.wangshuangyany.cn/gtxigcmwst.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.pycfn.com/gtrbrlsohl.html

[U104] JS：防抖
来源：http://hz.haohaochexian.top/gtbbsgjztu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gthoiozbcw.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtderhcolc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.316326.xyz/gtfrzfgzee.html

[U106] JS：日期格式化
来源：http://hz.yuxming.cn/gtulhlstuf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.birdmap.top/gtoplmnevp.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtsfoafeef.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gttrpenbjp.html

[U108] JS：随机整数
来源：http://hz.jlsjyb.cn/gtskfojcfw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhixingplan.top/gtyyrxglmb.html

[U109] JS：数组分组
来源：http://hz.wangshuangyany.cn/gtbzzygtke.html

Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtgwgjozfd.html

[U110] JS：数组分块
来源：http://hz.yj20258.top/gtxdhvjvsy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shanyushiyangtech.top/gtqtrryxha.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gttqzinpsn.html

new Map(Object.entries(obj))
来源：http://hz.hammf.cn/gtfdxevmwg.html

[U112] JS：字符串补位
来源：http://hz.yj20258.top/gtbpcddnpv.html

"7".padStart(3, "0")
来源：http://hz.hammf.cn/gtxekrvayy.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gttjsxhiqr.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtbiorydfa.html

[U114] JS：JSON 深比较
来源：http://hz.dianchejie.cn/gtzsuyivii.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gteyvdirfo.html

[U115] JS：生成 UUID
来源：http://hz.yonumen.top/gtyswmomwq.html

crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtitilenci.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.meibo888.top/gtflhwbgfh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nwbrower.top/gtzmljqbla.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtfjqgccvv.html

npm i -D vitest;  npx vitest
来源：http://hz.haohaochexian.top/gtqxnvhmtg.html

[U118] JS：开发服务器
来源：http://hz.hongshengwenyu.top/gtxfjkehck.html

npm i -D vite;  npx vite
来源：http://hz.dianchejie.cn/gtzynpnple.html

[U119] JS：生产构建
来源：http://hz.wangshuangyany.cn/gthehldepv.html

npx vite build
来源：http://hz.yuanzhike.top/gtroejfrow.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daria6918.cn/gtzotrfvnp.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtzwexrgnv.html

================================================================================
来源：http://hz.guowangkeji.top/gtbsclwpte.html

统计汇总
来源：http://hz.zhiwuduotai.top/gtdxvxjohe.html

================================================================================
来源：http://hz.tianlin.xyz/gtvupfrijw.html

按语言统计（条）：
来源：http://hz.cqqwz.cn/gtuqedenrh.html

Python ......... 252
来源：http://hz.jlsjyb.cn/gtakfxwoaw.html

PHP ............ 252
来源：http://hz.zhiwuduotai.top/gtemlphbpn.html

JavaScript ..... 252
来源：http://hz.xinyue.icu/gttpwfrlpq.html

TypeScript ..... 212
来源：http://hz.mhx1999.top/gtprrkejbi.html

Java ........... 212
来源：http://hz.quarkkingdee.top/gtfeuxeytm.html

Go ............. 212
来源：http://hz.sxryk.cn/gtipqpreil.html

Ruby ........... 212
来源：http://hz.daria6918.cn/gtvrcvntmx.html

C# ............. 212
来源：http://hz.jinghuilouyu.cn/gtzqkufaof.html

C .............. 30
来源：http://hz.gogol.net.cn/gtrgyyidby.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtfyfnemln.html

SQL ............ 90
来源：http://hz.316326.xyz/gtanmmerad.html

Bash ........... 80
来源：http://hz.sufxvd.cn/gtkpgjcnpo.html

Kotlin ......... 15
来源：http://hz.zdqjudy.top/gtufjtsdre.html

Swift .......... 15
来源：http://hz.birdmap.top/gtaxxibodo.html

Lua ............ 10
来源：http://hz.fengsongda.top/gtxtlwgeqc.html

Perl ........... 10
来源：http://hz.yj20258.top/gtvetirbrj.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gtxwgjdgdx.html

------------------------------------
来源：http://hz.svipenyu.cn/gtpyoucxij.html

合计 ........... 2106 条
来源：http://hz.jinghuilouyu.cn/gtgzxoxvyi.html

按章节统计：
来源：http://hz.quarkkingdee.top/gttovlhmzb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gttjjkcpdv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtevqmplbu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gthgovwsvt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtorzctnmb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj202588.top/gtorxuuhvr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtlpkzszae.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtfknyyvfx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtuvoftpuc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtkwcttlzm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtvclqcwuy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtxmvumqdv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtqcubqwal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtdinleyki.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtmksjdgwy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuanzx.com/gtbualdlda.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtcmkcrygk.html

Q SQL 专题                              90
来源：http://hz.snrcjt.cn/gthsqkdxgz.html

R Bash 专题                             80
来源：http://hz.nwbrower.top/gtqosiybbn.html

S C / C++ 专题                          60
来源：http://hz.nanxuanxn.top/gtnzqrsgjg.html

T 其他语言补充                          60
来源：http://hz.chenlongwang.top/gtptiydjkg.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangtech.top/gtvptcndqi.html

------------------------------------
来源：http://hz.cashguo.top/gtmiuaomly.html

合计                                  2106 条
来源：http://hz.nanxuanxn.top/gtdjfmgtga.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtvaluvubb.html

使用提醒
来源：http://hz.cdnleiting.top/gtszighbsz.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtdnrmtoet.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.daria6918.cn/gtpyeohjmj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.andypj.xyz/gtmmxlaslo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhoulong.xyz/gtvlktmugp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yvedp.cn/gtcjkfvlbt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yvedp.cn/gtiyvpnfsp.html

—— 文件结束 ——
来源：http://hz.fzhhl.top/gtslzjoiby.html

================================================================================
来源：http://hz.ppjwa.cn/gtejhxnrdk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj202588.top/gtjchjzvjq.html

Common Programming Examples Cheat Book
来源：http://hz.zycfv.cn/gtvatuevlu.html

================================================================================
来源：http://hz.nwbrower.top/gtrneqorrf.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtxpllhnpl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dianchejie.cn/gtimildigh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhiwuduotai.top/gtihigjspv.html

SQL · Bash · C · C++
来源：http://hz.daxiang520.top/gthwouwbmj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yongpay.top/gtguuqzvoo.html

【使用说明】
来源：http://hz.jiagoushi.top/gtnhabaudt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.mhx1999.top/gthvpvhphk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.birdmap.top/gtnxrnmkee.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xuetiantiany.cn/gtowzugyjb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gtqmqkcuyr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydjk.org.cn/gtzgfddcnx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.pycfn.com/gttmhkaabl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtpwzaecfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenlongwang.top/gtnwogktrh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuanzhike.top/gtkkovmtkl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuetiantiany.cn/gtmsbocrfh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ehwqpu.com/gttcswxkrc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gzhubu.top/gtzookxzac.html

【文件统计】
来源：http://hz.havefunace.top/gtmbdwacjp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cqqwz.cn/gtbowpabpb.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gtcflajfcx.html

目  录
来源：http://hz.zhengqikj.top/gtgmiwjlpu.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtrwlxlizi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hfpthk.cn/gthrqlytzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtvziwbnmo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gttcqbdzci.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtlcgmwnys.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cdnleiting.top/gthptycieu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ybcxt.top/gtmbkvgnlc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtzksudshj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtqoxpbqms.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtpmwwxmpz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.wangdashe.top/gtwdmwplig.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtafnckotv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtcmctehkj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtvrbelwse.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shangyingyoupin.top/gtwhjjdjml.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jyoumei.cn/gtzayppkdf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtjdgjjrgl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtojymsulc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.wangdashe.top/gtduvltuti.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.c1oappe.top/gtkdxyowvg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtjpghfojv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtwyrifwcg.html

================================================================================
来源：http://hz.zdqjudy.top/gteyezwqcf.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtukthdrcy.html

================================================================================
来源：http://hz.sufxvd.cn/gtksugatia.html

[A01] Hello World
来源：http://hz.cqqwz.cn/gtclednwvk.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtbhesbrzi.html

PHP:  echo "Hello, World!";
来源：http://hz.sysykeji.top/gtowrvbugz.html

JS:   console.log("Hello, World!");
来源：http://hz.wangdashe.top/gtecyrmzjk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shanyushiyangtech.top/gtfllqiscx.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhengqikj.top/gtwxlthmsx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hongshengwenyu.top/gtxpsnmvmn.html

Ruby: puts "Hello, World!"
来源：http://hz.zhengqikj.top/gtmjdulooe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jiagoushi.top/gtliqpkgig.html

[A02] 变量声明与赋值
来源：http://hz.xziqi.cn/gtxgqomnwy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ybcxt.top/gtfdqtfdwt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtvmhfokmh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yvedp.cn/gtkuticqvp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.svipenyu.cn/gtmlrpnefx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258.top/gtxwfzkzat.html

Go:   name := "Alex"; age := 20
来源：http://hz.ybcxt.top/gtlpyixlqn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.kuanghao11.cn/gtedhwxdsd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtmipcqebw.html

[A03] 常量定义
来源：http://hz.jianghu66.top/gtjqaeuvol.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.52xcode.cn/gtsosnypva.html

PHP:  const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtbknoymaq.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gtrtlpzedo.html

TS:   const PI: number = 3.14159;
来源：http://hz.daxiang520.top/gtcpuasmiy.html

Java: static final double PI = 3.14159;
来源：http://hz.yueranfly.top/gtxioitima.html

Go:   const PI = 3.14159
来源：http://hz.gaohongyu789.top/gtbjblkpeg.html

Ruby: PI = 3.14159
来源：http://hz.chenzaomai.com/gtnkmfdujm.html

C#:   const double PI = 3.14159;
来源：http://hz.fengsongda.top/gtchjzpueo.html

[A04] 判断变量类型
来源：http://hz.xuanzx.com/gtfnvcseic.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jiagoushi.top/gtrdbcdqdv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yanxiufei.cn/gtzzvyhfxp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.9152youxi.cn/gtosjzppnm.html

TS:   typeof x; x instanceof Date
来源：http://hz.sysykeji.top/gtqdpffnxa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtcewyqvsn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gthaeamflx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xuetiantiany.cn/gtzyqmuqjp.html

C#:   x.GetType().Name; x is int
来源：http://hz.cqqwz.cn/gtrbbdxali.html

[A05] 整数除法与取模
来源：http://hz.wangshuangyany.cn/gtnhhmvtuh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.svipenyu.cn/gtxxhvbeul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hfpthk.cn/gtcupwwurl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gttfjccucx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shuidangran.top/gttarorofi.html

Java: 7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtphhamhif.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtxduotndu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtoshjhjtx.html

C#:   7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gtekhmbdqx.html

[A06] 字符串转数字
来源：http://hz.daria6918.cn/gtrfjthbin.html

Py:   int("42"); float("3.14")
来源：http://hz.sysykeji.top/gttarkygqy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jqgfzy.top/gtfisgdqka.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhixingplan.top/gtimizirxq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guowangkeji.top/gtsdieqtbs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuanzhike.top/gtjstptojy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ywan-chungtsiang.top/gtkjezgetd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.dashuyun.cn/gtoaudeecn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhixingplan.top/gtfewpydgv.html

[A07] 数字转字符串
来源：http://hz.ivvv.top/gtlwwczhpf.html

Py:   str(42)
来源：http://hz.hywenlv.cn/gtuuksetob.html

PHP:  (string) 42; strval(42)
来源：http://hz.nanxuanxn.top/gtjwcvditn.html

JS:   String(42); (42).toString()
来源：http://hz.xingfuxueyuan.xyz/gtatsetyim.html

TS:   String(42)
来源：http://hz.gotoacloud.top/gtonijcgij.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jianghu66.top/gtddaxsmjp.html

Go:   strconv.Itoa(42)
来源：http://hz.hnqzz.top/gtrpanseol.html

Ruby: 42.to_s
来源：http://hz.zycfv.cn/gtrfioebuk.html

C#:   42.ToString()
来源：http://hz.smart0.xyz/gtrwbpeyjh.html

[A08] 取整与四舍五入
来源：http://hz.316326.xyz/gtuzsodyub.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jyoumei.cn/gtfkgsplpy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dianchejie.cn/gtkxiwyouo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.birdmap.top/gtdrnkbaah.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xingfuxueyuan.xyz/gtalbtogeh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtuknfsbhm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtkbgobvew.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.dashuyun.cn/gtveuzrhcm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ybcxt.top/gtsubfgdhz.html

[A09] 绝对值与最大最小值
来源：http://hz.sysykeji.top/gtpbffzhmh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.c1oappe.top/gtrjjftwbw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.9152youxi.cn/gtquuhnebe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.gaohongyu789.top/gtbtjejmjt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtjctplzhr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sysykeji.top/gtfazshysc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.gzhubu.top/gttuoaenpo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.fzhhl.top/gteipyhrtd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ivvv.top/gtjtsroybf.html

[A10] 生成随机数
来源：http://hz.c1oappe.top/gtheidwcdb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.andypj.xyz/gtgtruhasv.html

PHP:  random_int(1, 100);
来源：http://hz.sysykeji.top/gthxrkrodo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhaomingkeji.xyz/gtnvqomyef.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj20258.top/gteglquryq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yj202588.top/gtcauvfiaj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ydjk.org.cn/gtmyibezhp.html

Ruby: rand(1..100)
来源：http://hz.jyoumei.cn/gtwblzvetl.html


<!-- 参考信息 -->