代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gtzrqotaaw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtyzlszasr.html

[U60] PHP：JSON 编解码
来源：http://hz.gogol.net.cn/gtjbfcsnee.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gthjsaixbr.html

[U61] PHP：正则
来源：http://hz.snrcjt.cn/gtycbeoiry.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtwbhpfnjc.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtcegzcnjy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tianlin.xyz/gtdshbtcaj.html

[U63] PHP：文件读写
来源：http://hz.cdnleiting.top/gtituravvk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sweek.top/gtbypilcih.html

[U64] PHP：目录遍历
来源：http://hz.tianlin.xyz/gtbpzmzjze.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinqigufen.top/gtqihhylhp.html

[U65] PHP：会话
来源：http://hz.yj202588.top/gtsknbsybj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtkvtvrqhh.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtqakqexix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yueranfly.top/gtqsukizfz.html

[U67] PHP：处理文件上传
来源：http://hz.zhiwuduotai.top/gtcdsfdsse.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhengqikj.top/gttlslyzby.html

[U68] PHP：PDO 连接
来源：http://hz.yvedp.cn/gtwjpplxrm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.guowangkeji.top/gtmptxpuyp.html

[U69] PHP：PDO 预处理
来源：http://hz.wangdashe.top/gteogtrnsa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yongpay.top/gtswagciaq.html

[U70] PHP：PDO 事务
来源：http://hz.yuxming.cn/gtzrjahdrc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ehwqpu.com/gtquynwpij.html

[U71] PHP：抛出异常
来源：http://hz.yvedp.cn/gtjiblfyjl.html

throw new RuntimeException("失败", 500);
来源：http://hz.yvedp.cn/gtjzmztokl.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gtagyxtgmx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ybcxt.top/gtnslcykpc.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gtrjeuefal.html

parse_ini_file("config.ini", true)
来源：http://hz.zhaomingkeji.xyz/gtgsgsflod.html

[U74] PHP：读取环境变量
来源：http://hz.vqdsnc.cn/gtzhaldyrb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenlongwang.top/gteevpbxbq.html

[U75] PHP：依赖注入
来源：http://hz.yuanzhike.top/gtnecfrgao.html

composer require psr/container
来源：http://hz.chenzaomai.com/gtavgyqsaf.html

[U76] PHP：简单路由
来源：http://hz.jlsjyb.cn/gtrkryjhen.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhixingplan.top/gtvnccdsgx.html

[U77] PHP：模板渲染
来源：http://hz.jinqigfzy.top/gtuxpxqbjt.html

composer require twig/twig
来源：http://hz.yuanzhike.top/gtkcszuezr.html

[U78] PHP：单元测试
来源：http://hz.xingfuxueyuan.xyz/gtcgphleke.html

composer require --dev phpunit/phpunit
来源：http://hz.shangyingyoupin.top/gtoitiyqyl.html

[U79] PHP：静态分析
来源：http://hz.gotoacloud.top/gtdfqmyunq.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtldycznco.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gtyqthadrf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hammf.cn/gtwtoozgaw.html

[U81] JS：初始化项目
来源：http://hz.jinyuanbaomall.cn/gtfgsqcdcw.html

npm init -y;  npm i express
来源：http://hz.xylfe.cn/gtdqjhaydl.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangtech.top/gtsazwubcs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtbpgetauv.html

[U83] JS：ES Module 导入导出
来源：http://hz.ehwqpu.com/gtfhpxxdvf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gthctgubfz.html

[U84] JS：CommonJS 写法
来源：http://hz.iojbl.cn/gtptxrmlem.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dashuyun.cn/gtnmqzswta.html

[U85] JS：可选链
来源：http://hz.hammf.cn/gtpdtmiynq.html

a?.b?.c
来源：http://hz.yueranfly.top/gtruwlpaes.html

[U86] JS：空值合并
来源：http://hz.yangfankeji.com/gtqmzrivfz.html

a ?? b
来源：http://hz.pengpengdd.cyou/gtybygbppv.html

[U87] JS：解构默认值
来源：http://hz.gogol.net.cn/gtcmnkpxcp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cheryme.top/gtndwuotzp.html

[U88] JS：对象展开合并
来源：http://hz.yangfankeji.com/gtibyhxzjo.html

{ ...a, ...b }
来源：http://hz.sxryk.cn/gtjbuqqpxp.html

[U89] JS：数组去重
来源：http://hz.mhx1999.top/gtbcszagjx.html

[...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtjcueesku.html

[U90] JS：数字数组排序
来源：http://hz.pycfn.com/gtphmxxuko.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtvonlwgeg.html

[U91] JS：对象键值遍历
来源：http://hz.zhengqikj.top/gtmokwevyt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hysaishi.cn/gtzgefyvml.html

[U92] JS：深拷贝
来源：http://hz.chenzaomai.com/gtnojtlbzt.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtaswgaovd.html

[U93] JS：模板字符串
来源：http://hz.zdqjudy.top/gtgdfzypah.html

`共 ${n} 条`
来源：http://hz.birdmap.top/gtmyiahmns.html

[U94] JS：箭头函数
来源：http://hz.andypj.xyz/gthjwawlfn.html

const double = x => x * 2;
来源：http://hz.zhijiandao.cn/gtwowsrref.html

[U95] JS：Promise 包装
来源：http://hz.guannengcc.top/gtnxiaoccp.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtgiswqzgy.html

[U96] JS：async/await 与异常
来源：http://hz.hywenlv.cn/gtncyupjjv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtqdqoklrt.html

[U97] JS：并发请求
来源：http://hz.jqgfzy.top/gtgcdqcmrp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtsgkxpyoc.html

[U98] JS：fetch 带 JSON
来源：http://hz.gotoacloud.top/gtveobiqch.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtzedlwfik.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtoqezraan.html

el.addEventListener("click", e => {})
来源：http://hz.xziqi.cn/gtfczlxeyj.html

[U100] JS：DOM 查询
来源：http://hz.tianlin.xyz/gtrjbcbffp.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtvhkpxbia.html

[U101] JS：classList 操作
来源：http://hz.yj20258.top/gtjcwcvgjm.html

el.classList.toggle("active")
来源：http://hz.andypj.xyz/gtskytcefx.html

[U102] JS：本地存储
来源：http://hz.chenzaomai.com/gtrdlbatuz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.redwolf501.top/gtqopdtnqj.html

[U103] JS：定时器
来源：http://hz.havefunace.top/gtycqbugnf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenjidiqi.icu/gtkgfksmcf.html

[U104] JS：防抖
来源：http://hz.daria6918.cn/gtclqmheud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtdzvyppog.html

[U105] JS：节流
来源：http://hz.chenjidiqi.icu/gtgaovldqt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gaohongyu789.top/gtfsvquvvx.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gtdnjmenou.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cucudq.cn/gtaxneqfvr.html

[U107] JS：数字千分位
来源：http://hz.shzxlz.cn/gtrauwtzsn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sufxvd.cn/gtwcfqohai.html

[U108] JS：随机整数
来源：http://hz.redwolf501.top/gtuudjgnoq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.dianchejie.cn/gtphdzvogo.html

[U109] JS：数组分组
来源：http://hz.ydjk.org.cn/gtrqvdypyd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtmonotmcz.html

[U110] JS：数组分块
来源：http://hz.chenzaomai.com/gtrgbmjvpa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangdashe.top/gtoaphjcuw.html

[U111] JS：对象转 Map
来源：http://hz.shuidangran.top/gtnjrcujhi.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtctgsqywd.html

[U112] JS：字符串补位
来源：http://hz.xuanzx.com/gtdtkdbqfg.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtpvbmpdkd.html

[U113] JS：正则替换全部
来源：http://hz.pycfn.com/gttbytrxha.html

s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gttipybogs.html

[U114] JS：JSON 深比较
来源：http://hz.ydjk.org.cn/gteojopgqn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtbhktyghx.html

[U115] JS：生成 UUID
来源：http://hz.snrcjt.cn/gtvyclhfbm.html

crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtjazjmksp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinyuanbaomall.cn/gtwjxpaxvj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.vqdsnc.cn/gtgtwfjotg.html

[U117] JS：单元测试
来源：http://hz.zhiwuduotai.top/gtggjvlehv.html

npm i -D vitest;  npx vitest
来源：http://hz.ydjk.org.cn/gthxaihdxt.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtrrgglfpl.html

npm i -D vite;  npx vite
来源：http://hz.hfpthk.cn/gtwkybfqus.html

[U119] JS：生产构建
来源：http://hz.guannengcc.top/gtzxyoufdg.html

npx vite build
来源：http://hz.birdmap.top/gtkfodqlji.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.havefunace.top/gtkfnazjla.html

import.meta.env.VITE_API_URL
来源：http://hz.ydzc1.top/gtnuboxuja.html

================================================================================
来源：http://hz.hammf.cn/gtvasfykrq.html

统计汇总
来源：http://hz.jinyuanbaomall.cn/gtbdqinzdf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtohcvyncu.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtwdvsjydp.html

Python ......... 252
来源：http://hz.birdmap.top/gtnzwqoyvr.html

PHP ............ 252
来源：http://hz.xziqi.cn/gtayudnkmd.html

JavaScript ..... 252
来源：http://hz.cashguo.top/gtsvdqxvjg.html

TypeScript ..... 212
来源：http://hz.jinghuilouyu.cn/gtksgruxyw.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtifcfwavc.html

Go ............. 212
来源：http://hz.daria6918.cn/gtsalrjutd.html

Ruby ........... 212
来源：http://hz.yj20258.top/gtwfvdghuw.html

C# ............. 212
来源：http://hz.jinqigufen.top/gtwzqarmuh.html

C .............. 30
来源：http://hz.redwolf501.top/gtxsbhetjt.html

C++ ............ 30
来源：http://hz.gotoacloud.top/gtqhndynef.html

SQL ............ 90
来源：http://hz.xingfuxueyuan.xyz/gtbynjpbia.html

Bash ........... 80
来源：http://hz.aibaodan.cn/gtcyqeqhwq.html

Kotlin ......... 15
来源：http://hz.hysaishi.cn/gtottfspka.html

Swift .......... 15
来源：http://hz.yangfankeji.com/gtanhignle.html

Lua ............ 10
来源：http://hz.pengpengdd.cyou/gtuybtpabw.html

Perl ........... 10
来源：http://hz.zhongyouzk.top/gtqjqwrtse.html

Scala .......... 10
来源：http://hz.yongpay.top/gtjxvblczr.html

------------------------------------
来源：http://hz.cqqwz.cn/gtazilkkap.html

合计 ........... 2106 条
来源：http://hz.zhaomingkeji.xyz/gtpgozncyp.html

按章节统计：
来源：http://hz.zycfv.cn/gtmjihpntq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gthdocopeh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtkextoepv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtbyqlundo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtbpionfbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtvkfcilli.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtptqjxood.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtemymxfdg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtugmclgzh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtqijrijbr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gteloohgkb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtbyjuzfkh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtyfadbxwx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtchgilwnr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nanxinkj.top/gtcnlnxerw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydzc1.top/gtciysazke.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtqdtgpebb.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtkidzbtav.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gtiyrotbwr.html

S C / C++ 专题                          60
来源：http://hz.9152youxi.cn/gtyqyfikkz.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtbewxluyf.html

U 高频实用片段                         120
来源：http://hz.zhaomingkeji.xyz/gtmfepqzwg.html

------------------------------------
来源：http://hz.tanke756.top/gteybfwslu.html

合计                                  2106 条
来源：http://hz.zycfv.cn/gtdtrebuqf.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtsvrcromy.html

使用提醒
来源：http://hz.nwbrower.top/gtwlvmktgs.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtbukiwshv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.havefunace.top/gtbfbcckkf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zdqjudy.top/gtwedctgvi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj202588.top/gteibzssyg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jiagoushi.top/gtbsnghrff.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhixingplan.top/gtosfagghf.html

—— 文件结束 ——
来源：http://hz.xuetiantiany.cn/gtzdhgysua.html

================================================================================
来源：http://hz.bjfxy.top/gtzxzwfzfg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xingfuxueyuan.xyz/gtitwhykre.html

Common Programming Examples Cheat Book
来源：http://hz.jyoumei.cn/gtbqwetknb.html

================================================================================
来源：http://hz.0kj1m.cn/gtogulbmxv.html

【收录内容】
来源：http://hz.jiagoushi.top/gtobvraxnp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yuxming.cn/gtcjpmfgtm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sweek.top/gtnrlqblpw.html

SQL · Bash · C · C++
来源：http://hz.0kj1m.cn/gtwcilchvr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtqjmdikha.html

【使用说明】
来源：http://hz.hammf.cn/gtwpvetlrp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jyoumei.cn/gtybwfwmyc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hfpthk.cn/gtwfqtveha.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinqigfzy.top/gtmbtiyonc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhoulong.xyz/gtvmdebckj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xylfe.cn/gtlilscsju.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cqqwz.cn/gtupsgqldc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pycfn.com/gtewfngxva.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.9152youxi.cn/gtlthrgmml.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtwxgccjzo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tianlin.xyz/gtrvleaxwa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daria6918.cn/gtafwvmokp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nwbrower.top/gtwralkara.html

【文件统计】
来源：http://hz.bjfxy.top/gtjqzelixy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtthgktkqo.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtivcrryak.html

目  录
来源：http://hz.dianchejie.cn/gtgomdpxvy.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtftkwpmaw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtkoxvesrk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.sweek.top/gtcnodmvvy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtrbtgwdyu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.gotoacloud.top/gtxnbrgypy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinqigufen.top/gttmiukzip.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gtygqjjoom.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtqjewoeju.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yuxming.cn/gtsodnfaip.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jqgfzy.top/gtzesbtfjy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtfjlglslp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtvpaepezw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtwshapvxf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtsufjxgyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtitsverak.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.redwolf501.top/gtddygnecb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtdwaimztn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258888.top/gtwyhtfeoo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xingfuxueyuan.xyz/gtulonxvgf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gotoacloud.top/gtnvwqrpph.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtuehcucmq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtscypwglk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtuotkhyhl.html

A. 基础语法与类型
来源：http://hz.cdnleiting.top/gthgbakspd.html

================================================================================
来源：http://hz.zdqjudy.top/gtgqinarxz.html

[A01] Hello World
来源：http://hz.gzhubu.top/gtvkudwwnq.html

Py:   print("Hello, World!")
来源：http://hz.zhijiandao.cn/gtdfiasrjm.html

PHP:  echo "Hello, World!";
来源：http://hz.pengpengdd.cyou/gtvtwnqmef.html

JS:   console.log("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtteffpbql.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhixingplan.top/gtqnhffiof.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhaomingkeji.xyz/gtvrrzrtbj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.c1oappe.top/gtbtwwbcpv.html

Ruby: puts "Hello, World!"
来源：http://hz.redwolf501.top/gtdihxrvtm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.nanxuanxn.top/gtckrrwidt.html

[A02] 变量声明与赋值
来源：http://hz.cdnleiting.top/gtekfhmjge.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.fengsongda.top/gtfevkfuph.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhongyouzk.top/gtrwfxakkp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zdqjudy.top/gtmoxectuv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.smart0.xyz/gtqxtywyij.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.svipenyu.cn/gtyiedkhjf.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhongyouzk.top/gtxgovxvvd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.quarkkingdee.top/gtycxvwvil.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xylfe.cn/gteazdgkzl.html

[A03] 常量定义
来源：http://hz.yongpay.top/gtafcppmys.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.9152youxi.cn/gtrqrggxfj.html

PHP:  const PI = 3.14159;
来源：http://hz.zhixingplan.top/gtxnlbqtwf.html

JS:   const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtoedxfhfh.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhoulong.xyz/gtqwruvluv.html

Java: static final double PI = 3.14159;
来源：http://hz.sxryk.cn/gtnvzxyive.html

Go:   const PI = 3.14159
来源：http://hz.ybcxt.top/gtgeyeqcbk.html

Ruby: PI = 3.14159
来源：http://hz.c1oappe.top/gtrbmjcery.html

C#:   const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtqqubswfx.html

[A04] 判断变量类型
来源：http://hz.jinyuanbaomall.cn/gtekalqdwj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhoulong.xyz/gtaqtwwqmv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guowangkeji.top/gtikjmsktw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.redwolf501.top/gtoxywzxzh.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinghuilouyu.cn/gtowcreghj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hysaishi.cn/gtpbqkgkso.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhaomingkeji.xyz/gtxyqeagaj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gtshfpnpid.html

C#:   x.GetType().Name; x is int
来源：http://hz.gaohongyu789.top/gtxmmvitiy.html

[A05] 整数除法与取模
来源：http://hz.havefunace.top/gtwerqbnxs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ivvv.top/gtxzxrfszt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xylfe.cn/gtafhomldt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gzhubu.top/gtniitkzkd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jianghu66.top/gtltkrpwuu.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtojgtjymr.html

Go:   7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtvlkzojoo.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gtrlkddgje.html

C#:   7 / 2; 7 % 2
来源：http://hz.hfpthk.cn/gtqfejhbnw.html

[A06] 字符串转数字
来源：http://hz.nanxuanxn.top/gtzdvnztke.html

Py:   int("42"); float("3.14")
来源：http://hz.chenlongwang.top/gtibmoupmx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shanyushiyangkeji.top/gtjsdljvqk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.gaohongyu789.top/gtwimpluym.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.tanke756.top/gtgvrmwnwj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.meibo888.top/gtbrxzeovq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.bjfxy.top/gtqkdvdpxr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.0kj1m.cn/gtvnctsiyb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gogol.net.cn/gtffauaqhn.html

[A07] 数字转字符串
来源：http://hz.nanxinkj.top/gtyxbedgbb.html

Py:   str(42)
来源：http://hz.shuidangran.top/gtpgsncomm.html

PHP:  (string) 42; strval(42)
来源：http://hz.ehwqpu.com/gtoezsnbiv.html

JS:   String(42); (42).toString()
来源：http://hz.shuidangran.top/gtqiunbepr.html

TS:   String(42)
来源：http://hz.gogol.net.cn/gttoemjzvp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yueranfly.top/gtucfpaztn.html

Go:   strconv.Itoa(42)
来源：http://hz.ydjk.org.cn/gtpmsjgmid.html

Ruby: 42.to_s
来源：http://hz.wangshuangyany.cn/gtztbuyojs.html

C#:   42.ToString()
来源：http://hz.shangyingyoupin.top/gttwlthqda.html

[A08] 取整与四舍五入
来源：http://hz.hammf.cn/gtgeaqnalt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cqqwz.cn/gtuwalqsus.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhixingplan.top/gtbiphvbvv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.mhx1999.top/gtmntbtflg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xziqi.cn/gtdwzczfdd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.redwolf501.top/gtmzvpsyus.html


<!-- 参考信息 -->