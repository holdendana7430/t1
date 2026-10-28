代发 wailian999

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtfjuwrmkf.html

[$a, $b] = $arr;
来源：http://hz.hywenlv.cn/gtkimmnmny.html

[U52] PHP：箭头函数
来源：http://hz.shzxlz.cn/gtmtartltj.html

$double = fn($x) => $x * 2;
来源：http://hz.cashguo.top/gtnmtqhdjk.html

[U53] PHP：空合并运算符
来源：http://hz.cashguo.top/gtuvwklsmc.html

$v = $a ?? $b ?? "default";
来源：http://hz.nwbrower.top/gtkhokisgy.html

[U54] PHP：空安全调用
来源：http://hz.svipenyu.cn/gtlljjyprs.html

$obj?->method()
来源：http://hz.yuanzhike.top/gtfaocsvhv.html

[U55] PHP：match 表达式
来源：http://hz.ppjwa.cn/gtavyfjopo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gzhubu.top/gtehmrdetq.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtuvxlyugw.html

f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtbessmfzh.html

[U57] PHP：字符串插值
来源：http://hz.yj202588.top/gtlospwump.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtdmpeiaqf.html

[U58] PHP：数组三件套
来源：http://hz.cashguo.top/gtfcrcykjl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jianghu66.top/gtelwptdmw.html

[U59] PHP：自定义排序
来源：http://hz.chenlongwang.top/gtushooerp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuetiantiany.cn/gtifqerjft.html

[U60] PHP：JSON 编解码
来源：http://hz.tianlin.xyz/gtmcqfhsdw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtywptbgum.html

[U61] PHP：正则
来源：http://hz.pycfn.com/gtipmustqa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtxvxroylt.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtpcbrfazy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuanzhike.top/gtrdhqhvuc.html

[U63] PHP：文件读写
来源：http://hz.gotoacloud.top/gtyraymjta.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zycfv.cn/gtoleiliog.html

[U64] PHP：目录遍历
来源：http://hz.jinqigfzy.top/gtkvsemcee.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtmrqgdnsq.html

[U65] PHP：会话
来源：http://hz.dianchejie.cn/gtyxqjtezv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangshuangyany.cn/gtmqktkeft.html

[U66] PHP：设置 Cookie
来源：http://hz.shangyingyoupin.top/gtpyhodvkx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigufen.top/gtyuplatew.html

[U67] PHP：处理文件上传
来源：http://hz.ppjwa.cn/gtlxbqdfkb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tianlin.xyz/gtnrzxqeby.html

[U68] PHP：PDO 连接
来源：http://hz.jqgfzy.top/gtazfwaxaf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hywenlv.cn/gtpllyiffs.html

[U69] PHP：PDO 预处理
来源：http://hz.hammf.cn/gtsgmyjmfb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xinyue.icu/gtijptnjfu.html

[U70] PHP：PDO 事务
来源：http://hz.zycfv.cn/gtdhmzcyzz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.0kj1m.cn/gtumkhmhqs.html

[U71] PHP：抛出异常
来源：http://hz.jinghuilouyu.cn/gtjhdqpkgo.html

throw new RuntimeException("失败", 500);
来源：http://hz.zdqjudy.top/gtbwkzhqao.html

[U72] PHP：写错误日志
来源：http://hz.chenjidiqi.icu/gtdadtjbnc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yueranfly.top/gtsjtjhmjx.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtguexvbzq.html

parse_ini_file("config.ini", true)
来源：http://hz.c1oappe.top/gthvqdfpee.html

[U74] PHP：读取环境变量
来源：http://hz.chenzaomai.com/gtceocmfda.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenjidiqi.icu/gtifpkjxkx.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtfdnpupbt.html

composer require psr/container
来源：http://hz.xylfe.cn/gtnrzsjczz.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtfqaxsbfy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangkeji.top/gtqezebzlx.html

[U77] PHP：模板渲染
来源：http://hz.yuanzhike.top/gthdpmvlcp.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gttpstiepq.html

[U78] PHP：单元测试
来源：http://hz.yangfankeji.com/gtwkzgvdys.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gthaywjmmr.html

[U79] PHP：静态分析
来源：http://hz.yvedp.cn/gtoljedodk.html

composer require --dev phpstan/phpstan
来源：http://hz.zhongyouzk.top/gtltheaqln.html

[U80] PHP：代码规范修复
来源：http://hz.guowangkeji.top/gtagakgrmd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sysykeji.top/gtpyhqqakg.html

[U81] JS：初始化项目
来源：http://hz.gaohongyu789.top/gtzjedpndl.html

npm init -y;  npm i express
来源：http://hz.hnqzz.top/gtwlhotnfw.html

[U82] JS：package.json 脚本
来源：http://hz.yonumen.top/gtunzrxsjn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hfpthk.cn/gtfmrjuocm.html

[U83] JS：ES Module 导入导出
来源：http://hz.daria6918.cn/gtkwdvpfcq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shangyingyoupin.top/gtkwfoiylb.html

[U84] JS：CommonJS 写法
来源：http://hz.shuidangran.top/gtgjcuvrpw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtzpdowhkw.html

[U85] JS：可选链
来源：http://hz.xylfe.cn/gtxdsmyobx.html

a?.b?.c
来源：http://hz.andypj.xyz/gttmsivfgu.html

[U86] JS：空值合并
来源：http://hz.redwolf501.top/gtcjjfldar.html

a ?? b
来源：http://hz.yueranfly.top/gtzqhvbskl.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtjieetcbo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tian-w.cn/gtcpkqxduh.html

[U88] JS：对象展开合并
来源：http://hz.0kj1m.cn/gtcmvgtuwp.html

{ ...a, ...b }
来源：http://hz.52xcode.cn/gtlkcutqon.html

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtysihieii.html

[...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtxgsmgleo.html

[U90] JS：数字数组排序
来源：http://hz.jiagoushi.top/gtzjgbbcpo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtnnosxtnl.html

[U91] JS：对象键值遍历
来源：http://hz.shzxlz.cn/gtxzccmkvp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.snrcjt.cn/gtqsbztqxy.html

[U92] JS：深拷贝
来源：http://hz.tanke756.top/gthsvcakel.html

structuredClone(obj)
来源：http://hz.xziqi.cn/gteyxwrasn.html

[U93] JS：模板字符串
来源：http://hz.redwolf501.top/gtlkrxfzzq.html

`共 ${n} 条`
来源：http://hz.chenlongwang.top/gtoxxsirqv.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gtestjkjxx.html

const double = x => x * 2;
来源：http://hz.fengsongda.top/gtghpguiab.html

[U95] JS：Promise 包装
来源：http://hz.yvedp.cn/gtjzkvudhf.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gtckdzrimf.html

[U96] JS：async/await 与异常
来源：http://hz.shzxlz.cn/gtroegpcae.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtjsipmjkm.html

[U97] JS：并发请求
来源：http://hz.ydjk.org.cn/gtxtqqpevm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtyzhmapnc.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtozjqybdb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydzc1.top/gtkbmicpmy.html

[U99] JS：事件监听
来源：http://hz.shuidangran.top/gtlyrsdmjm.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangkeji.top/gtgkopqodf.html

[U100] JS：DOM 查询
来源：http://hz.pengpengdd.cyou/gtyeuoyakv.html

document.querySelector(".item")
来源：http://hz.hywenlv.cn/gtvoolgcly.html

[U101] JS：classList 操作
来源：http://hz.jyoumei.cn/gtrulijjsq.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtpmuwbddv.html

[U102] JS：本地存储
来源：http://hz.iojbl.cn/gtjpjgnzfr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cqqwz.cn/gtmbjfnaha.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtnlivkshc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gtngbkfajr.html

[U104] JS：防抖
来源：http://hz.jyoumei.cn/gtcdsrcsae.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtnnriadzr.html

[U105] JS：节流
来源：http://hz.gaohongyu789.top/gtynezrede.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhaomingkeji.xyz/gthscgccnl.html

[U106] JS：日期格式化
来源：http://hz.vqdsnc.cn/gtwoqdlgdt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shzxlz.cn/gtuadalzcv.html

[U107] JS：数字千分位
来源：http://hz.daxiang520.top/gtjyhprvsd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yj20258888.top/gtqcpgizpj.html

[U108] JS：随机整数
来源：http://hz.shzxlz.cn/gtbkwmpghf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuetiantiany.cn/gthmgalznx.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtgzpxucvg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtouhurwof.html

[U110] JS：数组分块
来源：http://hz.yj20258888.top/gtewvnbjrl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtvqqzxoaz.html

[U111] JS：对象转 Map
来源：http://hz.ydjk.org.cn/gtnlrrkoxx.html

new Map(Object.entries(obj))
来源：http://hz.jiagoushi.top/gtrymkqppv.html

[U112] JS：字符串补位
来源：http://hz.xziqi.cn/gtqasgoxnj.html

"7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtsvmzftny.html

[U113] JS：正则替换全部
来源：http://hz.0kj1m.cn/gtfpjyuduk.html

s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtspdeeixf.html

[U114] JS：JSON 深比较
来源：http://hz.dianchejie.cn/gthqdnsbso.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydjk.org.cn/gtaqckylyx.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtqpxbzusj.html

crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtccofaxpg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jianghu66.top/gtnvxrdhag.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgfzy.top/gtevzueifd.html

[U117] JS：单元测试
来源：http://hz.snrcjt.cn/gtcygvhhrs.html

npm i -D vitest;  npx vitest
来源：http://hz.sweek.top/gtkjglqqvk.html

[U118] JS：开发服务器
来源：http://hz.aibaodan.cn/gtzqalxnvq.html

npm i -D vite;  npx vite
来源：http://hz.yj20258.top/gtahbfbwds.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangkeji.top/gtlbqlvwke.html

npx vite build
来源：http://hz.hammf.cn/gtpaoaakbt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtmprgbjpa.html

import.meta.env.VITE_API_URL
来源：http://hz.quarkkingdee.top/gtkdaqkthl.html

================================================================================
来源：http://hz.svipenyu.cn/gtgdekamap.html

统计汇总
来源：http://hz.feifeiyinyue.top/gtkybrgeou.html

================================================================================
来源：http://hz.wangdashe.top/gtdjntxnra.html

按语言统计（条）：
来源：http://hz.ehwqpu.com/gtzaakvcyc.html

Python ......... 252
来源：http://hz.ybcxt.top/gtqkdhmiyt.html

PHP ............ 252
来源：http://hz.shzxlz.cn/gtvgnogals.html

JavaScript ..... 252
来源：http://hz.sxryk.cn/gtxxuapqor.html

TypeScript ..... 212
来源：http://hz.316326.xyz/gtamtupnwa.html

Java ........... 212
来源：http://hz.52xcode.cn/gtfspnciec.html

Go ............. 212
来源：http://hz.meibo888.top/gtfenpeina.html

Ruby ........... 212
来源：http://hz.chenlongwang.top/gtpdqhdqbe.html

C# ............. 212
来源：http://hz.hnxiangtu.top/gtfcyvpuyy.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtizopyrvo.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtlaurmaqr.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtwlykbuxv.html

Bash ........... 80
来源：http://hz.cqqwz.cn/gtkljwhxdu.html

Kotlin ......... 15
来源：http://hz.ybcxt.top/gtrnbvfluv.html

Swift .......... 15
来源：http://hz.zycfv.cn/gtogbtzrqi.html

Lua ............ 10
来源：http://hz.zycfv.cn/gtevooeioc.html

Perl ........... 10
来源：http://hz.tanke756.top/gtwtweptut.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtwswucnhy.html

------------------------------------
来源：http://hz.ehwqpu.com/gtrkwyudra.html

合计 ........... 2106 条
来源：http://hz.fzhhl.top/gtzqynhqwa.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtzczkszer.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtvuxioqrx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtkgencamw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtkcwqfupk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gtkjflgbhh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aibaodan.cn/gtgwjboegl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtffevbaxf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtnxcydpid.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtpouyiuwr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtnjjbhyaz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tianlin.xyz/gtoxaavyzv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtvpjkfrjb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtfkzfexvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtbjncujwb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtdghowxmq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhixingplan.top/gtktqpugdw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtfpdzznkr.html

Q SQL 专题                              90
来源：http://hz.gzhubu.top/gtqkuzisry.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtyqoqdfcy.html

S C / C++ 专题                          60
来源：http://hz.tanke756.top/gtjvbueyxe.html

T 其他语言补充                          60
来源：http://hz.zhoulong.xyz/gtybiyfdiq.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtcebgsktd.html

------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtngyxxvqu.html

合计                                  2106 条
来源：http://hz.shzxlz.cn/gtpmdjanmv.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtmnnvjbak.html

使用提醒
来源：http://hz.wangdashe.top/gtnulinmrl.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtbjlnqswz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tian-w.cn/gtpljzuciy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.wangdashe.top/gtjcmcyyeo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jyoumei.cn/gtzdeqiufg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj20258888.top/gtoqdhladh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fengsongda.top/gtcenkgghx.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtxhahukab.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmnpnzvtk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guowangkeji.top/gttxivctdh.html

Common Programming Examples Cheat Book
来源：http://hz.redwolf501.top/gtcarplrqc.html

================================================================================
来源：http://hz.ybcxt.top/gtgdqspanq.html

【收录内容】
来源：http://hz.zycfv.cn/gtsyxpjiuf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtupszwppy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.wangshuangyany.cn/gtkfagukik.html

SQL · Bash · C · C++
来源：http://hz.yongpay.top/gtnztaujmu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hammf.cn/gtiwlfanbg.html

【使用说明】
来源：http://hz.iojbl.cn/gtqmzfmduc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ydzc1.top/gtycevrxra.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hfpthk.cn/gtiyxuqzio.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gtxrmgjvjx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.havefunace.top/gtsdmzonat.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.mhx1999.top/gtepdczewl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.daria6918.cn/gtttpvovdx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.nanxuanxn.top/gtgtvklcie.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtaqclhovr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yueranfly.top/gtcrgjmhah.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.meibo888.top/gthjgroiqk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhongyouzk.top/gtstuurxiy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jiagoushi.top/gtwfgwfbcv.html

【文件统计】
来源：http://hz.xingfuxueyuan.xyz/gtvxgdngle.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hywenlv.cn/gtcqesbtiz.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtlafeazgo.html

目  录
来源：http://hz.hysaishi.cn/gtfufhmndi.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtfmxhkhgf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtshuwjofz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtiiqwxblq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtgburbpuz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.andypj.xyz/gtxzquoqqm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pengpengdd.cyou/gtwolxbssp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinyuanbaomall.cn/gtuaewzcqx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtwlvafjfa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtqchuefeu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtljpilvxv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtiheuztlx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtaooiquvd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtwantndnf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtbutafhhz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.c1oappe.top/gttokwbwdk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxuanxn.top/gtjylbflxo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtidmetvqn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jyoumei.cn/gtkflaseou.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxinkj.top/gtsobmwhce.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ywan-chungtsiang.top/gtdscsfvna.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtdbwgynve.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtplehzetx.html

================================================================================
来源：http://hz.cucudq.cn/gtrqfezpzq.html

A. 基础语法与类型
来源：http://hz.guowangkeji.top/gtqgacsplj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtusklldah.html

[A01] Hello World
来源：http://hz.zhengqikj.top/gthstxoknc.html

Py:   print("Hello, World!")
来源：http://hz.dashuyun.cn/gtmzionzna.html

PHP:  echo "Hello, World!";
来源：http://hz.yj20258.top/gtdmznobdm.html

JS:   console.log("Hello, World!");
来源：http://hz.gzhubu.top/gtcrklnebn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258.top/gtdrdiwall.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuxming.cn/gtnnwrbwbx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydjk.org.cn/gtoocuoluc.html

Ruby: puts "Hello, World!"
来源：http://hz.ybcxt.top/gtbomlahgx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cucudq.cn/gtcmrtmtoo.html

[A02] 变量声明与赋值
来源：http://hz.hnqzz.top/gtpltkmsue.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yueranfly.top/gtzfghpsri.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nanxinkj.top/gtwbmxkjsv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cdnleiting.top/gtqowwqext.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xuetiantiany.cn/gtbquusdpn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.kuanghao11.cn/gtgtjtovrs.html

Go:   name := "Alex"; age := 20
来源：http://hz.shanyushiyangtech.top/gtjmkcrstc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hfpthk.cn/gtssbyhhhy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtjfxccczr.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtaaerjdmn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xylfe.cn/gtvoibnefm.html

PHP:  const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtqkmoajws.html

JS:   const PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtvkigdizk.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtrjhuymtc.html

Java: static final double PI = 3.14159;
来源：http://hz.c1oappe.top/gtiptnhpys.html

Go:   const PI = 3.14159
来源：http://hz.xingfuxueyuan.xyz/gtpmodsgim.html

Ruby: PI = 3.14159
来源：http://hz.chenjidiqi.icu/gtbompldno.html

C#:   const double PI = 3.14159;
来源：http://hz.yueranfly.top/gttebhjrwh.html

[A04] 判断变量类型
来源：http://hz.nanxinkj.top/gttyqprrjc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigufen.top/gtbmpiycdn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.316326.xyz/gtfpwewlzo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yanxiufei.cn/gtugvqjvmh.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtokgkhqnp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sxryk.cn/gtvmuwxdii.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnqzz.top/gtlpluouza.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sxryk.cn/gtgvkxmljd.html

C#:   x.GetType().Name; x is int
来源：http://hz.tian-w.cn/gtpjxvgzzz.html

[A05] 整数除法与取模
来源：http://hz.xuanzx.com/gtntbmxisg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangkeji.top/gtvzccvwcx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.0kj1m.cn/gtmtjmcelx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hysaishi.cn/gtdifvrxse.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuxming.cn/gtgmbklznp.html

Java: 7 / 2; 7 % 2
来源：http://hz.hnqzz.top/gtbxynrqsi.html

Go:   7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtlqjmzmax.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtcprxusjd.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtizftccyi.html

[A06] 字符串转数字
来源：http://hz.hnqzz.top/gtjuigbpqv.html

Py:   int("42"); float("3.14")
来源：http://hz.ydzc1.top/gtaeagukky.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.vqdsnc.cn/gtearcepyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cdnleiting.top/gttnojwyxd.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.birdmap.top/gtmbuqkgmw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zdqjudy.top/gtuepumiky.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xylfe.cn/gtyellbejk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yuanzhike.top/gtcjvuhgeb.html


<!-- 参考信息 -->