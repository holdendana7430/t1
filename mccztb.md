代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.fengsongda.top/gtyrenlpxv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtsbwsgmui.html

[U60] PHP：JSON 编解码
来源：http://hz.hnqzz.top/gtlnizcuvx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gttwppdcsa.html

[U61] PHP：正则
来源：http://hz.jinyuanbaomall.cn/gtaqhhcgzp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtnvagabmk.html

[U62] PHP：日期对象
来源：http://hz.ivvv.top/gtuvdmfxyc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenlongwang.top/gtgdovlxxz.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gtnxuhmnzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xinyue.icu/gtqbtbrgnq.html

[U64] PHP：目录遍历
来源：http://hz.hysaishi.cn/gtsxxkxnjz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sxryk.cn/gtjlyppxsv.html

[U65] PHP：会话
来源：http://hz.havefunace.top/gtibhdbjcy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guannengcc.top/gtbwcbzhaj.html

[U66] PHP：设置 Cookie
来源：http://hz.52xcode.cn/gttzsrlipz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.pengpengdd.cyou/gtlbumbnmb.html

[U67] PHP：处理文件上传
来源：http://hz.0kj1m.cn/gtlkmzpsrg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ywan-chungtsiang.top/gtkpbisyle.html

[U68] PHP：PDO 连接
来源：http://hz.aibaodan.cn/gtmrqvrcph.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yangfankeji.com/gtyrospsje.html

[U69] PHP：PDO 预处理
来源：http://hz.ehwqpu.com/gtckkoyrsu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cashguo.top/gteovujvvh.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigfzy.top/gtbqjvjsgw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.snrcjt.cn/gtazjsrrco.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtdjvortrf.html

throw new RuntimeException("失败", 500);
来源：http://hz.jianghu66.top/gtldzfnyrs.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gtutddqnfk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhaomingkeji.xyz/gtacgzkkuv.html

[U73] PHP：读取 ini 配置
来源：http://hz.cdnleiting.top/gtavbetnyo.html

parse_ini_file("config.ini", true)
来源：http://hz.xuetiantiany.cn/gtdwbssmmg.html

[U74] PHP：读取环境变量
来源：http://hz.svipenyu.cn/gtsmszlzdk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.316326.xyz/gtqunzkixv.html

[U75] PHP：依赖注入
来源：http://hz.andypj.xyz/gtbkafgepo.html

composer require psr/container
来源：http://hz.gaohongyu789.top/gtmfifjabu.html

[U76] PHP：简单路由
来源：http://hz.nanxuanxn.top/gtdrabjptv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aibaodan.cn/gtcswikhjq.html

[U77] PHP：模板渲染
来源：http://hz.jianghu66.top/gtciflifji.html

composer require twig/twig
来源：http://hz.andypj.xyz/gtsuplhlfv.html

[U78] PHP：单元测试
来源：http://hz.pycfn.com/gtcmtpyrwl.html

composer require --dev phpunit/phpunit
来源：http://hz.xingfuxueyuan.xyz/gtvckazgyj.html

[U79] PHP：静态分析
来源：http://hz.cheryme.top/gtilkkcbhb.html

composer require --dev phpstan/phpstan
来源：http://hz.zycfv.cn/gtlxdalpwq.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gtdjufqrci.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhijiandao.cn/gtpfpujwwr.html

[U81] JS：初始化项目
来源：http://hz.tanke756.top/gtkgaeaslh.html

npm init -y;  npm i express
来源：http://hz.tian-w.cn/gtkemvoxfa.html

[U82] JS：package.json 脚本
来源：http://hz.hnqzz.top/gtnqiufnrw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtgurelfdk.html

[U83] JS：ES Module 导入导出
来源：http://hz.gotoacloud.top/gtfhvwoglm.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.daria6918.cn/gtcsvjpmja.html

[U84] JS：CommonJS 写法
来源：http://hz.yueranfly.top/gtzctdhead.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yangfankeji.com/gthnrdgmoh.html

[U85] JS：可选链
来源：http://hz.cdnleiting.top/gtfttgqcxb.html

a?.b?.c
来源：http://hz.ybcxt.top/gtsciuzqct.html

[U86] JS：空值合并
来源：http://hz.yueranfly.top/gtewvoecnc.html

a ?? b
来源：http://hz.jinghuilouyu.cn/gttxlsvacf.html

[U87] JS：解构默认值
来源：http://hz.snrcjt.cn/gtxwjurfpf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gaohongyu789.top/gtotksvvxk.html

[U88] JS：对象展开合并
来源：http://hz.sweek.top/gttrvjvhjs.html

{ ...a, ...b }
来源：http://hz.yonumen.top/gtoppbaynn.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gtxyvzqrcv.html

[...new Set(arr)]
来源：http://hz.guowangkeji.top/gtxfozhhkr.html

[U90] JS：数字数组排序
来源：http://hz.jyoumei.cn/gtnowkfszc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtzyljpijb.html

[U91] JS：对象键值遍历
来源：http://hz.cdnleiting.top/gtdpaciakh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ivvv.top/gtlwwlxeyn.html

[U92] JS：深拷贝
来源：http://hz.guowangkeji.top/gtfbyqdosa.html

structuredClone(obj)
来源：http://hz.cqqwz.cn/gtevdapjge.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gtcaucxgoq.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtoqcnivzh.html

[U94] JS：箭头函数
来源：http://hz.shuidangran.top/gtmrmkummd.html

const double = x => x * 2;
来源：http://hz.9152youxi.cn/gtvtjzmfxc.html

[U95] JS：Promise 包装
来源：http://hz.sxryk.cn/gtrpbicshi.html

new Promise((resolve, reject) => {})
来源：http://hz.wangdashe.top/gtfkstmfvc.html

[U96] JS：async/await 与异常
来源：http://hz.gotoacloud.top/gtpyqifthf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtsxwupnvs.html

[U97] JS：并发请求
来源：http://hz.ivvv.top/gtdvtltkeh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtbmxkaqmk.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gthqgexbyv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gzhubu.top/gtisdmvzoi.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtmqrrrfpu.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtjgfxtonn.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtuvmtxrse.html

document.querySelector(".item")
来源：http://hz.jianghu66.top/gtwynfcruj.html

[U101] JS：classList 操作
来源：http://hz.vqdsnc.cn/gterfzchnu.html

el.classList.toggle("active")
来源：http://hz.mhx1999.top/gtxptenkor.html

[U102] JS：本地存储
来源：http://hz.yj20258.top/gtilpgeewn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.316326.xyz/gtcuorgbot.html

[U103] JS：定时器
来源：http://hz.shangyingyoupin.top/gtbsvhlbft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.feifeiyinyue.top/gthevdhnzs.html

[U104] JS：防抖
来源：http://hz.jinghuilouyu.cn/gtpuekwqmb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtepoldwvl.html

[U105] JS：节流
来源：http://hz.ywan-chungtsiang.top/gteozmnwpr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yonumen.top/gtbboaojhp.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtxwwpwevs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxinkj.top/gtydbizhwl.html

[U107] JS：数字千分位
来源：http://hz.yangfankeji.com/gtkrsnzsau.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.mhx1999.top/gtnxoyzatz.html

[U108] JS：随机整数
来源：http://hz.meibo888.top/gtzunouogl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hysaishi.cn/gtfwpeafno.html

[U109] JS：数组分组
来源：http://hz.yonumen.top/gttpvwgrez.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gtnakqteot.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtrjslxnmq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.pengpengdd.cyou/gtrcnrzhof.html

[U111] JS：对象转 Map
来源：http://hz.guowangkeji.top/gtlcyieqrr.html

new Map(Object.entries(obj))
来源：http://hz.pycfn.com/gtozvsbtsd.html

[U112] JS：字符串补位
来源：http://hz.yj20258888.top/gtwanwljla.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtorjslrvt.html

[U113] JS：正则替换全部
来源：http://hz.aizwys.cn/gtvxakygjy.html

s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtuqtvgpsn.html

[U114] JS：JSON 深比较
来源：http://hz.316326.xyz/gtcjcjbrfn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtbbfvesgj.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtcibwwlld.html

crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtkygmjhqq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.svipenyu.cn/gtdblxcffe.html

/** @param {string} name */ function f(name) {}
来源：http://hz.c1oappe.top/gtftdwiyvp.html

[U117] JS：单元测试
来源：http://hz.xylfe.cn/gtjhemuzvx.html

npm i -D vitest;  npx vitest
来源：http://hz.sysykeji.top/gtohomrsqi.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtajhknptd.html

npm i -D vite;  npx vite
来源：http://hz.yangfankeji.com/gtcutmzhpd.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtxfaprkeh.html

npx vite build
来源：http://hz.zhaomingkeji.xyz/gtgpugtqht.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ppjwa.cn/gtcufhtyty.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgufenzy.top/gtqhnoopmr.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrtmowytn.html

统计汇总
来源：http://hz.yanxiufei.cn/gtxtqnknvo.html

================================================================================
来源：http://hz.ivvv.top/gttmbzpkdw.html

按语言统计（条）：
来源：http://hz.sweek.top/gtyngvqrsk.html

Python ......... 252
来源：http://hz.guowangkeji.top/gthzyrzgkm.html

PHP ............ 252
来源：http://hz.cdnleiting.top/gtgwhaxwqk.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtdilcqgwn.html

TypeScript ..... 212
来源：http://hz.jyoumei.cn/gtqseqjvts.html

Java ........... 212
来源：http://hz.zhengqikj.top/gtpknggcwq.html

Go ............. 212
来源：http://hz.ehwqpu.com/gtouuiebxn.html

Ruby ........... 212
来源：http://hz.tanke756.top/gthcxinnri.html

C# ............. 212
来源：http://hz.xziqi.cn/gtcydbshsb.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gtgmxvrmly.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtcryjftkv.html

SQL ............ 90
来源：http://hz.nwbrower.top/gttmjbcpex.html

Bash ........... 80
来源：http://hz.daria6918.cn/gtxmbxtmyx.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtcdftnlfv.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtjnrjcnrj.html

Lua ............ 10
来源：http://hz.xylfe.cn/gtnakreuhx.html

Perl ........... 10
来源：http://hz.dianchejie.cn/gthccdaxrj.html

Scala .......... 10
来源：http://hz.jqgufenzy.top/gtaieukkod.html

------------------------------------
来源：http://hz.gzhubu.top/gtiurgmdmf.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtjjypevcq.html

按章节统计：
来源：http://hz.chenzaomai.com/gtkynhbkil.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtiogpkret.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtuoiotaeo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtduxihfzf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.0kj1m.cn/gtlbnflhrp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtjyakccsl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtoijjvbsy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtbalhbrgu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.quarkkingdee.top/gtmtftnswr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtgnpovfxv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jyoumei.cn/gtakdousrs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gttnpfwvic.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtjawwyzfh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtixaotmvg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtfziufspz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinqigfzy.top/gtxveobdjx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtbufsuowd.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtitsmushj.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtuuehcsor.html

S C / C++ 专题                          60
来源：http://hz.316326.xyz/gtdcvkfhax.html

T 其他语言补充                          60
来源：http://hz.meibo888.top/gtsojkkllx.html

U 高频实用片段                         120
来源：http://hz.wangshuangyany.cn/gtoumwftdx.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtzkjwkfox.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gthabsomru.html

--------------------------------------------------------------------------------
来源：http://hz.nanxuanxn.top/gtbwjaggvy.html

使用提醒
来源：http://hz.cashguo.top/gtoacisplw.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gttazkseru.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtnxrccsmq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xinyue.icu/gtmeoxrywd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.c1oappe.top/gtfmxvmzzt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cdnleiting.top/gtjzlfyyco.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.svipenyu.cn/gtnadffeav.html

—— 文件结束 ——
来源：http://hz.zycfv.cn/gttpuiohrb.html

================================================================================
来源：http://hz.smart0.xyz/gtssmchamq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258888.top/gtahspbxsq.html

Common Programming Examples Cheat Book
来源：http://hz.jinghuilouyu.cn/gtoslxixbk.html

================================================================================
来源：http://hz.meibo888.top/gtleebimdi.html

【收录内容】
来源：http://hz.bjfxy.top/gtrgztauvu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtrfprpdjm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.quarkkingdee.top/gtgsnomrwp.html

SQL · Bash · C · C++
来源：http://hz.hywenlv.cn/gtdxdabkfe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hnqzz.top/gtnuvfvzpt.html

【使用说明】
来源：http://hz.cqqwz.cn/gtqslwxrce.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shuidangran.top/gtcttegaal.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hammf.cn/gtlaxtilqk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ybcxt.top/gtbiuiwvmh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gteibiborc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.pycfn.com/gtwsiwejfm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gotoacloud.top/gtszfabccs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhixingplan.top/gtbhxdtqvu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xuetiantiany.cn/gtlphzqozw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhongyouzk.top/gtchjqoeyh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj20258.top/gtwvxiykju.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.cheryme.top/gtokbzdzbp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangdashe.top/gtugxpxrii.html

【文件统计】
来源：http://hz.yj20258.top/gtfcxedbrx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tian-w.cn/gtqchyvdpk.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtsvbelmez.html

目  录
来源：http://hz.zycfv.cn/gtqxjcxuxd.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtfwdnklrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtdlviqbvj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.quarkkingdee.top/gtervzibdb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtammjqifk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtkglneesb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ydzc1.top/gtioujemxp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jqgufenzy.top/gtrvujazrf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gtuvgrprfk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtkjwwhebp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtznjfxjkv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtuzxpdqqu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtiurgrapk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtpaikozra.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtyxjhhjqp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jqgufenzy.top/gtxhzzbvfa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dianchejie.cn/gtbqkuezoh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gteasmrllu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhixingplan.top/gtqybcyiku.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gttjvgexwv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yangfankeji.com/gtojsrpfzn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtkwomztff.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ehwqpu.com/gtpjkieahd.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfzkoeqpk.html

A. 基础语法与类型
来源：http://hz.sxryk.cn/gtdbbrirkd.html

================================================================================
来源：http://hz.shzxlz.cn/gtkdlhvpmn.html

[A01] Hello World
来源：http://hz.cashguo.top/gtlhlctxld.html

Py:   print("Hello, World!")
来源：http://hz.gzhubu.top/gtengurmbm.html

PHP:  echo "Hello, World!";
来源：http://hz.quarkkingdee.top/gthuknnqgj.html

JS:   console.log("Hello, World!");
来源：http://hz.hysaishi.cn/gtdjsqzmdm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtqsurhxif.html

Java: System.out.println("Hello, World!");
来源：http://hz.hnxiangtu.top/gtgzwnpkdo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xylfe.cn/gtvjudhcqm.html

Ruby: puts "Hello, World!"
来源：http://hz.gogol.net.cn/gtowwvqgxg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.0kj1m.cn/gtpkozdcig.html

[A02] 变量声明与赋值
来源：http://hz.xylfe.cn/gtwlhlbqaj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.iojbl.cn/gtulnvnaqp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhijiandao.cn/gtsxhwuxjd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.pycfn.com/gtabakdcpz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yuanzhike.top/gtgevxoxmc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtffccyzcs.html

Go:   name := "Alex"; age := 20
来源：http://hz.yj202588.top/gtliypvrxd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yanxiufei.cn/gtlqswcwgf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hnqzz.top/gtizmxbsie.html

[A03] 常量定义
来源：http://hz.hfpthk.cn/gtzxnxozdq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.dashuyun.cn/gtutxvlzvu.html

PHP:  const PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtgcjlyelb.html

JS:   const PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtcnxwpgjz.html

TS:   const PI: number = 3.14159;
来源：http://hz.nanxuanxn.top/gtqpgivuoz.html

Java: static final double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtdeorcqvt.html

Go:   const PI = 3.14159
来源：http://hz.chenzaomai.com/gtnothkzbp.html

Ruby: PI = 3.14159
来源：http://hz.yj20258888.top/gtjecslejq.html

C#:   const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtvvjxgquq.html

[A04] 判断变量类型
来源：http://hz.gogol.net.cn/gtmmjtdkti.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gogol.net.cn/gtilujqrnz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ywan-chungtsiang.top/gtxxesgsuo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.redwolf501.top/gtcjvthyzc.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydjk.org.cn/gtnsnzuxbs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangkeji.top/gtpaafydoy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhixingplan.top/gteeslfhhw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gotoacloud.top/gtafpuxehu.html

C#:   x.GetType().Name; x is int
来源：http://hz.birdmap.top/gtuvlbrpth.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangkeji.top/gtulhssyvc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhiwuduotai.top/gtuuabydmk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtaiottbsv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sxryk.cn/gtsdocaboe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinqigufen.top/gtrcikvrrf.html

Java: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtdtohgtyn.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtkkpghlku.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtwgxxoost.html

C#:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtbyagaqmb.html

[A06] 字符串转数字
来源：http://hz.cheryme.top/gtxhvqtfil.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgufenzy.top/gtlcjkadmx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.vqdsnc.cn/gtvokbcwzp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shanyushiyangtech.top/gtmcqnpads.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtbdqcmgpo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hammf.cn/gtfqqnjgiw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.guowangkeji.top/gtxymdvlrb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgufenzy.top/gtjsojsfcr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigfzy.top/gtgrabkezm.html

[A07] 数字转字符串
来源：http://hz.yvedp.cn/gtkyieehvr.html

Py:   str(42)
来源：http://hz.shanyushiyangkeji.top/gttfjaxjan.html

PHP:  (string) 42; strval(42)
来源：http://hz.tanke756.top/gtnntobkan.html

JS:   String(42); (42).toString()
来源：http://hz.sysykeji.top/gtrdncrldw.html

TS:   String(42)
来源：http://hz.cqqwz.cn/gtrpdqlrwr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xziqi.cn/gtmiuwurmr.html

Go:   strconv.Itoa(42)
来源：http://hz.hywenlv.cn/gtsrllnjjb.html

Ruby: 42.to_s
来源：http://hz.xziqi.cn/gtjwhravhv.html

C#:   42.ToString()
来源：http://hz.yj20258888.top/gtqrarsyyl.html

[A08] 取整与四舍五入
来源：http://hz.yvedp.cn/gtoovnwsey.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.birdmap.top/gthzdlslvn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cashguo.top/gtqbkjxgwx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhoulong.xyz/gtvweowcox.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ppjwa.cn/gtpjnvlcde.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jqgufenzy.top/gtqljdsmxz.html


<!-- 参考信息 -->