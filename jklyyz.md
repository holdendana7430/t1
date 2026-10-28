代发 wailian999

[U63] PHP：文件读写
来源：http://hz.smart0.xyz/gtkwohzevr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.guowangkeji.top/gtviebzvtb.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gttnzcssgv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.pengpengdd.cyou/gtrrrbnxmu.html

[U65] PHP：会话
来源：http://hz.jinqigfzy.top/gtqxvufdpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cheryme.top/gttdqcvgdl.html

[U66] PHP：设置 Cookie
来源：http://hz.jqgfzy.top/gtmawoujlc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cucudq.cn/gtntsenvfm.html

[U67] PHP：处理文件上传
来源：http://hz.yonumen.top/gtdolpfico.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.daria6918.cn/gtxjjlsjia.html

[U68] PHP：PDO 连接
来源：http://hz.wangshuangyany.cn/gtupgbzlbe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtgqqybqif.html

[U69] PHP：PDO 预处理
来源：http://hz.ppjwa.cn/gtfvchwctu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yongpay.top/gtkziirmdg.html

[U70] PHP：PDO 事务
来源：http://hz.dashuyun.cn/gtzxssliog.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gtqvdnokmr.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gtguwegfwt.html

throw new RuntimeException("失败", 500);
来源：http://hz.gogol.net.cn/gthofbbcof.html

[U72] PHP：写错误日志
来源：http://hz.hammf.cn/gtdxsxhhai.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenzaomai.com/gtrbmuswoq.html

[U73] PHP：读取 ini 配置
来源：http://hz.pycfn.com/gtvmycjika.html

parse_ini_file("config.ini", true)
来源：http://hz.zhoulong.xyz/gttzxsxqhp.html

[U74] PHP：读取环境变量
来源：http://hz.jiagoushi.top/gtulctnntf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinyuanbaomall.cn/gtlibkpypw.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gtfkossfrr.html

composer require psr/container
来源：http://hz.zhongyouzk.top/gtnwkqxekz.html

[U76] PHP：简单路由
来源：http://hz.hfpthk.cn/gtfnftwvhh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.9152youxi.cn/gtsihrgjsj.html

[U77] PHP：模板渲染
来源：http://hz.pycfn.com/gtfksrssaw.html

composer require twig/twig
来源：http://hz.nanxinkj.top/gtbdarkxgu.html

[U78] PHP：单元测试
来源：http://hz.gzhubu.top/gtosdxjiwq.html

composer require --dev phpunit/phpunit
来源：http://hz.chenzaomai.com/gttpcsnugg.html

[U79] PHP：静态分析
来源：http://hz.yj20258888.top/gttdpvdkqb.html

composer require --dev phpstan/phpstan
来源：http://hz.bjfxy.top/gtxckxsuvy.html

[U80] PHP：代码规范修复
来源：http://hz.yonumen.top/gtahimulqd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sweek.top/gtkwviuvzs.html

[U81] JS：初始化项目
来源：http://hz.quarkkingdee.top/gtbefwrbek.html

npm init -y;  npm i express
来源：http://hz.cheryme.top/gtiqssudub.html

[U82] JS：package.json 脚本
来源：http://hz.xuetiantiany.cn/gtalcrjmna.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.bjfxy.top/gtzuhalzhp.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydjk.org.cn/gthcbeaulp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tianlin.xyz/gtqopjvkvu.html

[U84] JS：CommonJS 写法
来源：http://hz.jlsjyb.cn/gtwimrqvuq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenzaomai.com/gtcocujuzg.html

[U85] JS：可选链
来源：http://hz.0kj1m.cn/gtavsylrcj.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtmzclfvpz.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gtpubtqyyl.html

a ?? b
来源：http://hz.cqqwz.cn/gthydngaco.html

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gtjkuskeqn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hysaishi.cn/gtktnosgzs.html

[U88] JS：对象展开合并
来源：http://hz.sxryk.cn/gtbnhpzpwq.html

{ ...a, ...b }
来源：http://hz.iojbl.cn/gtthekutwq.html

[U89] JS：数组去重
来源：http://hz.ybcxt.top/gtjnczmntu.html

[...new Set(arr)]
来源：http://hz.cheryme.top/gtfvtveoem.html

[U90] JS：数字数组排序
来源：http://hz.yueranfly.top/gtytqqahtu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gthzilzhzm.html

[U91] JS：对象键值遍历
来源：http://hz.cashguo.top/gtpvjaykld.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pengpengdd.cyou/gthjfdclyg.html

[U92] JS：深拷贝
来源：http://hz.jiagoushi.top/gtvnqesdnj.html

structuredClone(obj)
来源：http://hz.xziqi.cn/gtbkjvduek.html

[U93] JS：模板字符串
来源：http://hz.zhongyouzk.top/gtxhnepzfx.html

`共 ${n} 条`
来源：http://hz.yonumen.top/gthztynnqs.html

[U94] JS：箭头函数
来源：http://hz.guowangkeji.top/gtoznwvwwh.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtriubcavz.html

[U95] JS：Promise 包装
来源：http://hz.yongpay.top/gtweuatgzj.html

new Promise((resolve, reject) => {})
来源：http://hz.xingfuxueyuan.xyz/gtruikkjrh.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtesbdastj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtplwqgcnz.html

[U97] JS：并发请求
来源：http://hz.xziqi.cn/gttlipmkiu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtsrzvgphh.html

[U98] JS：fetch 带 JSON
来源：http://hz.sweek.top/gtzqkewgbi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnxiangtu.top/gteyvhcoxi.html

[U99] JS：事件监听
来源：http://hz.jinqigfzy.top/gtkhvvqrqm.html

el.addEventListener("click", e => {})
来源：http://hz.gaohongyu789.top/gtpjghcpsx.html

[U100] JS：DOM 查询
来源：http://hz.redwolf501.top/gthztqmwot.html

document.querySelector(".item")
来源：http://hz.jyoumei.cn/gttlgjhsyx.html

[U101] JS：classList 操作
来源：http://hz.jinqigufen.top/gttwykzciy.html

el.classList.toggle("active")
来源：http://hz.xziqi.cn/gtnxqdtapf.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gthebmxebv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258.top/gtkelwsfio.html

[U103] JS：定时器
来源：http://hz.ybcxt.top/gtzdusgxct.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gtelgfulyh.html

[U104] JS：防抖
来源：http://hz.kuanghao11.cn/gtkmypudau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtooqfcwar.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtxexajycn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.haohaochexian.top/gtwvjvsymn.html

[U106] JS：日期格式化
来源：http://hz.fzhhl.top/gtazxyfqxr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtpoqfvkaf.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtuupwenfe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtkmsvvikq.html

[U108] JS：随机整数
来源：http://hz.pycfn.com/gtdslowpoa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtkqphvmps.html

[U109] JS：数组分组
来源：http://hz.9152youxi.cn/gtwerbvlnp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gthiybbygp.html

[U110] JS：数组分块
来源：http://hz.jinghuilouyu.cn/gtnacvzfgu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gttxkxeliy.html

[U111] JS：对象转 Map
来源：http://hz.ivvv.top/gtbpvaaamv.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gtrwocjjxj.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtatpeyhyj.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtsoomqdgb.html

[U113] JS：正则替换全部
来源：http://hz.jqgufenzy.top/gtitlzhhla.html

s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gttfxjfojk.html

[U114] JS：JSON 深比较
来源：http://hz.fzhhl.top/gtkwsumpie.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtfskcftnk.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gtzeffpjyr.html

crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtfqkmrwrg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cheryme.top/gtjjmoxvok.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cucudq.cn/gtppcxdhfi.html

[U117] JS：单元测试
来源：http://hz.vqdsnc.cn/gtbxyqdjgn.html

npm i -D vitest;  npx vitest
来源：http://hz.zhijiandao.cn/gtkdvwblcz.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtkjlvzdrd.html

npm i -D vite;  npx vite
来源：http://hz.jlsjyb.cn/gtmooyozud.html

[U119] JS：生产构建
来源：http://hz.xingfuxueyuan.xyz/gtlxdnrbtj.html

npx vite build
来源：http://hz.quarkkingdee.top/gtovlurtrl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tanke756.top/gtfiohbudq.html

import.meta.env.VITE_API_URL
来源：http://hz.sufxvd.cn/gtwmdaerfo.html

================================================================================
来源：http://hz.zycfv.cn/gtcfdlayjz.html

统计汇总
来源：http://hz.gzhubu.top/gttdvdshzs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqfotvhfo.html

按语言统计（条）：
来源：http://hz.jinqigufen.top/gtkedwoprv.html

Python ......... 252
来源：http://hz.dianchejie.cn/gtrabsuysq.html

PHP ............ 252
来源：http://hz.yueranfly.top/gtxbhojiqf.html

JavaScript ..... 252
来源：http://hz.feifeiyinyue.top/gtpgtngsaw.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtivinxsho.html

Java ........... 212
来源：http://hz.hywenlv.cn/gtedarsufg.html

Go ............. 212
来源：http://hz.zycfv.cn/gtwqmyldan.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gttvewiube.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtljveilbg.html

C .............. 30
来源：http://hz.vqdsnc.cn/gtkqbvcnre.html

C++ ............ 30
来源：http://hz.birdmap.top/gtfbdaovws.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gtslcdxpys.html

Bash ........... 80
来源：http://hz.xinyue.icu/gtcjwillsz.html

Kotlin ......... 15
来源：http://hz.guowangkeji.top/gtsvtcpfez.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtrbqucbob.html

Lua ............ 10
来源：http://hz.yanxiufei.cn/gtussjhtnd.html

Perl ........... 10
来源：http://hz.daria6918.cn/gtlaclecgi.html

Scala .......... 10
来源：http://hz.jlsjyb.cn/gtugzebaxj.html

------------------------------------
来源：http://hz.hammf.cn/gtthhpdptm.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtkimatwgy.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtlqceucpa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gthwndxxyo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtiqvvgdig.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtagioquuh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gthowzszzm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.9152youxi.cn/gtvksmrdnt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.vqdsnc.cn/gthrpyhopc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gteqjcxmkc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtnznmgnpv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtxxdskuxd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtnklikbeq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtgseokaxz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtyouwgtlg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtvoovnfng.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daria6918.cn/gtaerqiufc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenjidiqi.icu/gtktxeufgj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtegfoeqrv.html

Q SQL 专题                              90
来源：http://hz.shangyingyoupin.top/gttrwrqkce.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtbdxnsbjj.html

S C / C++ 专题                          60
来源：http://hz.ywan-chungtsiang.top/gtejbatujj.html

T 其他语言补充                          60
来源：http://hz.gaohongyu789.top/gtcrxmcraa.html

U 高频实用片段                         120
来源：http://hz.gotoacloud.top/gthoaxgmzx.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtkrmbyacy.html

合计                                  2106 条
来源：http://hz.vqdsnc.cn/gtxcbogahz.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtyokhyadf.html

使用提醒
来源：http://hz.cucudq.cn/gtpyyctvby.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtjvueooqe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sysykeji.top/gtdqbixouy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.birdmap.top/gtwodygzas.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinqigfzy.top/gtcniacjhs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.aizwys.cn/gtymsqimup.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jlsjyb.cn/gtfpdmfmre.html

—— 文件结束 ——
来源：http://hz.wangshuangyany.cn/gttuhfxdfj.html

================================================================================
来源：http://hz.xziqi.cn/gthbtbcvbd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hongshengwenyu.top/gtvvuxzeoc.html

Common Programming Examples Cheat Book
来源：http://hz.cqqwz.cn/gtahrwqica.html

================================================================================
来源：http://hz.ivvv.top/gtchpvafbk.html

【收录内容】
来源：http://hz.tanke756.top/gtxqvcxyrh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhongyouzk.top/gtxtqtblev.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.316326.xyz/gthrsvzbrd.html

SQL · Bash · C · C++
来源：http://hz.dianchejie.cn/gtqrpulpvm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sxryk.cn/gtajqwfeon.html

【使用说明】
来源：http://hz.daxiang520.top/gtweprlhxq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinyuanbaomall.cn/gthqdcrivw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jianghu66.top/gtiosfahuq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xinyue.icu/gtemchjjnt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dianchejie.cn/gticlqshfb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yongpay.top/gtnyumzbdw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuxming.cn/gthzlxjxls.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinghuilouyu.cn/gtfuvahitl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cheryme.top/gtufjcnokh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yanxiufei.cn/gtddwrkxnv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gtpogrhrqm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.vqdsnc.cn/gtyawvbyfq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cucudq.cn/gtubmrdcrk.html

【文件统计】
来源：http://hz.fengsongda.top/gtxgensnkq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.daria6918.cn/gtceqymubf.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtkxddtdxh.html

目  录
来源：http://hz.zhijiandao.cn/gtpaqaakyi.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtjbdxwwoy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinghuilouyu.cn/gtkwenxeoq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gtsyuwvagt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sxryk.cn/gtwvuexbjc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xziqi.cn/gttvjmgyys.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aizwys.cn/gtxmhnomvh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.fzhhl.top/gtcbpzwztj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtedcpfftt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gtzabibjxa.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtqkzuqmbm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shangyingyoupin.top/gtqochnnei.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtgjaivzhw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtutgaxsfh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtilriukzf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtfotztpie.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hfpthk.cn/gtdgpunkub.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtvkgqiujc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.redwolf501.top/gthatzaiwq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jiagoushi.top/gtyixawgib.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gtjsfnfgtu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtvqgdpqcg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtrvajvcqz.html

================================================================================
来源：http://hz.smart0.xyz/gtaoozbgvo.html

A. 基础语法与类型
来源：http://hz.hywenlv.cn/gtgvnrurxq.html

================================================================================
来源：http://hz.yueranfly.top/gtanctiepb.html

[A01] Hello World
来源：http://hz.shuidangran.top/gtapicktpe.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtdcanbzzx.html

PHP:  echo "Hello, World!";
来源：http://hz.hammf.cn/gturjfrzvh.html

JS:   console.log("Hello, World!");
来源：http://hz.yj202588.top/gtzswskhcv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenzaomai.com/gthltzzluk.html

Java: System.out.println("Hello, World!");
来源：http://hz.c1oappe.top/gtljfugsah.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.vqdsnc.cn/gtaqshwnlf.html

Ruby: puts "Hello, World!"
来源：http://hz.zycfv.cn/gtabqwjloi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.iojbl.cn/gtnqgmggsj.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtqnkaiiku.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yongpay.top/gtdbjmfxpf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aizwys.cn/gtzkjzapsm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtofebgkgu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gtazmnrnaf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.9152youxi.cn/gtkpuoguwn.html

Go:   name := "Alex"; age := 20
来源：http://hz.tian-w.cn/gtcvjqrzci.html

Ruby: name = "Alex"; age = 20
来源：http://hz.nanxinkj.top/gtgovwbylv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.aibaodan.cn/gtjfseghsr.html

[A03] 常量定义
来源：http://hz.zhiwuduotai.top/gtwbeyznsh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.havefunace.top/gtkrybvokp.html

PHP:  const PI = 3.14159;
来源：http://hz.nwbrower.top/gtaxbrgkqz.html

JS:   const PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtrpwgbalv.html

TS:   const PI: number = 3.14159;
来源：http://hz.sxryk.cn/gtblmpmvqt.html

Java: static final double PI = 3.14159;
来源：http://hz.ppjwa.cn/gttghsaucq.html

Go:   const PI = 3.14159
来源：http://hz.tian-w.cn/gtzwkmsttc.html

Ruby: PI = 3.14159
来源：http://hz.zdqjudy.top/gtulrpknuj.html

C#:   const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtyohvaevl.html

[A04] 判断变量类型
来源：http://hz.meibo888.top/gtdwvheebv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.meibo888.top/gtvywvapci.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigfzy.top/gtvklavwmg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangdashe.top/gtezolokco.html

TS:   typeof x; x instanceof Date
来源：http://hz.jyoumei.cn/gtnreofnwa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangtech.top/gtsdhhhosg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhixingplan.top/gtsnjrnqvw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.birdmap.top/gtqrelgvek.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydzc1.top/gtledhhpej.html

[A05] 整数除法与取模
来源：http://hz.yongpay.top/gtidvkjydl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj20258.top/gtggwmlnlg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtrjswqpzp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guowangkeji.top/gtyinthkhm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cqqwz.cn/gtmdizoozs.html

Java: 7 / 2; 7 % 2
来源：http://hz.xylfe.cn/gtsdvumwaq.html

Go:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtrexarrjg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.kuanghao11.cn/gtmoedghqf.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtsqkthdzh.html

[A06] 字符串转数字
来源：http://hz.aizwys.cn/gtvcteflaf.html

Py:   int("42"); float("3.14")
来源：http://hz.xuanzx.com/gtvpdbsnhi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zycfv.cn/gtelbgloij.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.vqdsnc.cn/gthbdyberu.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.kuanghao11.cn/gtongxdcut.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhijiandao.cn/gtekgyetqm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gthirxdgwe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hongshengwenyu.top/gtowdimjxi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jlsjyb.cn/gtxfnjnfvh.html

[A07] 数字转字符串
来源：http://hz.ydzc1.top/gtfjnowrsm.html

Py:   str(42)
来源：http://hz.mhx1999.top/gtgriizgdz.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhiwuduotai.top/gtzclafodi.html

JS:   String(42); (42).toString()
来源：http://hz.yonumen.top/gtdxjbqjiy.html

TS:   String(42)
来源：http://hz.sufxvd.cn/gtefpoxzhq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hfpthk.cn/gtlfppmkcx.html

Go:   strconv.Itoa(42)
来源：http://hz.daxiang520.top/gtxxvwmafy.html

Ruby: 42.to_s
来源：http://hz.pycfn.com/gtjqcavwdj.html

C#:   42.ToString()
来源：http://hz.sysykeji.top/gtapmqiprk.html

[A08] 取整与四舍五入
来源：http://hz.jqgfzy.top/gtvzfyvffj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinqigufen.top/gtynekamox.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yongpay.top/gtigdsuapt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinqigfzy.top/gtfizltswm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ppjwa.cn/gtytsstopf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zycfv.cn/gttpdcfojr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tian-w.cn/gtkqjvtzma.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.pycfn.com/gtwmwdsjoo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.bjfxy.top/gthvrihdmz.html

[A09] 绝对值与最大最小值
来源：http://hz.mhx1999.top/gtailengiz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jyoumei.cn/gtndynindp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.haohaochexian.top/gtwhsfjwpf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.sxryk.cn/gtsrqvgmka.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.0kj1m.cn/gtrmdbddzh.html


<!-- 参考信息 -->