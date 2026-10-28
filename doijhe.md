代发 wailian999

[U61] PHP：正则
来源：http://hz.nanxinkj.top/gtoykgmxhw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.aibaodan.cn/gtatluyjys.html

[U62] PHP：日期对象
来源：http://hz.jlsjyb.cn/gtqbprzqdf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigufen.top/gtbxniwgpz.html

[U63] PHP：文件读写
来源：http://hz.nanxinkj.top/gtplinweoi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtaeznwlil.html

[U64] PHP：目录遍历
来源：http://hz.vqdsnc.cn/gtysjqtskl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtqwfjnltj.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtmjryfypd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.andypj.xyz/gtwzcehaca.html

[U66] PHP：设置 Cookie
来源：http://hz.yuxming.cn/gtzbdjwwqk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhongyouzk.top/gtedekbgpg.html

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gttupobkhg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yongpay.top/gtyvioeacv.html

[U68] PHP：PDO 连接
来源：http://hz.meibo888.top/gtsniyubll.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtkiojlfqi.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtyvqetxan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tanke756.top/gtmlkhxpxl.html

[U70] PHP：PDO 事务
来源：http://hz.shangyingyoupin.top/gtgsehmugv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pycfn.com/gtmicqnrjj.html

[U71] PHP：抛出异常
来源：http://hz.xziqi.cn/gtqzpkadww.html

throw new RuntimeException("失败", 500);
来源：http://hz.shzxlz.cn/gtfddmgccf.html

[U72] PHP：写错误日志
来源：http://hz.quarkkingdee.top/gtqhankiyl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yongpay.top/gtiqrtcvck.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinghuilouyu.cn/gtttgzfqmw.html

parse_ini_file("config.ini", true)
来源：http://hz.wangdashe.top/gtujwbltod.html

[U74] PHP：读取环境变量
来源：http://hz.cashguo.top/gtuwbzqxjb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ppjwa.cn/gtthucdrgk.html

[U75] PHP：依赖注入
来源：http://hz.fzhhl.top/gtyjwzdlke.html

composer require psr/container
来源：http://hz.xziqi.cn/gtolmomrcm.html

[U76] PHP：简单路由
来源：http://hz.nwbrower.top/gttnnlsuku.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yangfankeji.com/gtsmdryqhh.html

[U77] PHP：模板渲染
来源：http://hz.ydzc1.top/gtoqfadllm.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtsvupaojp.html

[U78] PHP：单元测试
来源：http://hz.shangyingyoupin.top/gtgxeoymql.html

composer require --dev phpunit/phpunit
来源：http://hz.shanyushiyangkeji.top/gthzlgwvhn.html

[U79] PHP：静态分析
来源：http://hz.9152youxi.cn/gtuyltvkih.html

composer require --dev phpstan/phpstan
来源：http://hz.zhongyouzk.top/gtcgwjjqoj.html

[U80] PHP：代码规范修复
来源：http://hz.bjfxy.top/gttwgakufu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daxiang520.top/gtdzwfscfe.html

[U81] JS：初始化项目
来源：http://hz.hfpthk.cn/gtswdphssj.html

npm init -y;  npm i express
来源：http://hz.gaohongyu789.top/gtdhwhgvhr.html

[U82] JS：package.json 脚本
来源：http://hz.ivvv.top/gtzemwbsdb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cashguo.top/gtqhkufpij.html

[U83] JS：ES Module 导入导出
来源：http://hz.fzhhl.top/gtgqartolt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.pengpengdd.cyou/gtpkefntuc.html

[U84] JS：CommonJS 写法
来源：http://hz.tian-w.cn/gtimcdftes.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sxryk.cn/gtodkyqxdx.html

[U85] JS：可选链
来源：http://hz.gzhubu.top/gtnqzfepoz.html

a?.b?.c
来源：http://hz.shuidangran.top/gtyagcjfur.html

[U86] JS：空值合并
来源：http://hz.zhixingplan.top/gtairmnfvc.html

a ?? b
来源：http://hz.dianchejie.cn/gtrhapwixr.html

[U87] JS：解构默认值
来源：http://hz.yonumen.top/gtvmffzebc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.vqdsnc.cn/gtwlzjekwg.html

[U88] JS：对象展开合并
来源：http://hz.xingfuxueyuan.xyz/gtdenufadw.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gturdlsved.html

[U89] JS：数组去重
来源：http://hz.pycfn.com/gttoaqjzqn.html

[...new Set(arr)]
来源：http://hz.hysaishi.cn/gtoqzmtesy.html

[U90] JS：数字数组排序
来源：http://hz.ybcxt.top/gtukhfbcsz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtbkkarogu.html

[U91] JS：对象键值遍历
来源：http://hz.c1oappe.top/gtqvdlhbzv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtuadyaloi.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtiwvhtljj.html

structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtkkihzmfp.html

[U93] JS：模板字符串
来源：http://hz.zhaomingkeji.xyz/gtnnlnhion.html

`共 ${n} 条`
来源：http://hz.jianghu66.top/gtleejsatj.html

[U94] JS：箭头函数
来源：http://hz.jinqigufen.top/gtmentniny.html

const double = x => x * 2;
来源：http://hz.zdqjudy.top/gtvskvkesm.html

[U95] JS：Promise 包装
来源：http://hz.gaohongyu789.top/gtoawekula.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtqrlxhyrg.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtknuawkre.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtlfynlqgg.html

[U97] JS：并发请求
来源：http://hz.hywenlv.cn/gtkayrekse.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gttsxirtad.html

[U98] JS：fetch 带 JSON
来源：http://hz.daria6918.cn/gtizemejji.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guannengcc.top/gtuumxtvlm.html

[U99] JS：事件监听
来源：http://hz.meibo888.top/gtipwpxvce.html

el.addEventListener("click", e => {})
来源：http://hz.svipenyu.cn/gtguzfivlw.html

[U100] JS：DOM 查询
来源：http://hz.bjfxy.top/gtjschgceo.html

document.querySelector(".item")
来源：http://hz.jinqigfzy.top/gtdujecovj.html

[U101] JS：classList 操作
来源：http://hz.haohaochexian.top/gtyuflwdle.html

el.classList.toggle("active")
来源：http://hz.gotoacloud.top/gtwlzjqrdk.html

[U102] JS：本地存储
来源：http://hz.zhengqikj.top/gtrgxxtmig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.redwolf501.top/gtztjjsffk.html

[U103] JS：定时器
来源：http://hz.ydjk.org.cn/gtsfdlrsgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zdqjudy.top/gtnesuhblb.html

[U104] JS：防抖
来源：http://hz.ppjwa.cn/gtuduxhfxx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtpaeggvod.html

[U105] JS：节流
来源：http://hz.birdmap.top/gtgowblnnw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.mhx1999.top/gtnoleojtt.html

[U106] JS：日期格式化
来源：http://hz.nwbrower.top/gtamnftyep.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnqzz.top/gtfilasefz.html

[U107] JS：数字千分位
来源：http://hz.kuanghao11.cn/gtypzrqmse.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.quarkkingdee.top/gtzibuckou.html

[U108] JS：随机整数
来源：http://hz.pycfn.com/gtvgxnxtwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xinyue.icu/gtugnbwtao.html

[U109] JS：数组分组
来源：http://hz.jinqigufen.top/gttvuhwbcj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtqhoomovf.html

[U110] JS：数组分块
来源：http://hz.tian-w.cn/gtmhljtmqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gtkatyvcky.html

[U111] JS：对象转 Map
来源：http://hz.sysykeji.top/gteovhpkwg.html

new Map(Object.entries(obj))
来源：http://hz.nwbrower.top/gtztlsxjvd.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtmxcmpybj.html

"7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtrtlcczns.html

[U113] JS：正则替换全部
来源：http://hz.guannengcc.top/gtdfxwwrzi.html

s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtonvbzshb.html

[U114] JS：JSON 深比较
来源：http://hz.hnxiangtu.top/gtlmvurytj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtdewgyvkd.html

[U115] JS：生成 UUID
来源：http://hz.ehwqpu.com/gtlukqjyol.html

crypto.randomUUID()
来源：http://hz.yuxming.cn/gtsaxesyhw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yanxiufei.cn/gtgrqpcynl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtsjrolada.html

[U117] JS：单元测试
来源：http://hz.andypj.xyz/gtzazkpndm.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gtadoxwdkj.html

[U118] JS：开发服务器
来源：http://hz.hnqzz.top/gtfvgiejkp.html

npm i -D vite;  npx vite
来源：http://hz.shangyingyoupin.top/gtzdxzdqgx.html

[U119] JS：生产构建
来源：http://hz.shangyingyoupin.top/gtvqzlecqw.html

npx vite build
来源：http://hz.hnxiangtu.top/gtkgddklic.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.bjfxy.top/gtkbyehvfc.html

import.meta.env.VITE_API_URL
来源：http://hz.ivvv.top/gtbbnsjpqt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdazijfwn.html

统计汇总
来源：http://hz.yuanzhike.top/gtmvujwjdw.html

================================================================================
来源：http://hz.ivvv.top/gtbxotxtcw.html

按语言统计（条）：
来源：http://hz.hysaishi.cn/gtjprtqupx.html

Python ......... 252
来源：http://hz.yvedp.cn/gtmmfqwghe.html

PHP ............ 252
来源：http://hz.nanxinkj.top/gtevrgxddb.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtkarazljy.html

TypeScript ..... 212
来源：http://hz.jyoumei.cn/gtgiuudeqn.html

Java ........... 212
来源：http://hz.yueranfly.top/gtvbaobaxn.html

Go ............. 212
来源：http://hz.chenlongwang.top/gtcotxyhax.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gttnjfhjsy.html

C# ............. 212
来源：http://hz.gotoacloud.top/gtpodoyuvk.html

C .............. 30
来源：http://hz.xinyue.icu/gtqmvicxcs.html

C++ ............ 30
来源：http://hz.yueranfly.top/gtfdjwugaq.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtxaahjcst.html

Bash ........... 80
来源：http://hz.jyoumei.cn/gtseunkwfj.html

Kotlin ......... 15
来源：http://hz.hysaishi.cn/gtjotkjpzg.html

Swift .......... 15
来源：http://hz.ywan-chungtsiang.top/gtarvwdzac.html

Lua ............ 10
来源：http://hz.jqgufenzy.top/gtgfjwmdts.html

Perl ........... 10
来源：http://hz.nwbrower.top/gtljhjxaia.html

Scala .......... 10
来源：http://hz.hnqzz.top/gttffivgec.html

------------------------------------
来源：http://hz.zycfv.cn/gttzfkefui.html

合计 ........... 2106 条
来源：http://hz.0kj1m.cn/gtubbptlfv.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtkijdaeft.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtcwwxoiog.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtlhxwacwk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtbeqbfvkp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gttjyesjcd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhiwuduotai.top/gtbdlsgxov.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtlothupsm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtmwmnsnaw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gtjprqqfbn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtioldyaqs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtfhgsteph.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtsnuqhlqm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtuxenqzhp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtjqjfugmz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gaohongyu789.top/gtdzeigafq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenlongwang.top/gtdpmhsoch.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtgrpzhwcz.html

Q SQL 专题                              90
来源：http://hz.jiagoushi.top/gthumcrgdq.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtrpmaymmu.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtqfzcmtxw.html

T 其他语言补充                          60
来源：http://hz.zhengqikj.top/gtvzafbojp.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gtdbxepcdn.html

------------------------------------
来源：http://hz.andypj.xyz/gtwjrnxawl.html

合计                                  2106 条
来源：http://hz.jyoumei.cn/gtcbrrxqmv.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtsgkloteb.html

使用提醒
来源：http://hz.bjfxy.top/gtxtdsnuva.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtxeqpwuei.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tian-w.cn/gtcdsdmsbe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nwbrower.top/gtgkyrpijj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fzhhl.top/gttwtgdkii.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ybcxt.top/gtmtltidle.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.quarkkingdee.top/gtftujjjgz.html

—— 文件结束 ——
来源：http://hz.yanxiufei.cn/gtyjqvfftt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjcolaxum.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.meibo888.top/gtlrwxftem.html

Common Programming Examples Cheat Book
来源：http://hz.gogol.net.cn/gtpfuqkqyx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtaogrdgah.html

【收录内容】
来源：http://hz.pycfn.com/gteeeglakt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.aizwys.cn/gtssjdqhci.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhongyouzk.top/gtmyybajug.html

SQL · Bash · C · C++
来源：http://hz.ydjk.org.cn/gtxsedabpa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nwbrower.top/gtqwhtosrd.html

【使用说明】
来源：http://hz.chenjidiqi.icu/gtjpuoxzft.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shangyingyoupin.top/gtdrtafflt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.redwolf501.top/gtrvmpctnq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.aizwys.cn/gtamedtxrm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenlongwang.top/gtkxgxeogf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.chenlongwang.top/gtelvdocsg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xziqi.cn/gtuphegwxd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.andypj.xyz/gtecgioeub.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yanxiufei.cn/gtwrrckrlg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.pengpengdd.cyou/gtssjvoxin.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinqigufen.top/gtoggkacll.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigufen.top/gtegqbipff.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xziqi.cn/gtedffkuhg.html

【文件统计】
来源：http://hz.shzxlz.cn/gtnighqkgp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.quarkkingdee.top/gtusxhagwg.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtdyotqaoo.html

目  录
来源：http://hz.xuetiantiany.cn/gtmzgxwjrc.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gticwxpune.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtzmszprau.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gtyjbvxkju.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gthjsnvyel.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtpvkdrohv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jianghu66.top/gtaqcefpuw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtpnvfsemc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtavgmghax.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tianlin.xyz/gtmpovjeht.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtimneepht.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yangfankeji.com/gtaneapyvv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtntpwqxaa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtkyimyhhl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtlijxmnfh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sysykeji.top/gthkivmfvt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangkeji.top/gtgokbbfqf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtpotsziwv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtjaplbkqn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxinkj.top/gtbvbsapjh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.52xcode.cn/gtefyllsxq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtcaopjkfg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtpxppkbna.html

================================================================================
来源：http://hz.cdnleiting.top/gtfocfkuon.html

A. 基础语法与类型
来源：http://hz.svipenyu.cn/gtmmpgfdtu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthymfkzdv.html

[A01] Hello World
来源：http://hz.xylfe.cn/gtstechbtw.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtzzgjwmkx.html

PHP:  echo "Hello, World!";
来源：http://hz.sufxvd.cn/gttrsdlfrp.html

JS:   console.log("Hello, World!");
来源：http://hz.guowangkeji.top/gtolhrmfwe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.316326.xyz/gtdpuszoks.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinghuilouyu.cn/gtjvgjesnd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yonumen.top/gtqenfdjpo.html

Ruby: puts "Hello, World!"
来源：http://hz.pengpengdd.cyou/gtkafoieeu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tianlin.xyz/gtminarpsm.html

[A02] 变量声明与赋值
来源：http://hz.hfpthk.cn/gtclauvywh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jlsjyb.cn/gtqjizkdpn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnxiangtu.top/gtlcvibaei.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenjidiqi.icu/gtqrcjrlul.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yanxiufei.cn/gtybhhnbxr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.iojbl.cn/gtvzuireai.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtxsvygsls.html

Ruby: name = "Alex"; age = 20
来源：http://hz.aizwys.cn/gtpzgokgkg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtvdzutdgd.html

[A03] 常量定义
来源：http://hz.zhoulong.xyz/gtbpuzkdbv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tian-w.cn/gtqvzqszfl.html

PHP:  const PI = 3.14159;
来源：http://hz.sxryk.cn/gtbdnjoaau.html

JS:   const PI = 3.14159;
来源：http://hz.xinyue.icu/gtrxanfmsr.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigufen.top/gtwdhxjtld.html

Java: static final double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtyxfmaemh.html

Go:   const PI = 3.14159
来源：http://hz.daria6918.cn/gtdxcxqkgp.html

Ruby: PI = 3.14159
来源：http://hz.pycfn.com/gtumtbhesf.html

C#:   const double PI = 3.14159;
来源：http://hz.ivvv.top/gtbuuvbbjf.html

[A04] 判断变量类型
来源：http://hz.hammf.cn/gtisqovvva.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangshuangyany.cn/gtmjfxieja.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.haohaochexian.top/gtjxdvzbll.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shuidangran.top/gtzgtrerub.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtnpdjovrw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hammf.cn/gtdsfrbmay.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj20258.top/gtgcsvsprg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.fzhhl.top/gtgdqokxll.html

C#:   x.GetType().Name; x is int
来源：http://hz.shanyushiyangtech.top/gtpeeoslvf.html

[A05] 整数除法与取模
来源：http://hz.chenlongwang.top/gtuzplmjxu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ywan-chungtsiang.top/gtuipzouoc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hnqzz.top/gtvjarovsf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tianlin.xyz/gtmbbeiyqj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuanzx.com/gtgbtxhvgm.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinqigfzy.top/gtppqrnryp.html

Go:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtzerdgptk.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jinqigufen.top/gtnlrroltg.html

C#:   7 / 2; 7 % 2
来源：http://hz.yangfankeji.com/gtvwrkzkyd.html

[A06] 字符串转数字
来源：http://hz.haohaochexian.top/gtzemiblyw.html

Py:   int("42"); float("3.14")
来源：http://hz.shangyingyoupin.top/gtyltmwdwu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.feifeiyinyue.top/gtpkzcmihy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.0kj1m.cn/gtwavvwwic.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jqgfzy.top/gtzugpnmpf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.0kj1m.cn/gtxivbuxrn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pycfn.com/gtyrbwnivv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.aibaodan.cn/gtlvdudfqn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj20258.top/gtfygaycws.html

[A07] 数字转字符串
来源：http://hz.c1oappe.top/gtvxtyeksg.html

Py:   str(42)
来源：http://hz.c1oappe.top/gtpfxmenxl.html

PHP:  (string) 42; strval(42)
来源：http://hz.haohaochexian.top/gtjcvdddih.html

JS:   String(42); (42).toString()
来源：http://hz.hongshengwenyu.top/gtxphaylkl.html

TS:   String(42)
来源：http://hz.ivvv.top/gtlhxzkeld.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gzhubu.top/gttokesoww.html

Go:   strconv.Itoa(42)
来源：http://hz.daria6918.cn/gthzsojsxm.html

Ruby: 42.to_s
来源：http://hz.smart0.xyz/gtqfdhxwty.html

C#:   42.ToString()
来源：http://hz.havefunace.top/gtfcasxyrf.html

[A08] 取整与四舍五入
来源：http://hz.xinyue.icu/gtzngcvukt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtboxeyovk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.52xcode.cn/gtsvrdsjqw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtjyhviivb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sufxvd.cn/gtxqlmrmal.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhiwuduotai.top/gtzvtxjaan.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.shangyingyoupin.top/gtzrhbczpg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yueranfly.top/gtletycrwd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shzxlz.cn/gthcgzabbh.html

[A09] 绝对值与最大最小值
来源：http://hz.nwbrower.top/gtywlawhhr.html


<!-- 参考信息 -->