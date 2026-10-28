代发 wailian999

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtiadhupxy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yuanzhike.top/gtpruobhye.html

[U56] PHP：命名参数
来源：http://hz.jinyuanbaomall.cn/gtwmwkbxws.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtpjbmsldg.html

[U57] PHP：字符串插值
来源：http://hz.guowangkeji.top/gtchhqxlwz.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtmymscont.html

[U58] PHP：数组三件套
来源：http://hz.xingfuxueyuan.xyz/gteahlshmq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.c1oappe.top/gtdbjbjmds.html

[U59] PHP：自定义排序
来源：http://hz.ydzc1.top/gtpqgacydi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtgxntrced.html

[U60] PHP：JSON 编解码
来源：http://hz.gaohongyu789.top/gtermenpne.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jiagoushi.top/gtduworolk.html

[U61] PHP：正则
来源：http://hz.jqgufenzy.top/gtknubldve.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtqsjexjjr.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtaioxkrai.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hysaishi.cn/gtbmdhfper.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtzolvunve.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhoulong.xyz/gtelinhunp.html

[U64] PHP：目录遍历
来源：http://hz.tanke756.top/gtzvaadltq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.quarkkingdee.top/gtyagsgiaz.html

[U65] PHP：会话
来源：http://hz.yuxming.cn/gtkvzunxxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yongpay.top/gtvozzyhty.html

[U66] PHP：设置 Cookie
来源：http://hz.yonumen.top/gtubigzqox.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fzhhl.top/gtirlaoeda.html

[U67] PHP：处理文件上传
来源：http://hz.xuetiantiany.cn/gttvsuerew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtqtuscvhl.html

[U68] PHP：PDO 连接
来源：http://hz.shangyingyoupin.top/gttiikbmfu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sysykeji.top/gtjfjycxzb.html

[U69] PHP：PDO 预处理
来源：http://hz.shzxlz.cn/gtqwnwugry.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gtpcoevtrc.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gtpayjjrou.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xziqi.cn/gtwsmcbtlc.html

[U71] PHP：抛出异常
来源：http://hz.guannengcc.top/gtkhzuthcp.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuanzx.com/gtptvurhli.html

[U72] PHP：写错误日志
来源：http://hz.jinghuilouyu.cn/gtjviuzchn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hysaishi.cn/gtnwxpeagv.html

[U73] PHP：读取 ini 配置
来源：http://hz.cashguo.top/gttsloytlv.html

parse_ini_file("config.ini", true)
来源：http://hz.tian-w.cn/gtacpndrab.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtizqvrixl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yangfankeji.com/gtopslnedg.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtjjtujope.html

composer require psr/container
来源：http://hz.zhoulong.xyz/gtwlnlhrmk.html

[U76] PHP：简单路由
来源：http://hz.kuanghao11.cn/gtbzktchvm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hysaishi.cn/gtdbanckuh.html

[U77] PHP：模板渲染
来源：http://hz.xylfe.cn/gtyrohphsx.html

composer require twig/twig
来源：http://hz.jqgufenzy.top/gtbxdhbmle.html

[U78] PHP：单元测试
来源：http://hz.fengsongda.top/gtkysxcplm.html

composer require --dev phpunit/phpunit
来源：http://hz.hywenlv.cn/gtohjisbmc.html

[U79] PHP：静态分析
来源：http://hz.jinyuanbaomall.cn/gtppcgnoyi.html

composer require --dev phpstan/phpstan
来源：http://hz.zhongyouzk.top/gtftkygrax.html

[U80] PHP：代码规范修复
来源：http://hz.sufxvd.cn/gtphfodgmc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yvedp.cn/gtihfhndco.html

[U81] JS：初始化项目
来源：http://hz.ybcxt.top/gtxehtrmgb.html

npm init -y;  npm i express
来源：http://hz.aizwys.cn/gtjdgnjpen.html

[U82] JS：package.json 脚本
来源：http://hz.wangdashe.top/gtwzxyqtnw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tanke756.top/gtlktblumx.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangshuangyany.cn/gtxgvmzlfk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xziqi.cn/gtizexgdlg.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gtihlxommh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hongshengwenyu.top/gtwbmmnokt.html

[U85] JS：可选链
来源：http://hz.jiagoushi.top/gtmizvjscb.html

a?.b?.c
来源：http://hz.shanyushiyangtech.top/gtyftoszyl.html

[U86] JS：空值合并
来源：http://hz.jinghuilouyu.cn/gtqdmsrtzk.html

a ?? b
来源：http://hz.zhiwuduotai.top/gtovkbsqgu.html

[U87] JS：解构默认值
来源：http://hz.dianchejie.cn/gtxlvhndzr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhiwuduotai.top/gtntatyikd.html

[U88] JS：对象展开合并
来源：http://hz.snrcjt.cn/gttwikhdlk.html

{ ...a, ...b }
来源：http://hz.gotoacloud.top/gtoubaewal.html

[U89] JS：数组去重
来源：http://hz.tanke756.top/gtflflcvap.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtruobxmyw.html

[U90] JS：数字数组排序
来源：http://hz.redwolf501.top/gtnmawkywc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtkolkgyok.html

[U91] JS：对象键值遍历
来源：http://hz.0kj1m.cn/gtdivceuqp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shangyingyoupin.top/gtqaqgsaia.html

[U92] JS：深拷贝
来源：http://hz.jinyuanbaomall.cn/gtjanqdpad.html

structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtyshlzhme.html

[U93] JS：模板字符串
来源：http://hz.cucudq.cn/gtagwdsemt.html

`共 ${n} 条`
来源：http://hz.svipenyu.cn/gtvkasurzd.html

[U94] JS：箭头函数
来源：http://hz.feifeiyinyue.top/gtbykmlqhf.html

const double = x => x * 2;
来源：http://hz.shanyushiyangkeji.top/gtmofwyxno.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtdiuexrge.html

new Promise((resolve, reject) => {})
来源：http://hz.daria6918.cn/gtyzgoqjln.html

[U96] JS：async/await 与异常
来源：http://hz.tanke756.top/gtoyrfcmmv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtibnnulch.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangtech.top/gtkgusyulc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtzvbzuslw.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenzaomai.com/gtebqewyqn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hysaishi.cn/gtwwvnjhkk.html

[U99] JS：事件监听
来源：http://hz.chenjidiqi.icu/gtcbsxpuuw.html

el.addEventListener("click", e => {})
来源：http://hz.zycfv.cn/gtzlzlzjwh.html

[U100] JS：DOM 查询
来源：http://hz.zhijiandao.cn/gtvhczcckj.html

document.querySelector(".item")
来源：http://hz.jyoumei.cn/gtplshklkx.html

[U101] JS：classList 操作
来源：http://hz.9152youxi.cn/gtrgdnccmn.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtusrnvhip.html

[U102] JS：本地存储
来源：http://hz.vqdsnc.cn/gtjnnwbqdn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fengsongda.top/gtmvisfypi.html

[U103] JS：定时器
来源：http://hz.sxryk.cn/gtfieooquc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gogol.net.cn/gtbebbmkil.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtdmewjjkc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtkzfxsbhq.html

[U105] JS：节流
来源：http://hz.jlsjyb.cn/gtcehqhdjz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.aizwys.cn/gtelntiaso.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtjpngrscr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sysykeji.top/gtuolzucvk.html

[U107] JS：数字千分位
来源：http://hz.zhaomingkeji.xyz/gtukbuabxa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtfkkanjai.html

[U108] JS：随机整数
来源：http://hz.yvedp.cn/gtdcyomgji.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtewylmndk.html

[U109] JS：数组分组
来源：http://hz.zycfv.cn/gtdecldfvq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtcbkgotuy.html

[U110] JS：数组分块
来源：http://hz.aibaodan.cn/gtxzwjmnzu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zycfv.cn/gtlhxiyaxu.html

[U111] JS：对象转 Map
来源：http://hz.yvedp.cn/gtsrznvhwe.html

new Map(Object.entries(obj))
来源：http://hz.redwolf501.top/gtuumssdej.html

[U112] JS：字符串补位
来源：http://hz.daxiang520.top/gtfjlxxqak.html

"7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtmlpuafqi.html

[U113] JS：正则替换全部
来源：http://hz.redwolf501.top/gtyunazxtq.html

s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtzudigvnf.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtrtqtcntl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtkzmadgei.html

[U115] JS：生成 UUID
来源：http://hz.xziqi.cn/gtnfmchfqj.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtolzknhcw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yueranfly.top/gtrccbegze.html

/** @param {string} name */ function f(name) {}
来源：http://hz.52xcode.cn/gtqarcbrow.html

[U117] JS：单元测试
来源：http://hz.birdmap.top/gtlpeljarf.html

npm i -D vitest;  npx vitest
来源：http://hz.ehwqpu.com/gtyyplsleh.html

[U118] JS：开发服务器
来源：http://hz.xziqi.cn/gtcaoqpwws.html

npm i -D vite;  npx vite
来源：http://hz.nanxuanxn.top/gtbkblovyz.html

[U119] JS：生产构建
来源：http://hz.pengpengdd.cyou/gtpxhfjxmy.html

npx vite build
来源：http://hz.haohaochexian.top/gtcyvrgaae.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.aizwys.cn/gtahjkecqr.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258888.top/gtbvoxjqne.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqboonhxn.html

统计汇总
来源：http://hz.9152youxi.cn/gttxnipfrb.html

================================================================================
来源：http://hz.zycfv.cn/gtuvnrsinu.html

按语言统计（条）：
来源：http://hz.shangyingyoupin.top/gtnxaypsfc.html

Python ......... 252
来源：http://hz.yangfankeji.com/gtlzgvlmoy.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtosaywvmy.html

JavaScript ..... 252
来源：http://hz.yangfankeji.com/gtdnbxegie.html

TypeScript ..... 212
来源：http://hz.jinqigfzy.top/gtxzohwaiv.html

Java ........... 212
来源：http://hz.yanxiufei.cn/gtnyyocfqt.html

Go ............. 212
来源：http://hz.chenjidiqi.icu/gtsysqqhdv.html

Ruby ........... 212
来源：http://hz.aizwys.cn/gtmdltwbby.html

C# ............. 212
来源：http://hz.andypj.xyz/gtmliwhzue.html

C .............. 30
来源：http://hz.aizwys.cn/gtkgqbyies.html

C++ ............ 30
来源：http://hz.zycfv.cn/gtmkesonof.html

SQL ............ 90
来源：http://hz.wangshuangyany.cn/gtiwyqyaot.html

Bash ........... 80
来源：http://hz.yj20258.top/gtdufgmich.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gtvxyqjhec.html

Swift .......... 15
来源：http://hz.yvedp.cn/gtaelitkjn.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtkrfvafdn.html

Perl ........... 10
来源：http://hz.ybcxt.top/gtueejlmqv.html

Scala .......... 10
来源：http://hz.dashuyun.cn/gtvpqptfzv.html

------------------------------------
来源：http://hz.52xcode.cn/gtdnmzlzid.html

合计 ........... 2106 条
来源：http://hz.birdmap.top/gtjknsymeo.html

按章节统计：
来源：http://hz.shangyingyoupin.top/gtyfgkhkbk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtlzyllxkv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtlkskdyjc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtvuaayotn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cheryme.top/gtmspcvmho.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tian-w.cn/gtpnmsdkdk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hfpthk.cn/gtkbgnfwth.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtdnxcmora.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258.top/gtfmprcjoi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtjtwyadvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtyjqymuiv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtrpfchxtl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtgweutook.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtgnztruie.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtcazjxfex.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.andypj.xyz/gtujagxwvo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtqhqngqka.html

Q SQL 专题                              90
来源：http://hz.jqgfzy.top/gtmqmztszt.html

R Bash 专题                             80
来源：http://hz.yvedp.cn/gteyplwmkc.html

S C / C++ 专题                          60
来源：http://hz.daxiang520.top/gtmpfbsssx.html

T 其他语言补充                          60
来源：http://hz.yongpay.top/gtxnxfgvgl.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gteabgwbfr.html

------------------------------------
来源：http://hz.snrcjt.cn/gtziqgprky.html

合计                                  2106 条
来源：http://hz.nwbrower.top/gtbckbbchh.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtxxopgtdi.html

使用提醒
来源：http://hz.xuanzx.com/gtoibsxxtl.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtreboznta.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gtbmwujuel.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nwbrower.top/gtymjyshgz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtevlnorgu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fengsongda.top/gtkwatmstr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtsiukifzl.html

—— 文件结束 ——
来源：http://hz.yuanzhike.top/gtiiwbqsoy.html

================================================================================
来源：http://hz.fzhhl.top/gtefnwwnah.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gttinfqakr.html

Common Programming Examples Cheat Book
来源：http://hz.cheryme.top/gtpfjtbnpj.html

================================================================================
来源：http://hz.yangfankeji.com/gtenodtvsr.html

【收录内容】
来源：http://hz.sufxvd.cn/gtnxlpqeba.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gotoacloud.top/gtxwansmdf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.pengpengdd.cyou/gtgmqkyxfs.html

SQL · Bash · C · C++
来源：http://hz.sufxvd.cn/gtmfrarhzy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xingfuxueyuan.xyz/gtgbtgyrep.html

【使用说明】
来源：http://hz.zycfv.cn/gtktxpwlnj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gthttwciqv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jlsjyb.cn/gtveinymsl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tianlin.xyz/gtyfkgwsys.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtbdrxebru.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xuanzx.com/gtfmtrzsex.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258.top/gtrguzeugt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.52xcode.cn/gtjovbeswx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fzhhl.top/gtukihlroh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.quarkkingdee.top/gtnjmjufms.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.quarkkingdee.top/gtlmnsoagn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shzxlz.cn/gtbbfctyfu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sweek.top/gtiofppdwn.html

【文件统计】
来源：http://hz.fzhhl.top/gtqligfgao.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.fengsongda.top/gtaqhggbrh.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtkvmvkmlf.html

目  录
来源：http://hz.jlsjyb.cn/gtkfwtslfx.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtjphykkro.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtmcrvitwz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.tanke756.top/gtbdpotqgm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtvgncugvw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gtmtaehzke.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gtxsfmrwap.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.dashuyun.cn/gtvotpbdnk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtlmxvvwgw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenjidiqi.icu/gttqmymcla.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtpbwcyxja.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtjlkawceh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtjeccfegp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtvauozzax.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtgvgsljvz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gthcueuerz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhongyouzk.top/gtfnlksfam.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtxhzuefsf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydzc1.top/gtqsaymfmc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinghuilouyu.cn/gtcdddwbrk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.9152youxi.cn/gtotwplkdm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtirmevrwz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtqmqvsmgk.html

================================================================================
来源：http://hz.jinqigufen.top/gtnmceygmr.html

A. 基础语法与类型
来源：http://hz.jqgufenzy.top/gtbtfztggl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtctzadeqv.html

[A01] Hello World
来源：http://hz.sxryk.cn/gticbdvnoz.html

Py:   print("Hello, World!")
来源：http://hz.birdmap.top/gtebdprqus.html

PHP:  echo "Hello, World!";
来源：http://hz.xingfuxueyuan.xyz/gtsyuhxcsz.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtvfbvbhpn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gaohongyu789.top/gtrhfzdtox.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj20258888.top/gteuzmazfp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtexubaedl.html

Ruby: puts "Hello, World!"
来源：http://hz.ydjk.org.cn/gtnofxddqm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtqtxhyvmf.html

[A02] 变量声明与赋值
来源：http://hz.xziqi.cn/gttrzbpwak.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xylfe.cn/gtcyimuywd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.mhx1999.top/gtoaletvmv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhongyouzk.top/gtxinmdyqw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jinyuanbaomall.cn/gtgdxfhdxk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtmveqhsfm.html

Go:   name := "Alex"; age := 20
来源：http://hz.zycfv.cn/gtqqqoutmq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yongpay.top/gtufetzjwr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuetiantiany.cn/gtwlculstv.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gthrmapafs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ppjwa.cn/gtsbftbswd.html

PHP:  const PI = 3.14159;
来源：http://hz.hnqzz.top/gtwkjmtoaf.html

JS:   const PI = 3.14159;
来源：http://hz.zhongyouzk.top/gttytooymy.html

TS:   const PI: number = 3.14159;
来源：http://hz.hysaishi.cn/gtajrsfixb.html

Java: static final double PI = 3.14159;
来源：http://hz.daria6918.cn/gtqimibuiw.html

Go:   const PI = 3.14159
来源：http://hz.yj20258.top/gtmhqccsnq.html

Ruby: PI = 3.14159
来源：http://hz.gaohongyu789.top/gthwhlogfp.html

C#:   const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtdusplqjt.html

[A04] 判断变量类型
来源：http://hz.jinghuilouyu.cn/gtetxiuadr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gaohongyu789.top/gtiwyacecj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtmhqzcyhk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinghuilouyu.cn/gthxqzitrv.html

TS:   typeof x; x instanceof Date
来源：http://hz.tian-w.cn/gtpwyxcgfs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jianghu66.top/gtngtavkgb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gtiwwbslnr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gogol.net.cn/gtntdatxbr.html

C#:   x.GetType().Name; x is int
来源：http://hz.cqqwz.cn/gtzywirvru.html

[A05] 整数除法与取模
来源：http://hz.redwolf501.top/gtmttpojgo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zycfv.cn/gtjfkgvulv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gthqvldyep.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenjidiqi.icu/gtvdeoqdtk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cdnleiting.top/gtdjiabpwo.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtkuzcowrk.html

Go:   7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gttmdrxrxr.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtujrzltwx.html

C#:   7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtpsmgszvq.html

[A06] 字符串转数字
来源：http://hz.c1oappe.top/gtnmsyipsy.html

Py:   int("42"); float("3.14")
来源：http://hz.zhongyouzk.top/gtjetpsypd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gotoacloud.top/gttfabrawb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.wangdashe.top/gtyzaxttse.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.andypj.xyz/gtpjaidjfq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.fzhhl.top/gtsjccqqzx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhixingplan.top/gtdvcmwari.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jianghu66.top/gtosiweafp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ydjk.org.cn/gtbgnajdjg.html

[A07] 数字转字符串
来源：http://hz.jinyuanbaomall.cn/gtztixisri.html

Py:   str(42)
来源：http://hz.ybcxt.top/gthitqydio.html

PHP:  (string) 42; strval(42)
来源：http://hz.ywan-chungtsiang.top/gtekcldfiu.html

JS:   String(42); (42).toString()
来源：http://hz.yonumen.top/gtdlrkqqaw.html

TS:   String(42)
来源：http://hz.aibaodan.cn/gtbzokfboe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.cheryme.top/gtzdijnpbq.html

Go:   strconv.Itoa(42)
来源：http://hz.yuanzhike.top/gtpzqonyis.html


<!-- 参考信息 -->