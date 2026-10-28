代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.chenjidiqi.icu/gtrggzrjmz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.snrcjt.cn/gtltmwakdn.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtbmgwbkto.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.nwbrower.top/gtsnjuvgth.html

[U71] PHP：抛出异常
来源：http://hz.hywenlv.cn/gtgzlydfdf.html

throw new RuntimeException("失败", 500);
来源：http://hz.fengsongda.top/gttmyshffl.html

[U72] PHP：写错误日志
来源：http://hz.haohaochexian.top/gtgfngbmdr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yj202588.top/gtlaeyxaol.html

[U73] PHP：读取 ini 配置
来源：http://hz.dianchejie.cn/gtvlydjuhe.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gtlbzgoego.html

[U74] PHP：读取环境变量
来源：http://hz.sxryk.cn/gtabkzrgov.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cheryme.top/gthhoalplo.html

[U75] PHP：依赖注入
来源：http://hz.hnxiangtu.top/gtigviymqv.html

composer require psr/container
来源：http://hz.cucudq.cn/gteoqpqgpa.html

[U76] PHP：简单路由
来源：http://hz.pycfn.com/gtxibijwqo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.quarkkingdee.top/gtrbcpsber.html

[U77] PHP：模板渲染
来源：http://hz.gotoacloud.top/gtjtxdfwwj.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtflpejozw.html

[U78] PHP：单元测试
来源：http://hz.gogol.net.cn/gtdrsejukt.html

composer require --dev phpunit/phpunit
来源：http://hz.sysykeji.top/gtpxjvywrm.html

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gtfxcnvfdx.html

composer require --dev phpstan/phpstan
来源：http://hz.redwolf501.top/gtykzngmto.html

[U80] PHP：代码规范修复
来源：http://hz.snrcjt.cn/gtsqykfvnr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.tanke756.top/gthbjqbpwn.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtepxltxck.html

npm init -y;  npm i express
来源：http://hz.hammf.cn/gtlahywtme.html

[U82] JS：package.json 脚本
来源：http://hz.daria6918.cn/gtzvtzznka.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gotoacloud.top/gtgegvbfhh.html

[U83] JS：ES Module 导入导出
来源：http://hz.guannengcc.top/gthkykvcyu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhixingplan.top/gtxlljchca.html

[U84] JS：CommonJS 写法
来源：http://hz.andypj.xyz/gtlgaicovo.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yonumen.top/gtbclbplva.html

[U85] JS：可选链
来源：http://hz.shuidangran.top/gtzmmyrvwh.html

a?.b?.c
来源：http://hz.cqqwz.cn/gtnnzuikqa.html

[U86] JS：空值合并
来源：http://hz.yanxiufei.cn/gtcefuocdt.html

a ?? b
来源：http://hz.pycfn.com/gtmqcjeqrr.html

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtvpdiolfp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cucudq.cn/gtbquuquzr.html

[U88] JS：对象展开合并
来源：http://hz.jinghuilouyu.cn/gtczmaobhq.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gtjbbyotdp.html

[U89] JS：数组去重
来源：http://hz.c1oappe.top/gtihjmqytx.html

[...new Set(arr)]
来源：http://hz.pycfn.com/gtctiwmktq.html

[U90] JS：数字数组排序
来源：http://hz.feifeiyinyue.top/gtrisqrzel.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtosenjrry.html

[U91] JS：对象键值遍历
来源：http://hz.daxiang520.top/gtqmwokfjd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.aibaodan.cn/gtekmnprer.html

[U92] JS：深拷贝
来源：http://hz.jianghu66.top/gtuntqvbfc.html

structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtgguhyesm.html

[U93] JS：模板字符串
来源：http://hz.yuanzhike.top/gtekzasljk.html

`共 ${n} 条`
来源：http://hz.wangdashe.top/gtkzepdxnh.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtqhxtjejt.html

const double = x => x * 2;
来源：http://hz.sxryk.cn/gtkpwaovjm.html

[U95] JS：Promise 包装
来源：http://hz.ywan-chungtsiang.top/gtgsgtdkyu.html

new Promise((resolve, reject) => {})
来源：http://hz.shzxlz.cn/gtjmqjnngv.html

[U96] JS：async/await 与异常
来源：http://hz.c1oappe.top/gtdsdrpzsu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtcfbauhsl.html

[U97] JS：并发请求
来源：http://hz.zhiwuduotai.top/gtvphsvaqh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtdbccaucr.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinqigfzy.top/gtbzrspxbz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj202588.top/gtorfkqfdh.html

[U99] JS：事件监听
来源：http://hz.bjfxy.top/gtwpplmkaz.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gttfjjrhua.html

[U100] JS：DOM 查询
来源：http://hz.mhx1999.top/gtcoaukeja.html

document.querySelector(".item")
来源：http://hz.bjfxy.top/gtwhfpxrzi.html

[U101] JS：classList 操作
来源：http://hz.dashuyun.cn/gtffdzouuk.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtyeybyapz.html

[U102] JS：本地存储
来源：http://hz.0kj1m.cn/gtoieymeif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yanxiufei.cn/gtmwnxvvit.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtvmzyssrw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gtmgmvbqve.html

[U104] JS：防抖
来源：http://hz.nanxuanxn.top/gtocdeydqe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtpmdwyyag.html

[U105] JS：节流
来源：http://hz.feifeiyinyue.top/gtrncfhpxb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnqzz.top/gtvmwqmurp.html

[U106] JS：日期格式化
来源：http://hz.xziqi.cn/gtsnnavsbw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtvceojpaq.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtgkkbexox.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.meibo888.top/gtsfcmgbgl.html

[U108] JS：随机整数
来源：http://hz.ydzc1.top/gtazufoime.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ppjwa.cn/gtkaxdowcr.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtcanijlfq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxinkj.top/gtlpfobntu.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtwtfhgqwh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.9152youxi.cn/gtxahjhkui.html

[U111] JS：对象转 Map
来源：http://hz.dashuyun.cn/gtethjtljq.html

new Map(Object.entries(obj))
来源：http://hz.aibaodan.cn/gtpuvvycgx.html

[U112] JS：字符串补位
来源：http://hz.gotoacloud.top/gtzprgrcdq.html

"7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtmnrbohil.html

[U113] JS：正则替换全部
来源：http://hz.hywenlv.cn/gtlpsqtknn.html

s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gthlvcodax.html

[U114] JS：JSON 深比较
来源：http://hz.gaohongyu789.top/gtobycpbdz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtoartztff.html

[U115] JS：生成 UUID
来源：http://hz.52xcode.cn/gtbkxyipsb.html

crypto.randomUUID()
来源：http://hz.yueranfly.top/gtuijaxqiu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.feifeiyinyue.top/gtgdnyfurk.html

/** @param {string} name */ function f(name) {}
来源：http://hz.iojbl.cn/gtpretijch.html

[U117] JS：单元测试
来源：http://hz.52xcode.cn/gtenzthhdv.html

npm i -D vitest;  npx vitest
来源：http://hz.jlsjyb.cn/gthtfkhgwr.html

[U118] JS：开发服务器
来源：http://hz.hywenlv.cn/gtegvoaytm.html

npm i -D vite;  npx vite
来源：http://hz.chenlongwang.top/gtnclmlkkm.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtwjvrvsgx.html

npx vite build
来源：http://hz.vqdsnc.cn/gtfnufkchu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtbipmcedq.html

import.meta.env.VITE_API_URL
来源：http://hz.sufxvd.cn/gtcyroncgx.html

================================================================================
来源：http://hz.daria6918.cn/gthipzfhns.html

统计汇总
来源：http://hz.dianchejie.cn/gthszwrrtq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxxxtjqzz.html

按语言统计（条）：
来源：http://hz.guowangkeji.top/gtrpaqdobq.html

Python ......... 252
来源：http://hz.nwbrower.top/gtycbambvo.html

PHP ............ 252
来源：http://hz.c1oappe.top/gtzvzqupss.html

JavaScript ..... 252
来源：http://hz.yj20258.top/gtmerbwwnw.html

TypeScript ..... 212
来源：http://hz.aibaodan.cn/gtgqmxlmjt.html

Java ........... 212
来源：http://hz.ydjk.org.cn/gtwzydhiiy.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtzeoipnxc.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtwoqtldti.html

C# ............. 212
来源：http://hz.ybcxt.top/gtwcwkbamw.html

C .............. 30
来源：http://hz.cucudq.cn/gtqbtsscrw.html

C++ ............ 30
来源：http://hz.haohaochexian.top/gtsvyspglz.html

SQL ............ 90
来源：http://hz.cucudq.cn/gtvmnzthal.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtsfbeyfdj.html

Kotlin ......... 15
来源：http://hz.svipenyu.cn/gtqppydgve.html

Swift .......... 15
来源：http://hz.birdmap.top/gtsexddptz.html

Lua ............ 10
来源：http://hz.xingfuxueyuan.xyz/gtyvujxhel.html

Perl ........... 10
来源：http://hz.0kj1m.cn/gtlkoaagsc.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gtojadxxkj.html

------------------------------------
来源：http://hz.bjfxy.top/gtwancgiiu.html

合计 ........... 2106 条
来源：http://hz.sufxvd.cn/gtmodntnfi.html

按章节统计：
来源：http://hz.pycfn.com/gtssnrbrhp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtzwkvcvet.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtfhdkqhge.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shuidangran.top/gtmnywaqxb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gtlvihmiyr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xylfe.cn/gtrmvnhfmb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtbbrdmuqg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gttlsojfrq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gtiqkjdoyd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.fengsongda.top/gtlwlotjar.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtenqnzqqf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtdbgtzocc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtpsacbory.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtjvotierr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinyuanbaomall.cn/gtstqsauvn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.vqdsnc.cn/gtmrsxmhee.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtvweyecaw.html

Q SQL 专题                              90
来源：http://hz.pycfn.com/gteprcufzt.html

R Bash 专题                             80
来源：http://hz.zdqjudy.top/gtuyvzzdcd.html

S C / C++ 专题                          60
来源：http://hz.yj20258.top/gtwgpceull.html

T 其他语言补充                          60
来源：http://hz.wangshuangyany.cn/gtxbarrazo.html

U 高频实用片段                         120
来源：http://hz.iojbl.cn/gtriiyvcdv.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtoisshmlx.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtxnpbbrcm.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtpcccomyi.html

使用提醒
来源：http://hz.bjfxy.top/gtrbivappy.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtbtxxcwve.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.snrcjt.cn/gtbgbbpyzw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.svipenyu.cn/gtxaufqcjb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhaomingkeji.xyz/gtyeupfryn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.redwolf501.top/gtcyfwqetd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtytznwbjk.html

—— 文件结束 ——
来源：http://hz.nanxinkj.top/gtybdtauth.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsqkvwobl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.daria6918.cn/gtfnaeydbt.html

Common Programming Examples Cheat Book
来源：http://hz.shuidangran.top/gthardxqgg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjxibotps.html

【收录内容】
来源：http://hz.jlsjyb.cn/gthleijhuc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnxiangtu.top/gtgkwoepjn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtbxdjnxaz.html

SQL · Bash · C · C++
来源：http://hz.redwolf501.top/gtxdupcxkw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.iojbl.cn/gtqdjwvwms.html

【使用说明】
来源：http://hz.fzhhl.top/gtwqlsqpve.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.snrcjt.cn/gtgicpkwxk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258888.top/gtiqlsncdj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.pycfn.com/gtdyrdfkto.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cucudq.cn/gtlobcvboq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cucudq.cn/gtjpgwaocr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.birdmap.top/gtpjqgcxrf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jyoumei.cn/gtvvniakwx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yangfankeji.com/gtqmcfrrup.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cqqwz.cn/gtbjnapvey.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hysaishi.cn/gtmsgjvolu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtxpouiret.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zdqjudy.top/gtbihztrmh.html

【文件统计】
来源：http://hz.zdqjudy.top/gtmwihjmei.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.kuanghao11.cn/gtoskanjqw.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtychzofkl.html

目  录
来源：http://hz.iojbl.cn/gtxifnjggw.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtelahdjwi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.316326.xyz/gtjnwqkozb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ywan-chungtsiang.top/gtjdcnjyfb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fengsongda.top/gtekhjhgrl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ehwqpu.com/gtbgbgisjl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.andypj.xyz/gtzxahulko.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtqnsgfymp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gturuebops.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hysaishi.cn/gtpbghvhgo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtyrbvrrsw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtstmuyfiv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtqjjvbwnf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtbfdbyijs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtujfqdgvk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.guowangkeji.top/gtsulmqieq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daria6918.cn/gtlfkanztr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtjjvvvzen.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258888.top/gtaoxcjyoa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.0kj1m.cn/gtxgxpkdcm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xuanzx.com/gtvehutirt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtqbcuqjgo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenjidiqi.icu/gtbdlhyngi.html

================================================================================
来源：http://hz.hammf.cn/gtdpcoaicc.html

A. 基础语法与类型
来源：http://hz.9152youxi.cn/gtopknqbrm.html

================================================================================
来源：http://hz.ydjk.org.cn/gtazfyayee.html

[A01] Hello World
来源：http://hz.ehwqpu.com/gtjeagjnzi.html

Py:   print("Hello, World!")
来源：http://hz.shangyingyoupin.top/gtipidqqte.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtvnuebiry.html

JS:   console.log("Hello, World!");
来源：http://hz.jqgufenzy.top/gtiexeckhf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gotoacloud.top/gtmdzjpxlv.html

Java: System.out.println("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtzcrazrhe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.daxiang520.top/gtsgmzgzdo.html

Ruby: puts "Hello, World!"
来源：http://hz.jinghuilouyu.cn/gtzaugxlpa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yonumen.top/gtnejgkqec.html

[A02] 变量声明与赋值
来源：http://hz.jqgfzy.top/gtkybwpauy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinyuanbaomall.cn/gtxgzkffdd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gtomiodjyj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hywenlv.cn/gtwhaoiqry.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.birdmap.top/gtlfmhhymq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cheryme.top/gtuzxjeouu.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtlubirjyq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shanyushiyangkeji.top/gtahflvrjx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.havefunace.top/gtlxrydmsd.html

[A03] 常量定义
来源：http://hz.ybcxt.top/gtlpnwfyhd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jyoumei.cn/gttfoixbhn.html

PHP:  const PI = 3.14159;
来源：http://hz.nwbrower.top/gtpvqutqkz.html

JS:   const PI = 3.14159;
来源：http://hz.yj20258.top/gtgxkblihs.html

TS:   const PI: number = 3.14159;
来源：http://hz.daria6918.cn/gtparipnii.html

Java: static final double PI = 3.14159;
来源：http://hz.pycfn.com/gtrwgnyubp.html

Go:   const PI = 3.14159
来源：http://hz.52xcode.cn/gteuadijhg.html

Ruby: PI = 3.14159
来源：http://hz.gaohongyu789.top/gtnpgfhitf.html

C#:   const double PI = 3.14159;
来源：http://hz.cashguo.top/gtiozehrzi.html

[A04] 判断变量类型
来源：http://hz.gzhubu.top/gtnyavbwkg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.vqdsnc.cn/gtbtxnucio.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhixingplan.top/gtxrrnkiqp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.svipenyu.cn/gthngwzpao.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinyuanbaomall.cn/gtkuwtcvlo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pengpengdd.cyou/gtlayktbzl.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.dashuyun.cn/gtkbmqgxbs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nwbrower.top/gtqgturwjm.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhixingplan.top/gtpwtxypnb.html

[A05] 整数除法与取模
来源：http://hz.wangdashe.top/gtfxsflwmg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.dashuyun.cn/gtsknpunlj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhixingplan.top/gthxuhmhme.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.52xcode.cn/gtfqdoqymq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtmyqbhcel.html

Java: 7 / 2; 7 % 2
来源：http://hz.aibaodan.cn/gtuvftllos.html

Go:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtcapfpyyx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtfgslikft.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtjmjpsyps.html

[A06] 字符串转数字
来源：http://hz.zhoulong.xyz/gtjnascfwo.html

Py:   int("42"); float("3.14")
来源：http://hz.yj20258888.top/gtambsktqe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.tianlin.xyz/gtvodnzgym.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.guannengcc.top/gtttjvbiki.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shanyushiyangkeji.top/gtybvdwumw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.haohaochexian.top/gtxehlngnx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhixingplan.top/gtyyoacekk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhengqikj.top/gtepeohzqf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangshuangyany.cn/gtiuxmqxvw.html

[A07] 数字转字符串
来源：http://hz.hysaishi.cn/gtjhrvinop.html

Py:   str(42)
来源：http://hz.shzxlz.cn/gtywjtezyy.html

PHP:  (string) 42; strval(42)
来源：http://hz.jyoumei.cn/gtfrkrgucx.html

JS:   String(42); (42).toString()
来源：http://hz.hammf.cn/gtdmodgona.html

TS:   String(42)
来源：http://hz.jinqigufen.top/gtcqmianhu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.bjfxy.top/gtxfiefygz.html

Go:   strconv.Itoa(42)
来源：http://hz.hnqzz.top/gtxfuutoyc.html

Ruby: 42.to_s
来源：http://hz.pycfn.com/gttsxclfxf.html

C#:   42.ToString()
来源：http://hz.fzhhl.top/gtmziftvpp.html

[A08] 取整与四舍五入
来源：http://hz.ybcxt.top/gtjzdmpcoj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ydzc1.top/gtqzozcnkl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xuanzx.com/gtajuocgkg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hysaishi.cn/gtkhqjdkss.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangkeji.top/gtnasrghib.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.andypj.xyz/gtnhcuntgh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.iojbl.cn/gtxmffciph.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xinyue.icu/gtrmgxnxai.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.andypj.xyz/gtecuilimy.html

[A09] 绝对值与最大最小值
来源：http://hz.daxiang520.top/gtuavctobc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jianghu66.top/gtlxmxxtpv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258888.top/gtlgvyxnyj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yanxiufei.cn/gtedtuerwi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gogol.net.cn/gtczpvlcnc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.aibaodan.cn/gtkrtofsar.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hysaishi.cn/gtuhczzzrn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.316326.xyz/gtqjygjkkt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hysaishi.cn/gtkblphqrv.html

[A10] 生成随机数
来源：http://hz.cucudq.cn/gtejniqyhb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ywan-chungtsiang.top/gtevfwudbx.html

PHP:  random_int(1, 100);
来源：http://hz.xylfe.cn/gtcnesuezs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shzxlz.cn/gtwwnjcxtb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jlsjyb.cn/gtlhlvvevm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cheryme.top/gtjddsasgt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinghuilouyu.cn/gtthuzhorq.html

Ruby: rand(1..100)
来源：http://hz.chenjidiqi.icu/gtfzosddkp.html


<!-- 参考信息 -->