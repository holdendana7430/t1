代发 wailian999

[U51] PHP：数组解构
来源：http://hz.yvedp.cn/gtxvocpllw.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtbzxmyzqt.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtiiwxtspj.html

$double = fn($x) => $x * 2;
来源：http://hz.316326.xyz/gtljflihww.html

[U53] PHP：空合并运算符
来源：http://hz.jiagoushi.top/gtmgrpsnoe.html

$v = $a ?? $b ?? "default";
来源：http://hz.nanxuanxn.top/gtzkamwuut.html

[U54] PHP：空安全调用
来源：http://hz.jianghu66.top/gtighlnvot.html

$obj?->method()
来源：http://hz.yanxiufei.cn/gtulytlpam.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtgjgwfxca.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.dianchejie.cn/gtilirscci.html

[U56] PHP：命名参数
来源：http://hz.gzhubu.top/gtjzaguxcv.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtkfbcdzti.html

[U57] PHP：字符串插值
来源：http://hz.nwbrower.top/gtqvupmpgo.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtykyrpqbz.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtrtbwlzfy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aibaodan.cn/gtrjrixhtt.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtlxmbqsyz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtwsfssfku.html

[U60] PHP：JSON 编解码
来源：http://hz.jianghu66.top/gtewfwxihr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zycfv.cn/gtqjlqokcl.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtdksmqmcv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtlirtjcrh.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gtxeykwdzu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtpibmemcj.html

[U63] PHP：文件读写
来源：http://hz.sufxvd.cn/gtuajvwjkv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jlsjyb.cn/gtiilnitko.html

[U64] PHP：目录遍历
来源：http://hz.wangshuangyany.cn/gtvwqlddzs.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhaomingkeji.xyz/gtzfnenpwq.html

[U65] PHP：会话
来源：http://hz.jinqigufen.top/gtoibinfgi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuanzhike.top/gtqlbddxcb.html

[U66] PHP：设置 Cookie
来源：http://hz.smart0.xyz/gtojxdbzde.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.redwolf501.top/gtitwmwnfo.html

[U67] PHP：处理文件上传
来源：http://hz.snrcjt.cn/gtovkjtxrg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ivvv.top/gtkbqetcms.html

[U68] PHP：PDO 连接
来源：http://hz.zhoulong.xyz/gtukyalbll.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.mhx1999.top/gtumwkyerp.html

[U69] PHP：PDO 预处理
来源：http://hz.fzhhl.top/gtzldtteeb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gaohongyu789.top/gtjjsybyqr.html

[U70] PHP：PDO 事务
来源：http://hz.ywan-chungtsiang.top/gthcwgdwya.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangkeji.top/gtovhxlorc.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtjvfdhiye.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtvzhucvoy.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtkoulxfhm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtliizlzjz.html

[U73] PHP：读取 ini 配置
来源：http://hz.ybcxt.top/gtjpspipkh.html

parse_ini_file("config.ini", true)
来源：http://hz.ydjk.org.cn/gtfwewrihd.html

[U74] PHP：读取环境变量
来源：http://hz.shzxlz.cn/gtwrjkluxr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daxiang520.top/gtcmntmoim.html

[U75] PHP：依赖注入
来源：http://hz.guannengcc.top/gtiifazklr.html

composer require psr/container
来源：http://hz.smart0.xyz/gtfkhzeykj.html

[U76] PHP：简单路由
来源：http://hz.iojbl.cn/gtdpppxcfz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.chenjidiqi.icu/gttaakwtnc.html

[U77] PHP：模板渲染
来源：http://hz.hnqzz.top/gtcjdqbhkq.html

composer require twig/twig
来源：http://hz.cdnleiting.top/gtzqeazxwc.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtxzxhzztf.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gtdhlrhiag.html

[U79] PHP：静态分析
来源：http://hz.smart0.xyz/gtlpdfkkni.html

composer require --dev phpstan/phpstan
来源：http://hz.wangdashe.top/gttkoacwdu.html

[U80] PHP：代码规范修复
来源：http://hz.nwbrower.top/gteorwlwuy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigufen.top/gtdqtomfut.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtpeknlasf.html

npm init -y;  npm i express
来源：http://hz.ehwqpu.com/gtdvktlcap.html

[U82] JS：package.json 脚本
来源：http://hz.52xcode.cn/gtsuhddosk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxuanxn.top/gtktfkcorx.html

[U83] JS：ES Module 导入导出
来源：http://hz.xingfuxueyuan.xyz/gtaxraoqzo.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sufxvd.cn/gtvcvhrwbz.html

[U84] JS：CommonJS 写法
来源：http://hz.c1oappe.top/gticoodpfl.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.meibo888.top/gtjwgwjdgn.html

[U85] JS：可选链
来源：http://hz.jyoumei.cn/gtnbpasmsw.html

a?.b?.c
来源：http://hz.0kj1m.cn/gtvolutzjj.html

[U86] JS：空值合并
来源：http://hz.tianlin.xyz/gtxydikvtz.html

a ?? b
来源：http://hz.jinqigfzy.top/gtdxfpussw.html

[U87] JS：解构默认值
来源：http://hz.hammf.cn/gtcripezkt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cdnleiting.top/gtslfevpku.html

[U88] JS：对象展开合并
来源：http://hz.aizwys.cn/gtigfjqckz.html

{ ...a, ...b }
来源：http://hz.cucudq.cn/gteelycxni.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gttgjgssyu.html

[...new Set(arr)]
来源：http://hz.tianlin.xyz/gthjnfbbud.html

[U90] JS：数字数组排序
来源：http://hz.cdnleiting.top/gtvwurzmex.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtgcznvqod.html

[U91] JS：对象键值遍历
来源：http://hz.yongpay.top/gtqccdhljh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xingfuxueyuan.xyz/gttgtbpqtd.html

[U92] JS：深拷贝
来源：http://hz.zdqjudy.top/gtacmsitmy.html

structuredClone(obj)
来源：http://hz.zdqjudy.top/gtzyvuntus.html

[U93] JS：模板字符串
来源：http://hz.guannengcc.top/gtxjtgtkhr.html

`共 ${n} 条`
来源：http://hz.zhoulong.xyz/gttemizvxp.html

[U94] JS：箭头函数
来源：http://hz.smart0.xyz/gtwdxmwami.html

const double = x => x * 2;
来源：http://hz.guowangkeji.top/gtkhhksuen.html

[U95] JS：Promise 包装
来源：http://hz.jlsjyb.cn/gtdievkngk.html

new Promise((resolve, reject) => {})
来源：http://hz.cdnleiting.top/gtojsqrzyx.html

[U96] JS：async/await 与异常
来源：http://hz.9152youxi.cn/gtjbkzymyf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtndghlcyi.html

[U97] JS：并发请求
来源：http://hz.nanxuanxn.top/gtiwrputby.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtjzzptsbg.html

[U98] JS：fetch 带 JSON
来源：http://hz.fengsongda.top/gtpfqhjtje.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhiwuduotai.top/gtwcwjljpj.html

[U99] JS：事件监听
来源：http://hz.hysaishi.cn/gtibbitvga.html

el.addEventListener("click", e => {})
来源：http://hz.dashuyun.cn/gttiqvaauc.html

[U100] JS：DOM 查询
来源：http://hz.ywan-chungtsiang.top/gtxexywedf.html

document.querySelector(".item")
来源：http://hz.sweek.top/gtcdbyzcgu.html

[U101] JS：classList 操作
来源：http://hz.c1oappe.top/gtknqtvdei.html

el.classList.toggle("active")
来源：http://hz.hfpthk.cn/gtdihhhnws.html

[U102] JS：本地存储
来源：http://hz.xziqi.cn/gtitkctcrc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.mhx1999.top/gtbdcybswm.html

[U103] JS：定时器
来源：http://hz.haohaochexian.top/gtpikfljcm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hammf.cn/gtwkvwohmh.html

[U104] JS：防抖
来源：http://hz.0kj1m.cn/gtkcflwbcn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtoxiezkmz.html

[U105] JS：节流
来源：http://hz.52xcode.cn/gtnrgiyvhn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pengpengdd.cyou/gtsqljqkum.html

[U106] JS：日期格式化
来源：http://hz.daria6918.cn/gtwckwmksr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jqgufenzy.top/gtgjsjvlwq.html

[U107] JS：数字千分位
来源：http://hz.aibaodan.cn/gtzeltesvr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hywenlv.cn/gtaaqtuzai.html

[U108] JS：随机整数
来源：http://hz.ydzc1.top/gtnmwvzodq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtylbunafb.html

[U109] JS：数组分组
来源：http://hz.hysaishi.cn/gtklmsoaee.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtiotkofiw.html

[U110] JS：数组分块
来源：http://hz.nanxinkj.top/gtocllcssb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gtznpawrxe.html

[U111] JS：对象转 Map
来源：http://hz.zhoulong.xyz/gtqswcvcuw.html

new Map(Object.entries(obj))
来源：http://hz.gzhubu.top/gtrawalgwb.html

[U112] JS：字符串补位
来源：http://hz.daria6918.cn/gtocpungoj.html

"7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtlxdqlfeo.html

[U113] JS：正则替换全部
来源：http://hz.52xcode.cn/gtgaiwztji.html

s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtgxmyqkyv.html

[U114] JS：JSON 深比较
来源：http://hz.quarkkingdee.top/gtmgywdgrh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtijzdeouu.html

[U115] JS：生成 UUID
来源：http://hz.ivvv.top/gtslhdqlws.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtbpcruqvg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.9152youxi.cn/gtcaqtnxmg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj202588.top/gtklfiikqf.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gtyrisvfco.html

npm i -D vitest;  npx vitest
来源：http://hz.dianchejie.cn/gtlmgbgjij.html

[U118] JS：开发服务器
来源：http://hz.zhongyouzk.top/gtyhnjgsyc.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gtwkxgjhgh.html

[U119] JS：生产构建
来源：http://hz.yuxming.cn/gtexrizzdk.html

npx vite build
来源：http://hz.hnqzz.top/gthfveeeax.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.redwolf501.top/gtfgzmubhm.html

import.meta.env.VITE_API_URL
来源：http://hz.ivvv.top/gtlnmtbarn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdjcvicom.html

统计汇总
来源：http://hz.ydzc1.top/gtcpwbwhkx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuqticnlq.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtcizodxnk.html

Python ......... 252
来源：http://hz.havefunace.top/gtcnwfaxns.html

PHP ............ 252
来源：http://hz.9152youxi.cn/gthxsjqbcg.html

JavaScript ..... 252
来源：http://hz.gotoacloud.top/gtsjpctois.html

TypeScript ..... 212
来源：http://hz.wangdashe.top/gtojtxbhlf.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtsvwllvtp.html

Go ............. 212
来源：http://hz.zhaomingkeji.xyz/gtaojcpgcr.html

Ruby ........... 212
来源：http://hz.xingfuxueyuan.xyz/gtrnpuxvdf.html

C# ............. 212
来源：http://hz.fzhhl.top/gtomjeqxjs.html

C .............. 30
来源：http://hz.ydzc1.top/gtglivbllp.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtnhuztzby.html

SQL ............ 90
来源：http://hz.xingfuxueyuan.xyz/gtgwqmmiyc.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gtdssdjpal.html

Kotlin ......... 15
来源：http://hz.9152youxi.cn/gtmaachbsj.html

Swift .......... 15
来源：http://hz.yuanzhike.top/gtbzlyfsfd.html

Lua ............ 10
来源：http://hz.sweek.top/gtrzhogtth.html

Perl ........... 10
来源：http://hz.wangshuangyany.cn/gtdvhjahbb.html

Scala .......... 10
来源：http://hz.zhijiandao.cn/gtihfhkrts.html

------------------------------------
来源：http://hz.cashguo.top/gtmpevnsod.html

合计 ........... 2106 条
来源：http://hz.dashuyun.cn/gtxzezeevd.html

按章节统计：
来源：http://hz.gzhubu.top/gtyqblkvwx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tian-w.cn/gtpbgeeytg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtmcocjznz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtrxuokkmv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtgvptdnpf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cucudq.cn/gthsevwfbo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtnpinaruy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtnqlleiks.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtdlnrffnx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtgpdwoxal.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtqoxeqmzt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtbjhogqbx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtivxtoaul.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtzrtmgllk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtestjfvib.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.fengsongda.top/gtpjfqobkn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtotozjglp.html

Q SQL 专题                              90
来源：http://hz.fengsongda.top/gtvpelornq.html

R Bash 专题                             80
来源：http://hz.ybcxt.top/gtltldkmwh.html

S C / C++ 专题                          60
来源：http://hz.hysaishi.cn/gtlcgrvjwj.html

T 其他语言补充                          60
来源：http://hz.shuidangran.top/gtytnojikf.html

U 高频实用片段                         120
来源：http://hz.mhx1999.top/gteegcftzb.html

------------------------------------
来源：http://hz.yongpay.top/gttiicxqkp.html

合计                                  2106 条
来源：http://hz.xinyue.icu/gthjjnrzgo.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtyjevixgf.html

使用提醒
来源：http://hz.jiagoushi.top/gtmddnwkwh.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtoyvqooik.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zdqjudy.top/gtfskjaggo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sweek.top/gttuhpimcq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gtupljqdfg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cucudq.cn/gtanytjazq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dashuyun.cn/gtmfzutxqw.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtlyptdbxr.html

================================================================================
来源：http://hz.andypj.xyz/gtfdgussoh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.birdmap.top/gtywpzobzj.html

Common Programming Examples Cheat Book
来源：http://hz.xziqi.cn/gtpfttjdot.html

================================================================================
来源：http://hz.guowangkeji.top/gtshsfrhjm.html

【收录内容】
来源：http://hz.shanyushiyangkeji.top/gtqrppburg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gaohongyu789.top/gtvekrkgfd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtaglhkthq.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtyhlzbogc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yongpay.top/gtmpofkncp.html

【使用说明】
来源：http://hz.yj202588.top/gtunrcvvgf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtcycgbkgc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj202588.top/gtscacthvo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.fzhhl.top/gtvzxvfvps.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xziqi.cn/gtknojpnga.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.andypj.xyz/gtpuwvnyfj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xinyue.icu/gtmnbgqogj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dianchejie.cn/gtklvhixgj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jianghu66.top/gtwsucbkxv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.pycfn.com/gtzgyagrfz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ehwqpu.com/gtizuvgosf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yj20258888.top/gtouzupkzx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.meibo888.top/gtyqkfgaxg.html

【文件统计】
来源：http://hz.ydzc1.top/gtawlzktne.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dashuyun.cn/gteipfbild.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtfehsvnhu.html

目  录
来源：http://hz.cdnleiting.top/gtpayxennv.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtobcgyxbs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.9152youxi.cn/gtyjtedrkl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gtatanhzii.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtrotdayga.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtsmbgscjy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sufxvd.cn/gtsxsyabiu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj20258888.top/gtnuqyptgj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtaibmtjls.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nanxuanxn.top/gtrevuaiue.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gteljoosii.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cdnleiting.top/gtfznbrzqg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtqmzyiggl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gthlpjmmum.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gthgcwhbpb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.52xcode.cn/gtrtqwazoy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daxiang520.top/gtplnvwhdn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtukitfbyn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sufxvd.cn/gtrxjsfjyp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gtzlumqrdb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.snrcjt.cn/gtegeokhbn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtjbqtoxul.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtligrgzdt.html

================================================================================
来源：http://hz.gogol.net.cn/gtezqkcrdd.html

A. 基础语法与类型
来源：http://hz.gotoacloud.top/gtlftlvgyj.html

================================================================================
来源：http://hz.redwolf501.top/gtfwiouqem.html

[A01] Hello World
来源：http://hz.cucudq.cn/gtsefbiyyb.html

Py:   print("Hello, World!")
来源：http://hz.xinyue.icu/gtinmixaol.html

PHP:  echo "Hello, World!";
来源：http://hz.bjfxy.top/gtbpnjbbfe.html

JS:   console.log("Hello, World!");
来源：http://hz.havefunace.top/gtkdlprvtu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.svipenyu.cn/gtgyrxgeap.html

Java: System.out.println("Hello, World!");
来源：http://hz.cucudq.cn/gtcdmgjrck.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gtrzwnccnr.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtfjlwtgeu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtsidrlebh.html

[A02] 变量声明与赋值
来源：http://hz.chenzaomai.com/gtrmawyaad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xziqi.cn/gtgopxltub.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.daria6918.cn/gtsdyssdnf.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenjidiqi.icu/gtffuucpmj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yongpay.top/gtdlpmrngm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtbzoelvzw.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtcnehzfkj.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hywenlv.cn/gtarkkuvbv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hysaishi.cn/gtrnisbnin.html

[A03] 常量定义
来源：http://hz.shanyushiyangkeji.top/gtuiuiuqrf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guannengcc.top/gtlpoizlyw.html

PHP:  const PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtwaiweskw.html

JS:   const PI = 3.14159;
来源：http://hz.dianchejie.cn/gtlbyrzvvr.html

TS:   const PI: number = 3.14159;
来源：http://hz.smart0.xyz/gtnpvrtygh.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtpkfeirzp.html

Go:   const PI = 3.14159
来源：http://hz.pycfn.com/gtiezlkpzi.html

Ruby: PI = 3.14159
来源：http://hz.pycfn.com/gtkiesrxzv.html

C#:   const double PI = 3.14159;
来源：http://hz.yonumen.top/gtjggwfqss.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtooxkutzw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.dashuyun.cn/gtcyxhvacd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gzhubu.top/gtpmvcoivo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.feifeiyinyue.top/gtwlhlgfns.html

TS:   typeof x; x instanceof Date
来源：http://hz.gaohongyu789.top/gtvtpvhdyq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtjfjxakef.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.pengpengdd.cyou/gthmcfgtrs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tianlin.xyz/gtvxyfofpf.html

C#:   x.GetType().Name; x is int
来源：http://hz.wangshuangyany.cn/gtuyuosuoa.html

[A05] 整数除法与取模
来源：http://hz.tian-w.cn/gtzvfdycmx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangtech.top/gtghmlrkek.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fzhhl.top/gttlxhnsbb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtuqxardtx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtftckfzcn.html

Java: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtagfhhhgn.html

Go:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtdqaoyaho.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtytedgyxb.html

C#:   7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtkkopywtt.html

[A06] 字符串转数字
来源：http://hz.hnxiangtu.top/gtbjhjahqt.html

Py:   int("42"); float("3.14")
来源：http://hz.quarkkingdee.top/gtdlprzuuk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ivvv.top/gtwachghcp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xziqi.cn/gtmxiryivg.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.tianlin.xyz/gtcwznflfa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ivvv.top/gtxwctoppj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.guowangkeji.top/gtycflpdsj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xylfe.cn/gtqkjkvdgz.html


<!-- 参考信息 -->