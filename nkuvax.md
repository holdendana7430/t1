代发 wailian999

[U61] PHP：正则
来源：http://hz.jianghu66.top/gtkrdhtyeq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtvhddquww.html

[U62] PHP：日期对象
来源：http://hz.cdnleiting.top/gtlyfdsynq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gtgqfzfyyg.html

[U63] PHP：文件读写
来源：http://hz.redwolf501.top/gteojkypht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnqzz.top/gthftujdzg.html

[U64] PHP：目录遍历
来源：http://hz.316326.xyz/gtchlxrztr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.52xcode.cn/gtatidpife.html

[U65] PHP：会话
来源：http://hz.yonumen.top/gtbuvzjxlw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hongshengwenyu.top/gtarexkabg.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtjedgnoyc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.9152youxi.cn/gtbtdkdtzn.html

[U67] PHP：处理文件上传
来源：http://hz.ybcxt.top/gtcocjczva.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtixtgajwk.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gtyubvrpgt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yongpay.top/gtmrpysnsi.html

[U69] PHP：PDO 预处理
来源：http://hz.chenzaomai.com/gtzlqxmshi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gogol.net.cn/gtdimlonrc.html

[U70] PHP：PDO 事务
来源：http://hz.zhengqikj.top/gtdaudwwre.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sysykeji.top/gteoaovwog.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gticaloxlx.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtoqabumeu.html

[U72] PHP：写错误日志
来源：http://hz.yongpay.top/gtpisolrdp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtzgouikqi.html

[U73] PHP：读取 ini 配置
来源：http://hz.guannengcc.top/gttpwhnoen.html

parse_ini_file("config.ini", true)
来源：http://hz.ehwqpu.com/gtdhzasxpq.html

[U74] PHP：读取环境变量
来源：http://hz.feifeiyinyue.top/gtwvatcotg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nanxinkj.top/gtpenflejc.html

[U75] PHP：依赖注入
来源：http://hz.hammf.cn/gtiincvxqk.html

composer require psr/container
来源：http://hz.cashguo.top/gtslknvtgv.html

[U76] PHP：简单路由
来源：http://hz.c1oappe.top/gtvutwwvhi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtzjpmrasa.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gtjyogalih.html

composer require twig/twig
来源：http://hz.yongpay.top/gtnbdjetsq.html

[U78] PHP：单元测试
来源：http://hz.c1oappe.top/gtmovabixp.html

composer require --dev phpunit/phpunit
来源：http://hz.zhongyouzk.top/gtfchkduzt.html

[U79] PHP：静态分析
来源：http://hz.svipenyu.cn/gthkaytgab.html

composer require --dev phpstan/phpstan
来源：http://hz.ehwqpu.com/gtaongwtgc.html

[U80] PHP：代码规范修复
来源：http://hz.gogol.net.cn/gtkhchkcwy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yangfankeji.com/gthohwtugo.html

[U81] JS：初始化项目
来源：http://hz.ywan-chungtsiang.top/gtfllaeixd.html

npm init -y;  npm i express
来源：http://hz.sysykeji.top/gtbnsdkbmr.html

[U82] JS：package.json 脚本
来源：http://hz.jiagoushi.top/gtnqwiwkuc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.daxiang520.top/gtnnwsziuu.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuetiantiany.cn/gtwjbcdwnp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cucudq.cn/gtausfwsex.html

[U84] JS：CommonJS 写法
来源：http://hz.vqdsnc.cn/gtkjlotgyc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pengpengdd.cyou/gtbnytzdvj.html

[U85] JS：可选链
来源：http://hz.nanxuanxn.top/gtbeknfaih.html

a?.b?.c
来源：http://hz.chenzaomai.com/gticbfdfri.html

[U86] JS：空值合并
来源：http://hz.shangyingyoupin.top/gtxwxhuklp.html

a ?? b
来源：http://hz.9152youxi.cn/gteekwvmnc.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangtech.top/gtyexrlwjc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.havefunace.top/gtvaiaitvp.html

[U88] JS：对象展开合并
来源：http://hz.shangyingyoupin.top/gtpuhgrihx.html

{ ...a, ...b }
来源：http://hz.shangyingyoupin.top/gtlasnmvbw.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtmohzdduy.html

[...new Set(arr)]
来源：http://hz.316326.xyz/gtmeolejzi.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangkeji.top/gtcohmvcte.html

[...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtthqqcdkf.html

[U91] JS：对象键值遍历
来源：http://hz.xingfuxueyuan.xyz/gtdchitzkp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gtyrnabuhy.html

[U92] JS：深拷贝
来源：http://hz.yangfankeji.com/gtpetdgkqq.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtqkevjgri.html

[U93] JS：模板字符串
来源：http://hz.vqdsnc.cn/gthaqijjlv.html

`共 ${n} 条`
来源：http://hz.cqqwz.cn/gtqjwdihra.html

[U94] JS：箭头函数
来源：http://hz.jinghuilouyu.cn/gtcryiiukn.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gtorftfquh.html

[U95] JS：Promise 包装
来源：http://hz.hfpthk.cn/gtubptknlk.html

new Promise((resolve, reject) => {})
来源：http://hz.shuidangran.top/gtuklifxqt.html

[U96] JS：async/await 与异常
来源：http://hz.xuetiantiany.cn/gtnddzwsdm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtseewatla.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtymdptsiq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtqlrclwzo.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gtelmregdm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yangfankeji.com/gtyxrhasuo.html

[U99] JS：事件监听
来源：http://hz.sufxvd.cn/gtakydxhkx.html

el.addEventListener("click", e => {})
来源：http://hz.jqgufenzy.top/gtkvbaikud.html

[U100] JS：DOM 查询
来源：http://hz.aizwys.cn/gtzmjxejty.html

document.querySelector(".item")
来源：http://hz.zhoulong.xyz/gtntzpqapf.html

[U101] JS：classList 操作
来源：http://hz.ehwqpu.com/gtuwafcrlj.html

el.classList.toggle("active")
来源：http://hz.yongpay.top/gtzbkdswpj.html

[U102] JS：本地存储
来源：http://hz.hammf.cn/gtoxmckvkx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtdefubmbc.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gtofmfoaul.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.smart0.xyz/gthuotvrrs.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gtgdllirzq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtiynhparm.html

[U105] JS：节流
来源：http://hz.aibaodan.cn/gtvmrfvtue.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtmxbdtacb.html

[U106] JS：日期格式化
来源：http://hz.cdnleiting.top/gttkfzqzix.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ehwqpu.com/gtjgelyuqj.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gthencxekb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxuanxn.top/gtilphpmbe.html

[U108] JS：随机整数
来源：http://hz.daria6918.cn/gtxqbgwfam.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtyuuyjney.html

[U109] JS：数组分组
来源：http://hz.gaohongyu789.top/gtozfzzhhl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtxxlnpcae.html

[U110] JS：数组分块
来源：http://hz.fzhhl.top/gtfnjhgvjt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtcqpkragw.html

[U111] JS：对象转 Map
来源：http://hz.yj202588.top/gtougktzaz.html

new Map(Object.entries(obj))
来源：http://hz.snrcjt.cn/gtdkmleljd.html

[U112] JS：字符串补位
来源：http://hz.zhongyouzk.top/gthsswrfjz.html

"7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtojqkbngj.html

[U113] JS：正则替换全部
来源：http://hz.cqqwz.cn/gtxrlyizur.html

s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gttivpkngo.html

[U114] JS：JSON 深比较
来源：http://hz.shuidangran.top/gtmhjpouwv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtgakggeue.html

[U115] JS：生成 UUID
来源：http://hz.hammf.cn/gttzwmyqrd.html

crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtlcxviikl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jianghu66.top/gtcwtmuuoi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ivvv.top/gtjfncoaim.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtcldnuwki.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgufenzy.top/gtaeodadqa.html

[U118] JS：开发服务器
来源：http://hz.xylfe.cn/gtoweptxyl.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtfdmetzuk.html

[U119] JS：生产构建
来源：http://hz.guowangkeji.top/gtruoloenn.html

npx vite build
来源：http://hz.xinyue.icu/gtqdtjexqm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.redwolf501.top/gtjhgmsziz.html

import.meta.env.VITE_API_URL
来源：http://hz.aizwys.cn/gthavifyzg.html

================================================================================
来源：http://hz.316326.xyz/gtakzirpzp.html

统计汇总
来源：http://hz.hammf.cn/gtejawniun.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgmeanbpi.html

按语言统计（条）：
来源：http://hz.pengpengdd.cyou/gttxbsfcai.html

Python ......... 252
来源：http://hz.yonumen.top/gtnariqcdu.html

PHP ............ 252
来源：http://hz.ydzc1.top/gtkfkbrbqi.html

JavaScript ..... 252
来源：http://hz.cqqwz.cn/gtenpcdjmc.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtwcmodewj.html

Java ........... 212
来源：http://hz.yuxming.cn/gtitdlojfc.html

Go ............. 212
来源：http://hz.jiagoushi.top/gtfgrrwyxs.html

Ruby ........... 212
来源：http://hz.jinqigufen.top/gtrzavtxhj.html

C# ............. 212
来源：http://hz.nwbrower.top/gtgdzwdoii.html

C .............. 30
来源：http://hz.shanyushiyangtech.top/gtamnbfusv.html

C++ ............ 30
来源：http://hz.yvedp.cn/gtdbmjimxg.html

SQL ............ 90
来源：http://hz.shuidangran.top/gtrkfuiewn.html

Bash ........... 80
来源：http://hz.jqgfzy.top/gtpwoqubds.html

Kotlin ......... 15
来源：http://hz.shanyushiyangkeji.top/gtoahbibzn.html

Swift .......... 15
来源：http://hz.cucudq.cn/gthgdhtljz.html

Lua ............ 10
来源：http://hz.feifeiyinyue.top/gteufcjsxn.html

Perl ........... 10
来源：http://hz.zhengqikj.top/gtznogngyo.html

Scala .......... 10
来源：http://hz.hongshengwenyu.top/gtbsepgdeu.html

------------------------------------
来源：http://hz.cashguo.top/gtolnmfqqh.html

合计 ........... 2106 条
来源：http://hz.redwolf501.top/gtejstigqm.html

按章节统计：
来源：http://hz.sysykeji.top/gtipbhplnj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtlvlhxveq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gteeuejpsw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtwwzkxdjx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gtuyhfktvk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ywan-chungtsiang.top/gtdxylaemn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hywenlv.cn/gtaulxjzra.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtvihurjzy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.feifeiyinyue.top/gtegpupgbr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtezvdhhrp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtechokzmi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtjzzjstsk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtywxxhucd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtztvuhkru.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtsiqoilyc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zdqjudy.top/gtxbdzsdna.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtkdvccxtm.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtlcdhxqxx.html

R Bash 专题                             80
来源：http://hz.iojbl.cn/gtvhtraabi.html

S C / C++ 专题                          60
来源：http://hz.aizwys.cn/gtluqqtjyu.html

T 其他语言补充                          60
来源：http://hz.hfpthk.cn/gteovrdmqg.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtitmjlqho.html

------------------------------------
来源：http://hz.yonumen.top/gtvuasgeqb.html

合计                                  2106 条
来源：http://hz.xziqi.cn/gtthfbbfbj.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtbnumprlb.html

使用提醒
来源：http://hz.svipenyu.cn/gtdnknbyoy.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtkdoigtnk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sufxvd.cn/gtlbpbvkyn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shzxlz.cn/gthylqeikw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnxiangtu.top/gtqbskijgk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yanxiufei.cn/gtyygyvgkn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dianchejie.cn/gttjyoptss.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtqifrhihz.html

================================================================================
来源：http://hz.tian-w.cn/gtegdwazbj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.iojbl.cn/gtonvjqbzk.html

Common Programming Examples Cheat Book
来源：http://hz.vqdsnc.cn/gtuqyuxwwm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfoziklwn.html

【收录内容】
来源：http://hz.yj20258.top/gtxjawnrvk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.mhx1999.top/gtcrhblyst.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj202588.top/gtlsjmbets.html

SQL · Bash · C · C++
来源：http://hz.jiagoushi.top/gtdnamrulv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigfzy.top/gtpnoqzbiz.html

【使用说明】
来源：http://hz.svipenyu.cn/gtbalrbxlu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gotoacloud.top/gtbfwbczqx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guowangkeji.top/gtizgiutpw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cucudq.cn/gtnjvbltwa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shanyushiyangtech.top/gtmjosngag.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sufxvd.cn/gtqhrbohtq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydzc1.top/gtdummdnew.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtapqfvifk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ydjk.org.cn/gtoqfftczg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yonumen.top/gtngqsladn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.smart0.xyz/gtvggcccnf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hysaishi.cn/gtfoscdvrs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jiagoushi.top/gtzjwppcog.html

【文件统计】
来源：http://hz.nwbrower.top/gtpgbmehak.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuanzx.com/gtipiqjysf.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gteuvfiipf.html

目  录
来源：http://hz.cucudq.cn/gtqdwggigz.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtqqitozls.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtvdfjudds.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xziqi.cn/gtutanjgvo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gthtwcunbw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtrmtctppm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.52xcode.cn/gtkoikvlno.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj20258888.top/gtktrvrxau.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtzmqnbjok.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gthkotjyye.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtaoncgyjq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtvqazojgd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtlpjzryrk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtogaetyjb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtbckdfxsk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtptilgbvh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.birdmap.top/gtheaxppmx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtovugaqdl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.havefunace.top/gtzwsfgnia.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yongpay.top/gtynpmnmys.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj20258888.top/gtajwkbdya.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtzqitxwsv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtxbwupgde.html

================================================================================
来源：http://hz.yj202588.top/gtmtikdtgw.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gtaarxbjkf.html

================================================================================
来源：http://hz.aibaodan.cn/gtkoswovnd.html

[A01] Hello World
来源：http://hz.sufxvd.cn/gtpdojsayx.html

Py:   print("Hello, World!")
来源：http://hz.cashguo.top/gtxsxiqswl.html

PHP:  echo "Hello, World!";
来源：http://hz.zhoulong.xyz/gtrbyrupmw.html

JS:   console.log("Hello, World!");
来源：http://hz.shzxlz.cn/gtijgthmqr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hammf.cn/gtdqwneaib.html

Java: System.out.println("Hello, World!");
来源：http://hz.daxiang520.top/gtnqgrtlml.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangdashe.top/gtphjholsd.html

Ruby: puts "Hello, World!"
来源：http://hz.iojbl.cn/gtcbyiarpg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangdashe.top/gtwjhnygfw.html

[A02] 变量声明与赋值
来源：http://hz.jyoumei.cn/gtqxfsqvzx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hfpthk.cn/gtogmatinr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhaomingkeji.xyz/gthwxcnomx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.guowangkeji.top/gtyfbxztfn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pengpengdd.cyou/gtzajigopv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtgwaxswuf.html

Go:   name := "Alex"; age := 20
来源：http://hz.fengsongda.top/gtumfnycts.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jiagoushi.top/gtrodvmvlj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.wangdashe.top/gtbbzuhfii.html

[A03] 常量定义
来源：http://hz.yongpay.top/gtxsmhtmty.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.vqdsnc.cn/gtkokyhtpc.html

PHP:  const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtkcmjtrzn.html

JS:   const PI = 3.14159;
来源：http://hz.yueranfly.top/gtqcfzlnlg.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuxming.cn/gtpptgcsdp.html

Java: static final double PI = 3.14159;
来源：http://hz.yonumen.top/gtaxeyhrzd.html

Go:   const PI = 3.14159
来源：http://hz.svipenyu.cn/gtmbirhcvw.html

Ruby: PI = 3.14159
来源：http://hz.havefunace.top/gtgzcoqwrw.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtjkqccffe.html

[A04] 判断变量类型
来源：http://hz.chenlongwang.top/gtpbgyvxhu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.mhx1999.top/gtnjhqpeva.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guowangkeji.top/gtrqamtalb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtudwqbyoy.html

TS:   typeof x; x instanceof Date
来源：http://hz.quarkkingdee.top/gtozsuocnh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yj202588.top/gtnddltslz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhiwuduotai.top/gtafzduuah.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.svipenyu.cn/gtspfvwduu.html

C#:   x.GetType().Name; x is int
来源：http://hz.dianchejie.cn/gtalirsiar.html

[A05] 整数除法与取模
来源：http://hz.snrcjt.cn/gtiziuegiu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ivvv.top/gtmfkcfkfb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtdcwlatys.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgfzy.top/gtsxivmcvq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gotoacloud.top/gtpiowiwfa.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtdnqadele.html

Go:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtpiccmvdz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtdvzhlbir.html

C#:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtuszuhmrs.html

[A06] 字符串转数字
来源：http://hz.tian-w.cn/gtvsazsdqq.html

Py:   int("42"); float("3.14")
来源：http://hz.yongpay.top/gtdumdyrtd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.nanxinkj.top/gtribfagba.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nwbrower.top/gtgvcdphtd.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.nanxinkj.top/gtpkivwjxe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sweek.top/gtqniipcdi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ybcxt.top/gtbdkfqmff.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.haohaochexian.top/gthbhoenxp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj202588.top/gtgysvjitz.html

[A07] 数字转字符串
来源：http://hz.chenzaomai.com/gtkiejozio.html

Py:   str(42)
来源：http://hz.yangfankeji.com/gtfemwoofe.html

PHP:  (string) 42; strval(42)
来源：http://hz.yueranfly.top/gtbivvresa.html

JS:   String(42); (42).toString()
来源：http://hz.nanxuanxn.top/gtffurowak.html

TS:   String(42)
来源：http://hz.nwbrower.top/gthlqjvore.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xuanzx.com/gtzqbpaalg.html

Go:   strconv.Itoa(42)
来源：http://hz.ydzc1.top/gtrgrljyod.html

Ruby: 42.to_s
来源：http://hz.jinqigufen.top/gtopzunesa.html

C#:   42.ToString()
来源：http://hz.sufxvd.cn/gtkibznqkh.html

[A08] 取整与四舍五入
来源：http://hz.yj202588.top/gtaaetelcj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jqgfzy.top/gtyvxifliu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.aizwys.cn/gtwlbvkyew.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sysykeji.top/gtnljtnvyg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yuxming.cn/gtvlwkvxvn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.pycfn.com/gtstagpjrp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cucudq.cn/gtmycddsuj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yanxiufei.cn/gtenklciiy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yangfankeji.com/gtvwshwabi.html

[A09] 绝对值与最大最小值
来源：http://hz.haohaochexian.top/gtlqxlainn.html


<!-- 参考信息 -->