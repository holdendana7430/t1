代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.guannengcc.top/gtkxgzantf.html

"值: {$a}"
来源：http://hz.vqdsnc.cn/gtgudkyibe.html

[U58] PHP：数组三件套
来源：http://hz.jiagoushi.top/gtoxazoobk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj202588.top/gtsgdkorun.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtrawrkrbj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinyuanbaomall.cn/gtirugffbi.html

[U60] PHP：JSON 编解码
来源：http://hz.pycfn.com/gtrtjuslse.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj202588.top/gtdbjelatr.html

[U61] PHP：正则
来源：http://hz.pycfn.com/gtvrbwmioz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtopzoapwv.html

[U62] PHP：日期对象
来源：http://hz.yuxming.cn/gtmyzvnnwr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.andypj.xyz/gtnxqzheif.html

[U63] PHP：文件读写
来源：http://hz.zhoulong.xyz/gtkyipvqaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pengpengdd.cyou/gtjxexdcdi.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtqrrccejn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhoulong.xyz/gtpzfisgfb.html

[U65] PHP：会话
来源：http://hz.52xcode.cn/gtciwdchum.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xinyue.icu/gtnmsetqnm.html

[U66] PHP：设置 Cookie
来源：http://hz.bjfxy.top/gtcplmzwhm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinyuanbaomall.cn/gteucxefwq.html

[U67] PHP：处理文件上传
来源：http://hz.sysykeji.top/gtcjrznlws.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinqigufen.top/gtpkbqbplw.html

[U68] PHP：PDO 连接
来源：http://hz.0kj1m.cn/gtxabimbyo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cdnleiting.top/gtjfxcpzpw.html

[U69] PHP：PDO 预处理
来源：http://hz.pengpengdd.cyou/gthsotihqi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.kuanghao11.cn/gtyldehdfz.html

[U70] PHP：PDO 事务
来源：http://hz.ppjwa.cn/gtiupezqli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtyjxlljey.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gtzlhyfqbu.html

throw new RuntimeException("失败", 500);
来源：http://hz.fzhhl.top/gtxoznslgm.html

[U72] PHP：写错误日志
来源：http://hz.gogol.net.cn/gttzoyxwfp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yj20258.top/gtoussatsb.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhoulong.xyz/gtojehympr.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gtxsqyrziy.html

[U74] PHP：读取环境变量
来源：http://hz.quarkkingdee.top/gtglvvlvmy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtyoehhhly.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtobluisvd.html

composer require psr/container
来源：http://hz.iojbl.cn/gtzhzvgrlb.html

[U76] PHP：简单路由
来源：http://hz.redwolf501.top/gtdnpitbbm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yueranfly.top/gtclsyzdce.html

[U77] PHP：模板渲染
来源：http://hz.gzhubu.top/gtjajkzmnr.html

composer require twig/twig
来源：http://hz.pengpengdd.cyou/gthxdcaltx.html

[U78] PHP：单元测试
来源：http://hz.daxiang520.top/gtoxqpdkpi.html

composer require --dev phpunit/phpunit
来源：http://hz.shuidangran.top/gtnszsruhd.html

[U79] PHP：静态分析
来源：http://hz.ppjwa.cn/gtgzrlxgkh.html

composer require --dev phpstan/phpstan
来源：http://hz.redwolf501.top/gtwgggngcp.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtjqfwzocj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shangyingyoupin.top/gtcdcvccdm.html

[U81] JS：初始化项目
来源：http://hz.birdmap.top/gtylrhojld.html

npm init -y;  npm i express
来源：http://hz.jyoumei.cn/gtohrrmbvk.html

[U82] JS：package.json 脚本
来源：http://hz.daxiang520.top/gtjvbatiiw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtjwcbhrxj.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuanzhike.top/gtpduaejkf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hnxiangtu.top/gtchbxmxcd.html

[U84] JS：CommonJS 写法
来源：http://hz.shzxlz.cn/gtjeztxdil.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jiagoushi.top/gtdhankwsw.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gtkzsjzruu.html

a?.b?.c
来源：http://hz.zhiwuduotai.top/gtevggwckf.html

[U86] JS：空值合并
来源：http://hz.zhixingplan.top/gtrfbcahpl.html

a ?? b
来源：http://hz.wangshuangyany.cn/gtytachqin.html

[U87] JS：解构默认值
来源：http://hz.jiagoushi.top/gtjfldcuoq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zdqjudy.top/gtkzdwhnxv.html

[U88] JS：对象展开合并
来源：http://hz.gogol.net.cn/gtapvabwbl.html

{ ...a, ...b }
来源：http://hz.hysaishi.cn/gthjhkvpoc.html

[U89] JS：数组去重
来源：http://hz.yueranfly.top/gtsaflgzgq.html

[...new Set(arr)]
来源：http://hz.xinyue.icu/gtwupnfivq.html

[U90] JS：数字数组排序
来源：http://hz.sxryk.cn/gtvmbeejup.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtvpgqeqpf.html

[U91] JS：对象键值遍历
来源：http://hz.xziqi.cn/gtshydamvd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gtpdbwcqhv.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gtpukozaok.html

structuredClone(obj)
来源：http://hz.jqgfzy.top/gtdyzwodnm.html

[U93] JS：模板字符串
来源：http://hz.yj20258.top/gtgrxwtvdr.html

`共 ${n} 条`
来源：http://hz.yuxming.cn/gtutpfslrf.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtwwfxciyk.html

const double = x => x * 2;
来源：http://hz.c1oappe.top/gtvklvjzxa.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtranmpfip.html

new Promise((resolve, reject) => {})
来源：http://hz.hywenlv.cn/gtqfdkayxg.html

[U96] JS：async/await 与异常
来源：http://hz.yj202588.top/gtlwyuknsg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtqbsbqtei.html

[U97] JS：并发请求
来源：http://hz.ybcxt.top/gtsnlhhykx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtipfghqoe.html

[U98] JS：fetch 带 JSON
来源：http://hz.hongshengwenyu.top/gtpamdidmh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258.top/gtsobydshq.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtrtplragr.html

el.addEventListener("click", e => {})
来源：http://hz.jinghuilouyu.cn/gtfkgngkkp.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gtghpadtrp.html

document.querySelector(".item")
来源：http://hz.hongshengwenyu.top/gtyujmmpzi.html

[U101] JS：classList 操作
来源：http://hz.aizwys.cn/gtwjefhkku.html

el.classList.toggle("active")
来源：http://hz.nanxuanxn.top/gtdajpysjm.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtqkvmlscz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuetiantiany.cn/gtusxawdzt.html

[U103] JS：定时器
来源：http://hz.quarkkingdee.top/gttbikgvps.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenzaomai.com/gtiposoxmu.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtuoqvkfqy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtiqrgyzmt.html

[U105] JS：节流
来源：http://hz.tanke756.top/gttglyzmag.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xingfuxueyuan.xyz/gtckuudejb.html

[U106] JS：日期格式化
来源：http://hz.0kj1m.cn/gtdkaspmms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gthzpcjjjo.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gtcwisachh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtruoczbco.html

[U108] JS：随机整数
来源：http://hz.smart0.xyz/gthmornfbh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangdashe.top/gtsyirsumq.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtnaciyyyz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtswfczeym.html

[U110] JS：数组分块
来源：http://hz.hysaishi.cn/gtqfkeamgc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jlsjyb.cn/gticwvjgcc.html

[U111] JS：对象转 Map
来源：http://hz.svipenyu.cn/gtsdzinfwz.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangkeji.top/gtkrlfqlxl.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtzbuztgrn.html

"7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gterikotkt.html

[U113] JS：正则替换全部
来源：http://hz.zhoulong.xyz/gtplexfrzx.html

s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtglloghpb.html

[U114] JS：JSON 深比较
来源：http://hz.quarkkingdee.top/gtjdpricll.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhoulong.xyz/gtyglewqmv.html

[U115] JS：生成 UUID
来源：http://hz.jqgfzy.top/gttrpblhis.html

crypto.randomUUID()
来源：http://hz.iojbl.cn/gtwvikiufy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.bjfxy.top/gtxzedijvh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.mhx1999.top/gtonavoxbl.html

[U117] JS：单元测试
来源：http://hz.zhoulong.xyz/gtwufwezar.html

npm i -D vitest;  npx vitest
来源：http://hz.jinyuanbaomall.cn/gttznleaea.html

[U118] JS：开发服务器
来源：http://hz.ppjwa.cn/gtgkwmaezd.html

npm i -D vite;  npx vite
来源：http://hz.cqqwz.cn/gtnyhxgiyz.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtzysxulgw.html

npx vite build
来源：http://hz.jlsjyb.cn/gtbemkkvpf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tian-w.cn/gtjtcietgy.html

import.meta.env.VITE_API_URL
来源：http://hz.tian-w.cn/gtmzkfpffv.html

================================================================================
来源：http://hz.chenlongwang.top/gtitroyfcy.html

统计汇总
来源：http://hz.cdnleiting.top/gtywkbesuc.html

================================================================================
来源：http://hz.guowangkeji.top/gtslkanfcu.html

按语言统计（条）：
来源：http://hz.wangshuangyany.cn/gtnslbmhvm.html

Python ......... 252
来源：http://hz.jinqigfzy.top/gtrsgomanl.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtspkwhpjw.html

JavaScript ..... 252
来源：http://hz.yj20258888.top/gtzmiqfmph.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtokfkmqvr.html

Java ........... 212
来源：http://hz.hywenlv.cn/gtekztlqnt.html

Go ............. 212
来源：http://hz.hysaishi.cn/gtgiofoahc.html

Ruby ........... 212
来源：http://hz.ydzc1.top/gtzssgdcjv.html

C# ............. 212
来源：http://hz.sweek.top/gtclxarnhc.html

C .............. 30
来源：http://hz.guannengcc.top/gtlltgffyw.html

C++ ............ 30
来源：http://hz.cdnleiting.top/gtjmrpydpt.html

SQL ............ 90
来源：http://hz.mhx1999.top/gtngscheah.html

Bash ........... 80
来源：http://hz.cqqwz.cn/gtsokjhfxn.html

Kotlin ......... 15
来源：http://hz.gaohongyu789.top/gtjxkfuxib.html

Swift .......... 15
来源：http://hz.zhixingplan.top/gtyrnzpmsu.html

Lua ............ 10
来源：http://hz.cdnleiting.top/gtilbxtbrf.html

Perl ........... 10
来源：http://hz.xylfe.cn/gttsyzondu.html

Scala .......... 10
来源：http://hz.yueranfly.top/gtcntrqxsk.html

------------------------------------
来源：http://hz.cashguo.top/gtlwhvijpz.html

合计 ........... 2106 条
来源：http://hz.jinyuanbaomall.cn/gtobvygzvi.html

按章节统计：
来源：http://hz.zhijiandao.cn/gtmqeqruda.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtfdbcmfsd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtpsgfivkk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gticolgzsn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtqtfvfyrs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.svipenyu.cn/gtcvelftyf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtzylnidtx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtppvbvgrf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtfvccatbu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtnocizqsl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtgfxtndfl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtrtpsbnmj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtgekxttsr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtfywtofom.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtuvipxjzw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.snrcjt.cn/gtxcrlafxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtzcwbtwax.html

Q SQL 专题                              90
来源：http://hz.bjfxy.top/gtapglzsks.html

R Bash 专题                             80
来源：http://hz.316326.xyz/gtxndalspz.html

S C / C++ 专题                          60
来源：http://hz.yuxming.cn/gtehewfysj.html

T 其他语言补充                          60
来源：http://hz.xylfe.cn/gtpmmjqdml.html

U 高频实用片段                         120
来源：http://hz.fengsongda.top/gtkmflcisw.html

------------------------------------
来源：http://hz.jlsjyb.cn/gtwzazzlxo.html

合计                                  2106 条
来源：http://hz.xuetiantiany.cn/gtofawxnou.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtaaarvinz.html

使用提醒
来源：http://hz.hnqzz.top/gteapvcjfz.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtanriubtp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhixingplan.top/gtbigdmncg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shzxlz.cn/gtgleqbiqc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shangyingyoupin.top/gtwwemqsps.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhixingplan.top/gtbbivrrtx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.smart0.xyz/gtogqvyhtt.html

—— 文件结束 ——
来源：http://hz.zhaomingkeji.xyz/gttkoliopj.html

================================================================================
来源：http://hz.iojbl.cn/gthhmhhkoz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtormhubcp.html

Common Programming Examples Cheat Book
来源：http://hz.tian-w.cn/gtlsmjcdlj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtstsgbzcc.html

【收录内容】
来源：http://hz.hysaishi.cn/gtouwepvld.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cashguo.top/gtpgbnhazz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hysaishi.cn/gtbghjhkiw.html

SQL · Bash · C · C++
来源：http://hz.xuetiantiany.cn/gtryqkcxkd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtmisccdrk.html

【使用说明】
来源：http://hz.52xcode.cn/gthnqzvazi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sweek.top/gtcuxdynlc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydjk.org.cn/gtvzizeihj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shangyingyoupin.top/gtqvuroqlx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxinkj.top/gtctistjze.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.c1oappe.top/gtgykyrwqr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhengqikj.top/gtrmpikizk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtkrfasivj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.svipenyu.cn/gtsbsawuig.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhengqikj.top/gtotlkoxtu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj20258.top/gtcigzsiik.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gotoacloud.top/gtvvkpjsrv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.andypj.xyz/gtvhdwnyyf.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtkxfoasmk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yuxming.cn/gtbnbqxnga.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gtcwcksxvc.html

目  录
来源：http://hz.daria6918.cn/gtkikdeacd.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtdjjazoka.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtfxzqedtu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtkuxedzwd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yongpay.top/gtzgwccziy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtztugxjuz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.0kj1m.cn/gtvakujfdl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtqdgixieb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtrvbfrxoy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtlggdapxi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtcxmwflxj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtrqaehycv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtwtbnhjuz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtvwcspmdh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtnfuehxzl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtbjuyiqlw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.haohaochexian.top/gtweudvogs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtzzoqpluu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtinqhbmcd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fengsongda.top/gtnkexkhzj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hammf.cn/gtjdxyufsa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtsuybpvhe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtjhohafku.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvjvvnrou.html

A. 基础语法与类型
来源：http://hz.snrcjt.cn/gtgjtzerpl.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgdmmshay.html

[A01] Hello World
来源：http://hz.shuidangran.top/gtclbeutvx.html

Py:   print("Hello, World!")
来源：http://hz.gotoacloud.top/gtymwoetyw.html

PHP:  echo "Hello, World!";
来源：http://hz.daria6918.cn/gtahpgvids.html

JS:   console.log("Hello, World!");
来源：http://hz.vqdsnc.cn/gtdjdkjzjq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ydjk.org.cn/gtqpmcgcxd.html

Java: System.out.println("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtffxighhb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.quarkkingdee.top/gtrmyegzox.html

Ruby: puts "Hello, World!"
来源：http://hz.xziqi.cn/gtdbcexifv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258.top/gtjmrohzjy.html

[A02] 变量声明与赋值
来源：http://hz.zhijiandao.cn/gtmhtxnxpv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.52xcode.cn/gttqrobzzb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhiwuduotai.top/gtagqaczza.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gaohongyu789.top/gtmrhmlakw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cheryme.top/gtxbtqutzd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.tanke756.top/gtlfrnphkv.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinqigfzy.top/gtztgorabe.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shangyingyoupin.top/gtccqgghiq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtlztapckq.html

[A03] 常量定义
来源：http://hz.hysaishi.cn/gtiouyqxst.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zdqjudy.top/gtdvfmszjm.html

PHP:  const PI = 3.14159;
来源：http://hz.daxiang520.top/gtrelorzld.html

JS:   const PI = 3.14159;
来源：http://hz.yangfankeji.com/gtheptpans.html

TS:   const PI: number = 3.14159;
来源：http://hz.yj20258.top/gtcqnzfmpq.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtqqwwbmtq.html

Go:   const PI = 3.14159
来源：http://hz.jinqigfzy.top/gttuqiucme.html

Ruby: PI = 3.14159
来源：http://hz.xingfuxueyuan.xyz/gtashesoas.html

C#:   const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtpmpqacdl.html

[A04] 判断变量类型
来源：http://hz.xuetiantiany.cn/gtjbhdsmqx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.c1oappe.top/gthqiqkbbp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.svipenyu.cn/gtnajyblfc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinghuilouyu.cn/gtjwyzqlgm.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigfzy.top/gtacdmewnt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cashguo.top/gtqprwugoa.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yonumen.top/gtlzduiina.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.snrcjt.cn/gticfghnjh.html

C#:   x.GetType().Name; x is int
来源：http://hz.xingfuxueyuan.xyz/gtgregbpae.html

[A05] 整数除法与取模
来源：http://hz.ydjk.org.cn/gthwixdvzp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.aizwys.cn/gtdvokpsso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhixingplan.top/gtsxcldvry.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.mhx1999.top/gtprfixtlo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.0kj1m.cn/gtfpfyqbtc.html

Java: 7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gthgzkjtxp.html

Go:   7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtuwgequza.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gttlpcjndi.html

C#:   7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtjwgjdftm.html

[A06] 字符串转数字
来源：http://hz.c1oappe.top/gtvbwppcjl.html

Py:   int("42"); float("3.14")
来源：http://hz.birdmap.top/gtzoequbhq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hywenlv.cn/gtqwbnoexh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aizwys.cn/gtbuqyswhu.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hammf.cn/gtjqlnablg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hfpthk.cn/gtuindrftb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj20258888.top/gtuoaibbry.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.quarkkingdee.top/gtkskqvcqc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yanxiufei.cn/gtuynvpyct.html

[A07] 数字转字符串
来源：http://hz.nanxuanxn.top/gtlxnujqht.html

Py:   str(42)
来源：http://hz.birdmap.top/gtafbncsdv.html

PHP:  (string) 42; strval(42)
来源：http://hz.yangfankeji.com/gthnkaaqlf.html

JS:   String(42); (42).toString()
来源：http://hz.chenzaomai.com/gthnwbgkgg.html

TS:   String(42)
来源：http://hz.c1oappe.top/gtdmudtlze.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhengqikj.top/gtrikncveo.html

Go:   strconv.Itoa(42)
来源：http://hz.gotoacloud.top/gtexjvmqqc.html

Ruby: 42.to_s
来源：http://hz.svipenyu.cn/gtidvggasy.html

C#:   42.ToString()
来源：http://hz.jinyuanbaomall.cn/gtjhracxwi.html

[A08] 取整与四舍五入
来源：http://hz.yongpay.top/gtsbupwmfl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.chenlongwang.top/gtpydhohdn.html


<!-- 参考信息 -->