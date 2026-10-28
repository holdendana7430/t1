代发 wailian999

[U63] PHP：文件读写
来源：http://hz.wangshuangyany.cn/gtclmpwlim.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gturliqvyw.html

[U64] PHP：目录遍历
来源：http://hz.jinghuilouyu.cn/gtviomxfps.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgufenzy.top/gtqpdpmwiy.html

[U65] PHP：会话
来源：http://hz.yonumen.top/gtupzadlyi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xuanzx.com/gtcemwwmtq.html

[U66] PHP：设置 Cookie
来源：http://hz.cdnleiting.top/gtikpvbphz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinyuanbaomall.cn/gtkfstszvp.html

[U67] PHP：处理文件上传
来源：http://hz.gaohongyu789.top/gtuqirbmws.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hongshengwenyu.top/gtteeihzsk.html

[U68] PHP：PDO 连接
来源：http://hz.sxryk.cn/gtorxmckjr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydjk.org.cn/gtntmdcfop.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtlttxevgg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sxryk.cn/gtbzmwscby.html

[U70] PHP：PDO 事务
来源：http://hz.zhixingplan.top/gtfxfbucfr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yangfankeji.com/gtmghyhxjd.html

[U71] PHP：抛出异常
来源：http://hz.sweek.top/gtocmnuyji.html

throw new RuntimeException("失败", 500);
来源：http://hz.smart0.xyz/gtijikryrf.html

[U72] PHP：写错误日志
来源：http://hz.zdqjudy.top/gtteghojxp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.dianchejie.cn/gtgyyaxleo.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtresxdiqg.html

parse_ini_file("config.ini", true)
来源：http://hz.yonumen.top/gtzmothqer.html

[U74] PHP：读取环境变量
来源：http://hz.xuetiantiany.cn/gtvomslval.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gthtedumwj.html

[U75] PHP：依赖注入
来源：http://hz.jiagoushi.top/gtnlldatzq.html

composer require psr/container
来源：http://hz.ydjk.org.cn/gtxthjiqrr.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtxlboameq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtatizbdjw.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gtilgaxoea.html

composer require twig/twig
来源：http://hz.havefunace.top/gterrrhnks.html

[U78] PHP：单元测试
来源：http://hz.ywan-chungtsiang.top/gtexnubepx.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gtujfmxoxi.html

[U79] PHP：静态分析
来源：http://hz.zhiwuduotai.top/gtuuupiifk.html

composer require --dev phpstan/phpstan
来源：http://hz.vqdsnc.cn/gtceezupeq.html

[U80] PHP：代码规范修复
来源：http://hz.hysaishi.cn/gtuairgbef.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtkxiqsufq.html

[U81] JS：初始化项目
来源：http://hz.gaohongyu789.top/gtxvebkwxe.html

npm init -y;  npm i express
来源：http://hz.fengsongda.top/gtonawqlcg.html

[U82] JS：package.json 脚本
来源：http://hz.pengpengdd.cyou/gthezvwvkx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnxiangtu.top/gtzunakcrr.html

[U83] JS：ES Module 导入导出
来源：http://hz.sufxvd.cn/gtftxzboum.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jianghu66.top/gthsaitvod.html

[U84] JS：CommonJS 写法
来源：http://hz.316326.xyz/gtxnmzlixq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hysaishi.cn/gtgstnhhuo.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtahtskzun.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtlnkruyal.html

[U86] JS：空值合并
来源：http://hz.aizwys.cn/gthaeuqzik.html

a ?? b
来源：http://hz.jinghuilouyu.cn/gtlflosqye.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gtteccrgqq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hywenlv.cn/gtujwyfzlp.html

[U88] JS：对象展开合并
来源：http://hz.mhx1999.top/gtrwtjhvaa.html

{ ...a, ...b }
来源：http://hz.daria6918.cn/gtinzklliu.html

[U89] JS：数组去重
来源：http://hz.fengsongda.top/gtsdxhiqxs.html

[...new Set(arr)]
来源：http://hz.ppjwa.cn/gtabtzcmtf.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangtech.top/gtbyhepian.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gteqiqnjfi.html

[U91] JS：对象键值遍历
来源：http://hz.haohaochexian.top/gtnhnujohb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.kuanghao11.cn/gtmrvzzkdg.html

[U92] JS：深拷贝
来源：http://hz.jlsjyb.cn/gtfjmpyngl.html

structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtyhcwwcag.html

[U93] JS：模板字符串
来源：http://hz.hywenlv.cn/gtyswyosfc.html

`共 ${n} 条`
来源：http://hz.xuetiantiany.cn/gtucgemwhg.html

[U94] JS：箭头函数
来源：http://hz.guannengcc.top/gtuchwnsca.html

const double = x => x * 2;
来源：http://hz.hnxiangtu.top/gtncaqriht.html

[U95] JS：Promise 包装
来源：http://hz.hammf.cn/gtilxbbhbe.html

new Promise((resolve, reject) => {})
来源：http://hz.quarkkingdee.top/gtfzgdwbqu.html

[U96] JS：async/await 与异常
来源：http://hz.yanxiufei.cn/gthnxplrlo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtsxmhyrgn.html

[U97] JS：并发请求
来源：http://hz.kuanghao11.cn/gtxbiwhctr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtinsocabh.html

[U98] JS：fetch 带 JSON
来源：http://hz.dianchejie.cn/gtbjbpleti.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.kuanghao11.cn/gtxawqtbft.html

[U99] JS：事件监听
来源：http://hz.tianlin.xyz/gtrrohbply.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtnmvwtzzi.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtrdnbawpv.html

document.querySelector(".item")
来源：http://hz.xziqi.cn/gtdfztbxme.html

[U101] JS：classList 操作
来源：http://hz.fengsongda.top/gtzcounbzy.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtmcrzjteu.html

[U102] JS：本地存储
来源：http://hz.pycfn.com/gtgwrsosvj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jyoumei.cn/gtyrqrbilz.html

[U103] JS：定时器
来源：http://hz.hammf.cn/gtnkjrzjve.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yonumen.top/gtroxpmucy.html

[U104] JS：防抖
来源：http://hz.hysaishi.cn/gtvrjsyczj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtwfxoezpw.html

[U105] JS：节流
来源：http://hz.gzhubu.top/gthxjnqrid.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xingfuxueyuan.xyz/gtskakugne.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtdylfpuji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtbryplsqq.html

[U107] JS：数字千分位
来源：http://hz.ivvv.top/gtoezvdpla.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yongpay.top/gteeijcimq.html

[U108] JS：随机整数
来源：http://hz.fzhhl.top/gthozslccq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.haohaochexian.top/gtxvroqomx.html

[U109] JS：数组分组
来源：http://hz.quarkkingdee.top/gtidcncaow.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtllgrnvtp.html

[U110] JS：数组分块
来源：http://hz.svipenyu.cn/gtrizknlbl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hywenlv.cn/gtqkegqxiz.html

[U111] JS：对象转 Map
来源：http://hz.tanke756.top/gtfjiqvjfo.html

new Map(Object.entries(obj))
来源：http://hz.gotoacloud.top/gtbuoowhjf.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtcdzetaru.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtoccplyyl.html

[U113] JS：正则替换全部
来源：http://hz.ydjk.org.cn/gtbjjevzjk.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gttkiambve.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtfwalwbsr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gteobbjocf.html

[U115] JS：生成 UUID
来源：http://hz.yvedp.cn/gtnzclddru.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtjhvwdghy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cdnleiting.top/gtgjuifvci.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yangfankeji.com/gtjqwkemmn.html

[U117] JS：单元测试
来源：http://hz.svipenyu.cn/gtofvfkzin.html

npm i -D vitest;  npx vitest
来源：http://hz.shangyingyoupin.top/gtnyefwldp.html

[U118] JS：开发服务器
来源：http://hz.guannengcc.top/gtvepgoidj.html

npm i -D vite;  npx vite
来源：http://hz.quarkkingdee.top/gtrdgabspt.html

[U119] JS：生产构建
来源：http://hz.yueranfly.top/gtlslbqlpv.html

npx vite build
来源：http://hz.shzxlz.cn/gtlrehlbee.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.52xcode.cn/gtpnllvczv.html

import.meta.env.VITE_API_URL
来源：http://hz.hnqzz.top/gtwunjphcz.html

================================================================================
来源：http://hz.hammf.cn/gtijbaapxy.html

统计汇总
来源：http://hz.pycfn.com/gtksdmmmkx.html

================================================================================
来源：http://hz.sufxvd.cn/gtetvneifx.html

按语言统计（条）：
来源：http://hz.yueranfly.top/gtxeguuykq.html

Python ......... 252
来源：http://hz.shuidangran.top/gtmlussaic.html

PHP ............ 252
来源：http://hz.hysaishi.cn/gtexmqlrla.html

JavaScript ..... 252
来源：http://hz.sxryk.cn/gtvrsnwqyv.html

TypeScript ..... 212
来源：http://hz.iojbl.cn/gtmtfgzqix.html

Java ........... 212
来源：http://hz.gotoacloud.top/gtrstdotli.html

Go ............. 212
来源：http://hz.cdnleiting.top/gtvyhyttcp.html

Ruby ........... 212
来源：http://hz.sweek.top/gtzojqfqik.html

C# ............. 212
来源：http://hz.mhx1999.top/gtnxwjditp.html

C .............. 30
来源：http://hz.hfpthk.cn/gtrnktfioh.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtdpewkfft.html

SQL ............ 90
来源：http://hz.pycfn.com/gtvguyneto.html

Bash ........... 80
来源：http://hz.hongshengwenyu.top/gtrbuhqmbk.html

Kotlin ......... 15
来源：http://hz.xylfe.cn/gteuezwlbb.html

Swift .......... 15
来源：http://hz.dianchejie.cn/gtvahiieve.html

Lua ............ 10
来源：http://hz.wangshuangyany.cn/gtckkzgpif.html

Perl ........... 10
来源：http://hz.yj202588.top/gtmhlanebv.html

Scala .......... 10
来源：http://hz.ydjk.org.cn/gtvuadcnke.html

------------------------------------
来源：http://hz.gogol.net.cn/gtjbdswrnm.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gtmqyqarwy.html

按章节统计：
来源：http://hz.andypj.xyz/gttqfxveuq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtstcbjfvt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtemidjnbu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gotoacloud.top/gtmgcafrqe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtxubzdbve.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xingfuxueyuan.xyz/gtcbszrloa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtjgdeghzq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtanrjdskt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtyqhjjwmy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtlrojbxiy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jqgufenzy.top/gtlqkfodda.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtgpqklfie.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtdvdhsdbr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtxdnwvvdz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtxneifews.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258888.top/gtrpbkvhyg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtczfozozg.html

Q SQL 专题                              90
来源：http://hz.xinyue.icu/gtojysqlgm.html

R Bash 专题                             80
来源：http://hz.sweek.top/gtbnlblzxe.html

S C / C++ 专题                          60
来源：http://hz.pycfn.com/gtbbsckmsx.html

T 其他语言补充                          60
来源：http://hz.havefunace.top/gtecxmjgsi.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gthfdbdzno.html

------------------------------------
来源：http://hz.0kj1m.cn/gtzsfumnjd.html

合计                                  2106 条
来源：http://hz.jiagoushi.top/gtfzxwintm.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtumzyqvqy.html

使用提醒
来源：http://hz.yj20258888.top/gtfjchkrqn.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtpuushket.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhongyouzk.top/gtzlnlawpr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangkeji.top/gtxpotipzy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.snrcjt.cn/gtaydnhxoz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sysykeji.top/gtqywoxmgm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.c1oappe.top/gtyblcacuh.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtckuyacjd.html

================================================================================
来源：http://hz.redwolf501.top/gtxrnoffxt.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yueranfly.top/gtmlgywrpq.html

Common Programming Examples Cheat Book
来源：http://hz.shanyushiyangkeji.top/gtpsyjccma.html

================================================================================
来源：http://hz.pycfn.com/gtkbsjepqh.html

【收录内容】
来源：http://hz.zhixingplan.top/gtrjwkamom.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtuslzniqo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shuidangran.top/gttpafgedl.html

SQL · Bash · C · C++
来源：http://hz.shanyushiyangkeji.top/gttzxvwtqq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.smart0.xyz/gtjxqkjhaw.html

【使用说明】
来源：http://hz.hysaishi.cn/gtpzzxbdke.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daxiang520.top/gtyynccnuo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgfzy.top/gthisopvya.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.fengsongda.top/gtemhifrrb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cashguo.top/gtmtehqprx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydzc1.top/gthtlvzozt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.0kj1m.cn/gtitqptavj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtkjjgiych.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.pycfn.com/gtgzrnktho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.andypj.xyz/gtblnoucim.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.iojbl.cn/gtwkxjeluj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tanke756.top/gtfqtipnbc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgufenzy.top/gtzhvkfwzj.html

【文件统计】
来源：http://hz.birdmap.top/gtgtjiuryf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gotoacloud.top/gtpprqikhy.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtsmvtgsqm.html

目  录
来源：http://hz.jlsjyb.cn/gtatqohaqu.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtqkgtwbud.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxinkj.top/gtctubhexf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aibaodan.cn/gtncsfazip.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtznxoawcp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtyhjozmnt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xinyue.icu/gtszniqbue.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.dianchejie.cn/gtfumcqkrk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtkomdlclr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sweek.top/gtnghmsmob.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtofmephvt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cqqwz.cn/gtorcvwlpd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtihvgvwjw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtzxrstrdm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtlisfzaqx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gteihezuch.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.redwolf501.top/gtewmckwgx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtsdtcijpc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gtkyjjaprf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cucudq.cn/gtvcdxrkeq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhengqikj.top/gtxwxhnyih.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtlloxtgab.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuanzx.com/gtdmoygwgj.html

================================================================================
来源：http://hz.havefunace.top/gthxmhtrlt.html

A. 基础语法与类型
来源：http://hz.c1oappe.top/gtkbpnsszh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqfbulzuv.html

[A01] Hello World
来源：http://hz.shangyingyoupin.top/gtooptbffv.html

Py:   print("Hello, World!")
来源：http://hz.ppjwa.cn/gtlcbznxam.html

PHP:  echo "Hello, World!";
来源：http://hz.zhoulong.xyz/gtdnxnjxyh.html

JS:   console.log("Hello, World!");
来源：http://hz.ivvv.top/gtlumebqql.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jyoumei.cn/gtmmspland.html

Java: System.out.println("Hello, World!");
来源：http://hz.fengsongda.top/gtonivaaln.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgfzy.top/gtigkfeaqk.html

Ruby: puts "Hello, World!"
来源：http://hz.tian-w.cn/gtudcbsmpx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shuidangran.top/gtbqulvilg.html

[A02] 变量声明与赋值
来源：http://hz.cheryme.top/gtvupgozts.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xingfuxueyuan.xyz/gtvbvyrgus.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.cucudq.cn/gthibgypbu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangkeji.top/gtjtqipcms.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sufxvd.cn/gtquxsvibq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shzxlz.cn/gttvnqxiaz.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangdashe.top/gtsuvpotka.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xylfe.cn/gtyydahrnd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtuyqzlofi.html

[A03] 常量定义
来源：http://hz.shanyushiyangtech.top/gtgdmsfuzg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zdqjudy.top/gtlrckcari.html

PHP:  const PI = 3.14159;
来源：http://hz.shuidangran.top/gtwrbykvwq.html

JS:   const PI = 3.14159;
来源：http://hz.nwbrower.top/gtpocuzjwb.html

TS:   const PI: number = 3.14159;
来源：http://hz.sufxvd.cn/gtjdnipdhr.html

Java: static final double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtiefnjdfj.html

Go:   const PI = 3.14159
来源：http://hz.zhengqikj.top/gtdmgjfldt.html

Ruby: PI = 3.14159
来源：http://hz.ybcxt.top/gtsakaxllm.html

C#:   const double PI = 3.14159;
来源：http://hz.cashguo.top/gtxpuekgkq.html

[A04] 判断变量类型
来源：http://hz.jinghuilouyu.cn/gtdtsnjbpt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxuanxn.top/gtvfjjtuuf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtyrwukvdd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jqgufenzy.top/gtxiefczii.html

TS:   typeof x; x instanceof Date
来源：http://hz.redwolf501.top/gtzblsztxi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yuanzhike.top/gtixncvaji.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnxiangtu.top/gtgrgloyep.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.vqdsnc.cn/gttcfxjpmz.html

C#:   x.GetType().Name; x is int
来源：http://hz.ppjwa.cn/gteybvlzrp.html

[A05] 整数除法与取模
来源：http://hz.yonumen.top/gtozwchaxq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shuidangran.top/gtfwqwbhlp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtrlomlxlu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sxryk.cn/gtnwwhaeai.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtacmeoimq.html

Java: 7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gtomdaavwt.html

Go:   7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtxtrekfrx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtftgernur.html

C#:   7 / 2; 7 % 2
来源：http://hz.tanke756.top/gtksbyakzk.html

[A06] 字符串转数字
来源：http://hz.wangdashe.top/gtiuwmncjz.html

Py:   int("42"); float("3.14")
来源：http://hz.jinqigufen.top/gtvqtrasxu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.havefunace.top/gtozacyfcl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.redwolf501.top/gtkzumxozc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xinyue.icu/gtihrhjxnl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shangyingyoupin.top/gtdgjgvqzm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xingfuxueyuan.xyz/gtofoybzsi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shanyushiyangtech.top/gtqwnvztjo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigfzy.top/gtvdbukisp.html

[A07] 数字转字符串
来源：http://hz.yueranfly.top/gtdnjfhjzw.html

Py:   str(42)
来源：http://hz.xuanzx.com/gtfqjugwmy.html

PHP:  (string) 42; strval(42)
来源：http://hz.cheryme.top/gthqqfiqke.html

JS:   String(42); (42).toString()
来源：http://hz.zhijiandao.cn/gtapporofa.html

TS:   String(42)
来源：http://hz.sysykeji.top/gtzgegwkbb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yangfankeji.com/gteyqiyiol.html

Go:   strconv.Itoa(42)
来源：http://hz.smart0.xyz/gtphgjbqya.html

Ruby: 42.to_s
来源：http://hz.wangdashe.top/gttavknvfw.html

C#:   42.ToString()
来源：http://hz.cqqwz.cn/gtsmsotjph.html

[A08] 取整与四舍五入
来源：http://hz.c1oappe.top/gtittevheq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gthbzypudn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cucudq.cn/gtlbcimvfl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hammf.cn/gtwrojvamb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangtech.top/gtsztlzqlx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.aibaodan.cn/gtnqnlwakb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tianlin.xyz/gtpvmtlbrx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.fengsongda.top/gtiwalryhr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yangfankeji.com/gtpievgzts.html

[A09] 绝对值与最大最小值
来源：http://hz.zhoulong.xyz/gtwoopzgsv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gzhubu.top/gtubznuqks.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ppjwa.cn/gtlvmczqej.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yj20258.top/gtfvchmfqh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxinkj.top/gtkrnkerdl.html


<!-- 参考信息 -->