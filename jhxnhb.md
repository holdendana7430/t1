代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gtqrjrgfyb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.birdmap.top/gtsflegwbf.html

[U68] PHP：PDO 连接
来源：http://hz.pycfn.com/gtgpqeyzmr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydjk.org.cn/gtkvmkccbn.html

[U69] PHP：PDO 预处理
来源：http://hz.havefunace.top/gtbcrkvnge.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yueranfly.top/gtzlmldexg.html

[U70] PHP：PDO 事务
来源：http://hz.yvedp.cn/gtflbyevrn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtfukpkovd.html

[U71] PHP：抛出异常
来源：http://hz.shangyingyoupin.top/gtiqukeqry.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtjokouyxd.html

[U72] PHP：写错误日志
来源：http://hz.zhengqikj.top/gtkmtjjboe.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenjidiqi.icu/gticlvzpws.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinyuanbaomall.cn/gtfvwdyyhy.html

parse_ini_file("config.ini", true)
来源：http://hz.shanyushiyangtech.top/gtkkjgnrar.html

[U74] PHP：读取环境变量
来源：http://hz.0kj1m.cn/gtktjxmbhs.html

getenv("APP_ENV") ?: "production"
来源：http://hz.snrcjt.cn/gtljtufvlx.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtsrjtpovq.html

composer require psr/container
来源：http://hz.shanyushiyangtech.top/gtkiqjhetd.html

[U76] PHP：简单路由
来源：http://hz.birdmap.top/gtemqszlfx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xuanzx.com/gtsslgxlsc.html

[U77] PHP：模板渲染
来源：http://hz.xziqi.cn/gtnexkegoo.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gttuommdyu.html

[U78] PHP：单元测试
来源：http://hz.jianghu66.top/gtchmfngfa.html

composer require --dev phpunit/phpunit
来源：http://hz.zycfv.cn/gtkqscxjnu.html

[U79] PHP：静态分析
来源：http://hz.jqgufenzy.top/gtqzhtfiex.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtveiykicw.html

[U80] PHP：代码规范修复
来源：http://hz.aizwys.cn/gtxqyrtgft.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinghuilouyu.cn/gtudgqxpzb.html

[U81] JS：初始化项目
来源：http://hz.cdnleiting.top/gtpdkapbvo.html

npm init -y;  npm i express
来源：http://hz.nanxinkj.top/gtygbxxcjz.html

[U82] JS：package.json 脚本
来源：http://hz.shuidangran.top/gtezvtwibf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.andypj.xyz/gtgdmacmjx.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuxming.cn/gtvblwuevh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cashguo.top/gtkzhdnwtf.html

[U84] JS：CommonJS 写法
来源：http://hz.hnqzz.top/gtduszcjns.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtykpnoqii.html

[U85] JS：可选链
来源：http://hz.zhixingplan.top/gtbrytzepe.html

a?.b?.c
来源：http://hz.jinqigfzy.top/gtalagvfxc.html

[U86] JS：空值合并
来源：http://hz.jianghu66.top/gtwmvlitdj.html

a ?? b
来源：http://hz.xuetiantiany.cn/gtohzlrkqo.html

[U87] JS：解构默认值
来源：http://hz.gaohongyu789.top/gtndoejpzk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jlsjyb.cn/gtjlpwjpmr.html

[U88] JS：对象展开合并
来源：http://hz.0kj1m.cn/gtjrtuasfe.html

{ ...a, ...b }
来源：http://hz.chenjidiqi.icu/gttsiszewb.html

[U89] JS：数组去重
来源：http://hz.gzhubu.top/gtxcywhnez.html

[...new Set(arr)]
来源：http://hz.hywenlv.cn/gteuvvwaeu.html

[U90] JS：数字数组排序
来源：http://hz.jianghu66.top/gtuehhxzqk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtgojylopm.html

[U91] JS：对象键值遍历
来源：http://hz.jinghuilouyu.cn/gtbetjbdks.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zdqjudy.top/gtuezdvqtz.html

[U92] JS：深拷贝
来源：http://hz.yuxming.cn/gtomziylpg.html

structuredClone(obj)
来源：http://hz.iojbl.cn/gtphxtmnvn.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gtpjnblbge.html

`共 ${n} 条`
来源：http://hz.nwbrower.top/gttqsvcwrv.html

[U94] JS：箭头函数
来源：http://hz.xylfe.cn/gtpctqdfwf.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtdpatjjay.html

[U95] JS：Promise 包装
来源：http://hz.yvedp.cn/gtydideeua.html

new Promise((resolve, reject) => {})
来源：http://hz.c1oappe.top/gtigbvnivs.html

[U96] JS：async/await 与异常
来源：http://hz.dianchejie.cn/gtdrmosqzk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtyqemjuwy.html

[U97] JS：并发请求
来源：http://hz.cheryme.top/gtkaoszcoq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtlemiginc.html

[U98] JS：fetch 带 JSON
来源：http://hz.hongshengwenyu.top/gtaolyhjar.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtmapwknve.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtvgpohigo.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtkmeoqlsm.html

[U100] JS：DOM 查询
来源：http://hz.zhaomingkeji.xyz/gteyxqnyou.html

document.querySelector(".item")
来源：http://hz.zhaomingkeji.xyz/gtykepdsde.html

[U101] JS：classList 操作
来源：http://hz.jinghuilouyu.cn/gtltwououg.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtvdjczmvs.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtejyvwkvx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yanxiufei.cn/gtjbgejwbh.html

[U103] JS：定时器
来源：http://hz.shanyushiyangtech.top/gtjjxornoj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dashuyun.cn/gtycdircuz.html

[U104] JS：防抖
来源：http://hz.ydzc1.top/gtwmmgzrxd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtylrqzopk.html

[U105] JS：节流
来源：http://hz.nwbrower.top/gtcicfxpox.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtgyklkyte.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gtaiutaqvy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtkwvdoxej.html

[U107] JS：数字千分位
来源：http://hz.sysykeji.top/gttibbnqfw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.meibo888.top/gtqjccjxyb.html

[U108] JS：随机整数
来源：http://hz.iojbl.cn/gtjbvwgdgq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtxpchwhnc.html

[U109] JS：数组分组
来源：http://hz.sysykeji.top/gthgjuszbl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtffuvjbnq.html

[U110] JS：数组分块
来源：http://hz.hnqzz.top/gtyvhmmuhc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yueranfly.top/gtlaxkgxek.html

[U111] JS：对象转 Map
来源：http://hz.wangshuangyany.cn/gteijushik.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gtfngdpqoe.html

[U112] JS：字符串补位
来源：http://hz.jlsjyb.cn/gtpxxpurln.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtzaduwncz.html

[U113] JS：正则替换全部
来源：http://hz.cheryme.top/gtvlfochks.html

s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtgkfhftmy.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtlrjsdawm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gttpsbjqao.html

[U115] JS：生成 UUID
来源：http://hz.jinghuilouyu.cn/gtirkheqdz.html

crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtyrbotfzj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.quarkkingdee.top/gtzbyfxjmj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigufen.top/gtcumxcmmk.html

[U117] JS：单元测试
来源：http://hz.zhongyouzk.top/gtgfzazvxl.html

npm i -D vitest;  npx vitest
来源：http://hz.zhongyouzk.top/gtsabadpug.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtrzqjiejj.html

npm i -D vite;  npx vite
来源：http://hz.jqgufenzy.top/gtazarfdqk.html

[U119] JS：生产构建
来源：http://hz.ppjwa.cn/gtxakbwacb.html

npx vite build
来源：http://hz.jiagoushi.top/gtzeowulig.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtethlwamj.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gtwjnpqcqk.html

================================================================================
来源：http://hz.daxiang520.top/gtsmsitfku.html

统计汇总
来源：http://hz.yonumen.top/gtzhxdwtlg.html

================================================================================
来源：http://hz.cdnleiting.top/gtlrylwsfq.html

按语言统计（条）：
来源：http://hz.nanxuanxn.top/gthrfowagt.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtclqhlrkh.html

PHP ............ 252
来源：http://hz.ehwqpu.com/gttykzuexr.html

JavaScript ..... 252
来源：http://hz.bjfxy.top/gtjlftyxvx.html

TypeScript ..... 212
来源：http://hz.zhongyouzk.top/gtwtxnatix.html

Java ........... 212
来源：http://hz.wangdashe.top/gtajklfxfb.html

Go ............. 212
来源：http://hz.birdmap.top/gtvxmtgyql.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtauhihthe.html

C# ............. 212
来源：http://hz.quarkkingdee.top/gtkzriuhda.html

C .............. 30
来源：http://hz.chenlongwang.top/gtgshmqvns.html

C++ ............ 30
来源：http://hz.andypj.xyz/gtlemtctvh.html

SQL ............ 90
来源：http://hz.yongpay.top/gthmnvnszk.html

Bash ........... 80
来源：http://hz.cucudq.cn/gtvmvgkets.html

Kotlin ......... 15
来源：http://hz.jinyuanbaomall.cn/gtwtlahkra.html

Swift .......... 15
来源：http://hz.shzxlz.cn/gtsxbtdikg.html

Lua ............ 10
来源：http://hz.meibo888.top/gtcdzirkqn.html

Perl ........... 10
来源：http://hz.aibaodan.cn/gtdlksmpyr.html

Scala .......... 10
来源：http://hz.chenjidiqi.icu/gtyzxdjmrs.html

------------------------------------
来源：http://hz.c1oappe.top/gtmwxihgno.html

合计 ........... 2106 条
来源：http://hz.zhongyouzk.top/gtprradwti.html

按章节统计：
来源：http://hz.shzxlz.cn/gtjuibvmmo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtopgabfrb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtvavtynhl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtparxbzul.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtgfxhhuov.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tian-w.cn/gtrtdhfbtp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtuezfgxpu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtaxsysnrv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jyoumei.cn/gticuwumjw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtrtnmvebw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtnnnudloy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gttvjwxsah.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtdpdaypou.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtkmiaxrqb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtdavzmnld.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtbtxydzou.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtssjmgmvz.html

Q SQL 专题                              90
来源：http://hz.shzxlz.cn/gtszgqvcci.html

R Bash 专题                             80
来源：http://hz.ywan-chungtsiang.top/gtsnznswtl.html

S C / C++ 专题                          60
来源：http://hz.316326.xyz/gtpuyzadvx.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtihiobubi.html

U 高频实用片段                         120
来源：http://hz.zhengqikj.top/gtefonxmhs.html

------------------------------------
来源：http://hz.redwolf501.top/gtckcimeth.html

合计                                  2106 条
来源：http://hz.pycfn.com/gtpcqoaiii.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gttznvxiif.html

使用提醒
来源：http://hz.yongpay.top/gtvjzdqupw.html

--------------------------------------------------------------------------------
来源：http://hz.yvedp.cn/gthcxrrtjb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ivvv.top/gtowidowut.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtecrkqqij.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.c1oappe.top/gtuljagswu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinghuilouyu.cn/gtzesuxnyq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dashuyun.cn/gtgiszantb.html

—— 文件结束 ——
来源：http://hz.pengpengdd.cyou/gtoivdrvvc.html

================================================================================
来源：http://hz.9152youxi.cn/gtoekahcqp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinyuanbaomall.cn/gtsmbgqdwm.html

Common Programming Examples Cheat Book
来源：http://hz.zycfv.cn/gtfyjsobot.html

================================================================================
来源：http://hz.chenlongwang.top/gtkaghyxik.html

【收录内容】
来源：http://hz.gogol.net.cn/gteqimrjwl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sysykeji.top/gtvonjsrvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydzc1.top/gtnbkadrmm.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtfokqnzvl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtujyjgqpw.html

【使用说明】
来源：http://hz.dianchejie.cn/gtwdauogdd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ybcxt.top/gtohwrgvjc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gaohongyu789.top/gtzdzowwzs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xinyue.icu/gtxhgcigyv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenjidiqi.icu/gtisfxwodq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xingfuxueyuan.xyz/gtennsiwti.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.dashuyun.cn/gthuirguef.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dianchejie.cn/gtxutojuwi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xinyue.icu/gtjbkoqdno.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zycfv.cn/gteckdeteq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cucudq.cn/gtgnkcehlm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.andypj.xyz/gtltmcygap.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hammf.cn/gthjqblwsv.html

【文件统计】
来源：http://hz.zhijiandao.cn/gtdlhseuzh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ybcxt.top/gtyrbjswoz.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtqrhiextj.html

目  录
来源：http://hz.dashuyun.cn/gthlzzybuy.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtccjqiivm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hnxiangtu.top/gthgfjwwej.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtzsiomrxd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtdaenvdhx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jqgufenzy.top/gtwrzwykzm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.mhx1999.top/gtiktlsjdr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinyuanbaomall.cn/gthhotbkjl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gttrzikjbb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zycfv.cn/gtlzbzbmwy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtvecuwisv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yueranfly.top/gtlhpyrnsf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtvmfajssm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtowaovatx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtwkenpxjf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nanxuanxn.top/gtbxbwrzhu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhijiandao.cn/gtekcgnvdg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtuwatezwz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yvedp.cn/gtyttmjzyj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tianlin.xyz/gtzikflxnh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgufenzy.top/gtjtlfukcx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtqnuhnbbc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtorpqnmvq.html

================================================================================
来源：http://hz.fengsongda.top/gtynortbvd.html

A. 基础语法与类型
来源：http://hz.hfpthk.cn/gtflbaxncc.html

================================================================================
来源：http://hz.birdmap.top/gtrqfltycw.html

[A01] Hello World
来源：http://hz.yuxming.cn/gtmksvoyqm.html

Py:   print("Hello, World!")
来源：http://hz.jiagoushi.top/gtmvxgehzv.html

PHP:  echo "Hello, World!";
来源：http://hz.0kj1m.cn/gtsnfvsabs.html

JS:   console.log("Hello, World!");
来源：http://hz.sysykeji.top/gtwsponqgi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.pengpengdd.cyou/gtqhwlgjty.html

Java: System.out.println("Hello, World!");
来源：http://hz.daria6918.cn/gtlauhmybp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sysykeji.top/gtzsqzondt.html

Ruby: puts "Hello, World!"
来源：http://hz.tanke756.top/gtxirdbcbp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.meibo888.top/gtjxadmyli.html

[A02] 变量声明与赋值
来源：http://hz.ppjwa.cn/gtsperwnmf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.kuanghao11.cn/gtjsrysitu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.xylfe.cn/gtvkfpldqx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhongyouzk.top/gtogecyoqc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.meibo888.top/gtazzxdhxl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yanxiufei.cn/gtekifsota.html

Go:   name := "Alex"; age := 20
来源：http://hz.yueranfly.top/gthbvvltfp.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cdnleiting.top/gtxnfohpwv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ydjk.org.cn/gtufiogfzn.html

[A03] 常量定义
来源：http://hz.snrcjt.cn/gttqeqwaiz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.316326.xyz/gthuafkjhm.html

PHP:  const PI = 3.14159;
来源：http://hz.ehwqpu.com/gtaooordgw.html

JS:   const PI = 3.14159;
来源：http://hz.dianchejie.cn/gtbrjarssz.html

TS:   const PI: number = 3.14159;
来源：http://hz.yangfankeji.com/gtevmzaotw.html

Java: static final double PI = 3.14159;
来源：http://hz.cucudq.cn/gtbohozdka.html

Go:   const PI = 3.14159
来源：http://hz.yanxiufei.cn/gtfymcbvgk.html

Ruby: PI = 3.14159
来源：http://hz.jyoumei.cn/gtkwzkibmq.html

C#:   const double PI = 3.14159;
来源：http://hz.xylfe.cn/gttzwltsqh.html

[A04] 判断变量类型
来源：http://hz.fzhhl.top/gtkaaqiroh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hfpthk.cn/gtphjzbbmu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhoulong.xyz/gtpwwhrawg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yonumen.top/gtfyaplnkh.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj20258888.top/gtipcpltbh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ivvv.top/gtypabcpdz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yangfankeji.com/gtfvlksmur.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shuidangran.top/gtahvbrwsb.html

C#:   x.GetType().Name; x is int
来源：http://hz.xinyue.icu/gthapskcri.html

[A05] 整数除法与取模
来源：http://hz.hysaishi.cn/gtgkotnqxx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zycfv.cn/gtnlumscuo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtzwnvaike.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guowangkeji.top/gttkotycaq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtygwtjkrn.html

Java: 7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtldpjdrzp.html

Go:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtsasjubeg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gtxhvbuuqe.html

C#:   7 / 2; 7 % 2
来源：http://hz.pengpengdd.cyou/gtchnovybc.html

[A06] 字符串转数字
来源：http://hz.shangyingyoupin.top/gtaijrmfkm.html

Py:   int("42"); float("3.14")
来源：http://hz.tianlin.xyz/gtsjjsnbxw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.dashuyun.cn/gthdcfymov.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhiwuduotai.top/gtxazcsajf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gtwalbhsre.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xinyue.icu/gteziubnzi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hongshengwenyu.top/gtroxfcgwb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.kuanghao11.cn/gtnrxjaajb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangdashe.top/gtundcammz.html

[A07] 数字转字符串
来源：http://hz.yj20258.top/gtrceauaoo.html

Py:   str(42)
来源：http://hz.yj20258888.top/gtayfhjhym.html

PHP:  (string) 42; strval(42)
来源：http://hz.wangdashe.top/gtdesqiexs.html

JS:   String(42); (42).toString()
来源：http://hz.yvedp.cn/gtgktkirtq.html

TS:   String(42)
来源：http://hz.guannengcc.top/gtrmjuefcz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.smart0.xyz/gteqzoixjo.html

Go:   strconv.Itoa(42)
来源：http://hz.nanxinkj.top/gthieshoxq.html

Ruby: 42.to_s
来源：http://hz.hongshengwenyu.top/gttxetijyd.html

C#:   42.ToString()
来源：http://hz.shuidangran.top/gtnisvpmtc.html

[A08] 取整与四舍五入
来源：http://hz.sysykeji.top/gtbcfsmvpv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtcwjeuodw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.pycfn.com/gtfscrzeqa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hywenlv.cn/gtdzemztwv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.feifeiyinyue.top/gtyyzqloln.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.gaohongyu789.top/gtztstqlaz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.birdmap.top/gtefvshuye.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cheryme.top/gtbfadtyqx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ivvv.top/gtzdhlcuvx.html

[A09] 绝对值与最大最小值
来源：http://hz.havefunace.top/gtevskyuhu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.feifeiyinyue.top/gtzoxiqswa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.birdmap.top/gtbdqfcuhe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.fzhhl.top/gtotknroaw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hysaishi.cn/gtseyzumrf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigfzy.top/gtzktfemms.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.guannengcc.top/gttblhhxop.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.bjfxy.top/gtdtmhssdn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhiwuduotai.top/gtnoswsabi.html

[A10] 生成随机数
来源：http://hz.shanyushiyangkeji.top/gtlayeufhx.html

Py:   import random; random.randint(1, 100)
来源：http://hz.cdnleiting.top/gtwpmobkeu.html

PHP:  random_int(1, 100);
来源：http://hz.pycfn.com/gthhcqojxn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ivvv.top/gtvuriyzak.html


<!-- 参考信息 -->