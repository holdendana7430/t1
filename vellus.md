代发 wailian999

[U49] PHP：只读属性
来源：http://hz.hnqzz.top/gtqmmjeomd.html

public readonly string $name
来源：http://hz.52xcode.cn/gtzcrxwrur.html

[U50] PHP：构造器属性提升
来源：http://hz.redwolf501.top/gtzdlspmpd.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtbehxtldq.html

[U51] PHP：数组解构
来源：http://hz.guannengcc.top/gtindasgkn.html

[$a, $b] = $arr;
来源：http://hz.svipenyu.cn/gtfgrucaoh.html

[U52] PHP：箭头函数
来源：http://hz.birdmap.top/gtdwdckudh.html

$double = fn($x) => $x * 2;
来源：http://hz.zhengqikj.top/gtdyhxpzxj.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigufen.top/gtrizczzso.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtetohbnyz.html

[U54] PHP：空安全调用
来源：http://hz.zhixingplan.top/gtrymmpmco.html

$obj?->method()
来源：http://hz.52xcode.cn/gthoplskpm.html

[U55] PHP：match 表达式
来源：http://hz.havefunace.top/gtrmzcwans.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gaohongyu789.top/gtmgaurtex.html

[U56] PHP：命名参数
来源：http://hz.hfpthk.cn/gtddnqdxgc.html

f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtahclwtde.html

[U57] PHP：字符串插值
来源：http://hz.yuanzhike.top/gtrpwfpivh.html

"值: {$a}"
来源：http://hz.iojbl.cn/gtoupnnjtu.html

[U58] PHP：数组三件套
来源：http://hz.cheryme.top/gtwlqhoevm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuetiantiany.cn/gtsipmidwr.html

[U59] PHP：自定义排序
来源：http://hz.zhoulong.xyz/gthdanhhog.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtvbvvpdxd.html

[U60] PHP：JSON 编解码
来源：http://hz.shzxlz.cn/gtsaonikld.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.mhx1999.top/gtauszmitx.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtqwbkchxm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.aibaodan.cn/gtqeanbuds.html

[U62] PHP：日期对象
来源：http://hz.sweek.top/gtuuhpdxga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ydzc1.top/gtygbsygwh.html

[U63] PHP：文件读写
来源：http://hz.nanxuanxn.top/gtnobxtpbv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jlsjyb.cn/gtryosogna.html

[U64] PHP：目录遍历
来源：http://hz.jinyuanbaomall.cn/gtrwmmtcrf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hammf.cn/gtxfdwzznn.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtucfssfmu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gtomnncqmd.html

[U66] PHP：设置 Cookie
来源：http://hz.ivvv.top/gtocoiyvfl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gzhubu.top/gtatfmsfmw.html

[U67] PHP：处理文件上传
来源：http://hz.zhiwuduotai.top/gtyupjhwvo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cheryme.top/gtptcwavbl.html

[U68] PHP：PDO 连接
来源：http://hz.quarkkingdee.top/gtbenbmyms.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cdnleiting.top/gtolmhrgww.html

[U69] PHP：PDO 预处理
来源：http://hz.hnxiangtu.top/gtpfkdypvs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtdxjeyzgb.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigfzy.top/gtddrrwqau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gtpvulxuzk.html

[U71] PHP：抛出异常
来源：http://hz.wangshuangyany.cn/gtqvsoingl.html

throw new RuntimeException("失败", 500);
来源：http://hz.gzhubu.top/gtvyuqkxrq.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gttpesjjav.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtgyaxpjeh.html

[U73] PHP：读取 ini 配置
来源：http://hz.xziqi.cn/gtlnqkofxy.html

parse_ini_file("config.ini", true)
来源：http://hz.zhengqikj.top/gtffsacpkr.html

[U74] PHP：读取环境变量
来源：http://hz.hysaishi.cn/gtcxchsnvj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dianchejie.cn/gtwdwaxyen.html

[U75] PHP：依赖注入
来源：http://hz.cqqwz.cn/gtbkqhgjge.html

composer require psr/container
来源：http://hz.yangfankeji.com/gtlattfdjj.html

[U76] PHP：简单路由
来源：http://hz.pengpengdd.cyou/gtmfcrfkir.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangtech.top/gtldcztgnz.html

[U77] PHP：模板渲染
来源：http://hz.cheryme.top/gthfoxnxjb.html

composer require twig/twig
来源：http://hz.xziqi.cn/gtkuficrmh.html

[U78] PHP：单元测试
来源：http://hz.shzxlz.cn/gttkrigtmz.html

composer require --dev phpunit/phpunit
来源：http://hz.xuetiantiany.cn/gtemjksrab.html

[U79] PHP：静态分析
来源：http://hz.kuanghao11.cn/gtiigacrlz.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxinkj.top/gthvmrwvzm.html

[U80] PHP：代码规范修复
来源：http://hz.feifeiyinyue.top/gtnnnpzrxo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.vqdsnc.cn/gtqjvhighe.html

[U81] JS：初始化项目
来源：http://hz.yuanzhike.top/gtimlnrixd.html

npm init -y;  npm i express
来源：http://hz.yueranfly.top/gtlktufsoz.html

[U82] JS：package.json 脚本
来源：http://hz.nanxinkj.top/gtofzdhaad.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhiwuduotai.top/gtxtzxexhh.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenjidiqi.icu/gtdtcwmcdw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gtvnyytpjp.html

[U84] JS：CommonJS 写法
来源：http://hz.shangyingyoupin.top/gthfunrkvc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigfzy.top/gtplunusnb.html

[U85] JS：可选链
来源：http://hz.tanke756.top/gtipryikry.html

a?.b?.c
来源：http://hz.hnxiangtu.top/gtvrrkldxh.html

[U86] JS：空值合并
来源：http://hz.cheryme.top/gtjnulevwt.html

a ?? b
来源：http://hz.nanxinkj.top/gtcplxfsgo.html

[U87] JS：解构默认值
来源：http://hz.nanxinkj.top/gtautwlcka.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gotoacloud.top/gtxntiqsci.html

[U88] JS：对象展开合并
来源：http://hz.hysaishi.cn/gttgbcrrub.html

{ ...a, ...b }
来源：http://hz.ybcxt.top/gtcdpbbcxp.html

[U89] JS：数组去重
来源：http://hz.shangyingyoupin.top/gtigsenezg.html

[...new Set(arr)]
来源：http://hz.snrcjt.cn/gtzrsjduzc.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtvvhqguwb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtwsmjyrsk.html

[U91] JS：对象键值遍历
来源：http://hz.jinyuanbaomall.cn/gtfjwtyvlx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cheryme.top/gtunsbzhwk.html

[U92] JS：深拷贝
来源：http://hz.jinghuilouyu.cn/gtrsfhfjer.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtpmhmpzix.html

[U93] JS：模板字符串
来源：http://hz.ybcxt.top/gtphgkyjmb.html

`共 ${n} 条`
来源：http://hz.yj20258888.top/gtglafjdhc.html

[U94] JS：箭头函数
来源：http://hz.pengpengdd.cyou/gtdyshgeuc.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtvujknxee.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtcvkyonqe.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtiicpzfgu.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigufen.top/gtdubtidgu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtjtrzpbnm.html

[U97] JS：并发请求
来源：http://hz.ywan-chungtsiang.top/gttrofjdot.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtpsmgpvnw.html

[U98] JS：fetch 带 JSON
来源：http://hz.iojbl.cn/gtfmwdkfvp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenjidiqi.icu/gtncmtpsyr.html

[U99] JS：事件监听
来源：http://hz.ydzc1.top/gtwcpcpxfe.html

el.addEventListener("click", e => {})
来源：http://hz.jiagoushi.top/gtkhkmqqcd.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtbwprchlo.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gtgvppiaoo.html

[U101] JS：classList 操作
来源：http://hz.tian-w.cn/gtlbuertdd.html

el.classList.toggle("active")
来源：http://hz.jianghu66.top/gtbmnwnahd.html

[U102] JS：本地存储
来源：http://hz.cheryme.top/gtrgxmtomu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtmvmfqdlo.html

[U103] JS：定时器
来源：http://hz.gotoacloud.top/gtvmjwjlqv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yonumen.top/gtrfssolvu.html

[U104] JS：防抖
来源：http://hz.yonumen.top/gtiwyztdfe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtlxnnpdvo.html

[U105] JS：节流
来源：http://hz.yangfankeji.com/gtiullitun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hywenlv.cn/gtxhotiynj.html

[U106] JS：日期格式化
来源：http://hz.hfpthk.cn/gtelodwedx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.mhx1999.top/gtnresiozu.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtqtzbhpyj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.0kj1m.cn/gtwxptibot.html

[U108] JS：随机整数
来源：http://hz.nanxinkj.top/gtlpoqzvum.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangkeji.top/gtivppeabf.html

[U109] JS：数组分组
来源：http://hz.bjfxy.top/gtnetyohqy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtrdxiimhn.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtxkjmfndy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fzhhl.top/gtyfmqdrmf.html

[U111] JS：对象转 Map
来源：http://hz.nwbrower.top/gtepualudp.html

new Map(Object.entries(obj))
来源：http://hz.hysaishi.cn/gtpamvlahy.html

[U112] JS：字符串补位
来源：http://hz.c1oappe.top/gthnptkklz.html

"7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtjriypaeb.html

[U113] JS：正则替换全部
来源：http://hz.xuanzx.com/gttcpuqqeg.html

s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtopfqhnrs.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtgkpilaiv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtgpzwabli.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtwmyqxtkn.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtmzdbgvcr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtsdgclnum.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jianghu66.top/gtxomzwomd.html

[U117] JS：单元测试
来源：http://hz.feifeiyinyue.top/gtoycmqust.html

npm i -D vitest;  npx vitest
来源：http://hz.shzxlz.cn/gtorlgcndn.html

[U118] JS：开发服务器
来源：http://hz.yvedp.cn/gtokzwvxlt.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gtxcphfaxj.html

[U119] JS：生产构建
来源：http://hz.aibaodan.cn/gtlxbapnzk.html

npx vite build
来源：http://hz.ppjwa.cn/gtgtsfaepr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daxiang520.top/gtiwzfatjo.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangkeji.top/gtygoujxlj.html

================================================================================
来源：http://hz.tanke756.top/gtxugpmyof.html

统计汇总
来源：http://hz.bjfxy.top/gtcyhatdiy.html

================================================================================
来源：http://hz.havefunace.top/gtqslipwwm.html

按语言统计（条）：
来源：http://hz.xinyue.icu/gtyydmlmgg.html

Python ......... 252
来源：http://hz.tanke756.top/gtvjsxgjne.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtfiyicahf.html

JavaScript ..... 252
来源：http://hz.ivvv.top/gtvupfxrct.html

TypeScript ..... 212
来源：http://hz.shanyushiyangtech.top/gtqdajdeca.html

Java ........... 212
来源：http://hz.birdmap.top/gtqajbgehr.html

Go ............. 212
来源：http://hz.gzhubu.top/gtouyiapti.html

Ruby ........... 212
来源：http://hz.hfpthk.cn/gtefyznkbv.html

C# ............. 212
来源：http://hz.tian-w.cn/gtqwapcpce.html

C .............. 30
来源：http://hz.ywan-chungtsiang.top/gtvatjvjql.html

C++ ............ 30
来源：http://hz.zhongyouzk.top/gtcqomlgfs.html

SQL ............ 90
来源：http://hz.9152youxi.cn/gtfyaqgske.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtsnusycih.html

Kotlin ......... 15
来源：http://hz.gotoacloud.top/gtttzpjgzu.html

Swift .......... 15
来源：http://hz.chenlongwang.top/gtdkxjgqul.html

Lua ............ 10
来源：http://hz.ybcxt.top/gtgikkwwjz.html

Perl ........... 10
来源：http://hz.hongshengwenyu.top/gtkngiamok.html

Scala .......... 10
来源：http://hz.hnxiangtu.top/gtlzgrrtfj.html

------------------------------------
来源：http://hz.cqqwz.cn/gtqbktjsvc.html

合计 ........... 2106 条
来源：http://hz.havefunace.top/gtglghoayy.html

按章节统计：
来源：http://hz.zhongyouzk.top/gtguotafgl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtvbkwwkxn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtmsskmgqb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtcykidwkx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtjdjgzcpn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shuidangran.top/gtjldjyhqc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtuihkuxlr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtgfeoidwd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtmgbgdwoa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtberkscbw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtyubsvlvi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtutvklxai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtbyssyswk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtrynlwpif.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtlhuukksw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.feifeiyinyue.top/gtmactgikr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gttwlprcwb.html

Q SQL 专题                              90
来源：http://hz.tanke756.top/gtjkhiajfg.html

R Bash 专题                             80
来源：http://hz.cheryme.top/gtqlbkwniw.html

S C / C++ 专题                          60
来源：http://hz.yuanzhike.top/gtjmtcschd.html

T 其他语言补充                          60
来源：http://hz.yj202588.top/gtcgggjubi.html

U 高频实用片段                         120
来源：http://hz.daxiang520.top/gtjxgwiten.html

------------------------------------
来源：http://hz.jinqigufen.top/gtbepruwtx.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gteovoocpv.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtlwurpsrt.html

使用提醒
来源：http://hz.hammf.cn/gtlworfrry.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtlbtlmmxy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtcgxltimi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.aizwys.cn/gthzzcdniu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.birdmap.top/gtpplnjhur.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.pengpengdd.cyou/gtwslyirva.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xuetiantiany.cn/gtgburzcfh.html

—— 文件结束 ——
来源：http://hz.gotoacloud.top/gtczjrkvim.html

================================================================================
来源：http://hz.yuxming.cn/gtyosjdnog.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.316326.xyz/gtupmahcec.html

Common Programming Examples Cheat Book
来源：http://hz.xinyue.icu/gtxzkmtell.html

================================================================================
来源：http://hz.yvedp.cn/gtmnkvcssu.html

【收录内容】
来源：http://hz.hnxiangtu.top/gthnhknuup.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.feifeiyinyue.top/gtqnbmdeoz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.316326.xyz/gtdrbqsbmy.html

SQL · Bash · C · C++
来源：http://hz.zhixingplan.top/gtimqgemgu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtmkgnuxyy.html

【使用说明】
来源：http://hz.svipenyu.cn/gtzsdukfia.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.meibo888.top/gtxlwoajmh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tanke756.top/gtnorhzxhb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gtemfqoacc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.kuanghao11.cn/gtrogffofb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhoulong.xyz/gtdjzbbukm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.quarkkingdee.top/gthgpbpomi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yueranfly.top/gtkkckosdl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gogol.net.cn/gtjhsownvo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinyuanbaomall.cn/gtfpntfxei.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ppjwa.cn/gtceiwmpqf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.quarkkingdee.top/gtmunkdyuj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ybcxt.top/gttroggmoq.html

【文件统计】
来源：http://hz.shzxlz.cn/gtvhkcnuii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ydzc1.top/gtvhloxahq.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gttkkfqztw.html

目  录
来源：http://hz.yj20258.top/gtfpxmchea.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtoogertzc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtkcntvcyw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtwihawgkx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenjidiqi.icu/gtyyezassi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gtpowhovlz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.haohaochexian.top/gtkftumxin.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtgyiggdec.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ywan-chungtsiang.top/gtdiicgmtu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cdnleiting.top/gtmhamtwlp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtacmfclcd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gteznqvwah.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gttcfwdblc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtjocxsztr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtjdtugclv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtgwdeqkol.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.mhx1999.top/gtpzpresvr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtciylxpvt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhaomingkeji.xyz/gtuksmjeoz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nwbrower.top/gtkqbtescb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhongyouzk.top/gttmirepmw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtuaoojicv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtyfbdmzdx.html

================================================================================
来源：http://hz.zhengqikj.top/gtmhbpypyx.html

A. 基础语法与类型
来源：http://hz.jyoumei.cn/gtdxfvxkzl.html

================================================================================
来源：http://hz.andypj.xyz/gtpjewxvir.html

[A01] Hello World
来源：http://hz.ybcxt.top/gtmncyfpho.html

Py:   print("Hello, World!")
来源：http://hz.yongpay.top/gtavepfuxo.html

PHP:  echo "Hello, World!";
来源：http://hz.hnqzz.top/gtinwwnbcf.html

JS:   console.log("Hello, World!");
来源：http://hz.birdmap.top/gtupvlyejy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.0kj1m.cn/gtyhprmaon.html

Java: System.out.println("Hello, World!");
来源：http://hz.jyoumei.cn/gtziijqsxi.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gtzjluxfjz.html

Ruby: puts "Hello, World!"
来源：http://hz.mhx1999.top/gtkglejyzl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnqzz.top/gtxyilusff.html

[A02] 变量声明与赋值
来源：http://hz.bjfxy.top/gtankbkegc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.dashuyun.cn/gtxkcmgvbq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yvedp.cn/gtbjwibbbb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenzaomai.com/gtwyfxnxfp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.iojbl.cn/gthshjivny.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sysykeji.top/gtnakdynyp.html

Go:   name := "Alex"; age := 20
来源：http://hz.nanxuanxn.top/gtfusvwqor.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hfpthk.cn/gtsoomxiuf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtxfgammzo.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtkwrklrxe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.316326.xyz/gtqyteavqs.html

PHP:  const PI = 3.14159;
来源：http://hz.jianghu66.top/gtgdckyclo.html

JS:   const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtgicblygf.html

TS:   const PI: number = 3.14159;
来源：http://hz.pengpengdd.cyou/gtbntveyfd.html

Java: static final double PI = 3.14159;
来源：http://hz.jianghu66.top/gtoxcghnli.html

Go:   const PI = 3.14159
来源：http://hz.snrcjt.cn/gtrolzaoxu.html

Ruby: PI = 3.14159
来源：http://hz.zhiwuduotai.top/gtsuuqfvoh.html

C#:   const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtibhnriad.html

[A04] 判断变量类型
来源：http://hz.mhx1999.top/gtklhvjaun.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zdqjudy.top/gtsyjxynht.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.0kj1m.cn/gtubbrftww.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yj202588.top/gtwshourls.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhijiandao.cn/gtdecmpzfj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ehwqpu.com/gthhptgqse.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj202588.top/gtdwlkjzcu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.birdmap.top/gtsqtljfwp.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtcphetpdk.html

[A05] 整数除法与取模
来源：http://hz.havefunace.top/gturejxjoc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj202588.top/gtsguvykcs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.birdmap.top/gtvsghwily.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cucudq.cn/gtltysargr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gtjyxquioc.html

Java: 7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtuqpedotq.html

Go:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtxjeessix.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtuebchrkv.html

C#:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtfhiuikss.html

[A06] 字符串转数字
来源：http://hz.sysykeji.top/gtnadbcviu.html

Py:   int("42"); float("3.14")
来源：http://hz.sweek.top/gtiiizcumx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.dianchejie.cn/gtxsfkhzlf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.quarkkingdee.top/gtybqesnqg.html


<!-- 参考信息 -->