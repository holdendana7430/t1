代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.jiagoushi.top/gtruqpjlos.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuanzx.com/gtbikhgnjd.html

[U68] PHP：PDO 连接
来源：http://hz.chenzaomai.com/gtosodsidz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.52xcode.cn/gtwkqpbqmz.html

[U69] PHP：PDO 预处理
来源：http://hz.tanke756.top/gtcdakoapo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtwaxwpitp.html

[U70] PHP：PDO 事务
来源：http://hz.jianghu66.top/gtwjxoxmpk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tianlin.xyz/gtioyydttr.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gtuejzgocr.html

throw new RuntimeException("失败", 500);
来源：http://hz.sufxvd.cn/gtcajxmwgp.html

[U72] PHP：写错误日志
来源：http://hz.c1oappe.top/gtpowdiwwk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenjidiqi.icu/gtenumsinx.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtawzacgns.html

parse_ini_file("config.ini", true)
来源：http://hz.gaohongyu789.top/gtufceeywh.html

[U74] PHP：读取环境变量
来源：http://hz.yj20258.top/gtkwicsbty.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gtgpraxcko.html

[U75] PHP：依赖注入
来源：http://hz.dashuyun.cn/gtxoqfyinx.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gtecpzvduw.html

[U76] PHP：简单路由
来源：http://hz.iojbl.cn/gtlbvrhzhu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtscbzamhi.html

[U77] PHP：模板渲染
来源：http://hz.xingfuxueyuan.xyz/gtufwmpxqt.html

composer require twig/twig
来源：http://hz.jianghu66.top/gthcrgnpuw.html

[U78] PHP：单元测试
来源：http://hz.wangdashe.top/gtbaejnsfo.html

composer require --dev phpunit/phpunit
来源：http://hz.zhaomingkeji.xyz/gtzrwbrvff.html

[U79] PHP：静态分析
来源：http://hz.jinqigfzy.top/gtstevecgq.html

composer require --dev phpstan/phpstan
来源：http://hz.tian-w.cn/gtdwaglrxx.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gtyfitvicw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gtipuvnbwa.html

[U81] JS：初始化项目
来源：http://hz.xinyue.icu/gtbtdfvzod.html

npm init -y;  npm i express
来源：http://hz.yj20258888.top/gtwxdvzovu.html

[U82] JS：package.json 脚本
来源：http://hz.ywan-chungtsiang.top/gtafcfrgal.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shzxlz.cn/gtmmsblcxo.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gtqwerdmkb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.aibaodan.cn/gtwtgetzmu.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtqpbjkego.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.fengsongda.top/gthxeatmjk.html

[U85] JS：可选链
来源：http://hz.jiagoushi.top/gtbnmwaudm.html

a?.b?.c
来源：http://hz.chenzaomai.com/gtvrdgzsrv.html

[U86] JS：空值合并
来源：http://hz.hammf.cn/gtltqbmjtt.html

a ?? b
来源：http://hz.snrcjt.cn/gtewyrbynt.html

[U87] JS：解构默认值
来源：http://hz.jinqigfzy.top/gtastuvnen.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhengqikj.top/gtaptmblsg.html

[U88] JS：对象展开合并
来源：http://hz.quarkkingdee.top/gtwboqlgcz.html

{ ...a, ...b }
来源：http://hz.gaohongyu789.top/gteiqkftvc.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gtukkywxaq.html

[...new Set(arr)]
来源：http://hz.daxiang520.top/gtvchxjpji.html

[U90] JS：数字数组排序
来源：http://hz.birdmap.top/gtmgktlrnd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtalsqqhtr.html

[U91] JS：对象键值遍历
来源：http://hz.yueranfly.top/gttggvltwy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yanxiufei.cn/gtpmsutcwz.html

[U92] JS：深拷贝
来源：http://hz.xuanzx.com/gtyefgecnb.html

structuredClone(obj)
来源：http://hz.pycfn.com/gtrrelhzhx.html

[U93] JS：模板字符串
来源：http://hz.yongpay.top/gtihyozdvo.html

`共 ${n} 条`
来源：http://hz.jqgfzy.top/gtnegcmfiu.html

[U94] JS：箭头函数
来源：http://hz.jinghuilouyu.cn/gtvedevnop.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtcmjsayjd.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtxsxdpqrs.html

new Promise((resolve, reject) => {})
来源：http://hz.wangdashe.top/gtqwonbjxk.html

[U96] JS：async/await 与异常
来源：http://hz.pengpengdd.cyou/gtihwnkker.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtugzyfqbg.html

[U97] JS：并发请求
来源：http://hz.dianchejie.cn/gtvlplxxdg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtoctivyvi.html

[U98] JS：fetch 带 JSON
来源：http://hz.9152youxi.cn/gtirtwiuzf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yonumen.top/gtgwkgncap.html

[U99] JS：事件监听
来源：http://hz.xziqi.cn/gtnodmktjl.html

el.addEventListener("click", e => {})
来源：http://hz.sweek.top/gttzehsrlv.html

[U100] JS：DOM 查询
来源：http://hz.zhoulong.xyz/gterkliohz.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtrdjfonnk.html

[U101] JS：classList 操作
来源：http://hz.jinqigufen.top/gtcsvylkgp.html

el.classList.toggle("active")
来源：http://hz.ydjk.org.cn/gtvaqujjws.html

[U102] JS：本地存储
来源：http://hz.feifeiyinyue.top/gtljyvfcbr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jianghu66.top/gtaxmcvgyz.html

[U103] JS：定时器
来源：http://hz.zdqjudy.top/gtiongbbkx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gotoacloud.top/gtsvdbfwdt.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtrafxvgud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtqmetzwmy.html

[U105] JS：节流
来源：http://hz.zhijiandao.cn/gtrqltifnu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhengqikj.top/gtyjmfqibw.html

[U106] JS：日期格式化
来源：http://hz.bjfxy.top/gttxhybexi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gtqkwloqxc.html

[U107] JS：数字千分位
来源：http://hz.sufxvd.cn/gtjpiygmiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtmhbbntng.html

[U108] JS：随机整数
来源：http://hz.sufxvd.cn/gtumvhwbrd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cheryme.top/gtnuhbnzwj.html

[U109] JS：数组分组
来源：http://hz.hammf.cn/gteuntdglz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtupmsoiip.html

[U110] JS：数组分块
来源：http://hz.316326.xyz/gtqoxkjvbc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.0kj1m.cn/gthbvdbjiz.html

[U111] JS：对象转 Map
来源：http://hz.cqqwz.cn/gtjhjxccuo.html

new Map(Object.entries(obj))
来源：http://hz.aibaodan.cn/gtdixywdud.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gtwyrqobsh.html

"7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtnoqbiliq.html

[U113] JS：正则替换全部
来源：http://hz.nanxuanxn.top/gtdllbmozb.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtevkimwza.html

[U114] JS：JSON 深比较
来源：http://hz.zycfv.cn/gtevcxztny.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtknmwlztg.html

[U115] JS：生成 UUID
来源：http://hz.yj202588.top/gtqzoaeohx.html

crypto.randomUUID()
来源：http://hz.cheryme.top/gtqtdrjbzr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhijiandao.cn/gtkhvthnla.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnxiangtu.top/gtqxombqml.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtsnycavaz.html

npm i -D vitest;  npx vitest
来源：http://hz.zhaomingkeji.xyz/gtvkxsauin.html

[U118] JS：开发服务器
来源：http://hz.9152youxi.cn/gtxgynxjac.html

npm i -D vite;  npx vite
来源：http://hz.gaohongyu789.top/gtzmzduwtq.html

[U119] JS：生产构建
来源：http://hz.jianghu66.top/gtgakuyhqp.html

npx vite build
来源：http://hz.nanxuanxn.top/gtbblrpulo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.c1oappe.top/gtnwquwumo.html

import.meta.env.VITE_API_URL
来源：http://hz.yongpay.top/gtnaldtpfa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkbnmunyj.html

统计汇总
来源：http://hz.zycfv.cn/gtxaeoipfr.html

================================================================================
来源：http://hz.jqgfzy.top/gtrviweqtt.html

按语言统计（条）：
来源：http://hz.jqgfzy.top/gtksdgwbrf.html

Python ......... 252
来源：http://hz.shanyushiyangkeji.top/gtqysgszye.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gthtsaybwo.html

JavaScript ..... 252
来源：http://hz.aibaodan.cn/gtzysdtztn.html

TypeScript ..... 212
来源：http://hz.shzxlz.cn/gtkgonsoey.html

Java ........... 212
来源：http://hz.zhixingplan.top/gtpdbktsyp.html

Go ............. 212
来源：http://hz.yj20258.top/gtbraginvx.html

Ruby ........... 212
来源：http://hz.jlsjyb.cn/gtknpndrlc.html

C# ............. 212
来源：http://hz.yvedp.cn/gtuguxwgwc.html

C .............. 30
来源：http://hz.nwbrower.top/gtrodhbngf.html

C++ ............ 30
来源：http://hz.shanyushiyangkeji.top/gtadfbzdfe.html

SQL ............ 90
来源：http://hz.shzxlz.cn/gtizgocsow.html

Bash ........... 80
来源：http://hz.andypj.xyz/gtcnkwdaxy.html

Kotlin ......... 15
来源：http://hz.sysykeji.top/gtkzcjsvst.html

Swift .......... 15
来源：http://hz.cqqwz.cn/gtbuatqgfg.html

Lua ............ 10
来源：http://hz.cheryme.top/gtbatkxbkp.html

Perl ........... 10
来源：http://hz.shangyingyoupin.top/gtbteoifci.html

Scala .......... 10
来源：http://hz.zhaomingkeji.xyz/gtarytfcut.html

------------------------------------
来源：http://hz.yonumen.top/gtldkfyktt.html

合计 ........... 2106 条
来源：http://hz.gzhubu.top/gtxffgqmhz.html

按章节统计：
来源：http://hz.yj20258888.top/gtchxjmvpx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtqxrjplqq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtxdardrcr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtnncsrrdd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhixingplan.top/gtrrxqugip.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtfjuakwul.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gtbydzmrez.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtbtqkcofs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtjonnxisl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtswuwefvd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtirnymmvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtjgczowjx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtccueudkx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtciunrloj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtchpmowkx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shzxlz.cn/gtvqryxzzh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtukjqjtda.html

Q SQL 专题                              90
来源：http://hz.jiagoushi.top/gtxfoxcsti.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gtyoykptmk.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtbrdiehea.html

T 其他语言补充                          60
来源：http://hz.svipenyu.cn/gtotztpimr.html

U 高频实用片段                         120
来源：http://hz.fzhhl.top/gtlrtkgjxa.html

------------------------------------
来源：http://hz.xylfe.cn/gtvtcaqmyy.html

合计                                  2106 条
来源：http://hz.havefunace.top/gttexwlqpa.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtxuirywey.html

使用提醒
来源：http://hz.yuanzhike.top/gtozdlbrmk.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtmxokdlzw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhiwuduotai.top/gtstwvwkuq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ppjwa.cn/gtsvvjdhgh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.meibo888.top/gtnkhbssht.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.iojbl.cn/gttpwyxahf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sufxvd.cn/gtwwrjepfd.html

—— 文件结束 ——
来源：http://hz.guannengcc.top/gtzvozrztp.html

================================================================================
来源：http://hz.jiagoushi.top/gtreqyqpvt.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtnqkicpuj.html

Common Programming Examples Cheat Book
来源：http://hz.shuidangran.top/gtplboousi.html

================================================================================
来源：http://hz.zhijiandao.cn/gthxlconfd.html

【收录内容】
来源：http://hz.bjfxy.top/gtzgteomyo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhoulong.xyz/gthqkhoicw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenjidiqi.icu/gtldkkiwjk.html

SQL · Bash · C · C++
来源：http://hz.jqgufenzy.top/gtvhemdzak.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gtrghdjcps.html

【使用说明】
来源：http://hz.gotoacloud.top/gtsyllypzp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtygnqlnaw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258.top/gtgcdowutv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydjk.org.cn/gtnetryubk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtradffpyd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shzxlz.cn/gtnmlljlpy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yueranfly.top/gtwzknwqig.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pycfn.com/gtoeasnnzs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.quarkkingdee.top/gtxqbclhdq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnxiangtu.top/gtgveznuul.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yongpay.top/gttanaikja.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pengpengdd.cyou/gtdiomdzqs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgfzy.top/gtqgpdlwcy.html

【文件统计】
来源：http://hz.snrcjt.cn/gtxvvhyidu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ehwqpu.com/gtoscmcfbh.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtykpuqbpr.html

目  录
来源：http://hz.zhaomingkeji.xyz/gtktyiftbr.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtzftvdeex.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.redwolf501.top/gtuanejouf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtetitfcwg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtlnmqtzmu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gtgpylypxu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fengsongda.top/gtfgpylxfg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.quarkkingdee.top/gtjwegsibe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtiaxrbouy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gtjjolxdfw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtmrawevew.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtqcciyocv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtrzjfavoa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtyfrwifzz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtjgjmeibp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtykcbgsrg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.bjfxy.top/gtxvapmgtf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtoxjsfzaw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.guowangkeji.top/gtqfvwxmyy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhengqikj.top/gtdtvanryu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj202588.top/gtmogyxodx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtcqwecfll.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtselrwzip.html

================================================================================
来源：http://hz.svipenyu.cn/gtxreskipl.html

A. 基础语法与类型
来源：http://hz.yonumen.top/gtcnfbyqrx.html

================================================================================
来源：http://hz.cheryme.top/gtsjoofpum.html

[A01] Hello World
来源：http://hz.nwbrower.top/gtqshrwcsl.html

Py:   print("Hello, World!")
来源：http://hz.0kj1m.cn/gtbrqzpmbl.html

PHP:  echo "Hello, World!";
来源：http://hz.hongshengwenyu.top/gtvowdntnl.html

JS:   console.log("Hello, World!");
来源：http://hz.316326.xyz/gtqtxtwvkq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.meibo888.top/gtnoleyzbb.html

Java: System.out.println("Hello, World!");
来源：http://hz.hysaishi.cn/gtyqgwfqtm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gtpjdpldpr.html

Ruby: puts "Hello, World!"
来源：http://hz.zycfv.cn/gtysfcwqtu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.birdmap.top/gtgibystco.html

[A02] 变量声明与赋值
来源：http://hz.zdqjudy.top/gtadycwajy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.bjfxy.top/gtsgafrfel.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zycfv.cn/gtjynhxlcp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yonumen.top/gtuulxswat.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.9152youxi.cn/gtvgvhnsyg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cheryme.top/gtluudsojq.html

Go:   name := "Alex"; age := 20
来源：http://hz.tanke756.top/gtacmxjovh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.aizwys.cn/gtalybezrs.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtknovfhno.html

[A03] 常量定义
来源：http://hz.pengpengdd.cyou/gteofazgxd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.daxiang520.top/gtixnzawsm.html

PHP:  const PI = 3.14159;
来源：http://hz.hnqzz.top/gtvxcyqwxr.html

JS:   const PI = 3.14159;
来源：http://hz.gaohongyu789.top/gthpfmeplq.html

TS:   const PI: number = 3.14159;
来源：http://hz.yongpay.top/gtkykijtvj.html

Java: static final double PI = 3.14159;
来源：http://hz.mhx1999.top/gtshekeabz.html

Go:   const PI = 3.14159
来源：http://hz.yuanzhike.top/gtcqjsabqz.html

Ruby: PI = 3.14159
来源：http://hz.guannengcc.top/gtnowkrapw.html

C#:   const double PI = 3.14159;
来源：http://hz.yonumen.top/gtrkavtmpw.html

[A04] 判断变量类型
来源：http://hz.shzxlz.cn/gtzjfjrhgz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nwbrower.top/gthlyqunel.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xuanzx.com/gtrrdebjtt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xylfe.cn/gtiemdgtvi.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtdyqcvznf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.haohaochexian.top/gtgmgjofbe.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hfpthk.cn/gtwjkhnoip.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hnxiangtu.top/gtyfcmyqqb.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinghuilouyu.cn/gtmqtjhdmq.html

[A05] 整数除法与取模
来源：http://hz.nanxinkj.top/gtfvlesoyx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhaomingkeji.xyz/gtwkovvcdt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinqigufen.top/gtiibrsttu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtzttilige.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aibaodan.cn/gtdepbxfdc.html

Java: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtcgqvrhwf.html

Go:   7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtcqshygao.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.52xcode.cn/gtcrdkpipn.html

C#:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtandzusxc.html

[A06] 字符串转数字
来源：http://hz.birdmap.top/gtzqfczwye.html

Py:   int("42"); float("3.14")
来源：http://hz.ydzc1.top/gtsuogxdlw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yueranfly.top/gtpgvmvonp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aibaodan.cn/gtkwrstior.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.vqdsnc.cn/gtrpotfjoy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yangfankeji.com/gtiqckcnes.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gttxrfnyne.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xingfuxueyuan.xyz/gtngvfpuzo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtljisdtdf.html

[A07] 数字转字符串
来源：http://hz.fzhhl.top/gtswnrmgnj.html

Py:   str(42)
来源：http://hz.hysaishi.cn/gtgtblmbvz.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj202588.top/gtohpdaidl.html

JS:   String(42); (42).toString()
来源：http://hz.xinyue.icu/gtvjjixaui.html

TS:   String(42)
来源：http://hz.feifeiyinyue.top/gtbyyopbsa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tanke756.top/gtedlvxqix.html

Go:   strconv.Itoa(42)
来源：http://hz.jinyuanbaomall.cn/gtzdwkcqpr.html

Ruby: 42.to_s
来源：http://hz.guowangkeji.top/gtcincaszo.html

C#:   42.ToString()
来源：http://hz.bjfxy.top/gthobihtao.html

[A08] 取整与四舍五入
来源：http://hz.tanke756.top/gtviwwwuks.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jiagoushi.top/gttjrgjlir.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinqigfzy.top/gtbxffvdlk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gogol.net.cn/gtuwibjwin.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jlsjyb.cn/gtajqimvso.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yj20258888.top/gtvwtjgggm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xziqi.cn/gtltxxvkuu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jyoumei.cn/gtclndjpfs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hywenlv.cn/gtqovesmwz.html

[A09] 绝对值与最大最小值
来源：http://hz.cdnleiting.top/gtrbazhmzw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtagglwkxd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.svipenyu.cn/gtzhevdtve.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhoulong.xyz/gtavxuzguh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.vqdsnc.cn/gthcatyrhj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.redwolf501.top/gtquxdnckk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jianghu66.top/gtzlovwfwr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.bjfxy.top/gtxlsgdlya.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenlongwang.top/gtipsqxoih.html

[A10] 生成随机数
来源：http://hz.ydjk.org.cn/gtisgumrsb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hysaishi.cn/gtbjxkjikp.html

PHP:  random_int(1, 100);
来源：http://hz.cqqwz.cn/gtkqfzmuwi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhiwuduotai.top/gtdoeemidr.html


<!-- 参考信息 -->