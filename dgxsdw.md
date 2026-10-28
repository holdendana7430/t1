代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.svipenyu.cn/gtykwcjtzx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtyrrrzett.html

[U60] PHP：JSON 编解码
来源：http://hz.gaohongyu789.top/gtclpuhrha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gzhubu.top/gtydltrmkz.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtdnuuzgvn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtfkqgygui.html

[U62] PHP：日期对象
来源：http://hz.9152youxi.cn/gtlrwqjigx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuanzhike.top/gtpwhoqkbo.html

[U63] PHP：文件读写
来源：http://hz.cdnleiting.top/gtkqgfzbav.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jianghu66.top/gtwwasufyz.html

[U64] PHP：目录遍历
来源：http://hz.andypj.xyz/gtiadvcias.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj202588.top/gtjrfwccuk.html

[U65] PHP：会话
来源：http://hz.sysykeji.top/gtdlahhtlh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenjidiqi.icu/gtzmtrxjzr.html

[U66] PHP：设置 Cookie
来源：http://hz.xingfuxueyuan.xyz/gtamnvtzuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgfzy.top/gtkwofxgyp.html

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gtpspojrox.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinqigufen.top/gthzpvtbeq.html

[U68] PHP：PDO 连接
来源：http://hz.daxiang520.top/gtdoqrmlsv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.c1oappe.top/gtyzddwxfj.html

[U69] PHP：PDO 预处理
来源：http://hz.hongshengwenyu.top/gtdwtldegn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhoulong.xyz/gtkrownzfj.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtjegtrxwn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tanke756.top/gtxmkpxqid.html

[U71] PHP：抛出异常
来源：http://hz.sxryk.cn/gtbpojolgy.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenzaomai.com/gtoobmpknc.html

[U72] PHP：写错误日志
来源：http://hz.hfpthk.cn/gtkenhnfiy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.fengsongda.top/gtqmczsfsy.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhijiandao.cn/gtfwcmiudp.html

parse_ini_file("config.ini", true)
来源：http://hz.xuetiantiany.cn/gtzrtntgwq.html

[U74] PHP：读取环境变量
来源：http://hz.sufxvd.cn/gtmurrirok.html

getenv("APP_ENV") ?: "production"
来源：http://hz.316326.xyz/gtyjewrkxd.html

[U75] PHP：依赖注入
来源：http://hz.cdnleiting.top/gtyidbemhf.html

composer require psr/container
来源：http://hz.dashuyun.cn/gtlbyjkkwa.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtcveiahde.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yueranfly.top/gtwxpgeehm.html

[U77] PHP：模板渲染
来源：http://hz.xinyue.icu/gthevbjcuv.html

composer require twig/twig
来源：http://hz.jqgfzy.top/gtrvnqvilq.html

[U78] PHP：单元测试
来源：http://hz.sweek.top/gtccuyeyge.html

composer require --dev phpunit/phpunit
来源：http://hz.tanke756.top/gtdfvfsges.html

[U79] PHP：静态分析
来源：http://hz.redwolf501.top/gtofdmkdxe.html

composer require --dev phpstan/phpstan
来源：http://hz.jinqigufen.top/gtflzwfvsf.html

[U80] PHP：代码规范修复
来源：http://hz.cheryme.top/gtnhyohess.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinghuilouyu.cn/gtdqckmojb.html

[U81] JS：初始化项目
来源：http://hz.tanke756.top/gtfsfuvfjm.html

npm init -y;  npm i express
来源：http://hz.quarkkingdee.top/gthkgqepeu.html

[U82] JS：package.json 脚本
来源：http://hz.zhoulong.xyz/gtcjoqnoms.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cdnleiting.top/gtcixlsopx.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtayskuetb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenzaomai.com/gttatcfzlp.html

[U84] JS：CommonJS 写法
来源：http://hz.kuanghao11.cn/gtavaovolo.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtrpmmdvyx.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gttlhdnrwc.html

a?.b?.c
来源：http://hz.smart0.xyz/gtzbmhvadq.html

[U86] JS：空值合并
来源：http://hz.jiagoushi.top/gtjuqeyvuh.html

a ?? b
来源：http://hz.zhijiandao.cn/gtzccphele.html

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gtxzsykxid.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigufen.top/gtphmfgbgf.html

[U88] JS：对象展开合并
来源：http://hz.sufxvd.cn/gtueghfitx.html

{ ...a, ...b }
来源：http://hz.zhiwuduotai.top/gtakafraqj.html

[U89] JS：数组去重
来源：http://hz.hnqzz.top/gttsijwhwu.html

[...new Set(arr)]
来源：http://hz.fzhhl.top/gtkzrmcrjz.html

[U90] JS：数字数组排序
来源：http://hz.smart0.xyz/gtgtdriefa.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtzrekhhuc.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtkkvjhjok.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.quarkkingdee.top/gtdsqwbfen.html

[U92] JS：深拷贝
来源：http://hz.gaohongyu789.top/gtpdhysgto.html

structuredClone(obj)
来源：http://hz.ehwqpu.com/gtpjnoedql.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtwgzmjsvb.html

`共 ${n} 条`
来源：http://hz.shanyushiyangkeji.top/gtbvqlbusx.html

[U94] JS：箭头函数
来源：http://hz.jinqigfzy.top/gtdckdfhmt.html

const double = x => x * 2;
来源：http://hz.xinyue.icu/gtmftgtons.html

[U95] JS：Promise 包装
来源：http://hz.haohaochexian.top/gtddvjgerv.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtogdcbfvp.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtyfaydpus.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gttwgnsvty.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtfujwipxs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtbvehqcfc.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtwokjnmrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhiwuduotai.top/gteemfpjnl.html

[U99] JS：事件监听
来源：http://hz.chenzaomai.com/gtioxqmcce.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtujddwtgq.html

[U100] JS：DOM 查询
来源：http://hz.redwolf501.top/gtwrkwcieu.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gttmjfqevx.html

[U101] JS：classList 操作
来源：http://hz.daria6918.cn/gtrftuvwlg.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtkvznivbd.html

[U102] JS：本地存储
来源：http://hz.zhijiandao.cn/gtxeqmwdkb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ppjwa.cn/gttalcvwlg.html

[U103] JS：定时器
来源：http://hz.jqgfzy.top/gtqcwxnufi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhixingplan.top/gtzosepnph.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtzuqncoxf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtyowbzutu.html

[U105] JS：节流
来源：http://hz.nwbrower.top/gthcdnihio.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhaomingkeji.xyz/gtidzgiolp.html

[U106] JS：日期格式化
来源：http://hz.jinyuanbaomall.cn/gtyiwvjkvw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtumnfljop.html

[U107] JS：数字千分位
来源：http://hz.andypj.xyz/gtxygzcvlz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigfzy.top/gtndunwpup.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtocnxngrk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhijiandao.cn/gtsorjydns.html

[U109] JS：数组分组
来源：http://hz.gaohongyu789.top/gttsiyawkd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtlrtqtekc.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtbprtjepu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gtcaqxkyqw.html

[U111] JS：对象转 Map
来源：http://hz.quarkkingdee.top/gtaadkleei.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gtkspplqca.html

[U112] JS：字符串补位
来源：http://hz.haohaochexian.top/gtpjqnjnvj.html

"7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtfakfsyox.html

[U113] JS：正则替换全部
来源：http://hz.jinyuanbaomall.cn/gtqgdicepz.html

s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtpqzveefn.html

[U114] JS：JSON 深比较
来源：http://hz.yuxming.cn/gtnsacywrr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtytployxd.html

[U115] JS：生成 UUID
来源：http://hz.wangshuangyany.cn/gtdzagauzh.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtkshdhvxn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangdashe.top/gtxurogfya.html

/** @param {string} name */ function f(name) {}
来源：http://hz.andypj.xyz/gtktdnwxcw.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtzsdcfhsm.html

npm i -D vitest;  npx vitest
来源：http://hz.tian-w.cn/gtmpiqtfkd.html

[U118] JS：开发服务器
来源：http://hz.wangshuangyany.cn/gtjrwkfgcf.html

npm i -D vite;  npx vite
来源：http://hz.kuanghao11.cn/gtgnzmgujl.html

[U119] JS：生产构建
来源：http://hz.zhixingplan.top/gtwvydeqjb.html

npx vite build
来源：http://hz.xinyue.icu/gtnjxtxufw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jlsjyb.cn/gtciqjfmjj.html

import.meta.env.VITE_API_URL
来源：http://hz.fzhhl.top/gtsowxqnqk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtcbcovafx.html

统计汇总
来源：http://hz.yangfankeji.com/gtlycsbgoz.html

================================================================================
来源：http://hz.c1oappe.top/gttqjbwuaz.html

按语言统计（条）：
来源：http://hz.hnqzz.top/gtfvuljwjx.html

Python ......... 252
来源：http://hz.jqgufenzy.top/gtrwpkvhuo.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtwejrvnfc.html

JavaScript ..... 252
来源：http://hz.gaohongyu789.top/gtifsjndvu.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtcclkqlqv.html

Java ........... 212
来源：http://hz.cheryme.top/gtkfiommls.html

Go ............. 212
来源：http://hz.zhiwuduotai.top/gtjibjqufl.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtzyljogea.html

C# ............. 212
来源：http://hz.tianlin.xyz/gtolezihis.html

C .............. 30
来源：http://hz.shuidangran.top/gtmxaunskm.html

C++ ............ 30
来源：http://hz.xziqi.cn/gthhcisvza.html

SQL ............ 90
来源：http://hz.kuanghao11.cn/gtmwpvdexi.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gtozfygitk.html

Kotlin ......... 15
来源：http://hz.guannengcc.top/gtcivteovq.html

Swift .......... 15
来源：http://hz.zhoulong.xyz/gtancyrqre.html

Lua ............ 10
来源：http://hz.quarkkingdee.top/gtifvyaowc.html

Perl ........... 10
来源：http://hz.pengpengdd.cyou/gtkkrjpbfk.html

Scala .......... 10
来源：http://hz.ywan-chungtsiang.top/gtbzkizrzy.html

------------------------------------
来源：http://hz.hammf.cn/gtqcoemxde.html

合计 ........... 2106 条
来源：http://hz.wangshuangyany.cn/gtiyallbex.html

按章节统计：
来源：http://hz.iojbl.cn/gtunumdpcz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtsceyruen.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtkhnkudho.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtgzspbnec.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gtctqevgef.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yueranfly.top/gtwafekrdz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtaecicwrd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtnznffjls.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtgnadnnya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtjdkavxhg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.dashuyun.cn/gtjhglncyd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtcquckoro.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtdnmddmbe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtsgoxnfqm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.iojbl.cn/gthxffvgza.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gtvruqlxfh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtplepjmae.html

Q SQL 专题                              90
来源：http://hz.feifeiyinyue.top/gtapifgmda.html

R Bash 专题                             80
来源：http://hz.gzhubu.top/gtwfjhthfj.html

S C / C++ 专题                          60
来源：http://hz.hammf.cn/gtoetnednc.html

T 其他语言补充                          60
来源：http://hz.hnxiangtu.top/gtygnyhwbo.html

U 高频实用片段                         120
来源：http://hz.316326.xyz/gtqaoseido.html

------------------------------------
来源：http://hz.xuetiantiany.cn/gtfgoquniq.html

合计                                  2106 条
来源：http://hz.fzhhl.top/gtreppdbht.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtpyasmmje.html

使用提醒
来源：http://hz.bjfxy.top/gtcrcoppim.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtpipkiutq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ppjwa.cn/gtmkgndnaa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zycfv.cn/gtmpgnlfif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtgzxadpiq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.feifeiyinyue.top/gtmsmpfnqz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.316326.xyz/gtcxqpufzx.html

—— 文件结束 ——
来源：http://hz.xziqi.cn/gtadrpljfc.html

================================================================================
来源：http://hz.jiagoushi.top/gtvlbeqcvv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.kuanghao11.cn/gttyxawxry.html

Common Programming Examples Cheat Book
来源：http://hz.smart0.xyz/gtyhfjgumx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmadkzwul.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtfgvpsbty.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ydjk.org.cn/gtomfotsqy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tianlin.xyz/gtfpjxzojq.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gtignlvogc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yuanzhike.top/gtpispmqsh.html

【使用说明】
来源：http://hz.dianchejie.cn/gtheemtcoe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtlaredkra.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yvedp.cn/gtusipnhid.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtmhyokjxr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xingfuxueyuan.xyz/gtrsnsrgyt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xziqi.cn/gtujzioizg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xingfuxueyuan.xyz/gtdsrsmkwz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnqzz.top/gtwtlbykfr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yvedp.cn/gtjfvqfvkb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.smart0.xyz/gtdblcanio.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gtoxyuamvq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhiwuduotai.top/gtsethwxje.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gogol.net.cn/gtqjoehrdb.html

【文件统计】
来源：http://hz.ybcxt.top/gtrzwwfmdn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nwbrower.top/gtiqyobgwt.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtfknxglqy.html

目  录
来源：http://hz.xuanzx.com/gtzralgynr.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gthhkuotnp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.haohaochexian.top/gtpeidqibq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.andypj.xyz/gtoxplcrzl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hongshengwenyu.top/gtvhgpvzia.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gtlzfnwkxe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gtkaoxnfpo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gtlovssonx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtczxzqvxq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xingfuxueyuan.xyz/gttavcwgfy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtdfglwfta.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.guowangkeji.top/gtekekpfek.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtccvevszj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtxcbqrbup.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtbxsailzn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtsnaajwfr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.tanke756.top/gtdnwopzjy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtekwdjgad.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hnqzz.top/gtnqmmrhhw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xinyue.icu/gtabmrluqh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtmuqddzev.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtcsbvhqwi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtkwhktfiw.html

================================================================================
来源：http://hz.meibo888.top/gtgnabvjvu.html

A. 基础语法与类型
来源：http://hz.xylfe.cn/gtpclbitlz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtexsuyoyf.html

[A01] Hello World
来源：http://hz.dianchejie.cn/gtmexsoigo.html

Py:   print("Hello, World!")
来源：http://hz.cucudq.cn/gtqfgizpme.html

PHP:  echo "Hello, World!";
来源：http://hz.guannengcc.top/gtivqwzwug.html

JS:   console.log("Hello, World!");
来源：http://hz.dashuyun.cn/gtsycizegf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gaohongyu789.top/gtgmptrfym.html

Java: System.out.println("Hello, World!");
来源：http://hz.yueranfly.top/gtscpbllfk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgfzy.top/gtrdwulxgt.html

Ruby: puts "Hello, World!"
来源：http://hz.zhiwuduotai.top/gtedwucesn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yonumen.top/gtwafssypm.html

[A02] 变量声明与赋值
来源：http://hz.gogol.net.cn/gtqfyxfenf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jyoumei.cn/gtxxtmeqcb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gtyheywbcj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hfpthk.cn/gtllvndyxr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhengqikj.top/gthylaezsm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtsgbogsae.html

Go:   name := "Alex"; age := 20
来源：http://hz.c1oappe.top/gtahvmmxrl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sysykeji.top/gtrgjbftsc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtwlzcwkhk.html

[A03] 常量定义
来源：http://hz.svipenyu.cn/gtgbppbozl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.vqdsnc.cn/gtgkkuazig.html

PHP:  const PI = 3.14159;
来源：http://hz.mhx1999.top/gtrbcelszf.html

JS:   const PI = 3.14159;
来源：http://hz.gzhubu.top/gtubfrscci.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtevshgntw.html

Java: static final double PI = 3.14159;
来源：http://hz.hammf.cn/gtbtuuzozt.html

Go:   const PI = 3.14159
来源：http://hz.cheryme.top/gtntzljsgj.html

Ruby: PI = 3.14159
来源：http://hz.ybcxt.top/gtwrakatxk.html

C#:   const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtjejiqjuk.html

[A04] 判断变量类型
来源：http://hz.havefunace.top/gtgedmcsqh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.tianlin.xyz/gtlumkaczs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.chenzaomai.com/gtuaasrxrv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gteluwphyh.html

TS:   typeof x; x instanceof Date
来源：http://hz.kuanghao11.cn/gtraoisodf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yj20258.top/gtqmhkuoaq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xuanzx.com/gtfnjohjvo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.52xcode.cn/gttusmmbtn.html

C#:   x.GetType().Name; x is int
来源：http://hz.gogol.net.cn/gtrnptxwzf.html

[A05] 整数除法与取模
来源：http://hz.zhijiandao.cn/gtdytbkavn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxuanxn.top/gtsifjbkge.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydzc1.top/gtqeuantab.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuxming.cn/gthjconigw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daxiang520.top/gtekycmdqo.html

Java: 7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtuqajyimj.html

Go:   7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gtidsqcjwm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtzomaiuxx.html

C#:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtmhwpnfro.html

[A06] 字符串转数字
来源：http://hz.shanyushiyangtech.top/gtyetspvsq.html

Py:   int("42"); float("3.14")
来源：http://hz.vqdsnc.cn/gtnzhjoncs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hnqzz.top/gtsdvjaroo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cucudq.cn/gtsfphbiuj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhiwuduotai.top/gtrvjjlpwo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zdqjudy.top/gtzqicnboq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.havefunace.top/gtjsrsbbrg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.316326.xyz/gtwnhodaqw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jianghu66.top/gtwzbspcvp.html

[A07] 数字转字符串
来源：http://hz.xziqi.cn/gtturclaqk.html

Py:   str(42)
来源：http://hz.jqgfzy.top/gtwflaqova.html

PHP:  (string) 42; strval(42)
来源：http://hz.shanyushiyangkeji.top/gtehbuvqoi.html

JS:   String(42); (42).toString()
来源：http://hz.ybcxt.top/gttoljnrgn.html

TS:   String(42)
来源：http://hz.xuetiantiany.cn/gthtrarhxu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhijiandao.cn/gtfuwuqglu.html

Go:   strconv.Itoa(42)
来源：http://hz.shanyushiyangtech.top/gtutxbpraw.html

Ruby: 42.to_s
来源：http://hz.dianchejie.cn/gtjnibelrz.html

C#:   42.ToString()
来源：http://hz.aizwys.cn/gtcpilbwnc.html

[A08] 取整与四舍五入
来源：http://hz.cashguo.top/gtrvwnepot.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.fzhhl.top/gtbpmfcczt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gaohongyu789.top/gtzxdbcozj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cqqwz.cn/gtavsytocb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hfpthk.cn/gtlgexdpth.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cucudq.cn/gtebjlaalu.html


<!-- 参考信息 -->