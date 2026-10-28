代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.guowangkeji.top/gtuqrhhron.html

$v = $a ?? $b ?? "default";
来源：http://hz.cucudq.cn/gtyxxlsvmf.html

[U54] PHP：空安全调用
来源：http://hz.shangyingyoupin.top/gtojxkaoby.html

$obj?->method()
来源：http://hz.aibaodan.cn/gtacajklex.html

[U55] PHP：match 表达式
来源：http://hz.dianchejie.cn/gtwzdlxorc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yuanzhike.top/gtejulsltm.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gttqjcgzqf.html

f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtphruurca.html

[U57] PHP：字符串插值
来源：http://hz.nanxinkj.top/gtgeqoelpc.html

"值: {$a}"
来源：http://hz.guowangkeji.top/gtwjdirhro.html

[U58] PHP：数组三件套
来源：http://hz.birdmap.top/gtqoyhtpfj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hysaishi.cn/gtrfaliuik.html

[U59] PHP：自定义排序
来源：http://hz.hnqzz.top/gtsdoguvgm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtutxeuahv.html

[U60] PHP：JSON 编解码
来源：http://hz.xziqi.cn/gtbrwvsopq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gaohongyu789.top/gtvlgjrxyr.html

[U61] PHP：正则
来源：http://hz.cqqwz.cn/gtthosbiml.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtgagvcose.html

[U62] PHP：日期对象
来源：http://hz.nanxinkj.top/gtoiytvcwk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ehwqpu.com/gtefauefee.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gtogqipfoe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shuidangran.top/gtknqcyvae.html

[U64] PHP：目录遍历
来源：http://hz.ydjk.org.cn/gtwryesvxy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.andypj.xyz/gtjrebdxfs.html

[U65] PHP：会话
来源：http://hz.52xcode.cn/gtxhczpnfg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.c1oappe.top/gtnssbfuun.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gthvgbrake.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.chenjidiqi.icu/gtvjosokwb.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigufen.top/gttpxlifpp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pengpengdd.cyou/gtcvitrldh.html

[U68] PHP：PDO 连接
来源：http://hz.jyoumei.cn/gtzqjjkqfv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtkcigyrkn.html

[U69] PHP：PDO 预处理
来源：http://hz.cashguo.top/gtjoegvwug.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnqzz.top/gtzqlicdug.html

[U70] PHP：PDO 事务
来源：http://hz.hammf.cn/gtcfzrfeyc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jlsjyb.cn/gtoaafyecv.html

[U71] PHP：抛出异常
来源：http://hz.sysykeji.top/gtfwujfgsu.html

throw new RuntimeException("失败", 500);
来源：http://hz.jyoumei.cn/gtichgvddd.html

[U72] PHP：写错误日志
来源：http://hz.sysykeji.top/gtixmbcfqp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shangyingyoupin.top/gtupvqadif.html

[U73] PHP：读取 ini 配置
来源：http://hz.aibaodan.cn/gtasatprct.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtpudibyjk.html

[U74] PHP：读取环境变量
来源：http://hz.hnqzz.top/gtjcqaqaor.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenjidiqi.icu/gtnsdqrefy.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtufsgmzyu.html

composer require psr/container
来源：http://hz.gzhubu.top/gtdhvipawd.html

[U76] PHP：简单路由
来源：http://hz.jyoumei.cn/gtlyttsfrv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yanxiufei.cn/gtkwkyqrjv.html

[U77] PHP：模板渲染
来源：http://hz.hnqzz.top/gtrzxyxsuh.html

composer require twig/twig
来源：http://hz.yangfankeji.com/gtlkgtsicf.html

[U78] PHP：单元测试
来源：http://hz.bjfxy.top/gtccrjeyca.html

composer require --dev phpunit/phpunit
来源：http://hz.haohaochexian.top/gtvncazdbz.html

[U79] PHP：静态分析
来源：http://hz.yangfankeji.com/gtmrarytqd.html

composer require --dev phpstan/phpstan
来源：http://hz.sufxvd.cn/gtjxfpxtuh.html

[U80] PHP：代码规范修复
来源：http://hz.jlsjyb.cn/gtpjejsfyd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daria6918.cn/gtpxjwbgcp.html

[U81] JS：初始化项目
来源：http://hz.tian-w.cn/gtyshohpur.html

npm init -y;  npm i express
来源：http://hz.redwolf501.top/gtutlmqfsf.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258.top/gtpwfmpbuv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zdqjudy.top/gtokvigzdu.html

[U83] JS：ES Module 导入导出
来源：http://hz.shanyushiyangtech.top/gtwrgfyphf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hnxiangtu.top/gtylmvqvda.html

[U84] JS：CommonJS 写法
来源：http://hz.meibo888.top/gtxvjtgfkx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydzc1.top/gtyvovgplf.html

[U85] JS：可选链
来源：http://hz.hammf.cn/gtogwcnlzq.html

a?.b?.c
来源：http://hz.ydzc1.top/gtzqeblzrh.html

[U86] JS：空值合并
来源：http://hz.mhx1999.top/gtifoxaniv.html

a ?? b
来源：http://hz.zhongyouzk.top/gtgrgqwimk.html

[U87] JS：解构默认值
来源：http://hz.ydjk.org.cn/gtebgmzkge.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gzhubu.top/gtizohakej.html

[U88] JS：对象展开合并
来源：http://hz.wangdashe.top/gtzrbbcnej.html

{ ...a, ...b }
来源：http://hz.cdnleiting.top/gtivhonqsl.html

[U89] JS：数组去重
来源：http://hz.9152youxi.cn/gtlvjkmzhg.html

[...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtoisumsqn.html

[U90] JS：数字数组排序
来源：http://hz.mhx1999.top/gttdvevufl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtaetojyqs.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtkuduygrg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.dashuyun.cn/gtlqrndbga.html

[U92] JS：深拷贝
来源：http://hz.tian-w.cn/gtuweqhsqw.html

structuredClone(obj)
来源：http://hz.fengsongda.top/gtifozghqz.html

[U93] JS：模板字符串
来源：http://hz.haohaochexian.top/gtasjqockc.html

`共 ${n} 条`
来源：http://hz.snrcjt.cn/gtlphsruod.html

[U94] JS：箭头函数
来源：http://hz.xylfe.cn/gtubkcwdyw.html

const double = x => x * 2;
来源：http://hz.shuidangran.top/gthwepedlo.html

[U95] JS：Promise 包装
来源：http://hz.yj20258.top/gtifpgdbrl.html

new Promise((resolve, reject) => {})
来源：http://hz.yonumen.top/gtpbokvxrs.html

[U96] JS：async/await 与异常
来源：http://hz.jqgfzy.top/gtpdssvbco.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtjynfyalx.html

[U97] JS：并发请求
来源：http://hz.ywan-chungtsiang.top/gtbsunktmp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtmaszagxd.html

[U98] JS：fetch 带 JSON
来源：http://hz.0kj1m.cn/gtjmqvltnj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daxiang520.top/gtektoyrxy.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtecixbcsk.html

el.addEventListener("click", e => {})
来源：http://hz.hnxiangtu.top/gtzxrbbhgh.html

[U100] JS：DOM 查询
来源：http://hz.yj202588.top/gtwlfqlegf.html

document.querySelector(".item")
来源：http://hz.dianchejie.cn/gtwqnjslxl.html

[U101] JS：classList 操作
来源：http://hz.dianchejie.cn/gteinevcmt.html

el.classList.toggle("active")
来源：http://hz.tanke756.top/gthblwueed.html

[U102] JS：本地存储
来源：http://hz.quarkkingdee.top/gtqxtgxqzr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cashguo.top/gtehrqjygr.html

[U103] JS：定时器
来源：http://hz.jinyuanbaomall.cn/gtluxnsquc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guowangkeji.top/gtfhebcvwk.html

[U104] JS：防抖
来源：http://hz.chenjidiqi.icu/gtyteaetvx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtnrogrzxc.html

[U105] JS：节流
来源：http://hz.cdnleiting.top/gthrjkzexr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nwbrower.top/gtmqzgixrh.html

[U106] JS：日期格式化
来源：http://hz.zhijiandao.cn/gtdanscsnj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cheryme.top/gttdxrsfds.html

[U107] JS：数字千分位
来源：http://hz.zhaomingkeji.xyz/gtkrytnlil.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnqzz.top/gtqbsxndub.html

[U108] JS：随机整数
来源：http://hz.birdmap.top/gtpijuukma.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtwgqahcxa.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gtwpyucvqr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gthvudlwxp.html

[U110] JS：数组分块
来源：http://hz.52xcode.cn/gtgzvsrmqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shanyushiyangkeji.top/gtlgltpnwr.html

[U111] JS：对象转 Map
来源：http://hz.hnxiangtu.top/gtnkdxbtrz.html

new Map(Object.entries(obj))
来源：http://hz.yj202588.top/gtrywrfuhs.html

[U112] JS：字符串补位
来源：http://hz.hywenlv.cn/gtmdxkqqwm.html

"7".padStart(3, "0")
来源：http://hz.ivvv.top/gtczvzadko.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtevwhrqpx.html

s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtotgxltsn.html

[U114] JS：JSON 深比较
来源：http://hz.yanxiufei.cn/gtnilrcpql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtaifiljsz.html

[U115] JS：生成 UUID
来源：http://hz.xuetiantiany.cn/gtaskaddfq.html

crypto.randomUUID()
来源：http://hz.tian-w.cn/gtiindhscu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yonumen.top/gtqomxwgis.html

/** @param {string} name */ function f(name) {}
来源：http://hz.redwolf501.top/gtgcqwfsio.html

[U117] JS：单元测试
来源：http://hz.xinyue.icu/gtztxzmtel.html

npm i -D vitest;  npx vitest
来源：http://hz.yonumen.top/gtwvlhukkv.html

[U118] JS：开发服务器
来源：http://hz.c1oappe.top/gtdkhcveje.html

npm i -D vite;  npx vite
来源：http://hz.zdqjudy.top/gtngnznluz.html

[U119] JS：生产构建
来源：http://hz.zhiwuduotai.top/gtppcoqxpe.html

npx vite build
来源：http://hz.jinyuanbaomall.cn/gtcovdpkqw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnxiangtu.top/gtwortspfk.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gtabltyyjt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtzwgnunkq.html

统计汇总
来源：http://hz.hnxiangtu.top/gthmszdrsc.html

================================================================================
来源：http://hz.yj202588.top/gtonvvpkkn.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtellvjxmk.html

Python ......... 252
来源：http://hz.yuanzhike.top/gtgmpuhkll.html

PHP ............ 252
来源：http://hz.jinyuanbaomall.cn/gtcqjmjbcv.html

JavaScript ..... 252
来源：http://hz.yj20258888.top/gtsmiphkbz.html

TypeScript ..... 212
来源：http://hz.hnxiangtu.top/gtbhdexsub.html

Java ........... 212
来源：http://hz.daria6918.cn/gtpvcdckuh.html

Go ............. 212
来源：http://hz.jyoumei.cn/gtqnqnjchi.html

Ruby ........... 212
来源：http://hz.yj20258888.top/gtdbumjprn.html

C# ............. 212
来源：http://hz.gotoacloud.top/gtgcejtjug.html

C .............. 30
来源：http://hz.daria6918.cn/gtpqopvhze.html

C++ ............ 30
来源：http://hz.hammf.cn/gtquafedac.html

SQL ............ 90
来源：http://hz.daxiang520.top/gtevwkmxxp.html

Bash ........... 80
来源：http://hz.birdmap.top/gteiyvlymf.html

Kotlin ......... 15
来源：http://hz.cqqwz.cn/gtiheefcls.html

Swift .......... 15
来源：http://hz.sufxvd.cn/gtrvkrtpmg.html

Lua ............ 10
来源：http://hz.yonumen.top/gtnhgbiwzd.html

Perl ........... 10
来源：http://hz.ydjk.org.cn/gtoydueift.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtanwvztsr.html

------------------------------------
来源：http://hz.gaohongyu789.top/gtxomwazfx.html

合计 ........... 2106 条
来源：http://hz.hywenlv.cn/gtmdxrlgic.html

按章节统计：
来源：http://hz.birdmap.top/gthjijrseu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtqviqhakm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtmynzuskd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtxmlshslb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtkbfwrwnw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.gaohongyu789.top/gthfdyeeuw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtlqnpqvot.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtnzbykozs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shuidangran.top/gtftwpirzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtgwtsiwdp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtdzwbipph.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtfpmisdzk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtyyntojwf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtwemuhpuz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtlvkgqfgb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gttxcxoiga.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtxqbetyui.html

Q SQL 专题                              90
来源：http://hz.hongshengwenyu.top/gtkijtwyab.html

R Bash 专题                             80
来源：http://hz.guannengcc.top/gtvcciwrnq.html

S C / C++ 专题                          60
来源：http://hz.yonumen.top/gttfaxxevj.html

T 其他语言补充                          60
来源：http://hz.xuetiantiany.cn/gtzhavtopc.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtwmchmxfu.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtmijoneru.html

合计                                  2106 条
来源：http://hz.cheryme.top/gtzzyvcckl.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gttfxgmmiv.html

使用提醒
来源：http://hz.cdnleiting.top/gtgheohuyf.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtjsswqtop.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gtagquflqn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.svipenyu.cn/gtofptedkl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.daxiang520.top/gtqduqakot.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.52xcode.cn/gtvdzadcpd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.havefunace.top/gtwkhylcnx.html

—— 文件结束 ——
来源：http://hz.sweek.top/gtehsjkied.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgvcfzxjl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj202588.top/gtstycozrh.html

Common Programming Examples Cheat Book
来源：http://hz.aibaodan.cn/gtqcxoubhr.html

================================================================================
来源：http://hz.yuxming.cn/gtskcqudhk.html

【收录内容】
来源：http://hz.guannengcc.top/gtfjxzplrb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.52xcode.cn/gtsilljuug.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jqgfzy.top/gtddosqwdh.html

SQL · Bash · C · C++
来源：http://hz.zhongyouzk.top/gtlhbvjcdc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yongpay.top/gtlflqchxs.html

【使用说明】
来源：http://hz.ybcxt.top/gtimtfimxb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgfzy.top/gtomeslvko.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yuxming.cn/gtvoqeqpgw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tanke756.top/gtahswngsj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shangyingyoupin.top/gtlfpawslr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.svipenyu.cn/gtbqytcpeu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zdqjudy.top/gtlsugduhc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shzxlz.cn/gtfkdjmsxx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtchtcfyhu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ppjwa.cn/gtnwvyjnkf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuanzx.com/gtxndeyhzf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnxiangtu.top/gtsutyikal.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daria6918.cn/gtnrvfcbuf.html

【文件统计】
来源：http://hz.haohaochexian.top/gtyrbagklq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hfpthk.cn/gtwbhavrvm.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtqawcnwjs.html

目  录
来源：http://hz.gaohongyu789.top/gtwgcdnixc.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gttudvpnri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.gaohongyu789.top/gtaesyykdh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtsbfikpki.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gttrdwrixg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtveeprshw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinqigfzy.top/gtdqxvnrua.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gtfpqostre.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtfkgzhpfn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.wangdashe.top/gtrrsyifqc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtfwvdzilf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ppjwa.cn/gtaddqhpyw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtvxzkznyb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtyvegsyeg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtqlcarjma.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtmtrekixg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.bjfxy.top/gttvpgnehm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtpusvcuzv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.feifeiyinyue.top/gtdxwsfzcx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.birdmap.top/gtapwqspmw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.aibaodan.cn/gtzvgpjxql.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gttanbytkc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtauvrmxsg.html

================================================================================
来源：http://hz.pycfn.com/gtjoflgwyu.html

A. 基础语法与类型
来源：http://hz.svipenyu.cn/gtfqujzojd.html

================================================================================
来源：http://hz.fzhhl.top/gtyrphrciu.html

[A01] Hello World
来源：http://hz.quarkkingdee.top/gtiiympurt.html

Py:   print("Hello, World!")
来源：http://hz.jiagoushi.top/gtvdltktjd.html

PHP:  echo "Hello, World!";
来源：http://hz.c1oappe.top/gtquvrfkka.html

JS:   console.log("Hello, World!");
来源：http://hz.aibaodan.cn/gtdnzxeald.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.snrcjt.cn/gtgohubdnm.html

Java: System.out.println("Hello, World!");
来源：http://hz.xylfe.cn/gtwutghmhu.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtwhvkfome.html

Ruby: puts "Hello, World!"
来源：http://hz.zhaomingkeji.xyz/gtitexnzkl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tanke756.top/gtetrhhmie.html

[A02] 变量声明与赋值
来源：http://hz.ppjwa.cn/gtegumrxrp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shuidangran.top/gtpjsdtiaw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sysykeji.top/gtdspijimm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.guannengcc.top/gtzzdzqphv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guowangkeji.top/gtatsgxcxi.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtgkkgcavc.html

Go:   name := "Alex"; age := 20
来源：http://hz.tian-w.cn/gtdocthojx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.redwolf501.top/gtiugcqvmz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtdfozslle.html

[A03] 常量定义
来源：http://hz.shanyushiyangkeji.top/gtjasrpgcl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hnxiangtu.top/gtgtjtfhxb.html

PHP:  const PI = 3.14159;
来源：http://hz.iojbl.cn/gtbpfefdgv.html

JS:   const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtcqoifeaz.html

TS:   const PI: number = 3.14159;
来源：http://hz.aizwys.cn/gtvgtkfcds.html

Java: static final double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtspqvujsr.html

Go:   const PI = 3.14159
来源：http://hz.ywan-chungtsiang.top/gtvnuhrzjw.html

Ruby: PI = 3.14159
来源：http://hz.wangshuangyany.cn/gtkwunbhcp.html

C#:   const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtgwihcdnx.html

[A04] 判断变量类型
来源：http://hz.daria6918.cn/gtrhgoequj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxinkj.top/gtqdtcvfiv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhaomingkeji.xyz/gtkcmemner.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sweek.top/gttktzcevz.html

TS:   typeof x; x instanceof Date
来源：http://hz.cheryme.top/gtbsporvhi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gtoppzdkqz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jlsjyb.cn/gtoklqlhas.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxinkj.top/gttexvkrlh.html

C#:   x.GetType().Name; x is int
来源：http://hz.birdmap.top/gtiemvtqaw.html

[A05] 整数除法与取模
来源：http://hz.jinqigufen.top/gtyfkeycfu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tianlin.xyz/gtkjxmkqmy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.snrcjt.cn/gtsdidhlnu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gtbabcwlew.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.havefunace.top/gtlknrfkib.html

Java: 7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtocmmtrln.html

Go:   7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gtvgudiinh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtaxhxgmva.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gtvrjtqryy.html

[A06] 字符串转数字
来源：http://hz.nwbrower.top/gtwaeqfuje.html

Py:   int("42"); float("3.14")
来源：http://hz.hysaishi.cn/gtlioukivd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yonumen.top/gtcilrvlyf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.feifeiyinyue.top/gtszkcmapk.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.gzhubu.top/gtlspxbrki.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.guowangkeji.top/gtlsnoqfcx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.nanxinkj.top/gtqckglhod.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xziqi.cn/gtxrbtigwv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.snrcjt.cn/gtvwykylpi.html

[A07] 数字转字符串
来源：http://hz.jqgfzy.top/gtjgumapna.html

Py:   str(42)
来源：http://hz.hongshengwenyu.top/gtmrobzyzu.html

PHP:  (string) 42; strval(42)
来源：http://hz.nwbrower.top/gtyuimliwy.html


<!-- 参考信息 -->