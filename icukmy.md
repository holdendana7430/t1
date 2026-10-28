代发 wailian999

[U61] PHP：正则
来源：http://hz.shzxlz.cn/gtxgkqukxk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtlzoiqlsq.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtcexcduor.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.0kj1m.cn/gtlodtaujj.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gthklnkzeh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtrvgwqeqi.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtpkitonze.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aibaodan.cn/gtnqktgkgm.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtxnpncuqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gtaujgamdp.html

[U66] PHP：设置 Cookie
来源：http://hz.fengsongda.top/gtgzyrwjme.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhixingplan.top/gtmdkgnlnm.html

[U67] PHP：处理文件上传
来源：http://hz.jinghuilouyu.cn/gtciutvqzr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhaomingkeji.xyz/gtrhnmiavl.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtreyqlaal.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxinkj.top/gtslmpinel.html

[U69] PHP：PDO 预处理
来源：http://hz.cqqwz.cn/gtnhldqpid.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tian-w.cn/gtgdzpipqr.html

[U70] PHP：PDO 事务
来源：http://hz.dashuyun.cn/gtoqkiqycm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.mhx1999.top/gtzyetatzg.html

[U71] PHP：抛出异常
来源：http://hz.xuetiantiany.cn/gtudfpsugx.html

throw new RuntimeException("失败", 500);
来源：http://hz.daria6918.cn/gteasmcmwd.html

[U72] PHP：写错误日志
来源：http://hz.cucudq.cn/gtruizurod.html

error_log("失败: " . $e->getMessage());
来源：http://hz.snrcjt.cn/gtwftxwsrj.html

[U73] PHP：读取 ini 配置
来源：http://hz.haohaochexian.top/gtezecmfbm.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtayvygrha.html

[U74] PHP：读取环境变量
来源：http://hz.jinqigufen.top/gtpqgbkdwc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tian-w.cn/gtalrkbwsh.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtadkpzdht.html

composer require psr/container
来源：http://hz.jlsjyb.cn/gtrjsemoks.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangtech.top/gtodloifds.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cdnleiting.top/gtzsitwknt.html

[U77] PHP：模板渲染
来源：http://hz.zycfv.cn/gtrkpamnea.html

composer require twig/twig
来源：http://hz.meibo888.top/gtbmircvek.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtsepxpqjd.html

composer require --dev phpunit/phpunit
来源：http://hz.feifeiyinyue.top/gtjroitxeg.html

[U79] PHP：静态分析
来源：http://hz.feifeiyinyue.top/gtvprbxlzv.html

composer require --dev phpstan/phpstan
来源：http://hz.wangdashe.top/gtwcovdsuh.html

[U80] PHP：代码规范修复
来源：http://hz.gogol.net.cn/gtffteovtf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ydjk.org.cn/gtaxtppusn.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtzoibachf.html

npm init -y;  npm i express
来源：http://hz.shangyingyoupin.top/gthotqitlp.html

[U82] JS：package.json 脚本
来源：http://hz.yueranfly.top/gtmzrswqqa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.dashuyun.cn/gtoskyugtj.html

[U83] JS：ES Module 导入导出
来源：http://hz.jyoumei.cn/gtfpxrrdaa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tian-w.cn/gtshbbcanc.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gteqezppls.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangshuangyany.cn/gtplcokgrx.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gtinmpjiit.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtacmhmrto.html

[U86] JS：空值合并
来源：http://hz.nwbrower.top/gtwwedohgw.html

a ?? b
来源：http://hz.fengsongda.top/gtiseeuhjg.html

[U87] JS：解构默认值
来源：http://hz.havefunace.top/gtzlvexrxj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtrmajwkch.html

[U88] JS：对象展开合并
来源：http://hz.fengsongda.top/gtuuvikspy.html

{ ...a, ...b }
来源：http://hz.sweek.top/gtyolpdjpp.html

[U89] JS：数组去重
来源：http://hz.zhixingplan.top/gtlooxrciy.html

[...new Set(arr)]
来源：http://hz.sxryk.cn/gtzyigxuvh.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gtghchwhdw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtvslwulau.html

[U91] JS：对象键值遍历
来源：http://hz.andypj.xyz/gtohiijikq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gotoacloud.top/gtrkkqpbym.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtryfgbxcy.html

structuredClone(obj)
来源：http://hz.yangfankeji.com/gtdzdoajuc.html

[U93] JS：模板字符串
来源：http://hz.iojbl.cn/gtixxzpdwo.html

`共 ${n} 条`
来源：http://hz.quarkkingdee.top/gtbeebwyai.html

[U94] JS：箭头函数
来源：http://hz.ydjk.org.cn/gtoagtycbh.html

const double = x => x * 2;
来源：http://hz.zhongyouzk.top/gtdkbfuomh.html

[U95] JS：Promise 包装
来源：http://hz.xylfe.cn/gttpvfwnpz.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtccwqnoue.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gtytlpduyf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtvoekstln.html

[U97] JS：并发请求
来源：http://hz.shangyingyoupin.top/gtzqdsaima.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtkodppfab.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenzaomai.com/gtwsqdeqta.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zdqjudy.top/gtwbghknjy.html

[U99] JS：事件监听
来源：http://hz.yueranfly.top/gtqblrxudc.html

el.addEventListener("click", e => {})
来源：http://hz.vqdsnc.cn/gtjcvcecve.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtqyusudfy.html

document.querySelector(".item")
来源：http://hz.iojbl.cn/gtbaplvtrl.html

[U101] JS：classList 操作
来源：http://hz.52xcode.cn/gtmfgrhsky.html

el.classList.toggle("active")
来源：http://hz.yj202588.top/gtcbdadebo.html

[U102] JS：本地存储
来源：http://hz.zhixingplan.top/gtjuhovgsq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhongyouzk.top/gtjmowpjqz.html

[U103] JS：定时器
来源：http://hz.sweek.top/gtkdqcyqos.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zycfv.cn/gtuimlshew.html

[U104] JS：防抖
来源：http://hz.jqgfzy.top/gtxsskavft.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtzhisdtvj.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtmpzramvw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yanxiufei.cn/gtnfikunix.html

[U106] JS：日期格式化
来源：http://hz.ivvv.top/gtscfvfxzh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtwghjetbr.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtskuxcczt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jianghu66.top/gtrccvatsl.html

[U108] JS：随机整数
来源：http://hz.feifeiyinyue.top/gtogjpcwbm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuetiantiany.cn/gttmppuldh.html

[U109] JS：数组分组
来源：http://hz.aibaodan.cn/gtqudbzoag.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtrirekvvg.html

[U110] JS：数组分块
来源：http://hz.ppjwa.cn/gtrqqnsaal.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dashuyun.cn/gtslorihab.html

[U111] JS：对象转 Map
来源：http://hz.nanxinkj.top/gtgtulabye.html

new Map(Object.entries(obj))
来源：http://hz.sxryk.cn/gtupasvxqt.html

[U112] JS：字符串补位
来源：http://hz.yvedp.cn/gtplolhysf.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtpqfbdivy.html

[U113] JS：正则替换全部
来源：http://hz.yvedp.cn/gtocftodjb.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtvxihawao.html

[U114] JS：JSON 深比较
来源：http://hz.zhongyouzk.top/gthjobxqti.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtddpxxwtu.html

[U115] JS：生成 UUID
来源：http://hz.snrcjt.cn/gtbdcxjzgr.html

crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtldsazrwb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnxiangtu.top/gtlnzkuerv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hongshengwenyu.top/gtitaulnts.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtbhgwcwgb.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtqhxerirm.html

[U118] JS：开发服务器
来源：http://hz.zdqjudy.top/gtjizpchkl.html

npm i -D vite;  npx vite
来源：http://hz.ywan-chungtsiang.top/gtqmyoqavv.html

[U119] JS：生产构建
来源：http://hz.xuanzx.com/gthcgmcefx.html

npx vite build
来源：http://hz.zhengqikj.top/gtvevzjoss.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtoqqaoqdx.html

import.meta.env.VITE_API_URL
来源：http://hz.mhx1999.top/gtdhbgtxvr.html

================================================================================
来源：http://hz.mhx1999.top/gtqnjtctub.html

统计汇总
来源：http://hz.iojbl.cn/gtaitmhshb.html

================================================================================
来源：http://hz.bjfxy.top/gtufcivqmk.html

按语言统计（条）：
来源：http://hz.jqgufenzy.top/gtujrzcpol.html

Python ......... 252
来源：http://hz.birdmap.top/gtjyyrozjp.html

PHP ............ 252
来源：http://hz.xinyue.icu/gtaebsawrm.html

JavaScript ..... 252
来源：http://hz.xylfe.cn/gtuewrljdl.html

TypeScript ..... 212
来源：http://hz.zhijiandao.cn/gtzzaoznev.html

Java ........... 212
来源：http://hz.meibo888.top/gtauozlxri.html

Go ............. 212
来源：http://hz.jiagoushi.top/gtpvzjfkjo.html

Ruby ........... 212
来源：http://hz.yj20258.top/gtzvoxflgq.html

C# ............. 212
来源：http://hz.haohaochexian.top/gtnkplhfdz.html

C .............. 30
来源：http://hz.gaohongyu789.top/gtdjjplaou.html

C++ ............ 30
来源：http://hz.52xcode.cn/gtemgtkasv.html

SQL ............ 90
来源：http://hz.hywenlv.cn/gtxlsxqvzy.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtlcesvsgq.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtgsrskpjz.html

Swift .......... 15
来源：http://hz.ybcxt.top/gtkokiwpjn.html

Lua ............ 10
来源：http://hz.jinyuanbaomall.cn/gtnqaftuoz.html

Perl ........... 10
来源：http://hz.wangdashe.top/gthxnollgy.html

Scala .......... 10
来源：http://hz.sysykeji.top/gtbxjwjltp.html

------------------------------------
来源：http://hz.ehwqpu.com/gtxykxpiui.html

合计 ........... 2106 条
来源：http://hz.gzhubu.top/gtritgtugq.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gtdwszjknj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gzhubu.top/gtcpjljlsi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gthgjlazwz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.guannengcc.top/gtycqrwtgv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtfjykfgwm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnxiangtu.top/gtniuehgmo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtdwartzle.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtgsfrnefd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtsnzmjgei.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtepivscdk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.vqdsnc.cn/gtjswejdbf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtpxzregun.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtvrwepeen.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtckstqwmv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hnqzz.top/gtuxrrpkud.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yueranfly.top/gtexjemlpx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtxaagxuiy.html

Q SQL 专题                              90
来源：http://hz.andypj.xyz/gtwfkiggbl.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gtzzcrrjvv.html

S C / C++ 专题                          60
来源：http://hz.jinghuilouyu.cn/gthmfgodix.html

T 其他语言补充                          60
来源：http://hz.yuanzhike.top/gtucwobnbg.html

U 高频实用片段                         120
来源：http://hz.hysaishi.cn/gtpkctcopb.html

------------------------------------
来源：http://hz.fzhhl.top/gtvytvdrts.html

合计                                  2106 条
来源：http://hz.chenjidiqi.icu/gtmlbdhxlg.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtssizrbwy.html

使用提醒
来源：http://hz.nanxinkj.top/gtjtqqumjm.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gttqmnrncl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.havefunace.top/gtxuyjhmjz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.redwolf501.top/gtcifrwrld.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258888.top/gtaimusqgk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shuidangran.top/gttmyjobhc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yonumen.top/gtccscrpbx.html

—— 文件结束 ——
来源：http://hz.xingfuxueyuan.xyz/gtufyiqdsu.html

================================================================================
来源：http://hz.yuxming.cn/gtpjhnkfrc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtmwjckatt.html

Common Programming Examples Cheat Book
来源：http://hz.kuanghao11.cn/gtuetutusv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkilqyupn.html

【收录内容】
来源：http://hz.aibaodan.cn/gtznztznhe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ppjwa.cn/gtdrajyuhh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gtaalkyvib.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtcrhumrii.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenlongwang.top/gtwobquxtp.html

【使用说明】
来源：http://hz.nwbrower.top/gtsalijabj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.dianchejie.cn/gtmpcgipig.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tian-w.cn/gtpjwkonhs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gtdnhipvlf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.guowangkeji.top/gtmwloaqup.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangdashe.top/gtwvvqjomb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gteorrqbem.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sweek.top/gtgbcsdfxu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xinyue.icu/gtmimaptqr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtkihsjygv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yanxiufei.cn/gtwzrldqna.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xylfe.cn/gtjlfwimnz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gttxgsokxh.html

【文件统计】
来源：http://hz.yj202588.top/gtwryhsfxy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gtrtyszzmd.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtbjnrsmrj.html

目  录
来源：http://hz.ivvv.top/gtoidymnug.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtnojfwsru.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhengqikj.top/gttlztgujv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shzxlz.cn/gtqnidikif.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtymilixic.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ehwqpu.com/gtdoyebjuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shanyushiyangkeji.top/gtvgcjzqwi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtjypiqzhz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zdqjudy.top/gtarxdeuic.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtgwfwaayu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtwdxeuxgp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tanke756.top/gtomjwbsph.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtlqilyfoi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gttulngaet.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtkpdcycte.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.andypj.xyz/gtnvgwmxtg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtduumydux.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtpbifcuyi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jlsjyb.cn/gtdcfswegm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtriblwnrt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gotoacloud.top/gtugmewreg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtozourrni.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtfthbgyyt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtkdrtfbdv.html

A. 基础语法与类型
来源：http://hz.tanke756.top/gtgnqbnhuh.html

================================================================================
来源：http://hz.gaohongyu789.top/gthraaubgp.html

[A01] Hello World
来源：http://hz.dashuyun.cn/gtfxbkffid.html

Py:   print("Hello, World!")
来源：http://hz.xinyue.icu/gtjuhupedk.html

PHP:  echo "Hello, World!";
来源：http://hz.feifeiyinyue.top/gtztcrmoqj.html

JS:   console.log("Hello, World!");
来源：http://hz.fengsongda.top/gtwmclgbzw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtdraymxac.html

Java: System.out.println("Hello, World!");
来源：http://hz.jlsjyb.cn/gtwchitskp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangshuangyany.cn/gtgfhcmdvi.html

Ruby: puts "Hello, World!"
来源：http://hz.jinghuilouyu.cn/gtrfdwtpqe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xuanzx.com/gtxdgjnnyi.html

[A02] 变量声明与赋值
来源：http://hz.xziqi.cn/gtussoerpq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinghuilouyu.cn/gtahcpfcfx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.c1oappe.top/gtfjauthxr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xylfe.cn/gtnucfhjdq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sxryk.cn/gtebamoowr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daxiang520.top/gteapqyzzi.html

Go:   name := "Alex"; age := 20
来源：http://hz.fzhhl.top/gtayjqrsho.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sufxvd.cn/gtrocdbcpn.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nanxuanxn.top/gtdbodlifh.html

[A03] 常量定义
来源：http://hz.chenzaomai.com/gtpgtzonsz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zdqjudy.top/gtxrnelhnj.html

PHP:  const PI = 3.14159;
来源：http://hz.yuanzhike.top/gtaukkrofr.html

JS:   const PI = 3.14159;
来源：http://hz.birdmap.top/gtqikywwrp.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgfzy.top/gtjatskvtl.html

Java: static final double PI = 3.14159;
来源：http://hz.xylfe.cn/gtkmxdpyla.html

Go:   const PI = 3.14159
来源：http://hz.bjfxy.top/gtepmysuyb.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtoegvlzgd.html

C#:   const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtfcblkbay.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtjgzcpxns.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.cdnleiting.top/gtchcilqhn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yuanzhike.top/gtotujyzku.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinghuilouyu.cn/gtmzpvlwsd.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinqigufen.top/gtfndgwlfn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangkeji.top/gtmvwdphzf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.sxryk.cn/gtihdebqvk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yueranfly.top/gtizlqdyhn.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinghuilouyu.cn/gtqimedyif.html

[A05] 整数除法与取模
来源：http://hz.hysaishi.cn/gtgeedqhia.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zycfv.cn/gtgjoqzytm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yonumen.top/gttetpngap.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtwedwteim.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgufenzy.top/gtiuwutcjj.html

Java: 7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gtvyhihdga.html

Go:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtxjzycrdw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtjrhfnfnr.html

C#:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtpsndoolt.html

[A06] 字符串转数字
来源：http://hz.cucudq.cn/gtcqdkjxgx.html

Py:   int("42"); float("3.14")
来源：http://hz.52xcode.cn/gtxykedsud.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinyuanbaomall.cn/gtafcgakwu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xinyue.icu/gtgbsrhwhc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cashguo.top/gtvnkmrear.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.quarkkingdee.top/gtrqaxzsdf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gzhubu.top/gtqnrrmuya.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.aibaodan.cn/gtldupashj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ydjk.org.cn/gtzuldubiz.html

[A07] 数字转字符串
来源：http://hz.pycfn.com/gtolrhhfzi.html

Py:   str(42)
来源：http://hz.shzxlz.cn/gthdhodwnb.html

PHP:  (string) 42; strval(42)
来源：http://hz.yangfankeji.com/gtqaxvxalx.html

JS:   String(42); (42).toString()
来源：http://hz.yuanzhike.top/gtvltduxjp.html

TS:   String(42)
来源：http://hz.xziqi.cn/gtwarcjxlk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nwbrower.top/gtmtubsegz.html

Go:   strconv.Itoa(42)
来源：http://hz.hysaishi.cn/gtjvmmevcq.html

Ruby: 42.to_s
来源：http://hz.vqdsnc.cn/gtgvkratlh.html

C#:   42.ToString()
来源：http://hz.xylfe.cn/gtgvwclhjc.html

[A08] 取整与四舍五入
来源：http://hz.daxiang520.top/gtswhqonxl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.guowangkeji.top/gtgwnummnn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xinyue.icu/gtwihpifpk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.chenzaomai.com/gtcndbhdjk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yongpay.top/gtijzszlvk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gtywvxlhgp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.aizwys.cn/gtupxcjdpm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.hnxiangtu.top/gtpdghnwqu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jlsjyb.cn/gtgftfvxjo.html

[A09] 绝对值与最大最小值
来源：http://hz.52xcode.cn/gtfitxhpsf.html


<!-- 参考信息 -->