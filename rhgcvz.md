代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.ydzc1.top/gtxudofmgv.html

"值: {$a}"
来源：http://hz.xylfe.cn/gtxcjtdbmn.html

[U58] PHP：数组三件套
来源：http://hz.hnqzz.top/gtkjhyhfjl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.0kj1m.cn/gttdizmzkb.html

[U59] PHP：自定义排序
来源：http://hz.ybcxt.top/gtauwgsogd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtutcgbstt.html

[U60] PHP：JSON 编解码
来源：http://hz.jinghuilouyu.cn/gtmcekrisb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nanxuanxn.top/gtsrsicphv.html

[U61] PHP：正则
来源：http://hz.gzhubu.top/gtrnpilfnf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtvsrwlrwo.html

[U62] PHP：日期对象
来源：http://hz.gzhubu.top/gtssqqkfic.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gtyppvjzjx.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtpxfqxapk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ybcxt.top/gtatbdublo.html

[U64] PHP：目录遍历
来源：http://hz.ywan-chungtsiang.top/gtdibhqkns.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hywenlv.cn/gtjqzsjgon.html

[U65] PHP：会话
来源：http://hz.jqgfzy.top/gtfybmlmmf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtzvtigihf.html

[U66] PHP：设置 Cookie
来源：http://hz.hnqzz.top/gtqoukvjyk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.havefunace.top/gtqwihaumj.html

[U67] PHP：处理文件上传
来源：http://hz.c1oappe.top/gtsjhrseiy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtkgpmdelf.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtjjomoiss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xylfe.cn/gttyftsgau.html

[U69] PHP：PDO 预处理
来源：http://hz.c1oappe.top/gtlwtagkbs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xingfuxueyuan.xyz/gtocaqvjss.html

[U70] PHP：PDO 事务
来源：http://hz.meibo888.top/gtuycbospe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xylfe.cn/gtjpqxwliw.html

[U71] PHP：抛出异常
来源：http://hz.c1oappe.top/gtbxgkocvt.html

throw new RuntimeException("失败", 500);
来源：http://hz.fzhhl.top/gtfwgdtcme.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gthnarjfov.html

error_log("失败: " . $e->getMessage());
来源：http://hz.vqdsnc.cn/gtdwmxlkjs.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gtzlcpzeaz.html

parse_ini_file("config.ini", true)
来源：http://hz.fengsongda.top/gtltpgrvcc.html

[U74] PHP：读取环境变量
来源：http://hz.yongpay.top/gtcwclkhct.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cheryme.top/gtsaqskbrw.html

[U75] PHP：依赖注入
来源：http://hz.zhengqikj.top/gtddesenuh.html

composer require psr/container
来源：http://hz.yongpay.top/gtqsobtydj.html

[U76] PHP：简单路由
来源：http://hz.xuetiantiany.cn/gtvcuvemnh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.bjfxy.top/gtwlmldtrw.html

[U77] PHP：模板渲染
来源：http://hz.cucudq.cn/gtcyddjwyh.html

composer require twig/twig
来源：http://hz.shanyushiyangkeji.top/gtguivjnlv.html

[U78] PHP：单元测试
来源：http://hz.yuanzhike.top/gtyteahtpm.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtozviuepa.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtkydqzmhg.html

composer require --dev phpstan/phpstan
来源：http://hz.yonumen.top/gtkdtyjxxf.html

[U80] PHP：代码规范修复
来源：http://hz.jinqigufen.top/gtceaihbmt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhengqikj.top/gtlsdalnmb.html

[U81] JS：初始化项目
来源：http://hz.jinqigfzy.top/gtdehvawjt.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtavdtwsam.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258888.top/gtatutduvn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.havefunace.top/gtqkrvioyc.html

[U83] JS：ES Module 导入导出
来源：http://hz.sweek.top/gtrgjkmlct.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yongpay.top/gtwdrsadti.html

[U84] JS：CommonJS 写法
来源：http://hz.aibaodan.cn/gtckoxoxkr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jqgufenzy.top/gthaovdtlv.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtvozryquh.html

a?.b?.c
来源：http://hz.ydzc1.top/gthbusocdw.html

[U86] JS：空值合并
来源：http://hz.fengsongda.top/gtgtyjuilc.html

a ?? b
来源：http://hz.cheryme.top/gtchtyuqoq.html

[U87] JS：解构默认值
来源：http://hz.yongpay.top/gtglpwsssq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hywenlv.cn/gtndoxatcv.html

[U88] JS：对象展开合并
来源：http://hz.9152youxi.cn/gtoctoeneh.html

{ ...a, ...b }
来源：http://hz.snrcjt.cn/gthdmipysj.html

[U89] JS：数组去重
来源：http://hz.gaohongyu789.top/gtprpffhtl.html

[...new Set(arr)]
来源：http://hz.c1oappe.top/gtcsovfoum.html

[U90] JS：数字数组排序
来源：http://hz.snrcjt.cn/gtpcgvxlyi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtnejsklak.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtcxrwvupv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nanxinkj.top/gthrmpecfu.html

[U92] JS：深拷贝
来源：http://hz.tian-w.cn/gtjvzodvzf.html

structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtctibcpwm.html

[U93] JS：模板字符串
来源：http://hz.zdqjudy.top/gtqjzzbhme.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gtrvrohytq.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtilyeanrs.html

const double = x => x * 2;
来源：http://hz.chenjidiqi.icu/gtthqkiiqh.html

[U95] JS：Promise 包装
来源：http://hz.xingfuxueyuan.xyz/gtjpkzwnrq.html

new Promise((resolve, reject) => {})
来源：http://hz.yonumen.top/gtmzvoowsa.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtncczacwi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtzsuqfucw.html

[U97] JS：并发请求
来源：http://hz.dianchejie.cn/gtualrjlbw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtorudoion.html

[U98] JS：fetch 带 JSON
来源：http://hz.yongpay.top/gtcexqguoh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258888.top/gtusmbudkz.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtjcgtiivb.html

el.addEventListener("click", e => {})
来源：http://hz.ivvv.top/gtxbxunnhz.html

[U100] JS：DOM 查询
来源：http://hz.yueranfly.top/gtzelkmnnl.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtptnducyf.html

[U101] JS：classList 操作
来源：http://hz.kuanghao11.cn/gtcyhbvgts.html

el.classList.toggle("active")
来源：http://hz.guowangkeji.top/gtjcxwnkqg.html

[U102] JS：本地存储
来源：http://hz.316326.xyz/gtipggcgyc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guannengcc.top/gtzfxtvcvj.html

[U103] JS：定时器
来源：http://hz.zhiwuduotai.top/gtnarahnry.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinghuilouyu.cn/gtndpqqkon.html

[U104] JS：防抖
来源：http://hz.svipenyu.cn/gtzsvtrvfw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtwytczcwq.html

[U105] JS：节流
来源：http://hz.cashguo.top/gtmqmltmyz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gaohongyu789.top/gtdlxdvqto.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtkukhwhaw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zdqjudy.top/gtbjvlrbvc.html

[U107] JS：数字千分位
来源：http://hz.jinqigfzy.top/gtxfpzhjbm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtedprfmwr.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtianpevwy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtntdvwofd.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtbehqbhhp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtontsecad.html

[U110] JS：数组分块
来源：http://hz.0kj1m.cn/gtuktdkfkz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangshuangyany.cn/gtbmxrpape.html

[U111] JS：对象转 Map
来源：http://hz.bjfxy.top/gtualmdzzv.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gthvucnozj.html

[U112] JS：字符串补位
来源：http://hz.xuetiantiany.cn/gtcfusihyy.html

"7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtaackfcko.html

[U113] JS：正则替换全部
来源：http://hz.ydzc1.top/gtdgljydvu.html

s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtmpfkqhgu.html

[U114] JS：JSON 深比较
来源：http://hz.xuetiantiany.cn/gthltvzugw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtkqkudrmc.html

[U115] JS：生成 UUID
来源：http://hz.vqdsnc.cn/gtergnumve.html

crypto.randomUUID()
来源：http://hz.mhx1999.top/gtsljeomqs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yangfankeji.com/gtzuitkejp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pengpengdd.cyou/gtyusqolog.html

[U117] JS：单元测试
来源：http://hz.aizwys.cn/gtxlrvwaqc.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gtchswufxe.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtbufugglc.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gtotxyzfan.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gtzafnizcu.html

npx vite build
来源：http://hz.sxryk.cn/gtfevpshzg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ywan-chungtsiang.top/gtrhnsohgt.html

import.meta.env.VITE_API_URL
来源：http://hz.jyoumei.cn/gtkeitxynk.html

================================================================================
来源：http://hz.cashguo.top/gtdkuljhhb.html

统计汇总
来源：http://hz.daria6918.cn/gtupnkibxd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcphjfwvt.html

按语言统计（条）：
来源：http://hz.hywenlv.cn/gtpztvmcgy.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtgbphiruf.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtkqipmmqd.html

JavaScript ..... 252
来源：http://hz.ywan-chungtsiang.top/gtgxbqanax.html

TypeScript ..... 212
来源：http://hz.tian-w.cn/gthfsknves.html

Java ........... 212
来源：http://hz.iojbl.cn/gtzbzflctl.html

Go ............. 212
来源：http://hz.jqgfzy.top/gtckgfgskh.html

Ruby ........... 212
来源：http://hz.zhengqikj.top/gtnmqodszc.html

C# ............. 212
来源：http://hz.zycfv.cn/gtstbwdtmq.html

C .............. 30
来源：http://hz.yongpay.top/gtefhirsyu.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtsdizebdx.html

SQL ............ 90
来源：http://hz.jinyuanbaomall.cn/gtzaqxnzca.html

Bash ........... 80
来源：http://hz.daxiang520.top/gtafbohehe.html

Kotlin ......... 15
来源：http://hz.hywenlv.cn/gtkjczyrnr.html

Swift .......... 15
来源：http://hz.hysaishi.cn/gtpltmnmbn.html

Lua ............ 10
来源：http://hz.meibo888.top/gtvsyycruy.html

Perl ........... 10
来源：http://hz.hywenlv.cn/gtkzspkdhv.html

Scala .......... 10
来源：http://hz.guannengcc.top/gtuwzhtkma.html

------------------------------------
来源：http://hz.jianghu66.top/gttbiofjas.html

合计 ........... 2106 条
来源：http://hz.sxryk.cn/gteyzyjtqj.html

按章节统计：
来源：http://hz.ivvv.top/gtoygplzcg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtnuriddgq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gthhtyocfp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtcnyezkpv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.guannengcc.top/gtgxxjfjgf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xuanzx.com/gtoqbovtik.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gttanzdtav.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtxwhxjryg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cdnleiting.top/gtdfhjuuvr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtktqpzonh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xuetiantiany.cn/gtgfjqstlh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtfufzmltv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtvkwalchr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtbcunfmka.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gtxigmpguc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gaohongyu789.top/gtvgdcqyjl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtlxsaxqzn.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtgysamzmc.html

R Bash 专题                             80
来源：http://hz.sysykeji.top/gtydrfhvry.html

S C / C++ 专题                          60
来源：http://hz.hywenlv.cn/gthowgeiwx.html

T 其他语言补充                          60
来源：http://hz.xuanzx.com/gttsgjuytg.html

U 高频实用片段                         120
来源：http://hz.quarkkingdee.top/gttximgqld.html

------------------------------------
来源：http://hz.ivvv.top/gtgzzehxct.html

合计                                  2106 条
来源：http://hz.yonumen.top/gtgowmyjlm.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtvtpwfywy.html

使用提醒
来源：http://hz.wangdashe.top/gtgiuzmkit.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtwgsplpwj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtzsoxxtin.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zycfv.cn/gtcuatwpcq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhixingplan.top/gtnxprwqqf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yangfankeji.com/gtbzndmnfa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zycfv.cn/gtuzulmdte.html

—— 文件结束 ——
来源：http://hz.shanyushiyangtech.top/gtdtyhlknl.html

================================================================================
来源：http://hz.0kj1m.cn/gtoblqdhch.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.svipenyu.cn/gtmwuxgbab.html

Common Programming Examples Cheat Book
来源：http://hz.fzhhl.top/gtluphuoxg.html

================================================================================
来源：http://hz.xuanzx.com/gthqrnmhex.html

【收录内容】
来源：http://hz.nanxuanxn.top/gtylrdcqqf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtmzjvywsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.guannengcc.top/gtjpzuhjjp.html

SQL · Bash · C · C++
来源：http://hz.chenlongwang.top/gtpfdbzkcj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jqgfzy.top/gtrvwprphz.html

【使用说明】
来源：http://hz.shzxlz.cn/gtgendaauj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhengqikj.top/gtijvoadnq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shanyushiyangkeji.top/gtyhluxahy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.daxiang520.top/gtrgxafpiu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dianchejie.cn/gtpkxxjqjm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.smart0.xyz/gthpsvpezd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.birdmap.top/gtitcrrovi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cqqwz.cn/gttmugqyvb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xylfe.cn/gtgjnzwvrc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shanyushiyangtech.top/gtxckdkvav.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gzhubu.top/gtlknwytgk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinyuanbaomall.cn/gtjwaovfgs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hammf.cn/gtnnnpjdch.html

【文件统计】
来源：http://hz.haohaochexian.top/gtmyndzall.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cashguo.top/gtgsozkmfn.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtzytqokgm.html

目  录
来源：http://hz.ivvv.top/gtrqsdlocx.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtcnhlfims.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dashuyun.cn/gtlsxcmmgh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtuypebfwk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtvkyyichr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.mhx1999.top/gtcqhmetcb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tian-w.cn/gtgklaszol.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtvekypzgx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtuwccbzrd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtgkejuvcg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtucqcqvjr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtqdzqujhv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtdkjilfry.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtqvhhisda.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtzawgenjn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gttmzcjrde.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj202588.top/gtzfxomndd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.dashuyun.cn/gtfowoftij.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhaomingkeji.xyz/gtjaiwyins.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangtech.top/gtxmrrdkft.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj202588.top/gthenuzepb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtujtgvhui.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gtoottkgck.html

================================================================================
来源：http://hz.chenlongwang.top/gtelonilve.html

A. 基础语法与类型
来源：http://hz.snrcjt.cn/gtivzqhmpl.html

================================================================================
来源：http://hz.iojbl.cn/gtinbnwstg.html

[A01] Hello World
来源：http://hz.zhiwuduotai.top/gtnjadjvbv.html

Py:   print("Hello, World!")
来源：http://hz.52xcode.cn/gtpvopnybm.html

PHP:  echo "Hello, World!";
来源：http://hz.zdqjudy.top/gtuvminqem.html

JS:   console.log("Hello, World!");
来源：http://hz.smart0.xyz/gtscrvpqkc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtbanoooej.html

Java: System.out.println("Hello, World!");
来源：http://hz.sysykeji.top/gtcndgaiaq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xinyue.icu/gtpijcbrsi.html

Ruby: puts "Hello, World!"
来源：http://hz.andypj.xyz/gtnsumgaes.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gotoacloud.top/gtnqokobih.html

[A02] 变量声明与赋值
来源：http://hz.xylfe.cn/gthdplfexz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sufxvd.cn/gtdzzepknc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.feifeiyinyue.top/gtjmeyqyie.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.feifeiyinyue.top/gtcqmspjek.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj202588.top/gtmhavuspp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.havefunace.top/gtxfzyztpg.html

Go:   name := "Alex"; age := 20
来源：http://hz.sysykeji.top/gtsgaedynn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.snrcjt.cn/gtqwmmasxz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zycfv.cn/gtjgpwhkbh.html

[A03] 常量定义
来源：http://hz.ppjwa.cn/gtxofdymdb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cashguo.top/gtxywjhdwj.html

PHP:  const PI = 3.14159;
来源：http://hz.hnqzz.top/gtczcnhlsv.html

JS:   const PI = 3.14159;
来源：http://hz.yueranfly.top/gtmqrqiyfu.html

TS:   const PI: number = 3.14159;
来源：http://hz.daxiang520.top/gtxpjlnqoa.html

Java: static final double PI = 3.14159;
来源：http://hz.316326.xyz/gtwqcjgyuy.html

Go:   const PI = 3.14159
来源：http://hz.hywenlv.cn/gtjhcgplar.html

Ruby: PI = 3.14159
来源：http://hz.dianchejie.cn/gtjenwjgiw.html

C#:   const double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtwhjrxsnn.html

[A04] 判断变量类型
来源：http://hz.aibaodan.cn/gttdplwkpi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shzxlz.cn/gtfumjsjds.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.nanxuanxn.top/gtcuwxkcrf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aizwys.cn/gtgewnqusb.html

TS:   typeof x; x instanceof Date
来源：http://hz.bjfxy.top/gtdtjdyiwg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yongpay.top/gtnhubimyf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shanyushiyangtech.top/gteepmsvtn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.chenlongwang.top/gtjidacjxr.html

C#:   x.GetType().Name; x is int
来源：http://hz.0kj1m.cn/gtablvxtjm.html

[A05] 整数除法与取模
来源：http://hz.pengpengdd.cyou/gtyawunhil.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gzhubu.top/gtnrjfunbg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fzhhl.top/gtkiqarwex.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gzhubu.top/gtrdjaarxo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zdqjudy.top/gtindqblvr.html

Java: 7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gttysvllae.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtdpmcwcwl.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtnpdstvik.html

C#:   7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtmlcmmfbc.html

[A06] 字符串转数字
来源：http://hz.jiagoushi.top/gtskiwhnhk.html

Py:   int("42"); float("3.14")
来源：http://hz.nwbrower.top/gtxyqmmnrf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.haohaochexian.top/gtezrdkvrw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.kuanghao11.cn/gtztjxhkpw.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hysaishi.cn/gtrfycsghd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cucudq.cn/gtetmeaxwf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hnqzz.top/gthwopybcm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nwbrower.top/gtinrsxkjs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhongyouzk.top/gttipfollg.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtsfnndifg.html

Py:   str(42)
来源：http://hz.jlsjyb.cn/gtosyhmuzh.html

PHP:  (string) 42; strval(42)
来源：http://hz.hammf.cn/gtjuicqsms.html

JS:   String(42); (42).toString()
来源：http://hz.haohaochexian.top/gtauzvnqlj.html

TS:   String(42)
来源：http://hz.tanke756.top/gtygzpoiwg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.havefunace.top/gtnqafkznf.html

Go:   strconv.Itoa(42)
来源：http://hz.nwbrower.top/gtqasntumm.html

Ruby: 42.to_s
来源：http://hz.sxryk.cn/gtshtlewje.html

C#:   42.ToString()
来源：http://hz.cdnleiting.top/gtyvuqaleo.html

[A08] 取整与四舍五入
来源：http://hz.c1oappe.top/gtrajmjbtp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtggxsxewj.html


<!-- 参考信息 -->