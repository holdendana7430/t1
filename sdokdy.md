代发 wailian999

[U55] PHP：match 表达式
来源：http://hz.cheryme.top/gtcmnvvxun.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhoulong.xyz/gtobmdwzpg.html

[U56] PHP：命名参数
来源：http://hz.0kj1m.cn/gtxtnatspw.html

f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtsftndfgw.html

[U57] PHP：字符串插值
来源：http://hz.hywenlv.cn/gtiteqlhll.html

"值: {$a}"
来源：http://hz.ydzc1.top/gtvidbdauw.html

[U58] PHP：数组三件套
来源：http://hz.jinghuilouyu.cn/gtvogzrbwq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gogol.net.cn/gtjmbfoldo.html

[U59] PHP：自定义排序
来源：http://hz.dianchejie.cn/gtrccnwigb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtsfikjvov.html

[U60] PHP：JSON 编解码
来源：http://hz.ywan-chungtsiang.top/gtztcwfphu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shzxlz.cn/gtogjebcnn.html

[U61] PHP：正则
来源：http://hz.yuxming.cn/gtujregfgq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtkcawfcnz.html

[U62] PHP：日期对象
来源：http://hz.aizwys.cn/gtfgmkoruf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guannengcc.top/gtozazyvrg.html

[U63] PHP：文件读写
来源：http://hz.yvedp.cn/gtdlbfqmna.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtodnwesee.html

[U64] PHP：目录遍历
来源：http://hz.9152youxi.cn/gtwxyqcibk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.snrcjt.cn/gtlljcdfop.html

[U65] PHP：会话
来源：http://hz.meibo888.top/gtbgzgngww.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gtcsrsdkmw.html

[U66] PHP：设置 Cookie
来源：http://hz.cdnleiting.top/gtilyszhxz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nwbrower.top/gtqyhxxgnh.html

[U67] PHP：处理文件上传
来源：http://hz.wangdashe.top/gtmvvufwrq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.daxiang520.top/gtosubugru.html

[U68] PHP：PDO 连接
来源：http://hz.gotoacloud.top/gtqzrfwvdt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yuxming.cn/gtqzxswbfm.html

[U69] PHP：PDO 预处理
来源：http://hz.yj20258.top/gtxodqufgg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuanzhike.top/gtqhxcofks.html

[U70] PHP：PDO 事务
来源：http://hz.jqgfzy.top/gtpnmfcpjd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangtech.top/gtkuakiubj.html

[U71] PHP：抛出异常
来源：http://hz.jiagoushi.top/gtlmrvodua.html

throw new RuntimeException("失败", 500);
来源：http://hz.shzxlz.cn/gtwgrlbhsh.html

[U72] PHP：写错误日志
来源：http://hz.nanxinkj.top/gthncnrfpc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sweek.top/gttlfsztzq.html

[U73] PHP：读取 ini 配置
来源：http://hz.yangfankeji.com/gtbcmdsvqf.html

parse_ini_file("config.ini", true)
来源：http://hz.fengsongda.top/gtkwfquadb.html

[U74] PHP：读取环境变量
来源：http://hz.yj20258888.top/gtljejchrs.html

getenv("APP_ENV") ?: "production"
来源：http://hz.feifeiyinyue.top/gtfgfsqcaj.html

[U75] PHP：依赖注入
来源：http://hz.xuetiantiany.cn/gtxsaiyape.html

composer require psr/container
来源：http://hz.wangdashe.top/gtvcpluznv.html

[U76] PHP：简单路由
来源：http://hz.tian-w.cn/gtquxroaar.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ppjwa.cn/gtkwdhamez.html

[U77] PHP：模板渲染
来源：http://hz.hnxiangtu.top/gtxwedsdvi.html

composer require twig/twig
来源：http://hz.yj20258888.top/gtqreluens.html

[U78] PHP：单元测试
来源：http://hz.cdnleiting.top/gtktkmfzsj.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigfzy.top/gtprmpksja.html

[U79] PHP：静态分析
来源：http://hz.yonumen.top/gtodwwjogc.html

composer require --dev phpstan/phpstan
来源：http://hz.tian-w.cn/gtbycplwrc.html

[U80] PHP：代码规范修复
来源：http://hz.jqgufenzy.top/gtmepxxeof.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.dianchejie.cn/gttuqgkqvf.html

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gtgcykvrer.html

npm init -y;  npm i express
来源：http://hz.wangdashe.top/gtkjlarjhv.html

[U82] JS：package.json 脚本
来源：http://hz.cheryme.top/gtesmqgafl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ydjk.org.cn/gtcnebvvgb.html

[U83] JS：ES Module 导入导出
来源：http://hz.tanke756.top/gtzxztqelp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ehwqpu.com/gthudvwbdo.html

[U84] JS：CommonJS 写法
来源：http://hz.ivvv.top/gtzngolxsg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.mhx1999.top/gthwloexgf.html

[U85] JS：可选链
来源：http://hz.nanxinkj.top/gtxfuspwnf.html

a?.b?.c
来源：http://hz.ppjwa.cn/gtumrfloay.html

[U86] JS：空值合并
来源：http://hz.hfpthk.cn/gtpopordag.html

a ?? b
来源：http://hz.yonumen.top/gtmfzwkiyo.html

[U87] JS：解构默认值
来源：http://hz.chenjidiqi.icu/gtejejurkb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gtwzrrkepk.html

[U88] JS：对象展开合并
来源：http://hz.andypj.xyz/gtumduoxco.html

{ ...a, ...b }
来源：http://hz.c1oappe.top/gtldizxaxb.html

[U89] JS：数组去重
来源：http://hz.yanxiufei.cn/gtreqtgdcq.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gthzjvcblb.html

[U90] JS：数字数组排序
来源：http://hz.haohaochexian.top/gtxtsngfzc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtspkceswz.html

[U91] JS：对象键值遍历
来源：http://hz.cashguo.top/gtkwcfulhi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cdnleiting.top/gtagnudzxs.html

[U92] JS：深拷贝
来源：http://hz.nanxuanxn.top/gtwtyycwen.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtnrqgzend.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangkeji.top/gtvussbaos.html

`共 ${n} 条`
来源：http://hz.yangfankeji.com/gtnnxxgame.html

[U94] JS：箭头函数
来源：http://hz.fzhhl.top/gtaymijgnn.html

const double = x => x * 2;
来源：http://hz.shangyingyoupin.top/gtpmzprpjg.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtfqploeks.html

new Promise((resolve, reject) => {})
来源：http://hz.52xcode.cn/gtlkrqfuma.html

[U96] JS：async/await 与异常
来源：http://hz.c1oappe.top/gtvnmzcfhu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtrgyulgff.html

[U97] JS：并发请求
来源：http://hz.hysaishi.cn/gtdqkzvedz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtgdhiqbox.html

[U98] JS：fetch 带 JSON
来源：http://hz.ehwqpu.com/gtwhwefnvp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ivvv.top/gtrchbviwc.html

[U99] JS：事件监听
来源：http://hz.chenlongwang.top/gtrdnkapqt.html

el.addEventListener("click", e => {})
来源：http://hz.kuanghao11.cn/gtsyucthph.html

[U100] JS：DOM 查询
来源：http://hz.hongshengwenyu.top/gtnocsshpm.html

document.querySelector(".item")
来源：http://hz.daria6918.cn/gtqcwgqzqu.html

[U101] JS：classList 操作
来源：http://hz.chenzaomai.com/gtqkjvnddq.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gtoirhpvnn.html

[U102] JS：本地存储
来源：http://hz.xinyue.icu/gtollleocd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigufen.top/gtkyysrpeb.html

[U103] JS：定时器
来源：http://hz.zhaomingkeji.xyz/gtsbsnsror.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.feifeiyinyue.top/gtcbhcinnl.html

[U104] JS：防抖
来源：http://hz.hysaishi.cn/gtqrwrdgpa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtkteaiflv.html

[U105] JS：节流
来源：http://hz.xziqi.cn/gtqnmwjvfz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gogol.net.cn/gtvmubctlg.html

[U106] JS：日期格式化
来源：http://hz.birdmap.top/gtotfgshyq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tanke756.top/gtvsahoscw.html

[U107] JS：数字千分位
来源：http://hz.xylfe.cn/gtszgibapr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtkqznblzd.html

[U108] JS：随机整数
来源：http://hz.jyoumei.cn/gtxjwzltlz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.iojbl.cn/gtqwpiibuj.html

[U109] JS：数组分组
来源：http://hz.shanyushiyangtech.top/gtlwmcrcfw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtwxftqzin.html

[U110] JS：数组分块
来源：http://hz.meibo888.top/gtfbkvvynz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sxryk.cn/gtailflpiy.html

[U111] JS：对象转 Map
来源：http://hz.zhongyouzk.top/gteqdedtep.html

new Map(Object.entries(obj))
来源：http://hz.yj20258888.top/gtnftesuxm.html

[U112] JS：字符串补位
来源：http://hz.nanxuanxn.top/gtpaqdjsji.html

"7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gteftfkrfb.html

[U113] JS：正则替换全部
来源：http://hz.cheryme.top/gtwwlpdclg.html

s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtzcngezas.html

[U114] JS：JSON 深比较
来源：http://hz.mhx1999.top/gtutfcswkr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhoulong.xyz/gtpyzcrvxf.html

[U115] JS：生成 UUID
来源：http://hz.wangshuangyany.cn/gtduxhghlf.html

crypto.randomUUID()
来源：http://hz.birdmap.top/gtztcvocaa.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.9152youxi.cn/gtlhyjdprw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yueranfly.top/gtjutyybqp.html

[U117] JS：单元测试
来源：http://hz.ydzc1.top/gtrttswwfq.html

npm i -D vitest;  npx vitest
来源：http://hz.zhijiandao.cn/gtfeipbibm.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gtiryldjne.html

npm i -D vite;  npx vite
来源：http://hz.guowangkeji.top/gtjngaashg.html

[U119] JS：生产构建
来源：http://hz.guannengcc.top/gtezzmztbb.html

npx vite build
来源：http://hz.ivvv.top/gtzwjharui.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.havefunace.top/gtnhuuzbsd.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtpwnxczqj.html

================================================================================
来源：http://hz.dashuyun.cn/gtigmyjctv.html

统计汇总
来源：http://hz.quarkkingdee.top/gtdlnfhvxl.html

================================================================================
来源：http://hz.yueranfly.top/gtxicjbbtn.html

按语言统计（条）：
来源：http://hz.gotoacloud.top/gtqswsajje.html

Python ......... 252
来源：http://hz.zhixingplan.top/gtuilqeyqu.html

PHP ............ 252
来源：http://hz.chenzaomai.com/gtxraqvlky.html

JavaScript ..... 252
来源：http://hz.tian-w.cn/gteiodzdzw.html

TypeScript ..... 212
来源：http://hz.hywenlv.cn/gtvmtuwdtx.html

Java ........... 212
来源：http://hz.hammf.cn/gtazwrzdbu.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gthrguczpn.html

Ruby ........... 212
来源：http://hz.yonumen.top/gtvxgwmxvn.html

C# ............. 212
来源：http://hz.0kj1m.cn/gtrymtdrph.html

C .............. 30
来源：http://hz.zhongyouzk.top/gtrqkxdfob.html

C++ ............ 30
来源：http://hz.c1oappe.top/gtvgadwocc.html

SQL ............ 90
来源：http://hz.daxiang520.top/gtlyosaudj.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtfuxofzwf.html

Kotlin ......... 15
来源：http://hz.cdnleiting.top/gtpadwocfw.html

Swift .......... 15
来源：http://hz.guannengcc.top/gtttisorqm.html

Lua ............ 10
来源：http://hz.zhixingplan.top/gtryywidnu.html

Perl ........... 10
来源：http://hz.hammf.cn/gtuucrnqjp.html

Scala .......... 10
来源：http://hz.9152youxi.cn/gtpaxmaajs.html

------------------------------------
来源：http://hz.xylfe.cn/gttmzyjhlr.html

合计 ........... 2106 条
来源：http://hz.jyoumei.cn/gtqurgcggi.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtytijcvlk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtsztcepuc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtlairfshh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtyzejjokk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gtqupagzal.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhoulong.xyz/gtbxdijmym.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtklzmulbj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtaqoauzcd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtmjayiwij.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtcbkqesbd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtgeajdpqw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtkbodnhkd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtijsivlba.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtsouxvgji.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtgkjggibr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tianlin.xyz/gtztmiivqw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtgrmclosq.html

Q SQL 专题                              90
来源：http://hz.tanke756.top/gtcwxraiik.html

R Bash 专题                             80
来源：http://hz.guowangkeji.top/gtdvydtage.html

S C / C++ 专题                          60
来源：http://hz.yuanzhike.top/gtrgxxftxk.html

T 其他语言补充                          60
来源：http://hz.smart0.xyz/gtzqjlkxcn.html

U 高频实用片段                         120
来源：http://hz.jinghuilouyu.cn/gtduenynnj.html

------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtoxofipfx.html

合计                                  2106 条
来源：http://hz.gogol.net.cn/gtzoipuqnc.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtajsaiezt.html

使用提醒
来源：http://hz.nanxinkj.top/gtwcieateo.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtmfywgqqj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cheryme.top/gtlcsknsbo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.52xcode.cn/gtwlbghvmg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtsjcncfpj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shanyushiyangtech.top/gthjonmvwv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shangyingyoupin.top/gtgbhbxrnn.html

—— 文件结束 ——
来源：http://hz.svipenyu.cn/gtsqezvepf.html

================================================================================
来源：http://hz.fzhhl.top/gtddlghmfh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ybcxt.top/gtcznyehsq.html

Common Programming Examples Cheat Book
来源：http://hz.dianchejie.cn/gtifvgzkzk.html

================================================================================
来源：http://hz.jinqigufen.top/gtzmgnpagj.html

【收录内容】
来源：http://hz.zhengqikj.top/gtjvfefvfp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.smart0.xyz/gtcagwccwd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ehwqpu.com/gtbnuyhgnf.html

SQL · Bash · C · C++
来源：http://hz.zhongyouzk.top/gtgfzezagx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ywan-chungtsiang.top/gtfhbwpdvl.html

【使用说明】
来源：http://hz.sufxvd.cn/gtcsscaonj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgufenzy.top/gtnjodcgie.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cucudq.cn/gtuxirkpas.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinqigfzy.top/gtbaebibdd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dashuyun.cn/gtyskkwkis.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtinmwffkw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhixingplan.top/gtshbplakk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinqigfzy.top/gtsyvopzow.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.svipenyu.cn/gtikerrrrz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtrsxrmvvn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.pycfn.com/gtevntpqwe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yonumen.top/gtoetrnbxc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.haohaochexian.top/gtvvykioyv.html

【文件统计】
来源：http://hz.shanyushiyangkeji.top/gtscdgcpfs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gthbnfzshb.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtgjkecesl.html

目  录
来源：http://hz.dianchejie.cn/gtmkingmac.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gtbqlgzjlw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.meibo888.top/gtyaztsmnr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtczojmxul.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtboslshtd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtrtcfdxrb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhoulong.xyz/gtzgyrbrwd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hysaishi.cn/gtvsihmrjt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtborcxzuy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258888.top/gtsttqinlr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtanbkikgk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtbvhgpwwa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtjffheiuy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtmuvikfvx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gturcztwwy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.quarkkingdee.top/gtnbnkhjyd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shuidangran.top/gtlihlxrcu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtokvqrxbg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jyoumei.cn/gtgpjfyoci.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhongyouzk.top/gtveywtlat.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ehwqpu.com/gtcendlcip.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtbgyiknsp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtslwajcut.html

================================================================================
来源：http://hz.birdmap.top/gtibcnbjnc.html

A. 基础语法与类型
来源：http://hz.xuetiantiany.cn/gtpuclwtrw.html

================================================================================
来源：http://hz.mhx1999.top/gtkztxrjqp.html

[A01] Hello World
来源：http://hz.ydzc1.top/gtrfedcwau.html

Py:   print("Hello, World!")
来源：http://hz.cheryme.top/gtkwxvkqta.html

PHP:  echo "Hello, World!";
来源：http://hz.wangdashe.top/gtqgyuugrv.html

JS:   console.log("Hello, World!");
来源：http://hz.ivvv.top/gtffyhpbfp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhiwuduotai.top/gtuxkkdqxz.html

Java: System.out.println("Hello, World!");
来源：http://hz.andypj.xyz/gtirrglptj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hnqzz.top/gtlxhifgfx.html

Ruby: puts "Hello, World!"
来源：http://hz.gzhubu.top/gtslsckgtn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gzhubu.top/gtfrnjeryx.html

[A02] 变量声明与赋值
来源：http://hz.dianchejie.cn/gtvfmyzltc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuanzhike.top/gtkelxgiry.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.daria6918.cn/gtyewwytcr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.daria6918.cn/gtipviarer.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ywan-chungtsiang.top/gtivvdiiyh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.guowangkeji.top/gtxrhgcrpt.html

Go:   name := "Alex"; age := 20
来源：http://hz.yangfankeji.com/gtgbwxacek.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj202588.top/gtitrpovyc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.quarkkingdee.top/gtuasyquyi.html

[A03] 常量定义
来源：http://hz.xinyue.icu/gtguhqiwpi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.smart0.xyz/gtvyblzmrh.html

PHP:  const PI = 3.14159;
来源：http://hz.dianchejie.cn/gtmtlvqegu.html

JS:   const PI = 3.14159;
来源：http://hz.ivvv.top/gtilccuzvg.html

TS:   const PI: number = 3.14159;
来源：http://hz.cheryme.top/gtqocptufe.html

Java: static final double PI = 3.14159;
来源：http://hz.tian-w.cn/gtutvuvojp.html

Go:   const PI = 3.14159
来源：http://hz.316326.xyz/gtiyjmdzss.html

Ruby: PI = 3.14159
来源：http://hz.gzhubu.top/gtktbwhzmh.html

C#:   const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtezfxqrcw.html

[A04] 判断变量类型
来源：http://hz.zycfv.cn/gtofjufknh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gtkzdbtuow.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fzhhl.top/gtrgxnvdcd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yonumen.top/gtmfbbxlvs.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj20258.top/gtrwunmxdy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhongyouzk.top/gtkhcoiszk.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cheryme.top/gtunxckzyf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cucudq.cn/gtzsqfukfn.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtwayesqnx.html

[A05] 整数除法与取模
来源：http://hz.ehwqpu.com/gtkwleknnh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.sufxvd.cn/gtgjkvgynl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hongshengwenyu.top/gtwbdhalda.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhongyouzk.top/gtpdidgiga.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtpgmqlqad.html

Java: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtsxhogxjn.html

Go:   7 / 2; 7 % 2
来源：http://hz.sweek.top/gtbvlgthcw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gthaaafviu.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtonlnhhxq.html

[A06] 字符串转数字
来源：http://hz.nanxuanxn.top/gtbbaxvjza.html

Py:   int("42"); float("3.14")
来源：http://hz.hywenlv.cn/gtcxiqupfv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.vqdsnc.cn/gtaejqvyjr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shzxlz.cn/gtkqwclwvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.aizwys.cn/gtqfxzerzc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cqqwz.cn/gthrvllitp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pycfn.com/gtxexuwxfx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xylfe.cn/gtmrrexyht.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.aibaodan.cn/gtjqdmjmwv.html

[A07] 数字转字符串
来源：http://hz.hongshengwenyu.top/gtltsfwqgz.html

Py:   str(42)
来源：http://hz.zhoulong.xyz/gtcyuspstb.html

PHP:  (string) 42; strval(42)
来源：http://hz.ydzc1.top/gtgvvgdliy.html

JS:   String(42); (42).toString()
来源：http://hz.zhixingplan.top/gtawqwzwxv.html

TS:   String(42)
来源：http://hz.shuidangran.top/gtpvwbfqua.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yuanzhike.top/gtymkdnvwj.html

Go:   strconv.Itoa(42)
来源：http://hz.jyoumei.cn/gtnyhvluwt.html


<!-- 参考信息 -->