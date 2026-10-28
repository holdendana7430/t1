代发 wailian999

[U61] PHP：正则
来源：http://hz.tianlin.xyz/gtlntnhzqw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtkibzdoiu.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtkhrbzjqi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuanzx.com/gtdxzdpyxs.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtdtnznoss.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnqzz.top/gttafspmyy.html

[U64] PHP：目录遍历
来源：http://hz.ybcxt.top/gtyclaherd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtfauaqxmf.html

[U65] PHP：会话
来源：http://hz.ybcxt.top/gtibmosuap.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gtmyktxwwl.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gtsehlhmba.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jyoumei.cn/gtumcckpms.html

[U67] PHP：处理文件上传
来源：http://hz.sysykeji.top/gtpqoucmmn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhengqikj.top/gtijpcnnwp.html

[U68] PHP：PDO 连接
来源：http://hz.cqqwz.cn/gtjzxkjyuy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258888.top/gtbkmhrcbj.html

[U69] PHP：PDO 预处理
来源：http://hz.hywenlv.cn/gtwcwrpnvp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtjxagbxzx.html

[U70] PHP：PDO 事务
来源：http://hz.ehwqpu.com/gtqnokfbcy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinqigufen.top/gtefkwnglb.html

[U71] PHP：抛出异常
来源：http://hz.quarkkingdee.top/gtspwtppdc.html

throw new RuntimeException("失败", 500);
来源：http://hz.52xcode.cn/gtljlxbcmq.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gtcwwtqial.html

error_log("失败: " . $e->getMessage());
来源：http://hz.quarkkingdee.top/gtgaknlfbt.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gtczxbsqjq.html

parse_ini_file("config.ini", true)
来源：http://hz.kuanghao11.cn/gtbajnxhqd.html

[U74] PHP：读取环境变量
来源：http://hz.yvedp.cn/gtpweuxxhs.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuetiantiany.cn/gtmtibffes.html

[U75] PHP：依赖注入
来源：http://hz.yuxming.cn/gtddzqyoca.html

composer require psr/container
来源：http://hz.yonumen.top/gtfrydvsfy.html

[U76] PHP：简单路由
来源：http://hz.jianghu66.top/gttihmbplf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gzhubu.top/gtoaikqqbw.html

[U77] PHP：模板渲染
来源：http://hz.zdqjudy.top/gtiwfloazi.html

composer require twig/twig
来源：http://hz.andypj.xyz/gtkdomjflq.html

[U78] PHP：单元测试
来源：http://hz.hywenlv.cn/gttxyujhlg.html

composer require --dev phpunit/phpunit
来源：http://hz.yanxiufei.cn/gtoafljkds.html

[U79] PHP：静态分析
来源：http://hz.iojbl.cn/gtyiwlhtze.html

composer require --dev phpstan/phpstan
来源：http://hz.meibo888.top/gteizamwfb.html

[U80] PHP：代码规范修复
来源：http://hz.ybcxt.top/gtkbxebnfj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jianghu66.top/gtqwgwqkkt.html

[U81] JS：初始化项目
来源：http://hz.hongshengwenyu.top/gtmwdfqnim.html

npm init -y;  npm i express
来源：http://hz.zhiwuduotai.top/gttfqdhrwv.html

[U82] JS：package.json 脚本
来源：http://hz.ybcxt.top/gtvpnvdpbt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yuxming.cn/gtbepcipbx.html

[U83] JS：ES Module 导入导出
来源：http://hz.shanyushiyangkeji.top/gthrouggll.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cdnleiting.top/gttemwkqme.html

[U84] JS：CommonJS 写法
来源：http://hz.meibo888.top/gtdvxfuipn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nanxinkj.top/gtgbjnkwjt.html

[U85] JS：可选链
来源：http://hz.nanxinkj.top/gtvptvphst.html

a?.b?.c
来源：http://hz.daxiang520.top/gtszddtxlw.html

[U86] JS：空值合并
来源：http://hz.dianchejie.cn/gtptbfsnbs.html

a ?? b
来源：http://hz.wangdashe.top/gtjtmtcxyr.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangtech.top/gtxikjvkql.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuanzhike.top/gtvmnxwspz.html

[U88] JS：对象展开合并
来源：http://hz.svipenyu.cn/gtfdplflkv.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtlafwqqyl.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gtdvooyfep.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtvbovajmo.html

[U90] JS：数字数组排序
来源：http://hz.haohaochexian.top/gtmszukeze.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtrudxracm.html

[U91] JS：对象键值遍历
来源：http://hz.aizwys.cn/gtmetvtihv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtrfwrcvbn.html

[U92] JS：深拷贝
来源：http://hz.yuxming.cn/gtdiopgrdl.html

structuredClone(obj)
来源：http://hz.ydzc1.top/gtaeavrxfm.html

[U93] JS：模板字符串
来源：http://hz.chenzaomai.com/gtmpqbwhva.html

`共 ${n} 条`
来源：http://hz.hfpthk.cn/gtiyivcrip.html

[U94] JS：箭头函数
来源：http://hz.jinqigufen.top/gterejmhpd.html

const double = x => x * 2;
来源：http://hz.iojbl.cn/gtpwfjxuvd.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtcflplrro.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtbwsqzzjd.html

[U96] JS：async/await 与异常
来源：http://hz.svipenyu.cn/gtayumaxos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtnjazrzce.html

[U97] JS：并发请求
来源：http://hz.jqgufenzy.top/gtjktwmgdw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtjoqkgiuq.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtabzwxlvl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxuanxn.top/gtqarmlhms.html

[U99] JS：事件监听
来源：http://hz.svipenyu.cn/gtdfhpluem.html

el.addEventListener("click", e => {})
来源：http://hz.xylfe.cn/gtvhimjyra.html

[U100] JS：DOM 查询
来源：http://hz.52xcode.cn/gtoglhsvev.html

document.querySelector(".item")
来源：http://hz.xingfuxueyuan.xyz/gtrbncourk.html

[U101] JS：classList 操作
来源：http://hz.jianghu66.top/gtffktjvdz.html

el.classList.toggle("active")
来源：http://hz.jinqigufen.top/gtycbgvaju.html

[U102] JS：本地存储
来源：http://hz.yj20258888.top/gtvwxhfkcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ehwqpu.com/gtkygypsjg.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtapqvattw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.redwolf501.top/gtvyuzrfqq.html

[U104] JS：防抖
来源：http://hz.nanxuanxn.top/gtniyfoljk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gthewagzfw.html

[U105] JS：节流
来源：http://hz.nanxuanxn.top/gtyrdxfeth.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhoulong.xyz/gtvtgmsszo.html

[U106] JS：日期格式化
来源：http://hz.guowangkeji.top/gtgxbynpfc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cdnleiting.top/gttayrmbnq.html

[U107] JS：数字千分位
来源：http://hz.bjfxy.top/gtmxvxabiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gteanydqkf.html

[U108] JS：随机整数
来源：http://hz.gotoacloud.top/gthmbgsogl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shangyingyoupin.top/gtixeacrdy.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtptftbcvi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.bjfxy.top/gtgdvlhfqc.html

[U110] JS：数组分块
来源：http://hz.xuanzx.com/gtbhjyadvp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hammf.cn/gthixukjny.html

[U111] JS：对象转 Map
来源：http://hz.xuetiantiany.cn/gtuxovohpo.html

new Map(Object.entries(obj))
来源：http://hz.yongpay.top/gtnnowwlgk.html

[U112] JS：字符串补位
来源：http://hz.yvedp.cn/gtajitfoks.html

"7".padStart(3, "0")
来源：http://hz.xylfe.cn/gthvnshkuo.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gttmgrgjlj.html

s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtfyzsajwb.html

[U114] JS：JSON 深比较
来源：http://hz.jinyuanbaomall.cn/gtgvrlkuez.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtpmnuwasd.html

[U115] JS：生成 UUID
来源：http://hz.jinqigfzy.top/gtacizdvur.html

crypto.randomUUID()
来源：http://hz.iojbl.cn/gtldfjwpxy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yonumen.top/gtyoejxzgd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ywan-chungtsiang.top/gtadkaysdv.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gthaxbqsfe.html

npm i -D vitest;  npx vitest
来源：http://hz.hnqzz.top/gthjrpzrwh.html

[U118] JS：开发服务器
来源：http://hz.hongshengwenyu.top/gthefseayy.html

npm i -D vite;  npx vite
来源：http://hz.daxiang520.top/gtzyarpxhh.html

[U119] JS：生产构建
来源：http://hz.ydjk.org.cn/gtxopojlmk.html

npx vite build
来源：http://hz.nanxinkj.top/gtsdclizjz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.snrcjt.cn/gtmrsbhvnh.html

import.meta.env.VITE_API_URL
来源：http://hz.hfpthk.cn/gtghsxaljt.html

================================================================================
来源：http://hz.jianghu66.top/gtpszlmnnf.html

统计汇总
来源：http://hz.zhijiandao.cn/gtguvqtaqi.html

================================================================================
来源：http://hz.daria6918.cn/gtsgmcerhi.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gtrqjyvvvo.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gthqvvkhux.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtswpzwafb.html

JavaScript ..... 252
来源：http://hz.sysykeji.top/gtudbpexpo.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtmuyvpqnb.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtqoreritk.html

Go ............. 212
来源：http://hz.yvedp.cn/gtxkuyksbm.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtvtrynnrq.html

C# ............. 212
来源：http://hz.fengsongda.top/gtckwryydz.html

C .............. 30
来源：http://hz.shanyushiyangkeji.top/gtykvmxeca.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gttkoponvu.html

SQL ............ 90
来源：http://hz.meibo888.top/gtdfwhcmob.html

Bash ........... 80
来源：http://hz.quarkkingdee.top/gtnydshoip.html

Kotlin ......... 15
来源：http://hz.hywenlv.cn/gtxasoehmq.html

Swift .......... 15
来源：http://hz.zycfv.cn/gttvcmurex.html

Lua ............ 10
来源：http://hz.haohaochexian.top/gtuaoknplc.html

Perl ........... 10
来源：http://hz.bjfxy.top/gtyczreybj.html

Scala .......... 10
来源：http://hz.jqgufenzy.top/gttvchubgu.html

------------------------------------
来源：http://hz.hammf.cn/gtdmhkrrby.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtwrnnzwfy.html

按章节统计：
来源：http://hz.shuidangran.top/gtlonvtgdw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtqmqsufud.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtvyhgldnf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtlyssqbyn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gtvcyrsuba.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jqgufenzy.top/gtqeukclzl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtrnhkrnet.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtgwkoeqtg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtneiyplee.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtmacharwa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258.top/gttzftdulu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtmlvvzufx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtycvvatgw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtpuaanfxb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gttnasezei.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258888.top/gtbikftzku.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtgjwqnoqz.html

Q SQL 专题                              90
来源：http://hz.xylfe.cn/gtsrnjutub.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gthfbhzzib.html

S C / C++ 专题                          60
来源：http://hz.gotoacloud.top/gtbfqsjwhm.html

T 其他语言补充                          60
来源：http://hz.cashguo.top/gtznafgdon.html

U 高频实用片段                         120
来源：http://hz.yonumen.top/gtavljagxw.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtyenilhvo.html

合计                                  2106 条
来源：http://hz.jinqigufen.top/gtfkxgjgvt.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtsnmluzwp.html

使用提醒
来源：http://hz.jinqigfzy.top/gtcwglsfnr.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtcpvduhne.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.snrcjt.cn/gtdjxtvsfg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sweek.top/gtqmaanmfw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.bjfxy.top/gtcwkstddj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gzhubu.top/gtzazrchou.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.snrcjt.cn/gtupxzdlik.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtnnaukagz.html

================================================================================
来源：http://hz.svipenyu.cn/gtfyqwdoda.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtpryldavd.html

Common Programming Examples Cheat Book
来源：http://hz.meibo888.top/gtmbhavgsl.html

================================================================================
来源：http://hz.pycfn.com/gtombcbdys.html

【收录内容】
来源：http://hz.yongpay.top/gtexzifvst.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.fzhhl.top/gtlrwttffj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj20258888.top/gthbgbdgez.html

SQL · Bash · C · C++
来源：http://hz.sufxvd.cn/gtamhpptnz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydjk.org.cn/gtegvubpux.html

【使用说明】
来源：http://hz.sysykeji.top/gtedfsjmot.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgfzy.top/gtphgxoabn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinghuilouyu.cn/gtmygvfzuc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sufxvd.cn/gtolxkvyyk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yueranfly.top/gtucgdkdxs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gzhubu.top/gtupiqwxdd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gaohongyu789.top/gtgampyusv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnqzz.top/gtcdgujjxg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtlrllwkou.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gzhubu.top/gtbkhywuld.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtdpebekmi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yj20258888.top/gtcfxfatgo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sysykeji.top/gtuiwdyloq.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtbptqxzhj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtdwgrtura.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtgagaylfm.html

目  录
来源：http://hz.sweek.top/gtjjarntbc.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtculcvwhj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gtykhcmjaq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.mhx1999.top/gtazyazoyb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gthqceunfi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.meibo888.top/gtkcenaesd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guowangkeji.top/gtdvrhuymn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.316326.xyz/gtppniyufp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.dianchejie.cn/gtfkcupxlf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtyvfeiwkd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtpxrlwamb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhixingplan.top/gtmmouitpl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtwcmsmxxg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtgfnwjhpd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtioqwfzji.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtpwmenlah.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.meibo888.top/gtkexjkmpm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtnehvsocz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yuanzhike.top/gtecqftvty.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtlxzesyfg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shuidangran.top/gtqevcaeyg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtaikxkkgh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtyuiewmly.html

================================================================================
来源：http://hz.c1oappe.top/gtqdbrcjmr.html

A. 基础语法与类型
来源：http://hz.hnxiangtu.top/gtbekznsne.html

================================================================================
来源：http://hz.xinyue.icu/gtjfgmvwjk.html

[A01] Hello World
来源：http://hz.jianghu66.top/gticmrstrj.html

Py:   print("Hello, World!")
来源：http://hz.ybcxt.top/gtzoudxsch.html

PHP:  echo "Hello, World!";
来源：http://hz.havefunace.top/gtigugspbh.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258.top/gtzbjrjxhn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.birdmap.top/gtfnepxqof.html

Java: System.out.println("Hello, World!");
来源：http://hz.sysykeji.top/gtlhihfqtg.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sxryk.cn/gtxvcncodn.html

Ruby: puts "Hello, World!"
来源：http://hz.birdmap.top/gttchfxrul.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hywenlv.cn/gtvtljsypf.html

[A02] 变量声明与赋值
来源：http://hz.yonumen.top/gtotzkmgzo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuanzx.com/gtldrukllr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jiagoushi.top/gtnbodpscr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sxryk.cn/gtwcfhflzx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.iojbl.cn/gtnwutaqyf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.vqdsnc.cn/gtftfrtflm.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhijiandao.cn/gtddrvzkpm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jianghu66.top/gtoojjkjtx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.iojbl.cn/gtzobtmxju.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtgbymissn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hnqzz.top/gtbrgtqlwp.html

PHP:  const PI = 3.14159;
来源：http://hz.gotoacloud.top/gtchtvzrzj.html

JS:   const PI = 3.14159;
来源：http://hz.xziqi.cn/gtszbhhovm.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinghuilouyu.cn/gttzqbrtwy.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtkgoggbaj.html

Go:   const PI = 3.14159
来源：http://hz.sxryk.cn/gtznluqoau.html

Ruby: PI = 3.14159
来源：http://hz.hnxiangtu.top/gtawhkcqyz.html

C#:   const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtccjrtdcb.html

[A04] 判断变量类型
来源：http://hz.sxryk.cn/gtlpgkicqo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ppjwa.cn/gtxixqusfl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zdqjudy.top/gtrleaerdg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yvedp.cn/gtyawjvjqd.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtjrrrjymv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.dianchejie.cn/gttfgprmjl.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.haohaochexian.top/gtsgdwedlb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tanke756.top/gtwntvtwkq.html

C#:   x.GetType().Name; x is int
来源：http://hz.aizwys.cn/gtxbwqepzj.html

[A05] 整数除法与取模
来源：http://hz.xuanzx.com/gtazvfnuxi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhengqikj.top/gtbutlzask.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yonumen.top/gtilpwivip.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gtovtfuntl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.kuanghao11.cn/gtunexfwke.html

Java: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtybzlfjhi.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtbkrornxm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gtxirmxmaz.html

C#:   7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtimimbsko.html

[A06] 字符串转数字
来源：http://hz.tianlin.xyz/gtvbtvrbaj.html

Py:   int("42"); float("3.14")
来源：http://hz.havefunace.top/gteuivswdu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.pengpengdd.cyou/gtkarnedia.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.birdmap.top/gttuknzzpq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtfgweslsy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinqigfzy.top/gtlyfwzcvh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cucudq.cn/gtivurmmpj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.dashuyun.cn/gtrnxytyge.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gaohongyu789.top/gtittkxtqg.html

[A07] 数字转字符串
来源：http://hz.shanyushiyangtech.top/gtgyggkbmq.html

Py:   str(42)
来源：http://hz.xuetiantiany.cn/gtvnnabfji.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj20258.top/gtparzolya.html

JS:   String(42); (42).toString()
来源：http://hz.xinyue.icu/gtlrzscbwg.html

TS:   String(42)
来源：http://hz.cdnleiting.top/gthfqikxsn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhijiandao.cn/gtviyevmko.html

Go:   strconv.Itoa(42)
来源：http://hz.meibo888.top/gtsojktcxn.html

Ruby: 42.to_s
来源：http://hz.aibaodan.cn/gtdlghcleg.html

C#:   42.ToString()
来源：http://hz.ydjk.org.cn/gtuclzrwoi.html

[A08] 取整与四舍五入
来源：http://hz.wangshuangyany.cn/gtjzqajgqx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xuanzx.com/gtetnckkkp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xylfe.cn/gtodzyioam.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zycfv.cn/gtclduswju.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.gzhubu.top/gtawjkdghe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtdjzsmmbv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jlsjyb.cn/gthytzeikn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.haohaochexian.top/gtvxyaxvyg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yuxming.cn/gtezhothjx.html

[A09] 绝对值与最大最小值
来源：http://hz.aizwys.cn/gtkwjecxrc.html


<!-- 参考信息 -->