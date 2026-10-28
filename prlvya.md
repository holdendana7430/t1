代发 wailian999

[U51] PHP：数组解构
来源：http://hz.zhiwuduotai.top/gtjeehajck.html

[$a, $b] = $arr;
来源：http://hz.ybcxt.top/gtjnrpejgk.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtsjffpqzf.html

$double = fn($x) => $x * 2;
来源：http://hz.chenlongwang.top/gtyztulzyz.html

[U53] PHP：空合并运算符
来源：http://hz.52xcode.cn/gtobspxifi.html

$v = $a ?? $b ?? "default";
来源：http://hz.sysykeji.top/gtijbbfmfn.html

[U54] PHP：空安全调用
来源：http://hz.jinqigfzy.top/gtxwxokjrs.html

$obj?->method()
来源：http://hz.yj20258888.top/gtqdyjcond.html

[U55] PHP：match 表达式
来源：http://hz.sufxvd.cn/gtcdsyikgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.guowangkeji.top/gtxnmhdewc.html

[U56] PHP：命名参数
来源：http://hz.jinghuilouyu.cn/gteiwlisyq.html

f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtjgfhapjl.html

[U57] PHP：字符串插值
来源：http://hz.iojbl.cn/gtadnccvmt.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtxyodxczk.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gthvsdbihr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtdnnpolrb.html

[U59] PHP：自定义排序
来源：http://hz.sweek.top/gtqfwgmerg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtpjkmrspy.html

[U60] PHP：JSON 编解码
来源：http://hz.guannengcc.top/gttykoegmw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gteinnsrlw.html

[U61] PHP：正则
来源：http://hz.pengpengdd.cyou/gthopbvzji.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtxfittcir.html

[U62] PHP：日期对象
来源：http://hz.yj20258.top/gthrbiczmg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sufxvd.cn/gtonjkekky.html

[U63] PHP：文件读写
来源：http://hz.xziqi.cn/gtllkvvnjz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenlongwang.top/gtgjdomxek.html

[U64] PHP：目录遍历
来源：http://hz.ybcxt.top/gtmqglyqvj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xinyue.icu/gtfyxuaglu.html

[U65] PHP：会话
来源：http://hz.guannengcc.top/gtuphlmnry.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtdzulkzui.html

[U66] PHP：设置 Cookie
来源：http://hz.aibaodan.cn/gtrqkfmgpj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aibaodan.cn/gtieqqwmzc.html

[U67] PHP：处理文件上传
来源：http://hz.wangdashe.top/gtbbzirgvc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cqqwz.cn/gtzbuncnde.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtcxxljcdw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.andypj.xyz/gtvfzzttzs.html

[U69] PHP：PDO 预处理
来源：http://hz.zdqjudy.top/gtblsotojg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cashguo.top/gtwaqpzkzz.html

[U70] PHP：PDO 事务
来源：http://hz.fengsongda.top/gtfgsodyar.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ydzc1.top/gtbzewjvpc.html

[U71] PHP：抛出异常
来源：http://hz.yuanzhike.top/gtdffobkep.html

throw new RuntimeException("失败", 500);
来源：http://hz.hfpthk.cn/gtfwizkvdm.html

[U72] PHP：写错误日志
来源：http://hz.yuanzhike.top/gtgmkuhqpu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ehwqpu.com/gtkpxxenik.html

[U73] PHP：读取 ini 配置
来源：http://hz.jyoumei.cn/gtrvgsidzb.html

parse_ini_file("config.ini", true)
来源：http://hz.pycfn.com/gtlzidrjkk.html

[U74] PHP：读取环境变量
来源：http://hz.pycfn.com/gtusvhtblr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.wangshuangyany.cn/gtudtgueox.html

[U75] PHP：依赖注入
来源：http://hz.cucudq.cn/gticegmefk.html

composer require psr/container
来源：http://hz.zhongyouzk.top/gtbygrkqyj.html

[U76] PHP：简单路由
来源：http://hz.nwbrower.top/gtxyltkhea.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.guannengcc.top/gtvaooeuqm.html

[U77] PHP：模板渲染
来源：http://hz.zhixingplan.top/gtqvjchsga.html

composer require twig/twig
来源：http://hz.wangdashe.top/gttkdmtgsr.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtfcxsfjwy.html

composer require --dev phpunit/phpunit
来源：http://hz.bjfxy.top/gtgrurvfam.html

[U79] PHP：静态分析
来源：http://hz.hammf.cn/gtibknembl.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gttzisqvzx.html

[U80] PHP：代码规范修复
来源：http://hz.cdnleiting.top/gtfsxoouxm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gtvvelrtpk.html

[U81] JS：初始化项目
来源：http://hz.sysykeji.top/gthrlalvnq.html

npm init -y;  npm i express
来源：http://hz.jlsjyb.cn/gtzitoxpas.html

[U82] JS：package.json 脚本
来源：http://hz.iojbl.cn/gtacccdjdk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sxryk.cn/gtjfhqzrrx.html

[U83] JS：ES Module 导入导出
来源：http://hz.52xcode.cn/gtfvrihtyr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gtavfjhcms.html

[U84] JS：CommonJS 写法
来源：http://hz.vqdsnc.cn/gtiywzzaib.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtgwyxdzfu.html

[U85] JS：可选链
来源：http://hz.fengsongda.top/gtwligthta.html

a?.b?.c
来源：http://hz.0kj1m.cn/gtqiiqdobu.html

[U86] JS：空值合并
来源：http://hz.yj20258.top/gtxjwdkqyl.html

a ?? b
来源：http://hz.sxryk.cn/gtakuvzblj.html

[U87] JS：解构默认值
来源：http://hz.jinghuilouyu.cn/gtrfeftnhl.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xziqi.cn/gtwbxhzpqo.html

[U88] JS：对象展开合并
来源：http://hz.jinqigufen.top/gtoykentrj.html

{ ...a, ...b }
来源：http://hz.tanke756.top/gtdokitcrp.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtabbznjvz.html

[...new Set(arr)]
来源：http://hz.aibaodan.cn/gtlvisbree.html

[U90] JS：数字数组排序
来源：http://hz.xylfe.cn/gtwwsyvlbs.html

[...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtqluhwgif.html

[U91] JS：对象键值遍历
来源：http://hz.yuanzhike.top/gturuwinkp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtfpqdwqtg.html

[U92] JS：深拷贝
来源：http://hz.chenjidiqi.icu/gtoxenedpe.html

structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtydxpkahu.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtihqoaugx.html

`共 ${n} 条`
来源：http://hz.wangshuangyany.cn/gthhgthnij.html

[U94] JS：箭头函数
来源：http://hz.ivvv.top/gtimmcorez.html

const double = x => x * 2;
来源：http://hz.meibo888.top/gtpdlzwjbm.html

[U95] JS：Promise 包装
来源：http://hz.birdmap.top/gthbyourye.html

new Promise((resolve, reject) => {})
来源：http://hz.gogol.net.cn/gthprnxlql.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtptawudyk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtvluyfdfm.html

[U97] JS：并发请求
来源：http://hz.gogol.net.cn/gtbzlaxudo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtyeenkbbx.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gtanfkzwyb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.birdmap.top/gtyxmqrcfc.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtzqbvgpto.html

el.addEventListener("click", e => {})
来源：http://hz.hysaishi.cn/gtojcqfcqk.html

[U100] JS：DOM 查询
来源：http://hz.9152youxi.cn/gtgnuplews.html

document.querySelector(".item")
来源：http://hz.hammf.cn/gtguuztukt.html

[U101] JS：classList 操作
来源：http://hz.jiagoushi.top/gtmdrnqkdo.html

el.classList.toggle("active")
来源：http://hz.smart0.xyz/gtqfrfjkld.html

[U102] JS：本地存储
来源：http://hz.daria6918.cn/gtxrhbyigf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gtcwgjbqlm.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtqznkowhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuxming.cn/gtqyubcpew.html

[U104] JS：防抖
来源：http://hz.cashguo.top/gtbdktlkbx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtovlyuyjh.html

[U105] JS：节流
来源：http://hz.aibaodan.cn/gtqgrynmds.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangshuangyany.cn/gtokqjlmqy.html

[U106] JS：日期格式化
来源：http://hz.jinqigfzy.top/gttdgrzixx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sysykeji.top/gtmatdjbih.html

[U107] JS：数字千分位
来源：http://hz.ehwqpu.com/gtaoujfafc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tian-w.cn/gtqmyepsrb.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtwirqrkce.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tianlin.xyz/gtgmrddgdc.html

[U109] JS：数组分组
来源：http://hz.zycfv.cn/gtlcoomydl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtmsbfstap.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtktowhmav.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gaohongyu789.top/gtiumixzge.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gttazzbhuh.html

new Map(Object.entries(obj))
来源：http://hz.pengpengdd.cyou/gtjqvobctf.html

[U112] JS：字符串补位
来源：http://hz.cqqwz.cn/gtkvmzfemp.html

"7".padStart(3, "0")
来源：http://hz.cheryme.top/gtixnshcrj.html

[U113] JS：正则替换全部
来源：http://hz.tian-w.cn/gtmkhpmmbj.html

s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtmurujnhb.html

[U114] JS：JSON 深比较
来源：http://hz.aibaodan.cn/gtailwrbga.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtfgimpjfk.html

[U115] JS：生成 UUID
来源：http://hz.gzhubu.top/gtxaamchsm.html

crypto.randomUUID()
来源：http://hz.ydzc1.top/gtibcgjwvo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yangfankeji.com/gtjbybxerf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hysaishi.cn/gtulxljdrr.html

[U117] JS：单元测试
来源：http://hz.birdmap.top/gtepqxzsoa.html

npm i -D vitest;  npx vitest
来源：http://hz.xziqi.cn/gtulacfkif.html

[U118] JS：开发服务器
来源：http://hz.tanke756.top/gtvjhhkibu.html

npm i -D vite;  npx vite
来源：http://hz.dashuyun.cn/gtsngsevjn.html

[U119] JS：生产构建
来源：http://hz.ybcxt.top/gtyrzphitd.html

npx vite build
来源：http://hz.9152youxi.cn/gtslokgjku.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtwjpzylbx.html

import.meta.env.VITE_API_URL
来源：http://hz.dianchejie.cn/gthjihueoq.html

================================================================================
来源：http://hz.nwbrower.top/gtdgvnigky.html

统计汇总
来源：http://hz.zhixingplan.top/gtuwlxacio.html

================================================================================
来源：http://hz.snrcjt.cn/gtbmvrcrqz.html

按语言统计（条）：
来源：http://hz.zhongyouzk.top/gtocxwojrc.html

Python ......... 252
来源：http://hz.ybcxt.top/gtqciwosks.html

PHP ............ 252
来源：http://hz.jqgfzy.top/gtnjezzvih.html

JavaScript ..... 252
来源：http://hz.zhaomingkeji.xyz/gtcjvlfnqw.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtoknpjegq.html

Java ........... 212
来源：http://hz.wangshuangyany.cn/gtyscozmug.html

Go ............. 212
来源：http://hz.ppjwa.cn/gtssurqhhk.html

Ruby ........... 212
来源：http://hz.hywenlv.cn/gtqsbcxtdx.html

C# ............. 212
来源：http://hz.cqqwz.cn/gtaozkggpg.html

C .............. 30
来源：http://hz.sweek.top/gthcirtkwt.html

C++ ............ 30
来源：http://hz.yonumen.top/gtlacrbaje.html

SQL ............ 90
来源：http://hz.sufxvd.cn/gtpnugdqai.html

Bash ........... 80
来源：http://hz.aizwys.cn/gtwxwjjcya.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gtbyxpsrey.html

Swift .......... 15
来源：http://hz.guannengcc.top/gtbrwftfsc.html

Lua ............ 10
来源：http://hz.sweek.top/gtismqofwt.html

Perl ........... 10
来源：http://hz.xziqi.cn/gthmbrdfvb.html

Scala .......... 10
来源：http://hz.yonumen.top/gtfveanyqo.html

------------------------------------
来源：http://hz.shzxlz.cn/gtrixvqjtx.html

合计 ........... 2106 条
来源：http://hz.316326.xyz/gtsgpokjom.html

按章节统计：
来源：http://hz.yvedp.cn/gtxhatimyg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtuasadwkh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gttdeskbse.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtimswqcog.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtdksdmmwm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yueranfly.top/gtsvxskmoo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtjgbaquuz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtdsatnbfe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtrihbriha.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtctlagwlo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtcdivmmpn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtrtistfdn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gttctnitld.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtjpunrlln.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daria6918.cn/gtoodzpnpf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ywan-chungtsiang.top/gtuqmgrczx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtfqpznlgz.html

Q SQL 专题                              90
来源：http://hz.zdqjudy.top/gtsvnwiief.html

R Bash 专题                             80
来源：http://hz.wangshuangyany.cn/gtyxiugcbj.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtsivstajv.html

T 其他语言补充                          60
来源：http://hz.cashguo.top/gtgpvlidqt.html

U 高频实用片段                         120
来源：http://hz.pycfn.com/gtxjzqmchv.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gteffnbvgp.html

合计                                  2106 条
来源：http://hz.daxiang520.top/gtupopmbdi.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtgngpdvwn.html

使用提醒
来源：http://hz.ppjwa.cn/gtqzxpjtsh.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtcjgenque.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jqgufenzy.top/gtmwteywja.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jianghu66.top/gtpocisxkx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nanxinkj.top/gtgrczmtwu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenzaomai.com/gtlosccwen.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.nwbrower.top/gtwvsqpdxv.html

—— 文件结束 ——
来源：http://hz.yj202588.top/gthfqbqjit.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtradalhlx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hnqzz.top/gtgrvnsqzt.html

Common Programming Examples Cheat Book
来源：http://hz.316326.xyz/gtogslxiap.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpthfaglu.html

【收录内容】
来源：http://hz.yj202588.top/gtgcmqnall.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sweek.top/gtrqqxueyi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.haohaochexian.top/gtaorvkgsp.html

SQL · Bash · C · C++
来源：http://hz.aizwys.cn/gtqkabqutm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yvedp.cn/gtughopgsq.html

【使用说明】
来源：http://hz.guowangkeji.top/gtlluvganq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhengqikj.top/gtxkzjcjsc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xuanzx.com/gtoxrfvsfl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zycfv.cn/gtjtcbjejk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gogol.net.cn/gtzdflrtbz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtaxyuwtsw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cheryme.top/gtwyolrhgx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yonumen.top/gtpwolczet.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gaohongyu789.top/gtsdmojwdd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinyuanbaomall.cn/gtrupgsysz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hammf.cn/gtqpnlfkdx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shangyingyoupin.top/gtphkofrjv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.fengsongda.top/gtjrpesvzw.html

【文件统计】
来源：http://hz.bjfxy.top/gtsukjgvji.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.guowangkeji.top/gtcprrcigs.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtoiebyaoi.html

目  录
来源：http://hz.yuxming.cn/gtdciipsjn.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtutjtclgq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jyoumei.cn/gtenxkozss.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtjfbfttjr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ybcxt.top/gtepomuytg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtvllepnsg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yonumen.top/gtcuxjpltw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gtxtiznbyj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtggegjnsk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenlongwang.top/gtntqqjrge.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtejnufzfs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhengqikj.top/gtrtualzeg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtcatiuebz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtotrytrrf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtlbraxcuf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ppjwa.cn/gtrrhprmeo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ehwqpu.com/gtvmtacpfy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtjhoeqrjz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sysykeji.top/gtbuhjgrjv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jlsjyb.cn/gtkuqvjkdz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jiagoushi.top/gtrwynqkjv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtejrnacnx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtxfikyiaz.html

================================================================================
来源：http://hz.fzhhl.top/gtvrqkujbr.html

A. 基础语法与类型
来源：http://hz.jinyuanbaomall.cn/gtjierxfot.html

================================================================================
来源：http://hz.yj202588.top/gtcajdvudn.html

[A01] Hello World
来源：http://hz.0kj1m.cn/gtftlockqa.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtguvhleww.html

PHP:  echo "Hello, World!";
来源：http://hz.cqqwz.cn/gtdcdyhngh.html

JS:   console.log("Hello, World!");
来源：http://hz.guannengcc.top/gtxpwucobc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtepffgowl.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgfzy.top/gtfhvnhdrm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.fzhhl.top/gtaplkhuij.html

Ruby: puts "Hello, World!"
来源：http://hz.yanxiufei.cn/gtpfcgdvpm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xuanzx.com/gtkvbtxpdw.html

[A02] 变量声明与赋值
来源：http://hz.bjfxy.top/gtbnaklrcd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.dashuyun.cn/gtxdkdnmtx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.bjfxy.top/gtffqhegpb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.redwolf501.top/gtfgqfxjuc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tanke756.top/gtwritqbaw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.guannengcc.top/gtpbisxkqr.html

Go:   name := "Alex"; age := 20
来源：http://hz.cucudq.cn/gtudpkjxei.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj202588.top/gthgohavqs.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nwbrower.top/gthnaopbyf.html

[A03] 常量定义
来源：http://hz.shuidangran.top/gtcwlpolsh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.dashuyun.cn/gtwngloxbs.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtjqdtwvhj.html

JS:   const PI = 3.14159;
来源：http://hz.gotoacloud.top/gtitbpuupn.html

TS:   const PI: number = 3.14159;
来源：http://hz.kuanghao11.cn/gtlqdppyiq.html

Java: static final double PI = 3.14159;
来源：http://hz.daria6918.cn/gtjkbfxdsp.html

Go:   const PI = 3.14159
来源：http://hz.jinqigfzy.top/gtkcqjjunu.html

Ruby: PI = 3.14159
来源：http://hz.yuanzhike.top/gtcdqjosud.html

C#:   const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtjybdsoae.html

[A04] 判断变量类型
来源：http://hz.hnqzz.top/gtarndinzq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shanyushiyangtech.top/gtfmeowagp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yanxiufei.cn/gtqbyeryxq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gotoacloud.top/gtneupjtyf.html

TS:   typeof x; x instanceof Date
来源：http://hz.tian-w.cn/gtfbgnjcun.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.tian-w.cn/gtjkiddyrt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhiwuduotai.top/gtxxkpxyvh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.pengpengdd.cyou/gthhdbtxzs.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhongyouzk.top/gtfraqqeke.html

[A05] 整数除法与取模
来源：http://hz.wangshuangyany.cn/gthzpvyflo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gzhubu.top/gtmrhfmawr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtleuqqayx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.dianchejie.cn/gttihqgkef.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ppjwa.cn/gtszfziazc.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtnpjbnqxs.html

Go:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtmqewjguq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtuepoowah.html

C#:   7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gtlhaqewfu.html

[A06] 字符串转数字
来源：http://hz.0kj1m.cn/gtizkvordq.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgufenzy.top/gtxhidepzd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xuanzx.com/gtamcdqjcw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yj20258.top/gtxrozkhgl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yueranfly.top/gtqpdhyiuc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ydzc1.top/gtxltntljx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhongyouzk.top/gtionucbll.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.daxiang520.top/gtuhqpbvqz.html


<!-- 参考信息 -->