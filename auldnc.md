代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.birdmap.top/gtcmuwwvvo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtpeubseda.html

[U60] PHP：JSON 编解码
来源：http://hz.jianghu66.top/gtylagatlb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigufen.top/gthesjsjqc.html

[U61] PHP：正则
来源：http://hz.yj20258.top/gtrdxzfbdd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtaisldgkd.html

[U62] PHP：日期对象
来源：http://hz.hywenlv.cn/gtgyokalnw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtmzoltuwf.html

[U63] PHP：文件读写
来源：http://hz.aibaodan.cn/gtkcgzzdwl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gttwadgrfd.html

[U64] PHP：目录遍历
来源：http://hz.mhx1999.top/gtltxyvmws.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xuanzx.com/gtptlovexj.html

[U65] PHP：会话
来源：http://hz.nanxuanxn.top/gtctvqeowv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gtxxfdullc.html

[U66] PHP：设置 Cookie
来源：http://hz.wangshuangyany.cn/gtyzuzxabd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtcqtygnxw.html

[U67] PHP：处理文件上传
来源：http://hz.hnqzz.top/gtvidnhxer.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gttqrusoqj.html

[U68] PHP：PDO 连接
来源：http://hz.dianchejie.cn/gtmxyqvpqx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hywenlv.cn/gtaenzqhhr.html

[U69] PHP：PDO 预处理
来源：http://hz.yangfankeji.com/gtebboibwg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtwqtbpmuz.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258888.top/gtogsvqdpt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gzhubu.top/gtztkniszg.html

[U71] PHP：抛出异常
来源：http://hz.tanke756.top/gteynbarqo.html

throw new RuntimeException("失败", 500);
来源：http://hz.hnxiangtu.top/gtmbyuvfwp.html

[U72] PHP：写错误日志
来源：http://hz.ybcxt.top/gtlezvzkgo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yonumen.top/gtwlwkmrzn.html

[U73] PHP：读取 ini 配置
来源：http://hz.sxryk.cn/gtvlqkdfcy.html

parse_ini_file("config.ini", true)
来源：http://hz.nwbrower.top/gtyheooety.html

[U74] PHP：读取环境变量
来源：http://hz.cheryme.top/gtbgyqoxxe.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sweek.top/gtgnbtpomh.html

[U75] PHP：依赖注入
来源：http://hz.tanke756.top/gtsysbpxnq.html

composer require psr/container
来源：http://hz.chenjidiqi.icu/gtiohzhrvo.html

[U76] PHP：简单路由
来源：http://hz.jqgfzy.top/gtopkfkkwh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258.top/gtajlxremd.html

[U77] PHP：模板渲染
来源：http://hz.chenjidiqi.icu/gtpfgwvtbh.html

composer require twig/twig
来源：http://hz.xinyue.icu/gtdlebyihj.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangtech.top/gthksizkhe.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangkeji.top/gtozgeqxjn.html

[U79] PHP：静态分析
来源：http://hz.tianlin.xyz/gtefutxuhg.html

composer require --dev phpstan/phpstan
来源：http://hz.nwbrower.top/gtoklwhvdx.html

[U80] PHP：代码规范修复
来源：http://hz.yonumen.top/gtizpsjeyx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhoulong.xyz/gtwivueotl.html

[U81] JS：初始化项目
来源：http://hz.yj20258888.top/gttjiyeskl.html

npm init -y;  npm i express
来源：http://hz.yonumen.top/gtxbotvemi.html

[U82] JS：package.json 脚本
来源：http://hz.yuxming.cn/gtzpftuqip.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhixingplan.top/gtdfakgrrg.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtpifwhudq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.aibaodan.cn/gtfxnuwutg.html

[U84] JS：CommonJS 写法
来源：http://hz.tian-w.cn/gtheglvqqv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nwbrower.top/gtftnsautd.html

[U85] JS：可选链
来源：http://hz.cashguo.top/gtuxpoxyxo.html

a?.b?.c
来源：http://hz.zhaomingkeji.xyz/gtlgqrumey.html

[U86] JS：空值合并
来源：http://hz.52xcode.cn/gtfixfdgaa.html

a ?? b
来源：http://hz.gaohongyu789.top/gtfjkblzso.html

[U87] JS：解构默认值
来源：http://hz.gaohongyu789.top/gtpsueyosp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ydjk.org.cn/gtgfnfsofx.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtxbkgdtzv.html

{ ...a, ...b }
来源：http://hz.tian-w.cn/gtzwhcqwpb.html

[U89] JS：数组去重
来源：http://hz.zhijiandao.cn/gtufekhhim.html

[...new Set(arr)]
来源：http://hz.cdnleiting.top/gtnxufuqyo.html

[U90] JS：数字数组排序
来源：http://hz.yangfankeji.com/gtrjikbuwi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtyrkokecy.html

[U91] JS：对象键值遍历
来源：http://hz.zhaomingkeji.xyz/gtkbjgsgtr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtyiqsanrw.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gttldyedfr.html

structuredClone(obj)
来源：http://hz.yvedp.cn/gtuoixmpru.html

[U93] JS：模板字符串
来源：http://hz.zhaomingkeji.xyz/gtajneqiaw.html

`共 ${n} 条`
来源：http://hz.chenlongwang.top/gtdgtjaedv.html

[U94] JS：箭头函数
来源：http://hz.vqdsnc.cn/gtyjjxszev.html

const double = x => x * 2;
来源：http://hz.dianchejie.cn/gttgxbipdd.html

[U95] JS：Promise 包装
来源：http://hz.daria6918.cn/gtqpbntpht.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtxbmsecxe.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtpimxbiwk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtnxatgfnb.html

[U97] JS：并发请求
来源：http://hz.yanxiufei.cn/gtsjzrultw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gttigzanry.html

[U98] JS：fetch 带 JSON
来源：http://hz.hfpthk.cn/gtptwvinih.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtvathhvkw.html

[U99] JS：事件监听
来源：http://hz.nanxuanxn.top/gtdjbxaaob.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gtjjsvawlc.html

[U100] JS：DOM 查询
来源：http://hz.andypj.xyz/gtomiqoack.html

document.querySelector(".item")
来源：http://hz.zdqjudy.top/gtghuzhrjk.html

[U101] JS：classList 操作
来源：http://hz.aibaodan.cn/gtbxlorhzm.html

el.classList.toggle("active")
来源：http://hz.pycfn.com/gtjjdtgvtf.html

[U102] JS：本地存储
来源：http://hz.cashguo.top/gtfyfmkxtj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhongyouzk.top/gtwzfhqyit.html

[U103] JS：定时器
来源：http://hz.guowangkeji.top/gtnethbgti.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cheryme.top/gtziffkfjq.html

[U104] JS：防抖
来源：http://hz.jinqigfzy.top/gtqowzfwpw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gthysbmikk.html

[U105] JS：节流
来源：http://hz.tianlin.xyz/gtaouhjqbs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhongyouzk.top/gtxialievd.html

[U106] JS：日期格式化
来源：http://hz.iojbl.cn/gtvxjgaiml.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinghuilouyu.cn/gtcyouaofr.html

[U107] JS：数字千分位
来源：http://hz.jqgfzy.top/gtnzvaarsv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.chenjidiqi.icu/gtxncsewld.html

[U108] JS：随机整数
来源：http://hz.hnqzz.top/gtfcyomnku.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ehwqpu.com/gtwbeyehsh.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtrdbayyzr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtzdcvuept.html

[U110] JS：数组分块
来源：http://hz.yanxiufei.cn/gtwixosedf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.bjfxy.top/gtbsxnjdak.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gtaoyzbgff.html

new Map(Object.entries(obj))
来源：http://hz.fzhhl.top/gtrrzbmphe.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gttpbinuuh.html

"7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtusakddaw.html

[U113] JS：正则替换全部
来源：http://hz.hnxiangtu.top/gtkojysvid.html

s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtqftwbhen.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtdqzogyqm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtafmhcrvw.html

[U115] JS：生成 UUID
来源：http://hz.ppjwa.cn/gtgedyyfbv.html

crypto.randomUUID()
来源：http://hz.sxryk.cn/gtqzedmifb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuanzx.com/gtidcnxfsf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jiagoushi.top/gtzvzkbwcn.html

[U117] JS：单元测试
来源：http://hz.yonumen.top/gtwihshsvj.html

npm i -D vitest;  npx vitest
来源：http://hz.xingfuxueyuan.xyz/gtjgieretj.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gthauakgtl.html

npm i -D vite;  npx vite
来源：http://hz.ywan-chungtsiang.top/gtvomolkna.html

[U119] JS：生产构建
来源：http://hz.hammf.cn/gtopwspqyg.html

npx vite build
来源：http://hz.ydjk.org.cn/gtaouvpxmh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.havefunace.top/gtxytbrjnu.html

import.meta.env.VITE_API_URL
来源：http://hz.guowangkeji.top/gtpiiaslyf.html

================================================================================
来源：http://hz.meibo888.top/gtppenxaza.html

统计汇总
来源：http://hz.svipenyu.cn/gthiaoxlsg.html

================================================================================
来源：http://hz.cucudq.cn/gtaignzfdc.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtazfqmxcd.html

Python ......... 252
来源：http://hz.hysaishi.cn/gtbtygjaln.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtjccmqsea.html

JavaScript ..... 252
来源：http://hz.meibo888.top/gtfdrrptig.html

TypeScript ..... 212
来源：http://hz.svipenyu.cn/gtosshxdvb.html

Java ........... 212
来源：http://hz.cucudq.cn/gtjbgluktt.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtfuxhenbr.html

Ruby ........... 212
来源：http://hz.xingfuxueyuan.xyz/gtuohachmb.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtippfboua.html

C .............. 30
来源：http://hz.jianghu66.top/gtegssitwu.html

C++ ............ 30
来源：http://hz.pengpengdd.cyou/gtgchpgnts.html

SQL ............ 90
来源：http://hz.vqdsnc.cn/gtuzqlvwqs.html

Bash ........... 80
来源：http://hz.xuetiantiany.cn/gtmiieehef.html

Kotlin ......... 15
来源：http://hz.haohaochexian.top/gtzzgusdvo.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtwmggqgdq.html

Lua ............ 10
来源：http://hz.redwolf501.top/gtrrfkxcmz.html

Perl ........... 10
来源：http://hz.yuanzhike.top/gtfkuuerqd.html

Scala .......... 10
来源：http://hz.mhx1999.top/gtqjucnxkq.html

------------------------------------
来源：http://hz.316326.xyz/gtnnysshur.html

合计 ........... 2106 条
来源：http://hz.hfpthk.cn/gtgukpgiyh.html

按章节统计：
来源：http://hz.hongshengwenyu.top/gtbautjxop.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtsycijjoz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtvhqoyrae.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtjngzgaxu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gthzomsrsu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuanzhike.top/gtafohxaax.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtvqbhslrx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtptcykyuw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtvhokrjbr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtqwtliqkv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gtigcerlll.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gthvyrglcu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtqxrujhal.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtlyozcxvc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yangfankeji.com/gtlcojdsya.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dianchejie.cn/gtdnujfgah.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtodfnuquh.html

Q SQL 专题                              90
来源：http://hz.yuxming.cn/gtigsjkmdo.html

R Bash 专题                             80
来源：http://hz.xinyue.icu/gtrowgvrbf.html

S C / C++ 专题                          60
来源：http://hz.gaohongyu789.top/gtdsygrblq.html

T 其他语言补充                          60
来源：http://hz.nanxuanxn.top/gtpbcnsahz.html

U 高频实用片段                         120
来源：http://hz.nwbrower.top/gtnfdrhxzn.html

------------------------------------
来源：http://hz.tanke756.top/gtbxetqipu.html

合计                                  2106 条
来源：http://hz.snrcjt.cn/gtjsjblwhc.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtdqzijpjv.html

使用提醒
来源：http://hz.mhx1999.top/gtsgcocygc.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtcjqaxgze.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shuidangran.top/gtqubwoihl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hfpthk.cn/gtszhejdaq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sysykeji.top/gtdmgdotwh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shzxlz.cn/gteivoxile.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.havefunace.top/gtlutsklje.html

—— 文件结束 ——
来源：http://hz.zhijiandao.cn/gtmapudurb.html

================================================================================
来源：http://hz.havefunace.top/gtvfpdgulo.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sweek.top/gteurldokn.html

Common Programming Examples Cheat Book
来源：http://hz.c1oappe.top/gtblemxrou.html

================================================================================
来源：http://hz.sysykeji.top/gttrmtvntw.html

【收录内容】
来源：http://hz.nwbrower.top/gtouvwazez.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xziqi.cn/gtkxdielkd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.c1oappe.top/gtdbzahnts.html

SQL · Bash · C · C++
来源：http://hz.yueranfly.top/gtuejlprcv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gotoacloud.top/gtzqsuhzyg.html

【使用说明】
来源：http://hz.havefunace.top/gtyqnnmzfc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ydjk.org.cn/gtgdgaiull.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gogol.net.cn/gtqbehbirs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hammf.cn/gtrngkhesk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sxryk.cn/gtonywonhv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtypnlqjdj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtfgfsxtwn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hfpthk.cn/gttqkmnbjn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.haohaochexian.top/gtjuczwqwb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtjacnbasq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgfzy.top/gtlylvnbus.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydzc1.top/gtwsraozdk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daxiang520.top/gtfsaotrav.html

【文件统计】
来源：http://hz.sweek.top/gtwmfwnivw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gtloupyjhc.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtvvshilfg.html

目  录
来源：http://hz.quarkkingdee.top/gtqazenppw.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtjmhqdclu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gttkssxfal.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aibaodan.cn/gtbddrgshg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtjwdbbftg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sxryk.cn/gtgraodluu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtrpeqjdsq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuxming.cn/gtjhevitqt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtjfvspmrz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nanxinkj.top/gtqocpiyiy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtsmaxxfbs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhaomingkeji.xyz/gtaywdpdmu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtsnioxslu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtgbkeraul.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gttphaqehe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yj20258.top/gtmplqrqcj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ivvv.top/gtoszeryau.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtngadsgtq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gaohongyu789.top/gtmykgpsfc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tianlin.xyz/gtvcmgxquo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zycfv.cn/gtooypjsav.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtsfkqcsoh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtgwxmktkr.html

================================================================================
来源：http://hz.mhx1999.top/gtfebwbooc.html

A. 基础语法与类型
来源：http://hz.kuanghao11.cn/gtgdegmsxq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdbhlfoud.html

[A01] Hello World
来源：http://hz.9152youxi.cn/gtrwnifajt.html

Py:   print("Hello, World!")
来源：http://hz.9152youxi.cn/gtubcyjlmh.html

PHP:  echo "Hello, World!";
来源：http://hz.meibo888.top/gttdkgexpp.html

JS:   console.log("Hello, World!");
来源：http://hz.cucudq.cn/gtttbzpfyd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yangfankeji.com/gtmrtdkyii.html

Java: System.out.println("Hello, World!");
来源：http://hz.cheryme.top/gtaugjmnbr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yuxming.cn/gtgdmdpwie.html

Ruby: puts "Hello, World!"
来源：http://hz.jinqigufen.top/gtqvcwljus.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.9152youxi.cn/gtoztmgcau.html

[A02] 变量声明与赋值
来源：http://hz.yj20258888.top/gtmeorkyub.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhongyouzk.top/gtxvivrddu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhoulong.xyz/gtyasmfmig.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hysaishi.cn/gtxzxbbluh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zdqjudy.top/gtlivvmpfk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daxiang520.top/gtelvanvev.html

Go:   name := "Alex"; age := 20
来源：http://hz.yangfankeji.com/gtgqrecttn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.iojbl.cn/gtmdpsoktk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhixingplan.top/gtqvvuebhj.html

[A03] 常量定义
来源：http://hz.jinqigufen.top/gtpuqtzzio.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hammf.cn/gtadawyxtn.html

PHP:  const PI = 3.14159;
来源：http://hz.shzxlz.cn/gtbgabittq.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gtcfcqzinw.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtcxontziw.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtkaradwai.html

Go:   const PI = 3.14159
来源：http://hz.gogol.net.cn/gtfsxgxodc.html

Ruby: PI = 3.14159
来源：http://hz.yvedp.cn/gtdzozrxhu.html

C#:   const double PI = 3.14159;
来源：http://hz.hammf.cn/gtijlcrxgv.html

[A04] 判断变量类型
来源：http://hz.iojbl.cn/gtcmlgpjzq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydjk.org.cn/gtfifypvwy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhiwuduotai.top/gtokcxwzeq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.fzhhl.top/gtrnsmrsol.html

TS:   typeof x; x instanceof Date
来源：http://hz.smart0.xyz/gtzuslqefk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jqgufenzy.top/gtzgwfelvh.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.9152youxi.cn/gtwbepbzgt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ybcxt.top/gtmpoijzrh.html

C#:   x.GetType().Name; x is int
来源：http://hz.meibo888.top/gtjdxfzoqb.html

[A05] 整数除法与取模
来源：http://hz.guannengcc.top/gtxsodpezz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jqgfzy.top/gtugyhqkdz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cqqwz.cn/gtdyxrcesf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gtzzeamrcu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtppcpaywu.html

Java: 7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gtpjihaimc.html

Go:   7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtrddqojlg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtkwrwpkbv.html

C#:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtslprbvqw.html

[A06] 字符串转数字
来源：http://hz.zhongyouzk.top/gtzdntdmcy.html

Py:   int("42"); float("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtmshyiksk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jiagoushi.top/gtnikgpwmz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hysaishi.cn/gtkfpxwshe.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hnqzz.top/gtkovajgqo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hnqzz.top/gtelcsalvw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gzhubu.top/gtlqkwooux.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nwbrower.top/gtugfkydpp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zdqjudy.top/gtnxnvqxig.html

[A07] 数字转字符串
来源：http://hz.dashuyun.cn/gtnnryvsow.html

Py:   str(42)
来源：http://hz.52xcode.cn/gtowfbbqbg.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj202588.top/gtewmovosp.html

JS:   String(42); (42).toString()
来源：http://hz.jinghuilouyu.cn/gtoyiabnnr.html

TS:   String(42)
来源：http://hz.hongshengwenyu.top/gtqbstxafm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zdqjudy.top/gtujrmarop.html

Go:   strconv.Itoa(42)
来源：http://hz.andypj.xyz/gtyjfkxlpg.html

Ruby: 42.to_s
来源：http://hz.jinyuanbaomall.cn/gtguxcqcgb.html

C#:   42.ToString()
来源：http://hz.zdqjudy.top/gtpxaqvbov.html

[A08] 取整与四舍五入
来源：http://hz.feifeiyinyue.top/gtqkvrttro.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nanxuanxn.top/gtahvwjmfk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.wangshuangyany.cn/gtsjoyycnc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.nanxuanxn.top/gttceqrktc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yongpay.top/gtepjlyaid.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yj202588.top/gtxkzkslnt.html


<!-- 参考信息 -->