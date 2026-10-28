代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtixgcuwmx.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtfiqwirpr.html

[U58] PHP：数组三件套
来源：http://hz.jqgfzy.top/gtnkaejcqx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.52xcode.cn/gttbewzefg.html

[U59] PHP：自定义排序
来源：http://hz.jqgfzy.top/gtfgytqhbt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtjilbwhnt.html

[U60] PHP：JSON 编解码
来源：http://hz.xuetiantiany.cn/gtgzpuuhdl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gthmvuipye.html

[U61] PHP：正则
来源：http://hz.jqgufenzy.top/gtvcvyemfd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtmqbsetdn.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtdrzzgqze.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj20258.top/gtsfcvufti.html

[U63] PHP：文件读写
来源：http://hz.daxiang520.top/gtpbzchstg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gtnjppkesj.html

[U64] PHP：目录遍历
来源：http://hz.xinyue.icu/gtddyixunl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nwbrower.top/gtbcumlfpr.html

[U65] PHP：会话
来源：http://hz.xuanzx.com/gtrxdxxkfe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gogol.net.cn/gtsixpehfr.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtmdrbpeqm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuetiantiany.cn/gtrhqkspnx.html

[U67] PHP：处理文件上传
来源：http://hz.gzhubu.top/gtkqnkrfsk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxuanxn.top/gtbigmtxsr.html

[U68] PHP：PDO 连接
来源：http://hz.vqdsnc.cn/gtwtcvfger.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hnqzz.top/gtudbaekam.html

[U69] PHP：PDO 预处理
来源：http://hz.hywenlv.cn/gtgivbakoz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj202588.top/gtkejhlvju.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtinnzdcch.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.9152youxi.cn/gtctfwjpik.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gtgtdxjvtf.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtchxfbcqo.html

[U72] PHP：写错误日志
来源：http://hz.iojbl.cn/gtotenrafl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sxryk.cn/gtbqesdujc.html

[U73] PHP：读取 ini 配置
来源：http://hz.hnqzz.top/gtehhtqrgb.html

parse_ini_file("config.ini", true)
来源：http://hz.zycfv.cn/gtqldjxvnr.html

[U74] PHP：读取环境变量
来源：http://hz.vqdsnc.cn/gtautizemt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ydjk.org.cn/gttqmkumjj.html

[U75] PHP：依赖注入
来源：http://hz.nanxinkj.top/gtqpsucwzf.html

composer require psr/container
来源：http://hz.shuidangran.top/gtxsmlfykm.html

[U76] PHP：简单路由
来源：http://hz.haohaochexian.top/gthfbbznca.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yonumen.top/gtrpeweedl.html

[U77] PHP：模板渲染
来源：http://hz.bjfxy.top/gtyholdgmm.html

composer require twig/twig
来源：http://hz.zhijiandao.cn/gtlnezqsnm.html

[U78] PHP：单元测试
来源：http://hz.ehwqpu.com/gtpmldskmg.html

composer require --dev phpunit/phpunit
来源：http://hz.snrcjt.cn/gtvwhbjept.html

[U79] PHP：静态分析
来源：http://hz.gaohongyu789.top/gtuogwrkif.html

composer require --dev phpstan/phpstan
来源：http://hz.guannengcc.top/gthdbrdcgh.html

[U80] PHP：代码规范修复
来源：http://hz.chenlongwang.top/gtumboiuss.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.haohaochexian.top/gtelmzjvpm.html

[U81] JS：初始化项目
来源：http://hz.jinyuanbaomall.cn/gtedbubtwh.html

npm init -y;  npm i express
来源：http://hz.guannengcc.top/gtvfmuybzc.html

[U82] JS：package.json 脚本
来源：http://hz.mhx1999.top/gtqfipxvrm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.svipenyu.cn/gtxwnaiohn.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtbsuagoof.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yonumen.top/gtcdunhxfs.html

[U84] JS：CommonJS 写法
来源：http://hz.smart0.xyz/gtsgggfxer.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hysaishi.cn/gtosvvdgrs.html

[U85] JS：可选链
来源：http://hz.shanyushiyangtech.top/gtdowmidck.html

a?.b?.c
来源：http://hz.pengpengdd.cyou/gtbnuoslcf.html

[U86] JS：空值合并
来源：http://hz.0kj1m.cn/gtmreonudq.html

a ?? b
来源：http://hz.cashguo.top/gtfoyovuic.html

[U87] JS：解构默认值
来源：http://hz.shangyingyoupin.top/gtesqjyghd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.316326.xyz/gtimhalxuc.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gtmveltcho.html

{ ...a, ...b }
来源：http://hz.guannengcc.top/gtahloevxc.html

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtilrsnhdi.html

[...new Set(arr)]
来源：http://hz.yueranfly.top/gtgqehnwuw.html

[U90] JS：数字数组排序
来源：http://hz.cdnleiting.top/gtuxbmxnzh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtdilqgmze.html

[U91] JS：对象键值遍历
来源：http://hz.ydjk.org.cn/gtuppyyjcd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nanxinkj.top/gtzpvcyjxj.html

[U92] JS：深拷贝
来源：http://hz.jinqigufen.top/gtscijviwf.html

structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtfbqewhmn.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtqzitsilm.html

`共 ${n} 条`
来源：http://hz.yj20258.top/gtkgvwilix.html

[U94] JS：箭头函数
来源：http://hz.daria6918.cn/gtgzymspjw.html

const double = x => x * 2;
来源：http://hz.hnxiangtu.top/gtehzwfyxj.html

[U95] JS：Promise 包装
来源：http://hz.gaohongyu789.top/gtoynigywb.html

new Promise((resolve, reject) => {})
来源：http://hz.52xcode.cn/gtaitbepma.html

[U96] JS：async/await 与异常
来源：http://hz.yj20258.top/gtxotqgcfu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtvhntdlhl.html

[U97] JS：并发请求
来源：http://hz.c1oappe.top/gtdycidcns.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtuxqoldjg.html

[U98] JS：fetch 带 JSON
来源：http://hz.vqdsnc.cn/gtbvtuhyry.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gotoacloud.top/gtxoetueyr.html

[U99] JS：事件监听
来源：http://hz.hfpthk.cn/gtdkrlhzqu.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gteinhbwbz.html

[U100] JS：DOM 查询
来源：http://hz.vqdsnc.cn/gtklrgmoaz.html

document.querySelector(".item")
来源：http://hz.316326.xyz/gtgpnxaoik.html

[U101] JS：classList 操作
来源：http://hz.jiagoushi.top/gtoibnxuwm.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtqledwqjo.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gtprbxrsof.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jqgufenzy.top/gtbzlnghgp.html

[U103] JS：定时器
来源：http://hz.daxiang520.top/gtjtbskzgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hnxiangtu.top/gtqbspqhca.html

[U104] JS：防抖
来源：http://hz.hongshengwenyu.top/gtmqdpgqcd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtlibcmyss.html

[U105] JS：节流
来源：http://hz.chenjidiqi.icu/gttqrooqws.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ybcxt.top/gthzxmltuj.html

[U106] JS：日期格式化
来源：http://hz.jlsjyb.cn/gtorntuqjb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gtiaoikbzh.html

[U107] JS：数字千分位
来源：http://hz.fzhhl.top/gtyaexhgiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yongpay.top/gtgzjpmhxv.html

[U108] JS：随机整数
来源：http://hz.wangshuangyany.cn/gtblpadzuz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtvrtvgpad.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtnkdsbqxa.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtqlwnrxii.html

[U110] JS：数组分块
来源：http://hz.guowangkeji.top/gtezysqycf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jqgfzy.top/gtgodiztoc.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtmqocimjc.html

new Map(Object.entries(obj))
来源：http://hz.vqdsnc.cn/gtlpbkzpvg.html

[U112] JS：字符串补位
来源：http://hz.zycfv.cn/gtjgisvjub.html

"7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtkocdrteh.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gtbvbdyzvr.html

s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtklcvquab.html

[U114] JS：JSON 深比较
来源：http://hz.9152youxi.cn/gtheixddqy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gthuckedxh.html

[U115] JS：生成 UUID
来源：http://hz.jianghu66.top/gtqehugatc.html

crypto.randomUUID()
来源：http://hz.hfpthk.cn/gthwclkbjc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jyoumei.cn/gtmatqczeg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tanke756.top/gthlegccpu.html

[U117] JS：单元测试
来源：http://hz.tian-w.cn/gthpjqmktb.html

npm i -D vitest;  npx vitest
来源：http://hz.feifeiyinyue.top/gtwwvtlkul.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gtbasuaakw.html

npm i -D vite;  npx vite
来源：http://hz.ydzc1.top/gtirrurrbs.html

[U119] JS：生产构建
来源：http://hz.yuanzhike.top/gtjyuhynzd.html

npx vite build
来源：http://hz.redwolf501.top/gtyxxzevfc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cqqwz.cn/gtpbklsnpi.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtzujjfqjc.html

================================================================================
来源：http://hz.guannengcc.top/gtohajpygt.html

统计汇总
来源：http://hz.xinyue.icu/gtovatqgdx.html

================================================================================
来源：http://hz.mhx1999.top/gttoslkfix.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtegskondt.html

Python ......... 252
来源：http://hz.ehwqpu.com/gthziuqlhr.html

PHP ............ 252
来源：http://hz.xylfe.cn/gttxaldlmm.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtdeolmdcl.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtsfkwjdrl.html

Java ........... 212
来源：http://hz.xingfuxueyuan.xyz/gtaxvkgiev.html

Go ............. 212
来源：http://hz.tianlin.xyz/gtjevgjzvl.html

Ruby ........... 212
来源：http://hz.xziqi.cn/gtbivmnpel.html

C# ............. 212
来源：http://hz.jianghu66.top/gtvjiycwsm.html

C .............. 30
来源：http://hz.jinqigfzy.top/gtubwrxsas.html

C++ ............ 30
来源：http://hz.jqgfzy.top/gthofvccnp.html

SQL ............ 90
来源：http://hz.tanke756.top/gtcfpfudcc.html

Bash ........... 80
来源：http://hz.zhengqikj.top/gthogicilq.html

Kotlin ......... 15
来源：http://hz.sweek.top/gtgvrmevtt.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtwakzdyht.html

Lua ............ 10
来源：http://hz.vqdsnc.cn/gtwjfkuthz.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtzjcaqjmd.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtxpcrwcvw.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtobieuveb.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtunyedzjx.html

按章节统计：
来源：http://hz.hnqzz.top/gtzvgxsovj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gttnorcjti.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtarnrffuf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gttpplkwfn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sweek.top/gtoxhobyer.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinqigufen.top/gtqowpjinv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtvwofmfht.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtlfkaxjma.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtuigfgxmn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtjytdnmks.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtqnoudxug.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gteewaguxr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtshoqustv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtcoeofxns.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gthgcavmav.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jyoumei.cn/gtuqusrmjo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gttkoyfwtq.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtoatgwwfe.html

R Bash 专题                             80
来源：http://hz.jiagoushi.top/gttooeuiyu.html

S C / C++ 专题                          60
来源：http://hz.fzhhl.top/gtjxmpfoig.html

T 其他语言补充                          60
来源：http://hz.jinyuanbaomall.cn/gtilwxqinh.html

U 高频实用片段                         120
来源：http://hz.yj202588.top/gtypmqpxqk.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtfktogvzz.html

合计                                  2106 条
来源：http://hz.xziqi.cn/gtkrpfjjsb.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtwebmbrwc.html

使用提醒
来源：http://hz.sysykeji.top/gtrnecjhbq.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtndgfdkee.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.daria6918.cn/gtumzceabp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xingfuxueyuan.xyz/gtapheobln.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.redwolf501.top/gttjliyobz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tianlin.xyz/gtdfsrytmm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj202588.top/gtynjcalrp.html

—— 文件结束 ——
来源：http://hz.yueranfly.top/gtnnbohqrn.html

================================================================================
来源：http://hz.havefunace.top/gtyapjubiv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aibaodan.cn/gtvgkvtves.html

Common Programming Examples Cheat Book
来源：http://hz.dashuyun.cn/gtgsdxwzfa.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthwxqgext.html

【收录内容】
来源：http://hz.quarkkingdee.top/gtblxvbcwm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cashguo.top/gtxvniygec.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xuetiantiany.cn/gtvfloeanw.html

SQL · Bash · C · C++
来源：http://hz.svipenyu.cn/gtdkdozdsr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hnxiangtu.top/gtmkgksrlk.html

【使用说明】
来源：http://hz.zhaomingkeji.xyz/gtanwcrkxk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnxiangtu.top/gtrilzkxtp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtjxisxwmy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtccwifjdj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aizwys.cn/gtmgxgeefq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.daria6918.cn/gtgvbcgyvf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cdnleiting.top/gtsfougcmd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yanxiufei.cn/gthfbmwshn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.guowangkeji.top/gthrdhvoft.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ywan-chungtsiang.top/gtuaoyheav.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.316326.xyz/gtuyeowizo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tianlin.xyz/gtgrvhmijr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gaohongyu789.top/gtcuuxlywk.html

【文件统计】
来源：http://hz.zhixingplan.top/gtrnskwkuj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxinkj.top/gttwjooozu.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtqlvaankx.html

目  录
来源：http://hz.shangyingyoupin.top/gthmoabobq.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtklykqjoa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtqglfczkq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtragpawym.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtqwwofbgb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gthskvpprw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hammf.cn/gtbdbzogcm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtjndecndz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtmaxuyilr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.snrcjt.cn/gtnsuwszpj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtkmahihqv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.daxiang520.top/gtyleoybwu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtmjwwjbor.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtkmylqtku.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtnlvkiugi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtzpinifmb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxinkj.top/gtfiemnybl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtdljozqym.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.redwolf501.top/gtubqgbsyg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tianlin.xyz/gtypsrfcjg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shanyushiyangtech.top/gtatbdybcx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtffkfhgob.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtxgmdicoq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqnbdespc.html

A. 基础语法与类型
来源：http://hz.chenjidiqi.icu/gtzbxwwrit.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpfskgycu.html

[A01] Hello World
来源：http://hz.jianghu66.top/gtigqpyjny.html

Py:   print("Hello, World!")
来源：http://hz.dianchejie.cn/gtgkvuphnq.html

PHP:  echo "Hello, World!";
来源：http://hz.gotoacloud.top/gtvhdnwvis.html

JS:   console.log("Hello, World!");
来源：http://hz.sxryk.cn/gtgwusslzp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shanyushiyangtech.top/gtpryncoqu.html

Java: System.out.println("Hello, World!");
来源：http://hz.zycfv.cn/gttddtmbic.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hfpthk.cn/gtsdmaucti.html

Ruby: puts "Hello, World!"
来源：http://hz.gogol.net.cn/gtevjjcctl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtcnkppfth.html

[A02] 变量声明与赋值
来源：http://hz.jqgfzy.top/gtqywgzuuk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhixingplan.top/gtinxcoqai.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.daria6918.cn/gtsldgzviz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangtech.top/gtdyslcfge.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xylfe.cn/gtmqqyceqb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtavnrvzdc.html

Go:   name := "Alex"; age := 20
来源：http://hz.xylfe.cn/gtmkxibdww.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zdqjudy.top/gtmchrywve.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtdehxlriq.html

[A03] 常量定义
来源：http://hz.yj202588.top/gttgfarbez.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shangyingyoupin.top/gtlecazoic.html

PHP:  const PI = 3.14159;
来源：http://hz.316326.xyz/gtisgeasov.html

JS:   const PI = 3.14159;
来源：http://hz.ydzc1.top/gtchfbpjam.html

TS:   const PI: number = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtdxibcmfm.html

Java: static final double PI = 3.14159;
来源：http://hz.cheryme.top/gtoglkcyoo.html

Go:   const PI = 3.14159
来源：http://hz.quarkkingdee.top/gtcxcjtbgf.html

Ruby: PI = 3.14159
来源：http://hz.cucudq.cn/gtirgmyolr.html

C#:   const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtfbjbxjgz.html

[A04] 判断变量类型
来源：http://hz.gaohongyu789.top/gtczhyvrvi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangdashe.top/gtwjjjpyxt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.chenjidiqi.icu/gtxyrnksgj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jyoumei.cn/gtruotnukq.html

TS:   typeof x; x instanceof Date
来源：http://hz.hongshengwenyu.top/gtrwktwrxo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gthynnnxzo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xinyue.icu/gtsuzvexzm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tianlin.xyz/gtqborfhqf.html

C#:   x.GetType().Name; x is int
来源：http://hz.hongshengwenyu.top/gtgtmdujcf.html

[A05] 整数除法与取模
来源：http://hz.yanxiufei.cn/gtjqluvfjl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hysaishi.cn/gtiozlpshz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.haohaochexian.top/gtuevmfwcc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhongyouzk.top/gtuifzynpl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenlongwang.top/gtjfvbnkxs.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangdashe.top/gtiavirlum.html

Go:   7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gtjaxzpboq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gthvbevfti.html

C#:   7 / 2; 7 % 2
来源：http://hz.xinyue.icu/gtnmutediy.html

[A06] 字符串转数字
来源：http://hz.quarkkingdee.top/gtextfghbt.html

Py:   int("42"); float("3.14")
来源：http://hz.guowangkeji.top/gtytqwwspa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinqigufen.top/gteqzaohmu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.mhx1999.top/gtdiofkwjn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.gotoacloud.top/gtyikniveu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ehwqpu.com/gtoikhzgzm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cucudq.cn/gtaxzglple.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shanyushiyangkeji.top/gtrclcbkdf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shuidangran.top/gtoegusrbt.html

[A07] 数字转字符串
来源：http://hz.shanyushiyangkeji.top/gtxgdhknxf.html

Py:   str(42)
来源：http://hz.sufxvd.cn/gtuvvxeguu.html

PHP:  (string) 42; strval(42)
来源：http://hz.ppjwa.cn/gtginlkicu.html

JS:   String(42); (42).toString()
来源：http://hz.tanke756.top/gtwcyjlcut.html

TS:   String(42)
来源：http://hz.feifeiyinyue.top/gtsizrxzhj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jqgufenzy.top/gtkopniuoo.html

Go:   strconv.Itoa(42)
来源：http://hz.dashuyun.cn/gtelmkacfq.html

Ruby: 42.to_s
来源：http://hz.jiagoushi.top/gtrdvkllrt.html

C#:   42.ToString()
来源：http://hz.jiagoushi.top/gtactpllnk.html

[A08] 取整与四舍五入
来源：http://hz.0kj1m.cn/gtfncfncpi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.vqdsnc.cn/gthvclacvq.html


<!-- 参考信息 -->