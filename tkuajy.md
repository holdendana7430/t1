代发 wailian999

[U65] PHP：会话
来源：http://hz.feifeiyinyue.top/gtzowppina.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxinkj.top/gthauejijt.html

[U66] PHP：设置 Cookie
来源：http://hz.cheryme.top/gthlekktld.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aizwys.cn/gthmuyibzb.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gtwghansvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.haohaochexian.top/gtupkpeaan.html

[U68] PHP：PDO 连接
来源：http://hz.ybcxt.top/gtaakblmgo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtolpferds.html

[U69] PHP：PDO 预处理
来源：http://hz.gotoacloud.top/gttzqgpxgy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yanxiufei.cn/gtpvwakelt.html

[U70] PHP：PDO 事务
来源：http://hz.52xcode.cn/gtuqdoxotl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daria6918.cn/gtclsbmlzj.html

[U71] PHP：抛出异常
来源：http://hz.wangshuangyany.cn/gtlswcnetv.html

throw new RuntimeException("失败", 500);
来源：http://hz.jiagoushi.top/gtpdbjfxwn.html

[U72] PHP：写错误日志
来源：http://hz.andypj.xyz/gtulrcgfpf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.haohaochexian.top/gtxtctqwhi.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gtcgjzzlkv.html

parse_ini_file("config.ini", true)
来源：http://hz.yvedp.cn/gtmqixfcgc.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtykmjcsci.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yangfankeji.com/gtzjvdcjif.html

[U75] PHP：依赖注入
来源：http://hz.mhx1999.top/gtyomfdwds.html

composer require psr/container
来源：http://hz.gogol.net.cn/gtmxtywywv.html

[U76] PHP：简单路由
来源：http://hz.svipenyu.cn/gtbzouunzi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhijiandao.cn/gtlbipyayp.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtgmlzhkik.html

composer require twig/twig
来源：http://hz.nwbrower.top/gtxlkpccoh.html

[U78] PHP：单元测试
来源：http://hz.daxiang520.top/gtdihndwdh.html

composer require --dev phpunit/phpunit
来源：http://hz.cashguo.top/gtauqywmib.html

[U79] PHP：静态分析
来源：http://hz.andypj.xyz/gtbnvvmhnd.html

composer require --dev phpstan/phpstan
来源：http://hz.hfpthk.cn/gthzrxehbp.html

[U80] PHP：代码规范修复
来源：http://hz.sysykeji.top/gtftaikcop.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hnqzz.top/gtuvtoncyi.html

[U81] JS：初始化项目
来源：http://hz.iojbl.cn/gtlypckgnu.html

npm init -y;  npm i express
来源：http://hz.xuetiantiany.cn/gtgjhkpxbh.html

[U82] JS：package.json 脚本
来源：http://hz.0kj1m.cn/gtvmhubnjr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.havefunace.top/gtswhivhvn.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gtupvtholg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cashguo.top/gtkkyjzxnp.html

[U84] JS：CommonJS 写法
来源：http://hz.ybcxt.top/gtgnvicxsq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhoulong.xyz/gtcdlfbkrp.html

[U85] JS：可选链
来源：http://hz.xuanzx.com/gtxsmdshni.html

a?.b?.c
来源：http://hz.aizwys.cn/gtbkixoson.html

[U86] JS：空值合并
来源：http://hz.havefunace.top/gtrlcitkcj.html

a ?? b
来源：http://hz.sysykeji.top/gtplpawlil.html

[U87] JS：解构默认值
来源：http://hz.yueranfly.top/gtdnhezjdr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zdqjudy.top/gtotqkayus.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangtech.top/gtaugfvwzv.html

{ ...a, ...b }
来源：http://hz.tianlin.xyz/gtblzbtuox.html

[U89] JS：数组去重
来源：http://hz.tianlin.xyz/gtognafvfe.html

[...new Set(arr)]
来源：http://hz.nwbrower.top/gtziimwbqg.html

[U90] JS：数字数组排序
来源：http://hz.hnqzz.top/gtjysghfgq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtbxdcllju.html

[U91] JS：对象键值遍历
来源：http://hz.quarkkingdee.top/gtnoawufdd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhijiandao.cn/gtmpqpudzv.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtfnjxqhjt.html

structuredClone(obj)
来源：http://hz.jyoumei.cn/gtoscfsieu.html

[U93] JS：模板字符串
来源：http://hz.wangdashe.top/gtwsjwwbgh.html

`共 ${n} 条`
来源：http://hz.ivvv.top/gtdlzcpwwa.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gtlgjkysdw.html

const double = x => x * 2;
来源：http://hz.shanyushiyangtech.top/gtxursxxth.html

[U95] JS：Promise 包装
来源：http://hz.svipenyu.cn/gtiunfyevb.html

new Promise((resolve, reject) => {})
来源：http://hz.kuanghao11.cn/gtrdtporzg.html

[U96] JS：async/await 与异常
来源：http://hz.ybcxt.top/gtxrkarxsa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtzzllihia.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtwsvsquwi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtewwagxnm.html

[U98] JS：fetch 带 JSON
来源：http://hz.ppjwa.cn/gtstjlysnr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhaomingkeji.xyz/gtvseaklvl.html

[U99] JS：事件监听
来源：http://hz.9152youxi.cn/gtbhyhglhl.html

el.addEventListener("click", e => {})
来源：http://hz.vqdsnc.cn/gteoetbqwq.html

[U100] JS：DOM 查询
来源：http://hz.gogol.net.cn/gtmevdesbj.html

document.querySelector(".item")
来源：http://hz.jinyuanbaomall.cn/gtbieurkps.html

[U101] JS：classList 操作
来源：http://hz.yj20258888.top/gttxlqbrnd.html

el.classList.toggle("active")
来源：http://hz.andypj.xyz/gtgnuvbutf.html

[U102] JS：本地存储
来源：http://hz.52xcode.cn/gtubtbspvv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hysaishi.cn/gtlolszand.html

[U103] JS：定时器
来源：http://hz.gaohongyu789.top/gtwzwkwlff.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj20258888.top/gtzrbudjme.html

[U104] JS：防抖
来源：http://hz.ywan-chungtsiang.top/gttkodjepj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtbxbpuqcw.html

[U105] JS：节流
来源：http://hz.jqgfzy.top/gtghaiqclm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ybcxt.top/gtojgfeopu.html

[U106] JS：日期格式化
来源：http://hz.meibo888.top/gtfxkgyibc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.aizwys.cn/gtsxuncfod.html

[U107] JS：数字千分位
来源：http://hz.9152youxi.cn/gtheglmkee.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtoexdaonf.html

[U108] JS：随机整数
来源：http://hz.hywenlv.cn/gtkbtjcgul.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtlexbukhh.html

[U109] JS：数组分组
来源：http://hz.ydjk.org.cn/gtameebosl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtkvzitvdt.html

[U110] JS：数组分块
来源：http://hz.nwbrower.top/gtaaeweuhq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gtcbmlouzi.html

[U111] JS：对象转 Map
来源：http://hz.smart0.xyz/gtitecqgjf.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtezbkldvo.html

[U112] JS：字符串补位
来源：http://hz.wangshuangyany.cn/gtqonkjzss.html

"7".padStart(3, "0")
来源：http://hz.hammf.cn/gtzkhzxsaq.html

[U113] JS：正则替换全部
来源：http://hz.jinyuanbaomall.cn/gtimhouawr.html

s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtvplkmlqw.html

[U114] JS：JSON 深比较
来源：http://hz.zhengqikj.top/gtbyhxzbic.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtgfqhmdut.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtaqiguecu.html

crypto.randomUUID()
来源：http://hz.guannengcc.top/gtrzytjluj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jiagoushi.top/gtzcuvzcxa.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigufen.top/gtghxrmphs.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gtvtewckwu.html

npm i -D vitest;  npx vitest
来源：http://hz.ybcxt.top/gtsjilxbsu.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtjkciujch.html

npm i -D vite;  npx vite
来源：http://hz.yj20258.top/gtngtbbcty.html

[U119] JS：生产构建
来源：http://hz.mhx1999.top/gtblmjldbu.html

npx vite build
来源：http://hz.fzhhl.top/gtnzfgmbcr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgfzy.top/gtvehyxgue.html

import.meta.env.VITE_API_URL
来源：http://hz.wangdashe.top/gtkqhlpfsp.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjbtnjebu.html

统计汇总
来源：http://hz.yj20258.top/gtwivjvphc.html

================================================================================
来源：http://hz.gotoacloud.top/gtlyupqwvq.html

按语言统计（条）：
来源：http://hz.shzxlz.cn/gtjvlpnauq.html

Python ......... 252
来源：http://hz.pycfn.com/gteeyfoayh.html

PHP ............ 252
来源：http://hz.zdqjudy.top/gthlfslbnb.html

JavaScript ..... 252
来源：http://hz.shanyushiyangkeji.top/gtaeqwvwfr.html

TypeScript ..... 212
来源：http://hz.zhixingplan.top/gtiifggzap.html

Java ........... 212
来源：http://hz.yangfankeji.com/gtlivsqzul.html

Go ............. 212
来源：http://hz.tanke756.top/gtcgswudbn.html

Ruby ........... 212
来源：http://hz.cucudq.cn/gtubbudgdg.html

C# ............. 212
来源：http://hz.ydzc1.top/gthiasqkah.html

C .............. 30
来源：http://hz.nanxinkj.top/gtnkudnybh.html

C++ ............ 30
来源：http://hz.zhijiandao.cn/gtvwxfgnds.html

SQL ............ 90
来源：http://hz.zdqjudy.top/gtgidzlvhc.html

Bash ........... 80
来源：http://hz.iojbl.cn/gtoiskufsj.html

Kotlin ......... 15
来源：http://hz.ydzc1.top/gtuytsllzo.html

Swift .......... 15
来源：http://hz.fzhhl.top/gtxktslpqe.html

Lua ............ 10
来源：http://hz.cucudq.cn/gtplgonrsi.html

Perl ........... 10
来源：http://hz.ybcxt.top/gtcqgemkrw.html

Scala .......... 10
来源：http://hz.yongpay.top/gtujsyqyme.html

------------------------------------
来源：http://hz.guowangkeji.top/gtrulftdol.html

合计 ........... 2106 条
来源：http://hz.havefunace.top/gtzstftufo.html

按章节统计：
来源：http://hz.chenzaomai.com/gtsnokhuht.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gthauzjyhp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtlnplommk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtrolmcanw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtijvnxqmn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zycfv.cn/gtmnbfoioh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgfzy.top/gtjhxdazzz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gturugwyzf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xingfuxueyuan.xyz/gtrirbdswo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtgarryqef.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gturwslilz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtosohxwgk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtzwcoqagq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtpqdskcdf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtaeocwkio.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gthmbvhekw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtbyjngjwy.html

Q SQL 专题                              90
来源：http://hz.meibo888.top/gtppvlcscf.html

R Bash 专题                             80
来源：http://hz.smart0.xyz/gtfdbgkpqz.html

S C / C++ 专题                          60
来源：http://hz.ydzc1.top/gtvrujfpxb.html

T 其他语言补充                          60
来源：http://hz.xylfe.cn/gtbzzkfpcm.html

U 高频实用片段                         120
来源：http://hz.yvedp.cn/gtrfgqurmx.html

------------------------------------
来源：http://hz.yuxming.cn/gtjrbifnlk.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtpfelaste.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtszjrlhnf.html

使用提醒
来源：http://hz.hfpthk.cn/gtowacmpck.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtxrmxgizo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cdnleiting.top/gtrhlefhld.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhaomingkeji.xyz/gtsgyrxugn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gaohongyu789.top/gtgvavgmru.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtfbepsanc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.meibo888.top/gtinxnedye.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtqeycpziu.html

================================================================================
来源：http://hz.cashguo.top/gtghbzkdmg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xziqi.cn/gtfowohaav.html

Common Programming Examples Cheat Book
来源：http://hz.dianchejie.cn/gtxuygzari.html

================================================================================
来源：http://hz.meibo888.top/gtvcphohap.html

【收录内容】
来源：http://hz.yonumen.top/gtjcuqntcc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yueranfly.top/gthefgqsep.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.aizwys.cn/gtucxgixia.html

SQL · Bash · C · C++
来源：http://hz.xingfuxueyuan.xyz/gtnjtqpoyd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhongyouzk.top/gtnxefozfo.html

【使用说明】
来源：http://hz.pengpengdd.cyou/gtsrmublkn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuxming.cn/gtmqnqzcei.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nanxinkj.top/gtfybtoumm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuanzhike.top/gtcnyupzen.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xinyue.icu/gtwxifbrbs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtxfupltpz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hysaishi.cn/gtmychybhe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xinyue.icu/gtlocqgrje.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.nanxuanxn.top/gtbcnrpbck.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ybcxt.top/gtiyxduyav.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gtyorkflds.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.iojbl.cn/gtqmevdayt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhiwuduotai.top/gtosmrxndq.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gtamdxubaa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ybcxt.top/gtokpupvfe.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtzitzxszp.html

目  录
来源：http://hz.pycfn.com/gtvfysrgxw.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtiwioukwn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtudeqazjo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtntohntcb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtzwqnbhpe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xziqi.cn/gttywosgdd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.vqdsnc.cn/gtqdjffroo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.vqdsnc.cn/gtjzlrtutw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xziqi.cn/gtuzncpmdk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtkitaafwu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtzrgnmkpz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtyzsngnde.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtuighsbyf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtbqgfbnii.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gttfdsyspe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gtiioweizg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xinyue.icu/gtvpcbptoq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gthpwaeljy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangshuangyany.cn/gtnruqfvts.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gtyyzcwzck.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.havefunace.top/gtmqetvvct.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtktdkayrn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtzvgeuwuq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqrezofki.html

A. 基础语法与类型
来源：http://hz.yvedp.cn/gtactrouys.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjxzuhwmk.html

[A01] Hello World
来源：http://hz.kuanghao11.cn/gttvehpsmr.html

Py:   print("Hello, World!")
来源：http://hz.zhengqikj.top/gtgbmawqey.html

PHP:  echo "Hello, World!";
来源：http://hz.pycfn.com/gttriurtry.html

JS:   console.log("Hello, World!");
来源：http://hz.yuxming.cn/gtlosvihvr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.redwolf501.top/gthnoopxkc.html

Java: System.out.println("Hello, World!");
来源：http://hz.hysaishi.cn/gtyoayozdv.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cdnleiting.top/gtenfuilvq.html

Ruby: puts "Hello, World!"
来源：http://hz.sxryk.cn/gtowtsracm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.vqdsnc.cn/gtixcynfkj.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtxgvwqcxd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tian-w.cn/gtonbkfzrm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jyoumei.cn/gtmyzhtlll.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hywenlv.cn/gttfemkhet.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hnqzz.top/gtwiyjimra.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.snrcjt.cn/gtwhddxmcc.html

Go:   name := "Alex"; age := 20
来源：http://hz.tian-w.cn/gtqxlooyvu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnxiangtu.top/gteqbqrelq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuetiantiany.cn/gtvawbiyyr.html

[A03] 常量定义
来源：http://hz.fzhhl.top/gtwqgyklyz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guannengcc.top/gtpwosttbl.html

PHP:  const PI = 3.14159;
来源：http://hz.jqgfzy.top/gttgdqwgee.html

JS:   const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtigqlauar.html

TS:   const PI: number = 3.14159;
来源：http://hz.yanxiufei.cn/gtwmjmeyid.html

Java: static final double PI = 3.14159;
来源：http://hz.52xcode.cn/gtaeolmtwm.html

Go:   const PI = 3.14159
来源：http://hz.sweek.top/gtyabzdyon.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtvxjmdnay.html

C#:   const double PI = 3.14159;
来源：http://hz.meibo888.top/gtcejtskfn.html

[A04] 判断变量类型
来源：http://hz.meibo888.top/gtqmbasxoh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangshuangyany.cn/gtwvbalobw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hammf.cn/gthbsmwpsx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.chenjidiqi.icu/gtohsmhekz.html

TS:   typeof x; x instanceof Date
来源：http://hz.gaohongyu789.top/gtkwaolkgz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.chenlongwang.top/gtuaczgysb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhixingplan.top/gtnxndalnr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hnqzz.top/gtpdrswude.html

C#:   x.GetType().Name; x is int
来源：http://hz.smart0.xyz/gtoparrbry.html

[A05] 整数除法与取模
来源：http://hz.xziqi.cn/gtsqolnkwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhijiandao.cn/gtsramrpua.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cashguo.top/gtkuhhfsya.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zdqjudy.top/gtwqnybsmz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangdashe.top/gtvwndztys.html

Java: 7 / 2; 7 % 2
来源：http://hz.sweek.top/gtecuipxjx.html

Go:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtmbhyfrds.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtxiwiusjn.html

C#:   7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtarotmjpf.html

[A06] 字符串转数字
来源：http://hz.yvedp.cn/gtalswgtga.html

Py:   int("42"); float("3.14")
来源：http://hz.xylfe.cn/gtufnbumuf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.redwolf501.top/gtqnzulvkl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.iojbl.cn/gtnxferwak.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhijiandao.cn/gtxkqemcls.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hongshengwenyu.top/gtaiclrhmg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tanke756.top/gtaulenawe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhijiandao.cn/gtywbhlztk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shanyushiyangtech.top/gtujwofphi.html

[A07] 数字转字符串
来源：http://hz.zhixingplan.top/gtoorojvna.html

Py:   str(42)
来源：http://hz.daxiang520.top/gtthjubduu.html

PHP:  (string) 42; strval(42)
来源：http://hz.cqqwz.cn/gtaywyjsgp.html

JS:   String(42); (42).toString()
来源：http://hz.yuanzhike.top/gtdcpixfuc.html

TS:   String(42)
来源：http://hz.shuidangran.top/gtxtshuvap.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.fzhhl.top/gtaxmwpmjj.html

Go:   strconv.Itoa(42)
来源：http://hz.52xcode.cn/gtqbkyojkw.html

Ruby: 42.to_s
来源：http://hz.cheryme.top/gtouvscgfs.html

C#:   42.ToString()
来源：http://hz.jlsjyb.cn/gtnhardrui.html

[A08] 取整与四舍五入
来源：http://hz.hnxiangtu.top/gtyriwtytb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hammf.cn/gtumneqhyx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhaomingkeji.xyz/gttudpbhby.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jqgfzy.top/gtufdnenmc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hammf.cn/gtsnclhmnt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xinyue.icu/gtndpqgzoz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jqgufenzy.top/gtueojgqml.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.kuanghao11.cn/gtjbrjovkz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ehwqpu.com/gtyunszwcf.html

[A09] 绝对值与最大最小值
来源：http://hz.jinqigfzy.top/gtuindgeez.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtifaofumc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tianlin.xyz/gtlmnbdhnj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.quarkkingdee.top/gtczvqytyu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtpzlrnyfn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxuanxn.top/gtkpvmhymw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hammf.cn/gttdlnxtpq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.pengpengdd.cyou/gtuedayukj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.9152youxi.cn/gtkvddgsaq.html


<!-- 参考信息 -->