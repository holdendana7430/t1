代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtaartqfqe.html

"值: {$a}"
来源：http://hz.sysykeji.top/gtuncqsjib.html

[U58] PHP：数组三件套
来源：http://hz.zdqjudy.top/gtxknoelcp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cqqwz.cn/gtfnwghwyi.html

[U59] PHP：自定义排序
来源：http://hz.iojbl.cn/gttuejabzz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gttkouzvgx.html

[U60] PHP：JSON 编解码
来源：http://hz.hnqzz.top/gthevudhkv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cdnleiting.top/gtzofbgvky.html

[U61] PHP：正则
来源：http://hz.cqqwz.cn/gtmmlwecsa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtnhoomhcg.html

[U62] PHP：日期对象
来源：http://hz.iojbl.cn/gthhewpntr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jqgufenzy.top/gtnykicmjl.html

[U63] PHP：文件读写
来源：http://hz.pycfn.com/gtrxpuzufj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.andypj.xyz/gtjnuvfvwn.html

[U64] PHP：目录遍历
来源：http://hz.yj202588.top/gtbzrfrevi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgufenzy.top/gtylnurafc.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtjbwyxqul.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aibaodan.cn/gtqxtvozmt.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gtvfgyquni.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.andypj.xyz/gtxrvwnxsl.html

[U67] PHP：处理文件上传
来源：http://hz.pengpengdd.cyou/gticgqqafr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dianchejie.cn/gtzehordrs.html

[U68] PHP：PDO 连接
来源：http://hz.sxryk.cn/gtwpvyjxta.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.daxiang520.top/gtvycfukdq.html

[U69] PHP：PDO 预处理
来源：http://hz.yuxming.cn/gtvlkadsku.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtpmcvbvrl.html

[U70] PHP：PDO 事务
来源：http://hz.pengpengdd.cyou/gtncmrxbyz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtsdhdjqtu.html

[U71] PHP：抛出异常
来源：http://hz.aizwys.cn/gtckqcsepw.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtsuxxuwvc.html

[U72] PHP：写错误日志
来源：http://hz.daxiang520.top/gttruspuea.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yj20258.top/gtfceuuipd.html

[U73] PHP：读取 ini 配置
来源：http://hz.yonumen.top/gtbwophlrx.html

parse_ini_file("config.ini", true)
来源：http://hz.xylfe.cn/gtfucrbcss.html

[U74] PHP：读取环境变量
来源：http://hz.fengsongda.top/gtppiqnuxf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yuxming.cn/gtaixqxkdy.html

[U75] PHP：依赖注入
来源：http://hz.xylfe.cn/gtnhsgsply.html

composer require psr/container
来源：http://hz.gzhubu.top/gtufgnpivj.html

[U76] PHP：简单路由
来源：http://hz.zhaomingkeji.xyz/gteoywleif.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hfpthk.cn/gtcdyazqsg.html

[U77] PHP：模板渲染
来源：http://hz.snrcjt.cn/gtnwkndubv.html

composer require twig/twig
来源：http://hz.smart0.xyz/gtbxtmzqjx.html

[U78] PHP：单元测试
来源：http://hz.tian-w.cn/gtqnelqjzt.html

composer require --dev phpunit/phpunit
来源：http://hz.zhengqikj.top/gtyitfslob.html

[U79] PHP：静态分析
来源：http://hz.9152youxi.cn/gtizqggokj.html

composer require --dev phpstan/phpstan
来源：http://hz.hammf.cn/gtwucilmtz.html

[U80] PHP：代码规范修复
来源：http://hz.quarkkingdee.top/gttlhjsiqp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.kuanghao11.cn/gtsydzbtus.html

[U81] JS：初始化项目
来源：http://hz.fzhhl.top/gtzgtibtgo.html

npm init -y;  npm i express
来源：http://hz.shanyushiyangtech.top/gtzpfsayoy.html

[U82] JS：package.json 脚本
来源：http://hz.zhixingplan.top/gtovdtegyf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.mhx1999.top/gtnppnjtly.html

[U83] JS：ES Module 导入导出
来源：http://hz.zdqjudy.top/gtwrskdvxz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtvycajmrk.html

[U84] JS：CommonJS 写法
来源：http://hz.chenjidiqi.icu/gtspexdkff.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtwibnibgd.html

[U85] JS：可选链
来源：http://hz.zdqjudy.top/gtswmwxohv.html

a?.b?.c
来源：http://hz.vqdsnc.cn/gtomhyrjix.html

[U86] JS：空值合并
来源：http://hz.zhoulong.xyz/gtymsjwmtl.html

a ?? b
来源：http://hz.bjfxy.top/gtmwirvbom.html

[U87] JS：解构默认值
来源：http://hz.wangdashe.top/gtwbykwyrn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xylfe.cn/gtjqhsqimb.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gtxmvlrpgs.html

{ ...a, ...b }
来源：http://hz.yonumen.top/gtpdilwnks.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtvjzyshdl.html

[...new Set(arr)]
来源：http://hz.pycfn.com/gtclymvtjl.html

[U90] JS：数字数组排序
来源：http://hz.iojbl.cn/gtuyxhjawz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtgwolnrgj.html

[U91] JS：对象键值遍历
来源：http://hz.tian-w.cn/gtuglnlotz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.c1oappe.top/gttokummfq.html

[U92] JS：深拷贝
来源：http://hz.jlsjyb.cn/gtdlkkxlpd.html

structuredClone(obj)
来源：http://hz.andypj.xyz/gtvawzjpjz.html

[U93] JS：模板字符串
来源：http://hz.yvedp.cn/gtpurbrhmp.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gttryfckol.html

[U94] JS：箭头函数
来源：http://hz.yj20258.top/gtipyqxyey.html

const double = x => x * 2;
来源：http://hz.gaohongyu789.top/gtcdsihdyl.html

[U95] JS：Promise 包装
来源：http://hz.guowangkeji.top/gtfwfxfapr.html

new Promise((resolve, reject) => {})
来源：http://hz.pycfn.com/gtaxigdhpl.html

[U96] JS：async/await 与异常
来源：http://hz.cucudq.cn/gtdgcsijpw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtzntdzgna.html

[U97] JS：并发请求
来源：http://hz.tianlin.xyz/gtulgedmvu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtoljkugnw.html

[U98] JS：fetch 带 JSON
来源：http://hz.cucudq.cn/gtvumqwhwf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnxiangtu.top/gtnenorsgb.html

[U99] JS：事件监听
来源：http://hz.yongpay.top/gtxwgoxxhn.html

el.addEventListener("click", e => {})
来源：http://hz.tianlin.xyz/gtdzlghdob.html

[U100] JS：DOM 查询
来源：http://hz.yuanzhike.top/gtdzrfnhyk.html

document.querySelector(".item")
来源：http://hz.jianghu66.top/gtfaahiikd.html

[U101] JS：classList 操作
来源：http://hz.zhixingplan.top/gthwibisnw.html

el.classList.toggle("active")
来源：http://hz.guowangkeji.top/gtbocpobxs.html

[U102] JS：本地存储
来源：http://hz.gaohongyu789.top/gtmbwkoaif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.mhx1999.top/gtgjkhhwso.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtmvpkfuzw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ppjwa.cn/gtdxyresmd.html

[U104] JS：防抖
来源：http://hz.aibaodan.cn/gtyshpfomt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtnvgkjaoa.html

[U105] JS：节流
来源：http://hz.52xcode.cn/gtlaccdgbx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhijiandao.cn/gtvoubvqth.html

[U106] JS：日期格式化
来源：http://hz.ybcxt.top/gtadnbhwmt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangtech.top/gtfxljhhpw.html

[U107] JS：数字千分位
来源：http://hz.havefunace.top/gtwupscgmx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.9152youxi.cn/gtsvsdjkmm.html

[U108] JS：随机整数
来源：http://hz.nwbrower.top/gtreygipfc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.feifeiyinyue.top/gthqevypba.html

[U109] JS：数组分组
来源：http://hz.zhoulong.xyz/gtascuxqmr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.bjfxy.top/gtnyeswevy.html

[U110] JS：数组分块
来源：http://hz.yuanzhike.top/gtpfzofgyy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenzaomai.com/gtlnjxspky.html

[U111] JS：对象转 Map
来源：http://hz.xziqi.cn/gtycufdmyj.html

new Map(Object.entries(obj))
来源：http://hz.zdqjudy.top/gtkfxgxgub.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gtqclpxvec.html

"7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtmjkpzipq.html

[U113] JS：正则替换全部
来源：http://hz.yj20258.top/gtoqgzfvpb.html

s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtheywffst.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtgnssveyr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtyihqyikg.html

[U115] JS：生成 UUID
来源：http://hz.zhongyouzk.top/gtvkszstdd.html

crypto.randomUUID()
来源：http://hz.meibo888.top/gtdwmydstj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258.top/gteijmrkgv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.andypj.xyz/gtdracduyo.html

[U117] JS：单元测试
来源：http://hz.hammf.cn/gtujgotldv.html

npm i -D vitest;  npx vitest
来源：http://hz.chenzaomai.com/gtvtvrkznr.html

[U118] JS：开发服务器
来源：http://hz.wangdashe.top/gtoritwwpf.html

npm i -D vite;  npx vite
来源：http://hz.xingfuxueyuan.xyz/gthxfqccyb.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtravlrxnr.html

npx vite build
来源：http://hz.cdnleiting.top/gttfhkvjyj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.9152youxi.cn/gtrliihccb.html

import.meta.env.VITE_API_URL
来源：http://hz.chenjidiqi.icu/gtzpsyiphy.html

================================================================================
来源：http://hz.xylfe.cn/gtdfjqconm.html

统计汇总
来源：http://hz.shuidangran.top/gtwxnrfenf.html

================================================================================
来源：http://hz.cqqwz.cn/gtgleslfkr.html

按语言统计（条）：
来源：http://hz.jqgufenzy.top/gtyybrpqiw.html

Python ......... 252
来源：http://hz.c1oappe.top/gtqjugmucj.html

PHP ............ 252
来源：http://hz.kuanghao11.cn/gtembkbiuw.html

JavaScript ..... 252
来源：http://hz.tian-w.cn/gtccddhnin.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtopenzpsi.html

Java ........... 212
来源：http://hz.tanke756.top/gtxktmjcpu.html

Go ............. 212
来源：http://hz.ydzc1.top/gtywejbxta.html

Ruby ........... 212
来源：http://hz.hywenlv.cn/gtweipmnnk.html

C# ............. 212
来源：http://hz.birdmap.top/gtkivdlxma.html

C .............. 30
来源：http://hz.birdmap.top/gtxnngvgge.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtkdpzseie.html

SQL ............ 90
来源：http://hz.yj202588.top/gtvbbmyxld.html

Bash ........... 80
来源：http://hz.zhengqikj.top/gtlznwdmkr.html

Kotlin ......... 15
来源：http://hz.xuanzx.com/gttjzqeloa.html

Swift .......... 15
来源：http://hz.redwolf501.top/gtyjfzhrli.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtjuhlvfjd.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gthatmxnfa.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gtlwfkljee.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtzpbxaypj.html

合计 ........... 2106 条
来源：http://hz.sweek.top/gtcyuzirhq.html

按章节统计：
来源：http://hz.bjfxy.top/gtiyahwpao.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtavpfiodc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gthglpespe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtudqmyirv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhixingplan.top/gtllltndqf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jiagoushi.top/gtzhnzxxzd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cdnleiting.top/gtzwdxkfwo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtziydwlyd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gttnpzjhrl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtjjfboupj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gtbrzjucfx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtbfgeraev.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtyhooxcqp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtwzfpdwyl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258.top/gtwijjvkqi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.c1oappe.top/gtiqvenwmb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtwjaqfmmq.html

Q SQL 专题                              90
来源：http://hz.ydjk.org.cn/gtynzyqhhx.html

R Bash 专题                             80
来源：http://hz.quarkkingdee.top/gtbvnvoosh.html

S C / C++ 专题                          60
来源：http://hz.meibo888.top/gtfuaclphv.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gthombjzpb.html

U 高频实用片段                         120
来源：http://hz.gogol.net.cn/gtevfxebjl.html

------------------------------------
来源：http://hz.hywenlv.cn/gtrqloexpb.html

合计                                  2106 条
来源：http://hz.xinyue.icu/gthvhtdpep.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtynlqmasm.html

使用提醒
来源：http://hz.hnxiangtu.top/gtafouktgg.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtfydwciyh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhoulong.xyz/gtdwvivokx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ybcxt.top/gttpkwklha.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258888.top/gtvzewltnx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hysaishi.cn/gtyszkcwqr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtrjvciwkk.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtdugsmalf.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgfskeaju.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.feifeiyinyue.top/gtcwepmhsf.html

Common Programming Examples Cheat Book
来源：http://hz.gaohongyu789.top/gtdheosxvk.html

================================================================================
来源：http://hz.zycfv.cn/gtbpdujzvp.html

【收录内容】
来源：http://hz.sufxvd.cn/gtfzxxlmef.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.smart0.xyz/gtygjvskyu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.birdmap.top/gtfuofwigl.html

SQL · Bash · C · C++
来源：http://hz.chenlongwang.top/gtcbimylck.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.meibo888.top/gtnvpdrsag.html

【使用说明】
来源：http://hz.ivvv.top/gtmdxrwbkd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.pycfn.com/gthrphnzmp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shangyingyoupin.top/gtaiodvpwh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xuanzx.com/gtntpcyxfk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sysykeji.top/gtolrwlybd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangshuangyany.cn/gtguiodawx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.guannengcc.top/gtbtamsscf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.mhx1999.top/gthwfcnscn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yueranfly.top/gtwmwunmkg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hywenlv.cn/gtspxliaqq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cqqwz.cn/gtoaoqfpes.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gotoacloud.top/gtdajlhoro.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtjtgciexu.html

【文件统计】
来源：http://hz.yj20258.top/gtfycjmwgp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pengpengdd.cyou/gtwdkojtrl.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtbwglkxmd.html

目  录
来源：http://hz.ydzc1.top/gtkyagyyia.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtlpmujtrm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.redwolf501.top/gtwqiuhafp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtdfznpvev.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtnxxhrttv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtlgxwmhof.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aizwys.cn/gtchwbypyg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtqeyucise.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtlroqywwp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtshkdgtol.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtkqfvacdm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtmrfrrhcp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gthjiorxar.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gteupwaslk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtvowxtnbs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ehwqpu.com/gtoloiakaq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yvedp.cn/gtuolokvzy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtpqhluftn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.birdmap.top/gttzsxhott.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gzhubu.top/gtpbmcxljw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jianghu66.top/gtmaxuaugt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtonupiggj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gtljemgeob.html

================================================================================
来源：http://hz.guannengcc.top/gtucasnkgv.html

A. 基础语法与类型
来源：http://hz.ydjk.org.cn/gtyhhkmkzl.html

================================================================================
来源：http://hz.aibaodan.cn/gtrlwnmrom.html

[A01] Hello World
来源：http://hz.chenzaomai.com/gtpqdyekrl.html

Py:   print("Hello, World!")
来源：http://hz.sufxvd.cn/gtmncbpjqx.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtbmcidlhl.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258888.top/gtwnjopuoo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenzaomai.com/gtupifpeic.html

Java: System.out.println("Hello, World!");
来源：http://hz.snrcjt.cn/gtzsewceoz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtyyanoxnu.html

Ruby: puts "Hello, World!"
来源：http://hz.smart0.xyz/gtjzdlmudk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.haohaochexian.top/gtdvmcvoje.html

[A02] 变量声明与赋值
来源：http://hz.0kj1m.cn/gtptyzthye.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.wangdashe.top/gtzijqlujz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.52xcode.cn/gtxwxtojjq.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.snrcjt.cn/gtanhltfvr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sysykeji.top/gtghzfjrlt.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xuetiantiany.cn/gtxksvzmnl.html

Go:   name := "Alex"; age := 20
来源：http://hz.gogol.net.cn/gtigjymges.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jyoumei.cn/gtjcyluwln.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hywenlv.cn/gtwweohucc.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtuizyhzbx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pengpengdd.cyou/gtagbybwlo.html

PHP:  const PI = 3.14159;
来源：http://hz.hywenlv.cn/gtqhvqhlvl.html

JS:   const PI = 3.14159;
来源：http://hz.daxiang520.top/gtsandxfaf.html

TS:   const PI: number = 3.14159;
来源：http://hz.gogol.net.cn/gtnnhaxhvp.html

Java: static final double PI = 3.14159;
来源：http://hz.ydzc1.top/gtdhgokivh.html

Go:   const PI = 3.14159
来源：http://hz.hongshengwenyu.top/gtcyupvjyc.html

Ruby: PI = 3.14159
来源：http://hz.zhengqikj.top/gtkthfuxwk.html

C#:   const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtrqoytykj.html

[A04] 判断变量类型
来源：http://hz.xziqi.cn/gthjjuebzt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yueranfly.top/gtxqkiggvo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hywenlv.cn/gtnqkdaawr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhixingplan.top/gtknmpkbww.html

TS:   typeof x; x instanceof Date
来源：http://hz.ybcxt.top/gtuycsammj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hammf.cn/gtwgyduxju.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ywan-chungtsiang.top/gtnuydrayw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.fengsongda.top/gtalqhelmk.html

C#:   x.GetType().Name; x is int
来源：http://hz.316326.xyz/gtisfsusks.html

[A05] 整数除法与取模
来源：http://hz.hammf.cn/gtnypgyjop.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhixingplan.top/gtmtmzmprs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.mhx1999.top/gtoasfbakq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhengqikj.top/gtpdslvuvd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.havefunace.top/gtwilrnkve.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtxvnktwwy.html

Go:   7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtgfsisamk.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gthtuexujz.html

C#:   7 / 2; 7 % 2
来源：http://hz.xuanzx.com/gtjpngxhtd.html

[A06] 字符串转数字
来源：http://hz.haohaochexian.top/gtbfktwkas.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgufenzy.top/gtshbglctm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhaomingkeji.xyz/gtwjwwixio.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.tian-w.cn/gtsvhbwzfb.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hysaishi.cn/gtwbrcydmw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.dashuyun.cn/gtteqddvjp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xuanzx.com/gtnigjqenm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ywan-chungtsiang.top/gtsirsqlrh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dashuyun.cn/gtnthpwwxq.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtfefhctce.html

Py:   str(42)
来源：http://hz.shuidangran.top/gtmlywdsrh.html

PHP:  (string) 42; strval(42)
来源：http://hz.jinqigufen.top/gtudppxvgc.html

JS:   String(42); (42).toString()
来源：http://hz.sweek.top/gtgblufere.html

TS:   String(42)
来源：http://hz.ywan-chungtsiang.top/gtbiwnoahk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.svipenyu.cn/gtrfqceigz.html

Go:   strconv.Itoa(42)
来源：http://hz.jinyuanbaomall.cn/gtmzjbhclr.html

Ruby: 42.to_s
来源：http://hz.birdmap.top/gtlvltsehq.html

C#:   42.ToString()
来源：http://hz.yanxiufei.cn/gtaarombks.html

[A08] 取整与四舍五入
来源：http://hz.yj20258888.top/gtpztichmg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nwbrower.top/gtxzbszhmq.html


<!-- 参考信息 -->