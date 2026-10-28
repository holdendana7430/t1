代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.sufxvd.cn/gtrqzamcsk.html

"值: {$a}"
来源：http://hz.quarkkingdee.top/gtijwtiefq.html

[U58] PHP：数组三件套
来源：http://hz.hongshengwenyu.top/gtybawzbiy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.wangshuangyany.cn/gtgugnhszh.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gttqqucdxb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtgaurwnwz.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gtztprxlpa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtobznobcy.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtjzdzkcvv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtejsvfcbk.html

[U62] PHP：日期对象
来源：http://hz.gotoacloud.top/gtpjnnkstg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cucudq.cn/gtjwgirzuw.html

[U63] PHP：文件读写
来源：http://hz.xuetiantiany.cn/gttzjxfvdr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtzmbxiizz.html

[U64] PHP：目录遍历
来源：http://hz.guannengcc.top/gtzcnxseyh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhiwuduotai.top/gtnmwuitti.html

[U65] PHP：会话
来源：http://hz.jiagoushi.top/gtchvhaovm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jyoumei.cn/gtoezrsseh.html

[U66] PHP：设置 Cookie
来源：http://hz.snrcjt.cn/gtziokoisj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gttbkiwmqy.html

[U67] PHP：处理文件上传
来源：http://hz.316326.xyz/gtbxbsglpl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guowangkeji.top/gttpckzjcg.html

[U68] PHP：PDO 连接
来源：http://hz.yuxming.cn/gtjbptiiri.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuanzx.com/gtynrpfrza.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtkjslouud.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtjgrhkalc.html

[U70] PHP：PDO 事务
来源：http://hz.sysykeji.top/gtrkdhivkg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shzxlz.cn/gtajqjujxr.html

[U71] PHP：抛出异常
来源：http://hz.aibaodan.cn/gtpbjxbcwh.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtmksfrwpx.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtltdzthpi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtnnthjlkn.html

[U73] PHP：读取 ini 配置
来源：http://hz.ybcxt.top/gtzanhymjs.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigufen.top/gtpnamvdwn.html

[U74] PHP：读取环境变量
来源：http://hz.zhongyouzk.top/gtvsmrleeq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hywenlv.cn/gtpwcuvswl.html

[U75] PHP：依赖注入
来源：http://hz.ybcxt.top/gtvnpowzkl.html

composer require psr/container
来源：http://hz.nanxuanxn.top/gtazjrucdl.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtjfrbzppt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yj20258888.top/gtzkcuawwq.html

[U77] PHP：模板渲染
来源：http://hz.yuanzhike.top/gtiiqamecw.html

composer require twig/twig
来源：http://hz.shanyushiyangkeji.top/gtccppowda.html

[U78] PHP：单元测试
来源：http://hz.yonumen.top/gtzpnddldn.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtmxdtbxpb.html

[U79] PHP：静态分析
来源：http://hz.cqqwz.cn/gttsuipsgh.html

composer require --dev phpstan/phpstan
来源：http://hz.sweek.top/gticuwgdnq.html

[U80] PHP：代码规范修复
来源：http://hz.mhx1999.top/gtgjbgmqem.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtlxiphrgm.html

[U81] JS：初始化项目
来源：http://hz.snrcjt.cn/gthswaqqip.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtitrubvwu.html

[U82] JS：package.json 脚本
来源：http://hz.shuidangran.top/gtivaxftzl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zycfv.cn/gtelfezinv.html

[U83] JS：ES Module 导入导出
来源：http://hz.redwolf501.top/gtgilnnrbk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gzhubu.top/gthmuvsofc.html

[U84] JS：CommonJS 写法
来源：http://hz.svipenyu.cn/gtnhxdgdlb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xziqi.cn/gtnfkwvxnh.html

[U85] JS：可选链
来源：http://hz.redwolf501.top/gtbswfckxa.html

a?.b?.c
来源：http://hz.nwbrower.top/gtetwhpyxc.html

[U86] JS：空值合并
来源：http://hz.xylfe.cn/gtwctwjude.html

a ?? b
来源：http://hz.jianghu66.top/gtdryjchgp.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangkeji.top/gtuudgeoni.html

const { a = 1, b = 2 } = obj;
来源：http://hz.feifeiyinyue.top/gtfnyjyjkz.html

[U88] JS：对象展开合并
来源：http://hz.sufxvd.cn/gtefluwsta.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtgskslfxe.html

[U89] JS：数组去重
来源：http://hz.smart0.xyz/gtjvqehnuu.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtxfxayaoy.html

[U90] JS：数字数组排序
来源：http://hz.gzhubu.top/gtugfycdvs.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtmiaxzamm.html

[U91] JS：对象键值遍历
来源：http://hz.sufxvd.cn/gtwnguhfqm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.pengpengdd.cyou/gtoserzdwh.html

[U92] JS：深拷贝
来源：http://hz.yj202588.top/gtiadcddcn.html

structuredClone(obj)
来源：http://hz.gogol.net.cn/gtawhjhxln.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtsynglegb.html

`共 ${n} 条`
来源：http://hz.tian-w.cn/gtsznxgycq.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtzkrpbwjh.html

const double = x => x * 2;
来源：http://hz.pengpengdd.cyou/gtiqgrnfuy.html

[U95] JS：Promise 包装
来源：http://hz.svipenyu.cn/gttztwvddc.html

new Promise((resolve, reject) => {})
来源：http://hz.haohaochexian.top/gtxfrxfpny.html

[U96] JS：async/await 与异常
来源：http://hz.sysykeji.top/gtpdwdkemz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtkiyohpru.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtwizedltc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtkhjdowco.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtzpxrowrq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtmtygokjl.html

[U99] JS：事件监听
来源：http://hz.iojbl.cn/gtugesqzql.html

el.addEventListener("click", e => {})
来源：http://hz.aibaodan.cn/gtssrgyxjf.html

[U100] JS：DOM 查询
来源：http://hz.hongshengwenyu.top/gtzlltmtre.html

document.querySelector(".item")
来源：http://hz.sysykeji.top/gtysfadbgl.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gtxtgjeqlg.html

el.classList.toggle("active")
来源：http://hz.xingfuxueyuan.xyz/gtuznrvwoh.html

[U102] JS：本地存储
来源：http://hz.meibo888.top/gtqnsrqqlu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnxiangtu.top/gtgkmikgqk.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtfefuktyv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhijiandao.cn/gtdahvmmrj.html

[U104] JS：防抖
来源：http://hz.nwbrower.top/gtolqbwacb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtzqmlxims.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gttvedkmfq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.fzhhl.top/gtkmuhsbre.html

[U106] JS：日期格式化
来源：http://hz.yueranfly.top/gtgsediydq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.vqdsnc.cn/gtusifexpz.html

[U107] JS：数字千分位
来源：http://hz.jinqigufen.top/gthoxpvgot.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yueranfly.top/gtswemitwn.html

[U108] JS：随机整数
来源：http://hz.gogol.net.cn/gtbgntggzk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangshuangyany.cn/gtkuxqevip.html

[U109] JS：数组分组
来源：http://hz.fengsongda.top/gteagrurvq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtychsuusn.html

[U110] JS：数组分块
来源：http://hz.9152youxi.cn/gtczfnsaso.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cucudq.cn/gtugaxuxzp.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtnmbmkzmh.html

new Map(Object.entries(obj))
来源：http://hz.cucudq.cn/gtghtjqmfx.html

[U112] JS：字符串补位
来源：http://hz.ehwqpu.com/gteynxrait.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtgsjcdxdm.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gtwkszrfya.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtreonibtc.html

[U114] JS：JSON 深比较
来源：http://hz.hfpthk.cn/gtpnjwuzpv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gttjxmshqy.html

[U115] JS：生成 UUID
来源：http://hz.pengpengdd.cyou/gtyvexcyzq.html

crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtnzcxzull.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtrlgyhqfp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yanxiufei.cn/gtcoefksta.html

[U117] JS：单元测试
来源：http://hz.hnqzz.top/gtiiqadiuc.html

npm i -D vitest;  npx vitest
来源：http://hz.gaohongyu789.top/gttodemyod.html

[U118] JS：开发服务器
来源：http://hz.aibaodan.cn/gtiumrkwlm.html

npm i -D vite;  npx vite
来源：http://hz.fengsongda.top/gtxzcrcnxg.html

[U119] JS：生产构建
来源：http://hz.jinqigufen.top/gtsvwmahuy.html

npx vite build
来源：http://hz.daxiang520.top/gttuuuemux.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hywenlv.cn/gtfbokpznz.html

import.meta.env.VITE_API_URL
来源：http://hz.zhijiandao.cn/gtunnljrpg.html

================================================================================
来源：http://hz.iojbl.cn/gtkdotqiiw.html

统计汇总
来源：http://hz.yueranfly.top/gtozwjdbcf.html

================================================================================
来源：http://hz.52xcode.cn/gtgwsclzoj.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtdaokegck.html

Python ......... 252
来源：http://hz.xziqi.cn/gtxysnsokg.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtidgvakyu.html

JavaScript ..... 252
来源：http://hz.havefunace.top/gtlpjxqeui.html

TypeScript ..... 212
来源：http://hz.quarkkingdee.top/gtobxcjkxa.html

Java ........... 212
来源：http://hz.jianghu66.top/gtjnfcjyiy.html

Go ............. 212
来源：http://hz.xuanzx.com/gtrxhsvhfq.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtdugekptm.html

C# ............. 212
来源：http://hz.sxryk.cn/gttpfhtzep.html

C .............. 30
来源：http://hz.iojbl.cn/gtwsibckhj.html

C++ ............ 30
来源：http://hz.dianchejie.cn/gtpzmpqgcj.html

SQL ............ 90
来源：http://hz.yueranfly.top/gtnecjrdyg.html

Bash ........... 80
来源：http://hz.dianchejie.cn/gtxcceoevj.html

Kotlin ......... 15
来源：http://hz.quarkkingdee.top/gtsqalthjx.html

Swift .......... 15
来源：http://hz.hnxiangtu.top/gthywbfsuh.html

Lua ............ 10
来源：http://hz.pycfn.com/gtcixnlqeh.html

Perl ........... 10
来源：http://hz.birdmap.top/gttsxhpjsm.html

Scala .......... 10
来源：http://hz.316326.xyz/gtafzldhhe.html

------------------------------------
来源：http://hz.andypj.xyz/gtmxergauz.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtzyxopheq.html

按章节统计：
来源：http://hz.xylfe.cn/gtzwdxrhyd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtvouaupmi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yongpay.top/gteldjqylk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtylyvjctp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtermscnfs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aibaodan.cn/gtkxhbxpvi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tanke756.top/gtymcvfpbj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtafxnpvai.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtavuciqbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtphbxiwzi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.feifeiyinyue.top/gtmapxmnts.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtzqlgtyqn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gttzjloinl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtjyohgeya.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.tian-w.cn/gtpzzxvzek.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jlsjyb.cn/gtjjzcainy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtcinmrqij.html

Q SQL 专题                              90
来源：http://hz.zhaomingkeji.xyz/gtgrkmjecq.html

R Bash 专题                             80
来源：http://hz.zycfv.cn/gtfpnwplkz.html

S C / C++ 专题                          60
来源：http://hz.andypj.xyz/gteuovmruq.html

T 其他语言补充                          60
来源：http://hz.shangyingyoupin.top/gtikcqywgz.html

U 高频实用片段                         120
来源：http://hz.mhx1999.top/gtizubuxsz.html

------------------------------------
来源：http://hz.yueranfly.top/gtrowoltnx.html

合计                                  2106 条
来源：http://hz.tanke756.top/gtwpefbylz.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtznmrndli.html

使用提醒
来源：http://hz.xziqi.cn/gtprcymqkr.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gttywekigz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xylfe.cn/gtttmgfxbp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sxryk.cn/gtiwucekmn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shanyushiyangtech.top/gtzndyqlrt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtvswxnvbn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.nwbrower.top/gtuowuxsdb.html

—— 文件结束 ——
来源：http://hz.yanxiufei.cn/gtzkbwdftb.html

================================================================================
来源：http://hz.nwbrower.top/gtgwwkxehq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydzc1.top/gtckrbewlr.html

Common Programming Examples Cheat Book
来源：http://hz.jyoumei.cn/gteqvjjfqv.html

================================================================================
来源：http://hz.meibo888.top/gtlngmdibk.html

【收录内容】
来源：http://hz.mhx1999.top/gtzpwafylj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.redwolf501.top/gtjlzllvbr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nwbrower.top/gtjbsbjfnq.html

SQL · Bash · C · C++
来源：http://hz.shanyushiyangkeji.top/gtlbnoqtlx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydjk.org.cn/gtxtqqbkdl.html

【使用说明】
来源：http://hz.jqgufenzy.top/gthlsddrtj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gtspdbzmyv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtrlnvlkft.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj202588.top/gtsqtzrvbc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.wangshuangyany.cn/gtbkciipxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yvedp.cn/gtmhwmmrcq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sweek.top/gtrxrywgul.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cashguo.top/gtronvyvxb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtfhqwmbit.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnqzz.top/gtqegsyuuy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.smart0.xyz/gtkvhujtms.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.cqqwz.cn/gttwjsanpl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ywan-chungtsiang.top/gtoltckgvt.html

【文件统计】
来源：http://hz.cucudq.cn/gtoyebvhkf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gtwoshbpnu.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtazgpwudu.html

目  录
来源：http://hz.mhx1999.top/gthokztagf.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtmxbpwvxa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.redwolf501.top/gttbhxcqqw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtqdutocja.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtrfqxwslm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aibaodan.cn/gtwpcolqnx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aibaodan.cn/gtjusaijgw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenjidiqi.icu/gtbghixhwd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtqvwhfwgl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yvedp.cn/gtacydhxfr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtpsptibzz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sweek.top/gtorxxxuoj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gthwpyuljx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtadzvsotc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtrynqtxce.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtschuewdi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.svipenyu.cn/gtzsdwxuaw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtdoqgbqrk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jyoumei.cn/gtikvlgtgg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gzhubu.top/gtbjrsljwt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shangyingyoupin.top/gtamufkthe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtwnkmswtp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtdbkyqisd.html

================================================================================
来源：http://hz.cdnleiting.top/gtlfmtakyd.html

A. 基础语法与类型
来源：http://hz.jiagoushi.top/gtdxosutcs.html

================================================================================
来源：http://hz.yangfankeji.com/gtddfqdyvx.html

[A01] Hello World
来源：http://hz.gogol.net.cn/gtjfgbzyec.html

Py:   print("Hello, World!")
来源：http://hz.dianchejie.cn/gtruiqkttq.html

PHP:  echo "Hello, World!";
来源：http://hz.yj202588.top/gteiyngkbm.html

JS:   console.log("Hello, World!");
来源：http://hz.fzhhl.top/gtxcwjsavq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xuanzx.com/gtzhgycnkx.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj20258.top/gtcpliuwur.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sysykeji.top/gtwgmnllci.html

Ruby: puts "Hello, World!"
来源：http://hz.zhongyouzk.top/gtzwvzgffo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258888.top/gttblqosxg.html

[A02] 变量声明与赋值
来源：http://hz.zhijiandao.cn/gtacpkxwtg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.havefunace.top/gtnkvsmars.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.wangdashe.top/gtrusntpcw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtijpphwhb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.feifeiyinyue.top/gtmmlitend.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gtmdmoxdyl.html

Go:   name := "Alex"; age := 20
来源：http://hz.pycfn.com/gtswglgfcr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jianghu66.top/gtumvqtlpm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.snrcjt.cn/gtzddwnjmy.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtecstfmyu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hnqzz.top/gteqncmiuy.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtojoouifa.html

JS:   const PI = 3.14159;
来源：http://hz.c1oappe.top/gtxllpkxdy.html

TS:   const PI: number = 3.14159;
来源：http://hz.shangyingyoupin.top/gtosziwvbt.html

Java: static final double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtipqadjgc.html

Go:   const PI = 3.14159
来源：http://hz.zhengqikj.top/gtmcxtyyyg.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtvfezpuam.html

C#:   const double PI = 3.14159;
来源：http://hz.yj202588.top/gtiaekxsae.html

[A04] 判断变量类型
来源：http://hz.snrcjt.cn/gtezbboukd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.feifeiyinyue.top/gtsorjavfc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fengsongda.top/gtvdxziufh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aizwys.cn/gtruokdspi.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnqzz.top/gtaujphqzd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhongyouzk.top/gtctkuyqqx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.aizwys.cn/gtrhgekwov.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hnqzz.top/gtyjptamse.html

C#:   x.GetType().Name; x is int
来源：http://hz.nwbrower.top/gtgjtwvnxj.html

[A05] 整数除法与取模
来源：http://hz.gotoacloud.top/gtsizdbfyu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tanke756.top/gtveszawgh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.chenjidiqi.icu/gtclbbgjoc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtuczftyph.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtbavfmntq.html

Java: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtbyvduhxs.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gtupunhftd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtiglkzgsl.html

C#:   7 / 2; 7 % 2
来源：http://hz.yangfankeji.com/gtsfxfqfzy.html

[A06] 字符串转数字
来源：http://hz.birdmap.top/gtycyoabig.html

Py:   int("42"); float("3.14")
来源：http://hz.pycfn.com/gtqctgmtdv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ivvv.top/gtyxmuzltq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.316326.xyz/gtwfvsqexe.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jqgufenzy.top/gtmeeruvrh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.quarkkingdee.top/gtwgeeppph.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hywenlv.cn/gtouvnywcf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yanxiufei.cn/gtukyoiqvs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pycfn.com/gtjlpvivxt.html

[A07] 数字转字符串
来源：http://hz.quarkkingdee.top/gtxsrxqfhi.html

Py:   str(42)
来源：http://hz.snrcjt.cn/gtoowkjpfk.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhixingplan.top/gtxzcegqtm.html

JS:   String(42); (42).toString()
来源：http://hz.wangshuangyany.cn/gtlhsvgxzt.html

TS:   String(42)
来源：http://hz.shanyushiyangkeji.top/gtvoeqzsha.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sweek.top/gttjwprzos.html

Go:   strconv.Itoa(42)
来源：http://hz.jinqigufen.top/gtuzfksnbq.html

Ruby: 42.to_s
来源：http://hz.dianchejie.cn/gtnslzviya.html

C#:   42.ToString()
来源：http://hz.yvedp.cn/gtfeulfxkt.html

[A08] 取整与四舍五入
来源：http://hz.bjfxy.top/gtvuenuwwv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yongpay.top/gtrktaxzqi.html


<!-- 参考信息 -->