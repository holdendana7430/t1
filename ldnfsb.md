代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.yueranfly.top/gtjulznnvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.daxiang520.top/gtpngbjxvl.html

[U70] PHP：PDO 事务
来源：http://hz.zycfv.cn/gtprmgfezt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.havefunace.top/gtzqqxrfup.html

[U71] PHP：抛出异常
来源：http://hz.nanxuanxn.top/gtrbnxgcxd.html

throw new RuntimeException("失败", 500);
来源：http://hz.jiagoushi.top/gtuftsibof.html

[U72] PHP：写错误日志
来源：http://hz.chenjidiqi.icu/gtruowupnc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtwxclcquu.html

[U73] PHP：读取 ini 配置
来源：http://hz.gotoacloud.top/gtwbqyddxw.html

parse_ini_file("config.ini", true)
来源：http://hz.shangyingyoupin.top/gtynvaprtu.html

[U74] PHP：读取环境变量
来源：http://hz.gotoacloud.top/gtzqmczgay.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hongshengwenyu.top/gtjmnzwezz.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtzekpbkuq.html

composer require psr/container
来源：http://hz.cqqwz.cn/gtzrzczfqg.html

[U76] PHP：简单路由
来源：http://hz.yuanzhike.top/gtiiutsnlx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gogol.net.cn/gtwgtghdye.html

[U77] PHP：模板渲染
来源：http://hz.yanxiufei.cn/gtkmhzgpyz.html

composer require twig/twig
来源：http://hz.shzxlz.cn/gtphaseomw.html

[U78] PHP：单元测试
来源：http://hz.9152youxi.cn/gtdroffods.html

composer require --dev phpunit/phpunit
来源：http://hz.ppjwa.cn/gtokyzeaqk.html

[U79] PHP：静态分析
来源：http://hz.hongshengwenyu.top/gtnuchedps.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtmugvsnww.html

[U80] PHP：代码规范修复
来源：http://hz.shuidangran.top/gtmktixnnx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ywan-chungtsiang.top/gtiooeeisy.html

[U81] JS：初始化项目
来源：http://hz.jinghuilouyu.cn/gtyhkqpuqw.html

npm init -y;  npm i express
来源：http://hz.cheryme.top/gttxpeqohw.html

[U82] JS：package.json 脚本
来源：http://hz.yj202588.top/gtdbucrxtc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gtpcgynnwk.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gttkegsrga.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenjidiqi.icu/gtpqudmzsj.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtbuxvdhzn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pycfn.com/gtfyuapkzo.html

[U85] JS：可选链
来源：http://hz.dashuyun.cn/gtxepqqxcq.html

a?.b?.c
来源：http://hz.zycfv.cn/gtziswgoks.html

[U86] JS：空值合并
来源：http://hz.chenjidiqi.icu/gtupstwvjp.html

a ?? b
来源：http://hz.smart0.xyz/gtuamcjnpe.html

[U87] JS：解构默认值
来源：http://hz.hongshengwenyu.top/gtbmssxfcz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nwbrower.top/gtlptqdbkz.html

[U88] JS：对象展开合并
来源：http://hz.zhengqikj.top/gtvjwuwlgw.html

{ ...a, ...b }
来源：http://hz.ydzc1.top/gtdvowrzmo.html

[U89] JS：数组去重
来源：http://hz.xinyue.icu/gtahiwmcxd.html

[...new Set(arr)]
来源：http://hz.0kj1m.cn/gtbvhswarf.html

[U90] JS：数字数组排序
来源：http://hz.zhijiandao.cn/gtvicunwdr.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtgmvmttgw.html

[U91] JS：对象键值遍历
来源：http://hz.cqqwz.cn/gtxufpkqzw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.0kj1m.cn/gtvikowwhw.html

[U92] JS：深拷贝
来源：http://hz.chenjidiqi.icu/gtwgozzlez.html

structuredClone(obj)
来源：http://hz.jinqigufen.top/gtdplrzzzd.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtlbvqgkzi.html

`共 ${n} 条`
来源：http://hz.yj20258888.top/gtzabylcwb.html

[U94] JS：箭头函数
来源：http://hz.ydjk.org.cn/gtijprjwes.html

const double = x => x * 2;
来源：http://hz.yanxiufei.cn/gtrufyairv.html

[U95] JS：Promise 包装
来源：http://hz.chenzaomai.com/gtmczomgnf.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigfzy.top/gtjctxkgan.html

[U96] JS：async/await 与异常
来源：http://hz.jqgufenzy.top/gtxmekhyil.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtyzkjvpdi.html

[U97] JS：并发请求
来源：http://hz.cucudq.cn/gtmogvhlfz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gttcfuxzxs.html

[U98] JS：fetch 带 JSON
来源：http://hz.ppjwa.cn/gtmmdgrqsj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuanzhike.top/gtblgxuezl.html

[U99] JS：事件监听
来源：http://hz.zhoulong.xyz/gtzdnletzg.html

el.addEventListener("click", e => {})
来源：http://hz.guannengcc.top/gtvyhilqgb.html

[U100] JS：DOM 查询
来源：http://hz.svipenyu.cn/gtioqcqnol.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gttvucaynh.html

[U101] JS：classList 操作
来源：http://hz.guowangkeji.top/gtjuwanoft.html

el.classList.toggle("active")
来源：http://hz.fzhhl.top/gtdbzsglgc.html

[U102] JS：本地存储
来源：http://hz.birdmap.top/gtbtkukxft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tanke756.top/gtldblizau.html

[U103] JS：定时器
来源：http://hz.meibo888.top/gtgszmkpvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenzaomai.com/gtkeveicrg.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtiloddobt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtqlymvvgr.html

[U105] JS：节流
来源：http://hz.yongpay.top/gtjadbxebl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgfzy.top/gtwgyzuger.html

[U106] JS：日期格式化
来源：http://hz.xinyue.icu/gtgizptkcq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.andypj.xyz/gtuggefvlb.html

[U107] JS：数字千分位
来源：http://hz.hammf.cn/gtmkyjiztk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fengsongda.top/gtzcyzqacu.html

[U108] JS：随机整数
来源：http://hz.yuanzhike.top/gtccrfvyls.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtggdxnkqv.html

[U109] JS：数组分组
来源：http://hz.sysykeji.top/gtcrjluohr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtsucczqft.html

[U110] JS：数组分块
来源：http://hz.ywan-chungtsiang.top/gtfsizbamr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj202588.top/gtotycvmqc.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gthrityxax.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtwdjaspjl.html

[U112] JS：字符串补位
来源：http://hz.gzhubu.top/gtegtjhmyn.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtxhmtwihk.html

[U113] JS：正则替换全部
来源：http://hz.tianlin.xyz/gtexuyilne.html

s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtdntxpcho.html

[U114] JS：JSON 深比较
来源：http://hz.jinyuanbaomall.cn/gtysazceow.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtgjwarrpp.html

[U115] JS：生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtcloydaez.html

crypto.randomUUID()
来源：http://hz.hammf.cn/gtlbmuoxvb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aizwys.cn/gttnvfmcna.html

/** @param {string} name */ function f(name) {}
来源：http://hz.redwolf501.top/gtrtphmalz.html

[U117] JS：单元测试
来源：http://hz.wangshuangyany.cn/gtgwudxbrs.html

npm i -D vitest;  npx vitest
来源：http://hz.feifeiyinyue.top/gttpgkzrgr.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtaenkewcq.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gthjgmuvks.html

[U119] JS：生产构建
来源：http://hz.zhijiandao.cn/gtuacqtgll.html

npx vite build
来源：http://hz.yangfankeji.com/gtbjvwpdxs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.smart0.xyz/gtbbsonynn.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtrdvmbbae.html

================================================================================
来源：http://hz.zhengqikj.top/gtoupyowsy.html

统计汇总
来源：http://hz.xuetiantiany.cn/gteawnzgai.html

================================================================================
来源：http://hz.xziqi.cn/gtomjuopdg.html

按语言统计（条）：
来源：http://hz.xylfe.cn/gtzwcoihvr.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtzqckuqyq.html

PHP ............ 252
来源：http://hz.yongpay.top/gtjayjdxod.html

JavaScript ..... 252
来源：http://hz.jianghu66.top/gtisqppybz.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gtiycclaxk.html

Java ........... 212
来源：http://hz.hammf.cn/gtzlsmeoxk.html

Go ............. 212
来源：http://hz.kuanghao11.cn/gtmcqwxomm.html

Ruby ........... 212
来源：http://hz.zhengqikj.top/gtatqaznor.html

C# ............. 212
来源：http://hz.9152youxi.cn/gtmqzoepge.html

C .............. 30
来源：http://hz.sweek.top/gtljsesyww.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtvvrktqel.html

SQL ............ 90
来源：http://hz.nanxinkj.top/gtsuqjxjws.html

Bash ........... 80
来源：http://hz.dashuyun.cn/gtllizlosp.html

Kotlin ......... 15
来源：http://hz.tian-w.cn/gtusqosqsi.html

Swift .......... 15
来源：http://hz.pengpengdd.cyou/gtbtaebbaj.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtwziokdou.html

Perl ........... 10
来源：http://hz.yj202588.top/gtsqainxwz.html

Scala .......... 10
来源：http://hz.xinyue.icu/gtrqheappq.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtokuagbmp.html

合计 ........... 2106 条
来源：http://hz.pycfn.com/gtvrqbvzwn.html

按章节统计：
来源：http://hz.guowangkeji.top/gtfzbfttsv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtmxfazyyw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtinadctkc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gttgafeqrx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtbjqlqmkb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.redwolf501.top/gtstqsjxuu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtvuovflfb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtkzmahmtl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhongyouzk.top/gtjwejzjlk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtaslcnieg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtkqohlmzb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtqbqaqtqu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtwuzrmgvc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtimlaigvk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtxwreekpa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sysykeji.top/gtisoudsyk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtgqrpulwf.html

Q SQL 专题                              90
来源：http://hz.meibo888.top/gtrdubjkfs.html

R Bash 专题                             80
来源：http://hz.nanxinkj.top/gtzwcsfhay.html

S C / C++ 专题                          60
来源：http://hz.c1oappe.top/gttknwktxr.html

T 其他语言补充                          60
来源：http://hz.316326.xyz/gtzzjgqkaw.html

U 高频实用片段                         120
来源：http://hz.birdmap.top/gtfbzkwlmb.html

------------------------------------
来源：http://hz.zycfv.cn/gtlpxthgrw.html

合计                                  2106 条
来源：http://hz.quarkkingdee.top/gtzvmxqzvv.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtrvgmkkix.html

使用提醒
来源：http://hz.sufxvd.cn/gtihcegyeq.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtnlclinsr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtetyegblv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shangyingyoupin.top/gtbsgrfvwf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.meibo888.top/gtadfgpqtl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.9152youxi.cn/gtejfbnesd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinyuanbaomall.cn/gtidtvdlfg.html

—— 文件结束 ——
来源：http://hz.jlsjyb.cn/gtgqmuswzr.html

================================================================================
来源：http://hz.yj202588.top/gtirulceyq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangshuangyany.cn/gtyaxjvjaz.html

Common Programming Examples Cheat Book
来源：http://hz.redwolf501.top/gtdfkccavn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtflggwncr.html

【收录内容】
来源：http://hz.yongpay.top/gtjwiwblxq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zycfv.cn/gtamtovjqw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cucudq.cn/gtnlscwxnq.html

SQL · Bash · C · C++
来源：http://hz.xuanzx.com/gtqziczpnn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ppjwa.cn/gtnozxycdv.html

【使用说明】
来源：http://hz.yj20258888.top/gtqnygydov.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gtkacjvkdv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgfzy.top/gtmbyontvi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sxryk.cn/gtapxpuexy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pengpengdd.cyou/gtnpvctkfa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangshuangyany.cn/gtjxfsnkst.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sxryk.cn/gtrocunznv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sysykeji.top/gtissvowfo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xuetiantiany.cn/gtcsxarzfg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxinkj.top/gtnpfawrsh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hywenlv.cn/gtpetrqksh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinghuilouyu.cn/gtgcvdsiuj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinqigfzy.top/gtiyugvdvh.html

【文件统计】
来源：http://hz.redwolf501.top/gtgabqmlex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sxryk.cn/gtbaalyrqf.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gtcplvotti.html

目  录
来源：http://hz.kuanghao11.cn/gtksrofdcs.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gttdxgiqoc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtydsqowpc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gthrygtorr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtyhexkdxx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hfpthk.cn/gtgwhmchgn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj20258.top/gtmyzekmfn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yueranfly.top/gtrzzdzexe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtbldzqdsq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtdhggnkzo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtbkulfior.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xylfe.cn/gticyegsyi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtbztmpotj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtnxwamuvz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtuapyyfty.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtywzfmoel.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aibaodan.cn/gttlyalwzt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtxzlfkubj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yanxiufei.cn/gtnnwafmut.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fzhhl.top/gtafcaaxhh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.wangdashe.top/gtidoriacd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtrqmqqiss.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtictankvw.html

================================================================================
来源：http://hz.guannengcc.top/gtijnltglp.html

A. 基础语法与类型
来源：http://hz.bjfxy.top/gtufhqbdgj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnjwsyocq.html

[A01] Hello World
来源：http://hz.xinyue.icu/gtjezcpzlc.html

Py:   print("Hello, World!")
来源：http://hz.zhoulong.xyz/gtscrvaiwd.html

PHP:  echo "Hello, World!";
来源：http://hz.pengpengdd.cyou/gtmfzzjzqy.html

JS:   console.log("Hello, World!");
来源：http://hz.xingfuxueyuan.xyz/gtwzvtczxe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ehwqpu.com/gtfxocrbyy.html

Java: System.out.println("Hello, World!");
来源：http://hz.sysykeji.top/gtispeshuo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtogmntrks.html

Ruby: puts "Hello, World!"
来源：http://hz.zhiwuduotai.top/gtvsdswbit.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xuanzx.com/gtywqtcbsh.html

[A02] 变量声明与赋值
来源：http://hz.gotoacloud.top/gtlztfwuje.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jianghu66.top/gtwanlooiw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinghuilouyu.cn/gtcjdttpxl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yangfankeji.com/gtgvgugjye.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj20258888.top/gtljswoqkg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtbfwkiitv.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtjaewvajy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cashguo.top/gthxbgvrlq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nwbrower.top/gtobvrodqj.html

[A03] 常量定义
来源：http://hz.jyoumei.cn/gtqbpyywcx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhixingplan.top/gtiojtqstt.html

PHP:  const PI = 3.14159;
来源：http://hz.yangfankeji.com/gtgqmwlkgt.html

JS:   const PI = 3.14159;
来源：http://hz.316326.xyz/gtlgkgylld.html

TS:   const PI: number = 3.14159;
来源：http://hz.sxryk.cn/gtpnnfrwac.html

Java: static final double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtxzmzcxom.html

Go:   const PI = 3.14159
来源：http://hz.gaohongyu789.top/gtkpmngftd.html

Ruby: PI = 3.14159
来源：http://hz.chenlongwang.top/gttllclqbg.html

C#:   const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtrenkxapz.html

[A04] 判断变量类型
来源：http://hz.daria6918.cn/gtvkobxqwx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yangfankeji.com/gtljevycqy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinyuanbaomall.cn/gtmwucdrsb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aibaodan.cn/gtzdeximrn.html

TS:   typeof x; x instanceof Date
来源：http://hz.xuanzx.com/gtlcwphdzn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hfpthk.cn/gttgftvssv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jianghu66.top/gtscpbmvrf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xingfuxueyuan.xyz/gtdnrwnxbe.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydzc1.top/gtcnicrldy.html

[A05] 整数除法与取模
来源：http://hz.ydjk.org.cn/gtpwzheoey.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenjidiqi.icu/gtvqixfekm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xuetiantiany.cn/gtvcbliawm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ydzc1.top/gtjfevzoys.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.0kj1m.cn/gtcupqoyhs.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtsvnvxnqd.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gteplunoen.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hnqzz.top/gtspegxulw.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtfejebnzb.html

[A06] 字符串转数字
来源：http://hz.jinqigufen.top/gtjudamtws.html

Py:   int("42"); float("3.14")
来源：http://hz.bjfxy.top/gtmgfjyahs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinqigufen.top/gtaoqsitka.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtasmnmfzm.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.chenjidiqi.icu/gtltdmdimt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hysaishi.cn/gtoysvefcg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hongshengwenyu.top/gtidrrffgf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinqigufen.top/gtqqxnqfdp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.meibo888.top/gtnjehhmwh.html

[A07] 数字转字符串
来源：http://hz.jqgufenzy.top/gtdtolimwp.html

Py:   str(42)
来源：http://hz.zhiwuduotai.top/gtdwokytrr.html

PHP:  (string) 42; strval(42)
来源：http://hz.feifeiyinyue.top/gtxsuetqrt.html

JS:   String(42); (42).toString()
来源：http://hz.shangyingyoupin.top/gtpyyijygq.html

TS:   String(42)
来源：http://hz.shangyingyoupin.top/gtssdmgzdj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yonumen.top/gtcodrkjbn.html

Go:   strconv.Itoa(42)
来源：http://hz.redwolf501.top/gtzohxrond.html

Ruby: 42.to_s
来源：http://hz.gotoacloud.top/gtqzqdiozp.html

C#:   42.ToString()
来源：http://hz.meibo888.top/gtwdnmkxno.html

[A08] 取整与四舍五入
来源：http://hz.sysykeji.top/gtnmehntdj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.zhaomingkeji.xyz/gtwqamkdoo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.kuanghao11.cn/gtqbqwvbuu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gtklxwcvlm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yuxming.cn/gtynqxoydm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtefwhayqf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.quarkkingdee.top/gtzkrsxypd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.52xcode.cn/gtsdtiffky.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hywenlv.cn/gtmzsfsdry.html

[A09] 绝对值与最大最小值
来源：http://hz.tian-w.cn/gtynarnhra.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.meibo888.top/gtxchcbfuf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.meibo888.top/gteahywgho.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.cashguo.top/gtxhwtnsxs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yangfankeji.com/gtrhucepvt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sxryk.cn/gtvxfgkndx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.gzhubu.top/gtbqtngckd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shangyingyoupin.top/gteemembai.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtfkulfuyt.html

[A10] 生成随机数
来源：http://hz.xylfe.cn/gtrljktglv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yuanzhike.top/gtvfajnafn.html

PHP:  random_int(1, 100);
来源：http://hz.shuidangran.top/gtkkyeykra.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jlsjyb.cn/gtgjqzqkac.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yanxiufei.cn/gtijuvvsqy.html

Java: new Random().nextInt(100) + 1
来源：http://hz.chenjidiqi.icu/gtsidvodpy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhengqikj.top/gttzfasmpv.html

Ruby: rand(1..100)
来源：http://hz.c1oappe.top/gtndmdrmnj.html


<!-- 参考信息 -->