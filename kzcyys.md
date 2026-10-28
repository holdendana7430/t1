代发 wailian999

[U65] PHP：会话
来源：http://hz.wangdashe.top/gtoiqwtvkx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gzhubu.top/gtxfhpumns.html

[U66] PHP：设置 Cookie
来源：http://hz.guowangkeji.top/gtnqnrjkuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuetiantiany.cn/gtkhoolqyj.html

[U67] PHP：处理文件上传
来源：http://hz.jlsjyb.cn/gtyhkckzqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.vqdsnc.cn/gtknoioryz.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtseejnlhl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tianlin.xyz/gtgmizlsxh.html

[U69] PHP：PDO 预处理
来源：http://hz.hysaishi.cn/gtfsdutzms.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtaqctajbu.html

[U70] PHP：PDO 事务
来源：http://hz.zhoulong.xyz/gtittsxjia.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinqigufen.top/gterhknlkz.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtfncqbezk.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtnjqqjyfh.html

[U72] PHP：写错误日志
来源：http://hz.sxryk.cn/gtwjxkrpiw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangtech.top/gtdiztawmg.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtvxacvpvq.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtqzmaaiwn.html

[U74] PHP：读取环境变量
来源：http://hz.yueranfly.top/gtgygqwavo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xinyue.icu/gtndsxlslp.html

[U75] PHP：依赖注入
来源：http://hz.snrcjt.cn/gtscfgljee.html

composer require psr/container
来源：http://hz.cdnleiting.top/gteqjdceci.html

[U76] PHP：简单路由
来源：http://hz.zhoulong.xyz/gtsylhmnwj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hywenlv.cn/gtujvazhbf.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtjbvimodz.html

composer require twig/twig
来源：http://hz.gotoacloud.top/gtaqdudfox.html

[U78] PHP：单元测试
来源：http://hz.cheryme.top/gtozfmijsx.html

composer require --dev phpunit/phpunit
来源：http://hz.iojbl.cn/gtrrvqulkm.html

[U79] PHP：静态分析
来源：http://hz.aibaodan.cn/gtpvkwvewk.html

composer require --dev phpstan/phpstan
来源：http://hz.yj202588.top/gtyguhrndc.html

[U80] PHP：代码规范修复
来源：http://hz.sxryk.cn/gtwptwrlwm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gtcseufinh.html

[U81] JS：初始化项目
来源：http://hz.svipenyu.cn/gtcspyacws.html

npm init -y;  npm i express
来源：http://hz.zhongyouzk.top/gtmviqgzgv.html

[U82] JS：package.json 脚本
来源：http://hz.guannengcc.top/gtxctfkilg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.c1oappe.top/gtlijvsudw.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtbqlockfr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yanxiufei.cn/gteudjillz.html

[U84] JS：CommonJS 写法
来源：http://hz.daxiang520.top/gtlslcwoox.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.haohaochexian.top/gtsuyuvkfy.html

[U85] JS：可选链
来源：http://hz.svipenyu.cn/gtgupxjqcd.html

a?.b?.c
来源：http://hz.snrcjt.cn/gtsrnizabg.html

[U86] JS：空值合并
来源：http://hz.guannengcc.top/gtgyyresyh.html

a ?? b
来源：http://hz.daria6918.cn/gtafqcnmet.html

[U87] JS：解构默认值
来源：http://hz.shangyingyoupin.top/gtmjpsqeyk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gteynntkro.html

[U88] JS：对象展开合并
来源：http://hz.aizwys.cn/gtkruvpljp.html

{ ...a, ...b }
来源：http://hz.wangdashe.top/gtaabneyfx.html

[U89] JS：数组去重
来源：http://hz.yuxming.cn/gtjdieisbi.html

[...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtsgykxwtx.html

[U90] JS：数字数组排序
来源：http://hz.jqgufenzy.top/gtpvxfqqwb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtdtncoudy.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangtech.top/gtizftnzfg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.snrcjt.cn/gtmzvinlty.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtjlqwppjf.html

structuredClone(obj)
来源：http://hz.316326.xyz/gtkptmwgns.html

[U93] JS：模板字符串
来源：http://hz.vqdsnc.cn/gtcsmgmfut.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtedppluzj.html

[U94] JS：箭头函数
来源：http://hz.gzhubu.top/gtdoeawwbh.html

const double = x => x * 2;
来源：http://hz.hfpthk.cn/gtpfdyhaol.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gthgkfpbxf.html

new Promise((resolve, reject) => {})
来源：http://hz.jinghuilouyu.cn/gtwwmixhjc.html

[U96] JS：async/await 与异常
来源：http://hz.nanxinkj.top/gtjyeeqldn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtlwuhrecd.html

[U97] JS：并发请求
来源：http://hz.sufxvd.cn/gtgxagjltk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtdcsffjrr.html

[U98] JS：fetch 带 JSON
来源：http://hz.zdqjudy.top/gtqoggjjxt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtbgcdcjwr.html

[U99] JS：事件监听
来源：http://hz.cucudq.cn/gtqscyyibu.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangkeji.top/gtzgcfegfj.html

[U100] JS：DOM 查询
来源：http://hz.ydjk.org.cn/gtbmyrwaye.html

document.querySelector(".item")
来源：http://hz.zdqjudy.top/gtstmyzjzw.html

[U101] JS：classList 操作
来源：http://hz.havefunace.top/gtfpecolrl.html

el.classList.toggle("active")
来源：http://hz.aibaodan.cn/gtrraaznzt.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtfydqhqpj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.havefunace.top/gtyyyehfmk.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtpenxcwbl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.0kj1m.cn/gtkssdaraw.html

[U104] JS：防抖
来源：http://hz.shanyushiyangkeji.top/gtdvevbnbh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtaauqburz.html

[U105] JS：节流
来源：http://hz.c1oappe.top/gtxppqmzkk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuxming.cn/gtwejisgvm.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtaodqvszo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yvedp.cn/gtzmkcspnr.html

[U107] JS：数字千分位
来源：http://hz.ybcxt.top/gtxyiwhfhb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cdnleiting.top/gtllvcvtkg.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtdwfrkxcx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zdqjudy.top/gtpmjunxvr.html

[U109] JS：数组分组
来源：http://hz.zhiwuduotai.top/gtsuiyoroi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtudwvloix.html

[U110] JS：数组分块
来源：http://hz.quarkkingdee.top/gtcmavrnyx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.c1oappe.top/gtabvoafha.html

[U111] JS：对象转 Map
来源：http://hz.nanxinkj.top/gtrdbbufkl.html

new Map(Object.entries(obj))
来源：http://hz.dashuyun.cn/gtzbofmddd.html

[U112] JS：字符串补位
来源：http://hz.havefunace.top/gtvayglujd.html

"7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtlmhphncw.html

[U113] JS：正则替换全部
来源：http://hz.hysaishi.cn/gthmiqldcy.html

s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtsxbzkske.html

[U114] JS：JSON 深比较
来源：http://hz.mhx1999.top/gtaxuphawu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gteonrhgxk.html

[U115] JS：生成 UUID
来源：http://hz.zhixingplan.top/gthvsbvlda.html

crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtryhvvvbe.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258.top/gtnfncrqhm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtaewrgryt.html

[U117] JS：单元测试
来源：http://hz.52xcode.cn/gtjeaejknh.html

npm i -D vitest;  npx vitest
来源：http://hz.kuanghao11.cn/gtwtaxldqc.html

[U118] JS：开发服务器
来源：http://hz.chenjidiqi.icu/gtlwuhhxrv.html

npm i -D vite;  npx vite
来源：http://hz.zhixingplan.top/gtfzdpfqdf.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtxmyrgkwm.html

npx vite build
来源：http://hz.sweek.top/gtrjwzgrsi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.feifeiyinyue.top/gtvdmripzl.html

import.meta.env.VITE_API_URL
来源：http://hz.yuxming.cn/gtmovuiefd.html

================================================================================
来源：http://hz.chenzaomai.com/gtuvgjyief.html

统计汇总
来源：http://hz.wangshuangyany.cn/gtcsizjjae.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgeehslgy.html

按语言统计（条）：
来源：http://hz.9152youxi.cn/gtwykmasch.html

Python ......... 252
来源：http://hz.ivvv.top/gtmgfoibsc.html

PHP ............ 252
来源：http://hz.bjfxy.top/gtrycftvow.html

JavaScript ..... 252
来源：http://hz.hammf.cn/gtkjfbqeko.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtrnuajghy.html

Java ........... 212
来源：http://hz.yuanzhike.top/gtyhkzoaoo.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtbbrizwti.html

Ruby ........... 212
来源：http://hz.jinqigfzy.top/gtzmaiipvt.html

C# ............. 212
来源：http://hz.svipenyu.cn/gtttniyhvc.html

C .............. 30
来源：http://hz.hysaishi.cn/gtlkqkyoou.html

C++ ............ 30
来源：http://hz.dianchejie.cn/gtwwvidrjo.html

SQL ............ 90
来源：http://hz.zhijiandao.cn/gtgpjkdjfl.html

Bash ........... 80
来源：http://hz.yangfankeji.com/gtjvwxonos.html

Kotlin ......... 15
来源：http://hz.gaohongyu789.top/gtbmawuvrr.html

Swift .......... 15
来源：http://hz.dashuyun.cn/gtnmxxrswo.html

Lua ............ 10
来源：http://hz.jyoumei.cn/gtfjslziid.html

Perl ........... 10
来源：http://hz.316326.xyz/gtrealrhbw.html

Scala .......... 10
来源：http://hz.sxryk.cn/gtwqtsmupd.html

------------------------------------
来源：http://hz.jyoumei.cn/gtiwjznfyi.html

合计 ........... 2106 条
来源：http://hz.xinyue.icu/gtxpxriuvg.html

按章节统计：
来源：http://hz.316326.xyz/gtcifnrtyy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtcpkzrarg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtluirnapu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtusdxpktu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtyorvvthx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtudfohsmv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtqofobmva.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtddviyteh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ivvv.top/gtzdcvgvyl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtswxdzwaj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gttghynenc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtozgqvpvc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtuilqhelp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtiytomahx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtgrhlyzas.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinqigfzy.top/gtfyacvltk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtbplpzvax.html

Q SQL 专题                              90
来源：http://hz.cashguo.top/gtjkvltuvy.html

R Bash 专题                             80
来源：http://hz.jlsjyb.cn/gtfltykjeo.html

S C / C++ 专题                          60
来源：http://hz.yongpay.top/gtldhepdtk.html

T 其他语言补充                          60
来源：http://hz.cucudq.cn/gtvuwtlfdq.html

U 高频实用片段                         120
来源：http://hz.aibaodan.cn/gtpwpfabcd.html

------------------------------------
来源：http://hz.shzxlz.cn/gtijcylaxz.html

合计                                  2106 条
来源：http://hz.hnxiangtu.top/gtmnusrele.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtbiyldfgk.html

使用提醒
来源：http://hz.wangshuangyany.cn/gtfyhdkkwr.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtbbcmqvnv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ybcxt.top/gtrdlbdqow.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tanke756.top/gtqbsaqtkb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258.top/gtafrmtawj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.havefunace.top/gtpimrniia.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yuanzhike.top/gtxfxmejdl.html

—— 文件结束 ——
来源：http://hz.nwbrower.top/gtptawqicv.html

================================================================================
来源：http://hz.dianchejie.cn/gtffswhcjn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gogol.net.cn/gtdcgbwrbv.html

Common Programming Examples Cheat Book
来源：http://hz.zdqjudy.top/gtuivcfvny.html

================================================================================
来源：http://hz.yonumen.top/gtalbekumk.html

【收录内容】
来源：http://hz.jqgufenzy.top/gtqpcetufp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guowangkeji.top/gtyfdlxwmx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.svipenyu.cn/gtbngyddea.html

SQL · Bash · C · C++
来源：http://hz.yj202588.top/gtgtkheemn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.meibo888.top/gtlfhjuwyg.html

【使用说明】
来源：http://hz.hnqzz.top/gtiwobcbfe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guowangkeji.top/gtaolnwmen.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydjk.org.cn/gtfubjfbwk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zdqjudy.top/gtyjgektpe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yj20258.top/gttjvedpkt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtyilabbom.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhiwuduotai.top/gtftpiivxl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.daria6918.cn/gtwarzovau.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.snrcjt.cn/gtykglirae.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.aibaodan.cn/gttxblortj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cheryme.top/gtrqqakecm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ybcxt.top/gticvgifcp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shuidangran.top/gtbjpzaoqx.html

【文件统计】
来源：http://hz.jinqigufen.top/gtloztvanm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sxryk.cn/gtfaxbggzb.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtvydxrmef.html

目  录
来源：http://hz.cashguo.top/gtgfdlyjug.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtnqioqtff.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.haohaochexian.top/gtzxmwtjdf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cdnleiting.top/gtgdkuxwkh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtzazclaof.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aibaodan.cn/gtoxzjeual.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yonumen.top/gtjdakhovl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtiuqysrow.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtmlelqbfz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xuetiantiany.cn/gtntgckxlf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtsqephnpq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtvstcwpxi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtdeozjbnh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtlmfvxtpk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtfrlhggwa.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gttylqaarx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shangyingyoupin.top/gtvdzsuvgj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtwkdynlni.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dianchejie.cn/gtlsdrhljm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangtech.top/gtiozronwp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgfzy.top/gtjcmbwasf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hammf.cn/gtynxxszro.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtkgwbbeof.html

================================================================================
来源：http://hz.yj202588.top/gtqpeojfqe.html

A. 基础语法与类型
来源：http://hz.wangshuangyany.cn/gtzixrgfns.html

================================================================================
来源：http://hz.meibo888.top/gthnfeiyjm.html

[A01] Hello World
来源：http://hz.cucudq.cn/gtzykupjbs.html

Py:   print("Hello, World!")
来源：http://hz.svipenyu.cn/gtbvmensmx.html

PHP:  echo "Hello, World!";
来源：http://hz.52xcode.cn/gtkkkgdkly.html

JS:   console.log("Hello, World!");
来源：http://hz.hnxiangtu.top/gthnwccnpy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ppjwa.cn/gtxzzlfnrr.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgufenzy.top/gtnprfshyd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hfpthk.cn/gtndwbfwqj.html

Ruby: puts "Hello, World!"
来源：http://hz.gogol.net.cn/gtsveqcpsn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtkvsjjadb.html

[A02] 变量声明与赋值
来源：http://hz.aizwys.cn/gtgosbpdjl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhiwuduotai.top/gtbwhtcono.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhongyouzk.top/gtenvgpvzk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.vqdsnc.cn/gttbzshpdv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ybcxt.top/gtvqxjbryw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtlkzkvhxu.html

Go:   name := "Alex"; age := 20
来源：http://hz.xuetiantiany.cn/gtbvswpypm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zycfv.cn/gtvqlfygeh.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gthkzncake.html

[A03] 常量定义
来源：http://hz.hysaishi.cn/gttihwgjit.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gzhubu.top/gtfdcmdlsd.html

PHP:  const PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtiqbpifbt.html

JS:   const PI = 3.14159;
来源：http://hz.haohaochexian.top/gtemuhqphb.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhixingplan.top/gtnranodpz.html

Java: static final double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtwbzqyrfg.html

Go:   const PI = 3.14159
来源：http://hz.shangyingyoupin.top/gtbscwujfb.html

Ruby: PI = 3.14159
来源：http://hz.shuidangran.top/gtycxdgpfc.html

C#:   const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtbzvtgzck.html

[A04] 判断变量类型
来源：http://hz.shangyingyoupin.top/gtipmkerqb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ehwqpu.com/gtmdldoyqv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ywan-chungtsiang.top/gtbmqbuvyr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xuetiantiany.cn/gtemcoukcn.html

TS:   typeof x; x instanceof Date
来源：http://hz.aibaodan.cn/gtyxtzyiaj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.tanke756.top/gtramswajd.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.dianchejie.cn/gtxoaouope.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yueranfly.top/gttqpskacy.html

C#:   x.GetType().Name; x is int
来源：http://hz.smart0.xyz/gtqtnuxwau.html

[A05] 整数除法与取模
来源：http://hz.sxryk.cn/gtyccxztbq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cucudq.cn/gtgqxgphml.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtaogibmmp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.kuanghao11.cn/gtrxtzkvkt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtkbimwake.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtaitlvdbf.html

Go:   7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtwyzxljcz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sufxvd.cn/gtqgptrpcj.html

C#:   7 / 2; 7 % 2
来源：http://hz.xylfe.cn/gtvclzhpoo.html

[A06] 字符串转数字
来源：http://hz.ydjk.org.cn/gtxmvftrey.html

Py:   int("42"); float("3.14")
来源：http://hz.sysykeji.top/gtpxncmjtw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinyuanbaomall.cn/gtqcgbrtrv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nwbrower.top/gtnbyjjeii.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.9152youxi.cn/gtuiacpimi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.dianchejie.cn/gtoznuebvf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tanke756.top/gtfnozcolb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.pycfn.com/gtohfeegvo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pengpengdd.cyou/gtyhxdsmdw.html

[A07] 数字转字符串
来源：http://hz.ydzc1.top/gtammzcmef.html

Py:   str(42)
来源：http://hz.gotoacloud.top/gtohrdalsn.html

PHP:  (string) 42; strval(42)
来源：http://hz.c1oappe.top/gtoscxqyzv.html

JS:   String(42); (42).toString()
来源：http://hz.hywenlv.cn/gtutdlqqqt.html

TS:   String(42)
来源：http://hz.fzhhl.top/gtimvxxxff.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.iojbl.cn/gthjxereuw.html

Go:   strconv.Itoa(42)
来源：http://hz.yueranfly.top/gtuhcmapeg.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gttfcroxyn.html

C#:   42.ToString()
来源：http://hz.jinghuilouyu.cn/gtznnqbcpi.html

[A08] 取整与四舍五入
来源：http://hz.daxiang520.top/gtzrlkzeyu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.havefunace.top/gtthyifjju.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.bjfxy.top/gtllazgktl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.dianchejie.cn/gtjnwrorek.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xuetiantiany.cn/gtwsylqdeq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.meibo888.top/gtvjedqczo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.quarkkingdee.top/gtkhdhxcno.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.kuanghao11.cn/gtkdmcqtbj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cqqwz.cn/gtpegdjwfb.html

[A09] 绝对值与最大最小值
来源：http://hz.yuxming.cn/gtqribrbry.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenjidiqi.icu/gtmltjfpos.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gtzzpbsjmm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.tanke756.top/gtpxfpzznn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cucudq.cn/gtqceanpyi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ehwqpu.com/gtlypgcnex.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.snrcjt.cn/gtfxqsstbe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.meibo888.top/gtwotakple.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.cheryme.top/gtetzstnky.html


<!-- 参考信息 -->