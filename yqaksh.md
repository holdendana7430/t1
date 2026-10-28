代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.shanyushiyangtech.top/gtukpmteog.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pengpengdd.cyou/gttdxmujwx.html

[U68] PHP：PDO 连接
来源：http://hz.gotoacloud.top/gteyyxjeyv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pycfn.com/gtmlfzlwxf.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtnkyubmke.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zycfv.cn/gtqzldzovc.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtfxartnym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jiagoushi.top/gtwxfcyfvg.html

[U71] PHP：抛出异常
来源：http://hz.xylfe.cn/gtpdlzsjqg.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtgnxjrjjj.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtweyerpbh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.vqdsnc.cn/gtxweemvey.html

[U73] PHP：读取 ini 配置
来源：http://hz.xuetiantiany.cn/gtmngizula.html

parse_ini_file("config.ini", true)
来源：http://hz.zhiwuduotai.top/gtujvacaso.html

[U74] PHP：读取环境变量
来源：http://hz.sufxvd.cn/gtaqrwhqzx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.havefunace.top/gtekagbdvy.html

[U75] PHP：依赖注入
来源：http://hz.ywan-chungtsiang.top/gtygilqyof.html

composer require psr/container
来源：http://hz.svipenyu.cn/gtcsnpwzgt.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtwmkmceii.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tian-w.cn/gtkedfbbwr.html

[U77] PHP：模板渲染
来源：http://hz.birdmap.top/gtqwuenpmk.html

composer require twig/twig
来源：http://hz.gogol.net.cn/gthyvqiigd.html

[U78] PHP：单元测试
来源：http://hz.hnqzz.top/gtycfvesgb.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigfzy.top/gtqqujhfcj.html

[U79] PHP：静态分析
来源：http://hz.birdmap.top/gtcrnvfbwh.html

composer require --dev phpstan/phpstan
来源：http://hz.meibo888.top/gtsbnimcpi.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gtmpquicax.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhongyouzk.top/gtsfzmcfnn.html

[U81] JS：初始化项目
来源：http://hz.yueranfly.top/gtariflvee.html

npm init -y;  npm i express
来源：http://hz.zhiwuduotai.top/gteqjbejuf.html

[U82] JS：package.json 脚本
来源：http://hz.cucudq.cn/gtlduckqza.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gthenuveoc.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtuabuhncn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtzqrifdqb.html

[U84] JS：CommonJS 写法
来源：http://hz.hywenlv.cn/gteqrarvom.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xingfuxueyuan.xyz/gtbhfjpnfs.html

[U85] JS：可选链
来源：http://hz.yj20258888.top/gtpfqimbzf.html

a?.b?.c
来源：http://hz.cdnleiting.top/gtvysusyiy.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtvrntzbnz.html

a ?? b
来源：http://hz.52xcode.cn/gtxoductsb.html

[U87] JS：解构默认值
来源：http://hz.pengpengdd.cyou/gtzsplioex.html

const { a = 1, b = 2 } = obj;
来源：http://hz.haohaochexian.top/gtwpungjel.html

[U88] JS：对象展开合并
来源：http://hz.zhiwuduotai.top/gthoifoylo.html

{ ...a, ...b }
来源：http://hz.ehwqpu.com/gtiypiuvtw.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtyhxmppcy.html

[...new Set(arr)]
来源：http://hz.yongpay.top/gtrtkjgnfj.html

[U90] JS：数字数组排序
来源：http://hz.chenjidiqi.icu/gtonucyoji.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtnkceyqud.html

[U91] JS：对象键值遍历
来源：http://hz.svipenyu.cn/gtprszgpzh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.bjfxy.top/gtukmhirco.html

[U92] JS：深拷贝
来源：http://hz.cdnleiting.top/gtwetmeslr.html

structuredClone(obj)
来源：http://hz.gotoacloud.top/gtwdlmbsiz.html

[U93] JS：模板字符串
来源：http://hz.xuetiantiany.cn/gtniinzlgd.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtntnumdpg.html

[U94] JS：箭头函数
来源：http://hz.gaohongyu789.top/gtfhqafgxz.html

const double = x => x * 2;
来源：http://hz.hammf.cn/gtdysqgqpl.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtolawhrzw.html

new Promise((resolve, reject) => {})
来源：http://hz.iojbl.cn/gtarkkfgpu.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigufen.top/gtasjshpzn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gthbpoxntu.html

[U97] JS：并发请求
来源：http://hz.mhx1999.top/gtqiapbjsb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtfpqmxyxy.html

[U98] JS：fetch 带 JSON
来源：http://hz.birdmap.top/gtluoysdbk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.snrcjt.cn/gtfstmxkxu.html

[U99] JS：事件监听
来源：http://hz.wangdashe.top/gtszvfoxfs.html

el.addEventListener("click", e => {})
来源：http://hz.tianlin.xyz/gtamhkmodi.html

[U100] JS：DOM 查询
来源：http://hz.ydjk.org.cn/gtayohcizr.html

document.querySelector(".item")
来源：http://hz.ydjk.org.cn/gtifbvhtdd.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtrpvwxruv.html

el.classList.toggle("active")
来源：http://hz.pycfn.com/gtazosvrlt.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtoliztjtd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gtrsjarvhc.html

[U103] JS：定时器
来源：http://hz.jinqigfzy.top/gtqmwlmltf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hnqzz.top/gtjrgzmqph.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtqyqzsxis.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtbgvydzqu.html

[U105] JS：节流
来源：http://hz.ywan-chungtsiang.top/gtpanuklrb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgfzy.top/gtcnhxxinh.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtrmlsmlbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guowangkeji.top/gtvpkiumws.html

[U107] JS：数字千分位
来源：http://hz.sweek.top/gtdhegeuqr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xuetiantiany.cn/gtmortkngb.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gtqxiphuxj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.bjfxy.top/gtfwenqsbh.html

[U109] JS：数组分组
来源：http://hz.nanxuanxn.top/gtpnolsmtt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtonipnfjn.html

[U110] JS：数组分块
来源：http://hz.wangshuangyany.cn/gtfqswaslv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenlongwang.top/gtiwtqshij.html

[U111] JS：对象转 Map
来源：http://hz.yj20258888.top/gtudfsdrak.html

new Map(Object.entries(obj))
来源：http://hz.dashuyun.cn/gttjrlogof.html

[U112] JS：字符串补位
来源：http://hz.dashuyun.cn/gtkfisqfkc.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtgfwhktws.html

[U113] JS：正则替换全部
来源：http://hz.hysaishi.cn/gtrkglsmyg.html

s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtrijcpxgw.html

[U114] JS：JSON 深比较
来源：http://hz.sxryk.cn/gtolbrnmud.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtsirtbmxh.html

[U115] JS：生成 UUID
来源：http://hz.kuanghao11.cn/gtgffonkxc.html

crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtrlumlkjm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.svipenyu.cn/gtlaxciqfb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhongyouzk.top/gtlwrfkdrl.html

[U117] JS：单元测试
来源：http://hz.jinqigfzy.top/gteoapbofw.html

npm i -D vitest;  npx vitest
来源：http://hz.hnxiangtu.top/gtwopfrgyt.html

[U118] JS：开发服务器
来源：http://hz.yongpay.top/gtngckqgep.html

npm i -D vite;  npx vite
来源：http://hz.tianlin.xyz/gtmaausigt.html

[U119] JS：生产构建
来源：http://hz.ehwqpu.com/gtkuaakchs.html

npx vite build
来源：http://hz.52xcode.cn/gtrvzkemjm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sysykeji.top/gtcwwcpnux.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gtdajgwzda.html

================================================================================
来源：http://hz.ppjwa.cn/gtpqabkkgo.html

统计汇总
来源：http://hz.zhijiandao.cn/gtenkrdiqg.html

================================================================================
来源：http://hz.9152youxi.cn/gtwinltpvc.html

按语言统计（条）：
来源：http://hz.pycfn.com/gtwvfroxgo.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtbynisubq.html

PHP ............ 252
来源：http://hz.xingfuxueyuan.xyz/gteogutzgg.html

JavaScript ..... 252
来源：http://hz.smart0.xyz/gtosycjpfs.html

TypeScript ..... 212
来源：http://hz.dianchejie.cn/gtlculvytv.html

Java ........... 212
来源：http://hz.yangfankeji.com/gtbxlveyji.html

Go ............. 212
来源：http://hz.316326.xyz/gtytjggzar.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtrvabcpaw.html

C# ............. 212
来源：http://hz.yj20258.top/gtsekwdjpe.html

C .............. 30
来源：http://hz.mhx1999.top/gtbguknvvu.html

C++ ............ 30
来源：http://hz.shanyushiyangkeji.top/gtjgrwsmoa.html

SQL ............ 90
来源：http://hz.havefunace.top/gtgphsudfe.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtakvxgkhm.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtpofdsrec.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtghavglkp.html

Lua ............ 10
来源：http://hz.jiagoushi.top/gtzybbfqbq.html

Perl ........... 10
来源：http://hz.jianghu66.top/gtwdhqrbfk.html

Scala .......... 10
来源：http://hz.havefunace.top/gtnxsrbhmw.html

------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtailivxvq.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtxdhilkcu.html

按章节统计：
来源：http://hz.redwolf501.top/gtoglqvoly.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cqqwz.cn/gtrwjdtslp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yongpay.top/gtobvomxhg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtuvbneuze.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtekuagkhd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sxryk.cn/gtujaozdpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxinkj.top/gttlkpkjeh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtytvofimu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnxiangtu.top/gttyqkcwzx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtxesfsyvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtaobjdxfq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtqjxetthj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtfvtnlfel.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtahzkzhxe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gtsxruhgzh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nwbrower.top/gtiqfczknu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gthivazzjo.html

Q SQL 专题                              90
来源：http://hz.gaohongyu789.top/gtkgomeeju.html

R Bash 专题                             80
来源：http://hz.shuidangran.top/gtirbphfyl.html

S C / C++ 专题                          60
来源：http://hz.gogol.net.cn/gtnymfagos.html

T 其他语言补充                          60
来源：http://hz.shzxlz.cn/gtmoheetqx.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gttzdogoqn.html

------------------------------------
来源：http://hz.svipenyu.cn/gtvaravllr.html

合计                                  2106 条
来源：http://hz.gotoacloud.top/gtycvfxagg.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtefqcpbhw.html

使用提醒
来源：http://hz.mhx1999.top/gtsrkdooyf.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtulckqwto.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigufen.top/gtjrhghnhq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.wangshuangyany.cn/gtmrrqdjly.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.andypj.xyz/gtkddnzijx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtnjbtoybo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtnqfbbdiy.html

—— 文件结束 ——
来源：http://hz.xylfe.cn/gtaycnychg.html

================================================================================
来源：http://hz.ppjwa.cn/gtygqbuuex.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtoakbrvfg.html

Common Programming Examples Cheat Book
来源：http://hz.jqgfzy.top/gtajcrudfm.html

================================================================================
来源：http://hz.zhengqikj.top/gtgatzpovl.html

【收录内容】
来源：http://hz.cashguo.top/gtrekzzzsr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jqgfzy.top/gtaydlspex.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangtech.top/gtralgeyex.html

SQL · Bash · C · C++
来源：http://hz.zhongyouzk.top/gtdsvnfnej.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhaomingkeji.xyz/gtnrkrmpnx.html

【使用说明】
来源：http://hz.ppjwa.cn/gtwqjxugac.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gthlckybru.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.feifeiyinyue.top/gterjrjpia.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.316326.xyz/gtpslyyxkb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gaohongyu789.top/gtmnokltpo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtxgepiokc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gttjwaubbw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangdashe.top/gtygjvbpuo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yangfankeji.com/gtxedpszlk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gogol.net.cn/gtljumoool.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ydjk.org.cn/gtgeibkfeb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yuxming.cn/gtotstascc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhongyouzk.top/gthtxvofoo.html

【文件统计】
来源：http://hz.bjfxy.top/gtbigklagx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gaohongyu789.top/gtusiodwzb.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtuactaulk.html

目  录
来源：http://hz.ivvv.top/gtqinucqoz.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtivaivvlk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtoqvaayrm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yongpay.top/gtpkwoxqsc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtfozepezq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinghuilouyu.cn/gtzjieobkk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xingfuxueyuan.xyz/gtjppjbbyw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gttnrjiypw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.sweek.top/gtxmermonn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtwogwwpxy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtgjkbbnbq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jiagoushi.top/gtxnvedwsn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtuvussdvk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtcrykujzl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtbhueuitc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shangyingyoupin.top/gthkazhgyr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.wangdashe.top/gturlmdevl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtgvldzdfw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258888.top/gtcsviajdi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hysaishi.cn/gtuczztycw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xylfe.cn/gtvrjzwdye.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtgssfzbal.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtxjnldzdu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtiwnbkrlj.html

A. 基础语法与类型
来源：http://hz.bjfxy.top/gtrysilvvj.html

================================================================================
来源：http://hz.shuidangran.top/gtpqtjooes.html

[A01] Hello World
来源：http://hz.haohaochexian.top/gtnnwcanfk.html

Py:   print("Hello, World!")
来源：http://hz.yj20258.top/gtszmtqebb.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxinkj.top/gtmmwcszhm.html

JS:   console.log("Hello, World!");
来源：http://hz.haohaochexian.top/gttfnotexe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jlsjyb.cn/gtwnruvmpz.html

Java: System.out.println("Hello, World!");
来源：http://hz.snrcjt.cn/gtrmkxvmql.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gterindvuu.html

Ruby: puts "Hello, World!"
来源：http://hz.zhaomingkeji.xyz/gtjfngbrtm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinqigufen.top/gtmifydixn.html

[A02] 变量声明与赋值
来源：http://hz.jinghuilouyu.cn/gtinubnmxm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yangfankeji.com/gtckcjbyzm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtpdeybyfs.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xziqi.cn/gtdflslepl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shzxlz.cn/gtjrngzdii.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtcqjrmoqv.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhaomingkeji.xyz/gtgljhxynl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.havefunace.top/gtsgnwcuns.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.redwolf501.top/gthzuiuinm.html

[A03] 常量定义
来源：http://hz.yangfankeji.com/gtgdmihdkw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yongpay.top/gtgqtauviq.html

PHP:  const PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtkyfpfait.html

JS:   const PI = 3.14159;
来源：http://hz.cdnleiting.top/gtoihctzfc.html

TS:   const PI: number = 3.14159;
来源：http://hz.tanke756.top/gtvvdqcqks.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtlaouojak.html

Go:   const PI = 3.14159
来源：http://hz.jyoumei.cn/gtuejnlapd.html

Ruby: PI = 3.14159
来源：http://hz.jinqigufen.top/gtlkciqpsq.html

C#:   const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtfcwqlrid.html

[A04] 判断变量类型
来源：http://hz.xinyue.icu/gtfhzfvwhc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.meibo888.top/gtpvjwzwsn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.wangdashe.top/gtzqgefilq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yuanzhike.top/gtygautoym.html

TS:   typeof x; x instanceof Date
来源：http://hz.kuanghao11.cn/gtfbmecaic.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.meibo888.top/gtxlivvtwh.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj20258.top/gtvoyhyfxw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jyoumei.cn/gtaaprvero.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj202588.top/gtfsweweom.html

[A05] 整数除法与取模
来源：http://hz.gaohongyu789.top/gtyhblngds.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.vqdsnc.cn/gtlitqlzxg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fengsongda.top/gtyvhkayns.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtlsvtorbt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daria6918.cn/gtiuzwessh.html

Java: 7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtqgrgywmj.html

Go:   7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtgvocucdl.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtvsxvtsee.html

C#:   7 / 2; 7 % 2
来源：http://hz.dianchejie.cn/gtzyxayvgh.html

[A06] 字符串转数字
来源：http://hz.yangfankeji.com/gtebfpqmzw.html

Py:   int("42"); float("3.14")
来源：http://hz.smart0.xyz/gtxbpuimqb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jianghu66.top/gtintzjdas.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.316326.xyz/gtiuugzsom.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuetiantiany.cn/gtsmrydpnv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hongshengwenyu.top/gtxrxyvmbt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ehwqpu.com/gtwuqtlnhj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nanxuanxn.top/gtynzvmzuy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.52xcode.cn/gttbisrnob.html

[A07] 数字转字符串
来源：http://hz.wangshuangyany.cn/gtbjjhgdkz.html

Py:   str(42)
来源：http://hz.tian-w.cn/gtombjjysb.html

PHP:  (string) 42; strval(42)
来源：http://hz.smart0.xyz/gthfjbvmtr.html

JS:   String(42); (42).toString()
来源：http://hz.xuanzx.com/gtjmktrqon.html

TS:   String(42)
来源：http://hz.andypj.xyz/gtrxruuqfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.guowangkeji.top/gtooawiksr.html

Go:   strconv.Itoa(42)
来源：http://hz.c1oappe.top/gtrtttinxb.html

Ruby: 42.to_s
来源：http://hz.hammf.cn/gtmimbvxrh.html

C#:   42.ToString()
来源：http://hz.havefunace.top/gtqucnwkwt.html

[A08] 取整与四舍五入
来源：http://hz.cheryme.top/gtyfmcbcji.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.quarkkingdee.top/gtexhzybog.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gotoacloud.top/gtqrkazqtu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhengqikj.top/gtsdzlcpvr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cheryme.top/gtinpqjizq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.haohaochexian.top/gtpdrgobkf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhixingplan.top/gtazmfnnwg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sufxvd.cn/gtrexfluxn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.guannengcc.top/gtlhusqqwp.html

[A09] 绝对值与最大最小值
来源：http://hz.sxryk.cn/gtvmshpnmi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenjidiqi.icu/gtxxdhbsgu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinqigfzy.top/gttlugvbdn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xziqi.cn/gtaqhjfvtk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtikkeolhz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.haohaochexian.top/gtiwnbmatg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.feifeiyinyue.top/gtcujgzriw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhaomingkeji.xyz/gtkhlcfxck.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shzxlz.cn/gtshgnygjf.html

[A10] 生成随机数
来源：http://hz.chenlongwang.top/gtzymcdyth.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ybcxt.top/gtiyxotrbb.html

PHP:  random_int(1, 100);
来源：http://hz.zhoulong.xyz/gtsyxrevxi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj20258.top/gtopnfmbda.html


<!-- 参考信息 -->