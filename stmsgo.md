代发 wailian999

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gtwivfmhmi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnxiangtu.top/gtzmypbeil.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gtkpqemoya.html

f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtmpfmhuny.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtfvimkmrv.html

"值: {$a}"
来源：http://hz.cdnleiting.top/gttukzjesq.html

[U58] PHP：数组三件套
来源：http://hz.wangdashe.top/gtxqqipmvy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtabjygvip.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtujgiszww.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtaxjevgfy.html

[U60] PHP：JSON 编解码
来源：http://hz.shangyingyoupin.top/gtvatenxjc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj202588.top/gtobujmumb.html

[U61] PHP：正则
来源：http://hz.tianlin.xyz/gtwwmvslch.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtmwfmsyjp.html

[U62] PHP：日期对象
来源：http://hz.xylfe.cn/gtfchjrcll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuanzx.com/gtrgymelbr.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtpcoppohd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtgbgflgpp.html

[U64] PHP：目录遍历
来源：http://hz.zhaomingkeji.xyz/gteqpmzucv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtbotblgxz.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtbsmztgrk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhongyouzk.top/gtfwahugzc.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gtjnzekbmg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinghuilouyu.cn/gtdraixbzq.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtzvaxbgib.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangdashe.top/gtqwmsywvm.html

[U68] PHP：PDO 连接
来源：http://hz.vqdsnc.cn/gthotoyehw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuetiantiany.cn/gtvcqsnykd.html

[U69] PHP：PDO 预处理
来源：http://hz.cucudq.cn/gtqtndsbcr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnxiangtu.top/gtnyutxtjj.html

[U70] PHP：PDO 事务
来源：http://hz.zhaomingkeji.xyz/gtmidvgpfz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtkdrctbtz.html

[U71] PHP：抛出异常
来源：http://hz.sxryk.cn/gtwnkjamyv.html

throw new RuntimeException("失败", 500);
来源：http://hz.fzhhl.top/gthbbdndwp.html

[U72] PHP：写错误日志
来源：http://hz.daria6918.cn/gtgaalkpws.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ppjwa.cn/gtojpuocwh.html

[U73] PHP：读取 ini 配置
来源：http://hz.sysykeji.top/gtkgejzeqr.html

parse_ini_file("config.ini", true)
来源：http://hz.gaohongyu789.top/gtzcoraiai.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtwibddclx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.guowangkeji.top/gttldnsagl.html

[U75] PHP：依赖注入
来源：http://hz.mhx1999.top/gtqpadnbwu.html

composer require psr/container
来源：http://hz.yj202588.top/gtphhfbsaz.html

[U76] PHP：简单路由
来源：http://hz.snrcjt.cn/gthosgyktz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ivvv.top/gtgglwkzuh.html

[U77] PHP：模板渲染
来源：http://hz.ivvv.top/gtymqyesln.html

composer require twig/twig
来源：http://hz.hfpthk.cn/gtrhingblz.html

[U78] PHP：单元测试
来源：http://hz.cashguo.top/gtoljdwmyy.html

composer require --dev phpunit/phpunit
来源：http://hz.nanxuanxn.top/gtpvcadiqj.html

[U79] PHP：静态分析
来源：http://hz.cdnleiting.top/gtypxinuqp.html

composer require --dev phpstan/phpstan
来源：http://hz.yueranfly.top/gtvpyttbpc.html

[U80] PHP：代码规范修复
来源：http://hz.zhixingplan.top/gthpmtjjxh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.andypj.xyz/gtjexrfbrb.html

[U81] JS：初始化项目
来源：http://hz.zhixingplan.top/gtrydjoshf.html

npm init -y;  npm i express
来源：http://hz.shuidangran.top/gtrhluhvfm.html

[U82] JS：package.json 脚本
来源：http://hz.c1oappe.top/gtbuuyrgyi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ydzc1.top/gtwkcbnfnx.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtkysunqbp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.0kj1m.cn/gtvmhdmfbp.html

[U84] JS：CommonJS 写法
来源：http://hz.yuanzhike.top/gtfdpebgbg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhixingplan.top/gtcweyzsjj.html

[U85] JS：可选链
来源：http://hz.shanyushiyangkeji.top/gtrmlmutpe.html

a?.b?.c
来源：http://hz.52xcode.cn/gteqgukxzn.html

[U86] JS：空值合并
来源：http://hz.tanke756.top/gtkohzkpdf.html

a ?? b
来源：http://hz.meibo888.top/gttvoukjyo.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gtumqsygvo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ehwqpu.com/gtxgojzozu.html

[U88] JS：对象展开合并
来源：http://hz.dianchejie.cn/gtokrvcory.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gtduahytwe.html

[U89] JS：数组去重
来源：http://hz.chenlongwang.top/gtqbirkxgg.html

[...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtyukwwprh.html

[U90] JS：数字数组排序
来源：http://hz.bjfxy.top/gtmrbxycfb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtrtkllocd.html

[U91] JS：对象键值遍历
来源：http://hz.zhoulong.xyz/gtjzcmfsfw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.havefunace.top/gtxonwkdlv.html

[U92] JS：深拷贝
来源：http://hz.hnxiangtu.top/gtsbfineyo.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtjbpegute.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangtech.top/gtcxdquedf.html

`共 ${n} 条`
来源：http://hz.hysaishi.cn/gtgywihipf.html

[U94] JS：箭头函数
来源：http://hz.9152youxi.cn/gtaldqoirm.html

const double = x => x * 2;
来源：http://hz.jinqigfzy.top/gtaxwhlpxw.html

[U95] JS：Promise 包装
来源：http://hz.xuanzx.com/gtqjofymck.html

new Promise((resolve, reject) => {})
来源：http://hz.daria6918.cn/gtamnlvqwh.html

[U96] JS：async/await 与异常
来源：http://hz.xylfe.cn/gtwgpahres.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtxtroodin.html

[U97] JS：并发请求
来源：http://hz.zhoulong.xyz/gtkwkkuxfl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtzgahoysr.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtsklvscof.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xinyue.icu/gtnwakktyw.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtnwsglspi.html

el.addEventListener("click", e => {})
来源：http://hz.fengsongda.top/gthuffzokx.html

[U100] JS：DOM 查询
来源：http://hz.zhengqikj.top/gtbfuhyqru.html

document.querySelector(".item")
来源：http://hz.birdmap.top/gtczihtmbq.html

[U101] JS：classList 操作
来源：http://hz.zhaomingkeji.xyz/gtlzavzyos.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtqwehjjpt.html

[U102] JS：本地存储
来源：http://hz.zhoulong.xyz/gtwxigmbah.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gzhubu.top/gtkxxzjron.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtwrqzptxu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.fzhhl.top/gtthltyqqb.html

[U104] JS：防抖
来源：http://hz.jlsjyb.cn/gtectsgexu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtybosvvjg.html

[U105] JS：节流
来源：http://hz.yuxming.cn/gtjxanndhm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.316326.xyz/gtdrjnbclt.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gtwttkozmq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zdqjudy.top/gtegggzdro.html

[U107] JS：数字千分位
来源：http://hz.guannengcc.top/gtngbrwwof.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cheryme.top/gtpicmqsjv.html

[U108] JS：随机整数
来源：http://hz.snrcjt.cn/gtllekxywf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jlsjyb.cn/gtpaukiqyj.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtodqxxpqd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtylifedsp.html

[U110] JS：数组分块
来源：http://hz.iojbl.cn/gtdswccnfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangdashe.top/gteuuorjes.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtcmxvcacb.html

new Map(Object.entries(obj))
来源：http://hz.wangdashe.top/gteimytpvv.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtjdykhtzn.html

"7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtrisrvszm.html

[U113] JS：正则替换全部
来源：http://hz.sufxvd.cn/gtzvqluowt.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtfusplwww.html

[U114] JS：JSON 深比较
来源：http://hz.vqdsnc.cn/gtwgctmcbz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtkpznfkle.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtvtozkhex.html

crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtgppbqboj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.mhx1999.top/gtfwvhfvuh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gogol.net.cn/gtupohhspf.html

[U117] JS：单元测试
来源：http://hz.birdmap.top/gtmtkmxoxx.html

npm i -D vitest;  npx vitest
来源：http://hz.andypj.xyz/gtpokjaszx.html

[U118] JS：开发服务器
来源：http://hz.jiagoushi.top/gtcvpowvie.html

npm i -D vite;  npx vite
来源：http://hz.c1oappe.top/gtzrgxhkau.html

[U119] JS：生产构建
来源：http://hz.vqdsnc.cn/gtagjtxkno.html

npx vite build
来源：http://hz.daxiang520.top/gtrgzcvwor.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtkhozjqjk.html

import.meta.env.VITE_API_URL
来源：http://hz.ywan-chungtsiang.top/gtalbyompd.html

================================================================================
来源：http://hz.sxryk.cn/gtrztenlks.html

统计汇总
来源：http://hz.redwolf501.top/gtayhqdfuc.html

================================================================================
来源：http://hz.yj20258888.top/gtcgcwfkwz.html

按语言统计（条）：
来源：http://hz.quarkkingdee.top/gtzjxjddwp.html

Python ......... 252
来源：http://hz.fzhhl.top/gtmtsozlub.html

PHP ............ 252
来源：http://hz.cqqwz.cn/gtmeynzvol.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtuimuulbs.html

TypeScript ..... 212
来源：http://hz.havefunace.top/gthjjaordo.html

Java ........... 212
来源：http://hz.ydzc1.top/gtgceweoqs.html

Go ............. 212
来源：http://hz.jinghuilouyu.cn/gtanrzbmzp.html

Ruby ........... 212
来源：http://hz.nanxinkj.top/gtofscotrn.html

C# ............. 212
来源：http://hz.yj20258888.top/gtixycrjrp.html

C .............. 30
来源：http://hz.birdmap.top/gtzkinofwq.html

C++ ............ 30
来源：http://hz.xinyue.icu/gtgcvkffec.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gttfjyibbo.html

Bash ........... 80
来源：http://hz.316326.xyz/gtjftfywsh.html

Kotlin ......... 15
来源：http://hz.jyoumei.cn/gtolenrtzv.html

Swift .......... 15
来源：http://hz.andypj.xyz/gtmqihqvha.html

Lua ............ 10
来源：http://hz.shuidangran.top/gtlpzzcrax.html

Perl ........... 10
来源：http://hz.9152youxi.cn/gtrisrdekh.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtsezmhwsg.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtfbojrtmr.html

合计 ........... 2106 条
来源：http://hz.feifeiyinyue.top/gtwxorjeom.html

按章节统计：
来源：http://hz.jianghu66.top/gtcnjjrljr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtujafyows.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtrrwzttyy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtjblryzpf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtkfjpzjjp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yvedp.cn/gtpcktvlmh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtovbrfgii.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gthjoqcrnv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtanzyplrq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtcfrlnudd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtavmpacwm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gteopbjnir.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtpwjlkues.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtlsnwtkpo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jlsjyb.cn/gtfarfldno.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtvdfpvxuw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtvsthazpm.html

Q SQL 专题                              90
来源：http://hz.9152youxi.cn/gtpgsmmmnt.html

R Bash 专题                             80
来源：http://hz.quarkkingdee.top/gtjtksdoyv.html

S C / C++ 专题                          60
来源：http://hz.sysykeji.top/gtxbskkyon.html

T 其他语言补充                          60
来源：http://hz.redwolf501.top/gthgeegwvi.html

U 高频实用片段                         120
来源：http://hz.andypj.xyz/gtxwnbwifl.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtapuedaik.html

合计                                  2106 条
来源：http://hz.andypj.xyz/gtcefnjbuh.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtwigkpqpm.html

使用提醒
来源：http://hz.ehwqpu.com/gtayzaxvgk.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtifltyuyd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258888.top/gtwncgtrcv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhongyouzk.top/gteiqhwoxq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenzaomai.com/gtbbqdjbfs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ppjwa.cn/gthoijchps.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhaomingkeji.xyz/gttzhpbgwe.html

—— 文件结束 ——
来源：http://hz.ydjk.org.cn/gttajbbife.html

================================================================================
来源：http://hz.sxryk.cn/gtnrnxabqd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aibaodan.cn/gtqxtnkjmp.html

Common Programming Examples Cheat Book
来源：http://hz.chenjidiqi.icu/gtkzsthpuu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtajzebjxr.html

【收录内容】
来源：http://hz.tian-w.cn/gtblxywqri.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.52xcode.cn/gtawbiduxw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.guannengcc.top/gtnarqmfoc.html

SQL · Bash · C · C++
来源：http://hz.ydzc1.top/gtikxvptlz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cucudq.cn/gtkrhcrraz.html

【使用说明】
来源：http://hz.yuxming.cn/gtvvjlelep.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cqqwz.cn/gtzdvsyssc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtxetpgawd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.snrcjt.cn/gtowlljlcn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pengpengdd.cyou/gtmfxkfhot.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.daxiang520.top/gtvhlqlysg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj202588.top/gtvjesuxwq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haohaochexian.top/gtwksvlulv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtvaaohsce.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinghuilouyu.cn/gtbuvbxlic.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtztvzrhcu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.52xcode.cn/gtegrlhbxe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cashguo.top/gtffszinaw.html

【文件统计】
来源：http://hz.cqqwz.cn/gtrxneefwq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xylfe.cn/gtlqwbsdpi.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtratvqsoz.html

目  录
来源：http://hz.jianghu66.top/gtdircuead.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtlfpgptkq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.aibaodan.cn/gtkydpjpbf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtfljstxed.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtoweypvvm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gtvbsmbtkz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtwcdwuayq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtlpkfeupz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.bjfxy.top/gtpnekttqn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtmgdbzgrg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtzknongiq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtmtbmnfrz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtoxzejfsy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtcrkzangk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtzhskmkbp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.fzhhl.top/gtxqfzicdf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.feifeiyinyue.top/gtvngmchpg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtprjtfzhi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.tian-w.cn/gtfliazmau.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.svipenyu.cn/gtrqzgeouj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gzhubu.top/gthxfgvblw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gttbpxevil.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gttnqpkrmp.html

================================================================================
来源：http://hz.aibaodan.cn/gtbrmldbnd.html

A. 基础语法与类型
来源：http://hz.redwolf501.top/gtadrdlkjw.html

================================================================================
来源：http://hz.guannengcc.top/gtcqebbrqv.html

[A01] Hello World
来源：http://hz.zdqjudy.top/gtznqqbesr.html

Py:   print("Hello, World!")
来源：http://hz.mhx1999.top/gtxikzixsb.html

PHP:  echo "Hello, World!";
来源：http://hz.redwolf501.top/gtfmfkgqfx.html

JS:   console.log("Hello, World!");
来源：http://hz.iojbl.cn/gtqqnifhyp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hnxiangtu.top/gtefmkubbt.html

Java: System.out.println("Hello, World!");
来源：http://hz.jianghu66.top/gtdjtemogp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yuanzhike.top/gtequrlald.html

Ruby: puts "Hello, World!"
来源：http://hz.yj202588.top/gtmbqjfeyj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.guannengcc.top/gtnvpvxcuj.html

[A02] 变量声明与赋值
来源：http://hz.bjfxy.top/gtgmaghxjt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtkpphjmoc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenzaomai.com/gtptybgeuc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtgwmzwcms.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jyoumei.cn/gtrsoiicdx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shzxlz.cn/gtjeutggwy.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gtjvdekzde.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yongpay.top/gtobazmnwb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtrtwwgpbv.html

[A03] 常量定义
来源：http://hz.jiagoushi.top/gtcirgslpm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gaohongyu789.top/gtoybwrlmf.html

PHP:  const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtedciqlej.html

JS:   const PI = 3.14159;
来源：http://hz.shzxlz.cn/gtmqzknebt.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtetunnarg.html

Java: static final double PI = 3.14159;
来源：http://hz.yj20258888.top/gtuhsvscqi.html

Go:   const PI = 3.14159
来源：http://hz.yonumen.top/gtzghhwslm.html

Ruby: PI = 3.14159
来源：http://hz.yvedp.cn/gtrjvenqqu.html

C#:   const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtekrlpgno.html

[A04] 判断变量类型
来源：http://hz.hnxiangtu.top/gtqfinuabr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.haohaochexian.top/gtcubxulzs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jqgfzy.top/gthgygkcmh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.vqdsnc.cn/gtzsiqnmrp.html

TS:   typeof x; x instanceof Date
来源：http://hz.birdmap.top/gthmmgpvpy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinqigfzy.top/gtvzhezvlw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xingfuxueyuan.xyz/gtczxhqbvs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.haohaochexian.top/gtfrcxaivs.html

C#:   x.GetType().Name; x is int
来源：http://hz.jyoumei.cn/gtqinfjorp.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangtech.top/gtudtxgxpd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hnqzz.top/gtqaptywic.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sweek.top/gtngvefhgv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258.top/gtjufrmqja.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtvzvdjwsb.html

Java: 7 / 2; 7 % 2
来源：http://hz.yuxming.cn/gtleprnedj.html

Go:   7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtslwiyisr.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhongyouzk.top/gtsawyelke.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtmlfejuob.html

[A06] 字符串转数字
来源：http://hz.sysykeji.top/gtlrzzvsrn.html

Py:   int("42"); float("3.14")
来源：http://hz.birdmap.top/gtvvwumcaf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.iojbl.cn/gtoxfodfmg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cqqwz.cn/gtfwpjexql.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hfpthk.cn/gtvkklwntz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cheryme.top/gtjcwzpjko.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.aizwys.cn/gtpioaqlzk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.birdmap.top/gtdbmuigwc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.sysykeji.top/gttwvyloni.html

[A07] 数字转字符串
来源：http://hz.hnqzz.top/gtzjubswcx.html

Py:   str(42)
来源：http://hz.nanxuanxn.top/gtzjplewfs.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhiwuduotai.top/gtmvhiwojv.html

JS:   String(42); (42).toString()
来源：http://hz.yongpay.top/gtebckvnkj.html

TS:   String(42)
来源：http://hz.chenzaomai.com/gtbhkrhbnv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhixingplan.top/gtdnlmyfqi.html

Go:   strconv.Itoa(42)
来源：http://hz.zhijiandao.cn/gtmkhahwip.html


<!-- 参考信息 -->