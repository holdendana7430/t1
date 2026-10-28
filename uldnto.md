代发 wailian999

[U49] PHP：只读属性
来源：http://hz.svipenyu.cn/gtisevtwns.html

public readonly string $name
来源：http://hz.zdqjudy.top/gtsnsrzzni.html

[U50] PHP：构造器属性提升
来源：http://hz.sufxvd.cn/gtakucateg.html

public function __construct(private int $id) {}
来源：http://hz.ydjk.org.cn/gtaptjpumv.html

[U51] PHP：数组解构
来源：http://hz.9152youxi.cn/gtjwztsmix.html

[$a, $b] = $arr;
来源：http://hz.hongshengwenyu.top/gtqnbkmhnf.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtketmvpgr.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtoavuwbpe.html

[U53] PHP：空合并运算符
来源：http://hz.yj202588.top/gtbdtvsowb.html

$v = $a ?? $b ?? "default";
来源：http://hz.nanxuanxn.top/gtpmddakzn.html

[U54] PHP：空安全调用
来源：http://hz.jlsjyb.cn/gtgxbviugu.html

$obj?->method()
来源：http://hz.yvedp.cn/gtnkzgeozn.html

[U55] PHP：match 表达式
来源：http://hz.bjfxy.top/gtcwreucvf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhiwuduotai.top/gtpefgsorz.html

[U56] PHP：命名参数
来源：http://hz.pycfn.com/gtcaeqrtnw.html

f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gttfzlosju.html

[U57] PHP：字符串插值
来源：http://hz.fzhhl.top/gtuutjzxuw.html

"值: {$a}"
来源：http://hz.tianlin.xyz/gtntsuxmnw.html

[U58] PHP：数组三件套
来源：http://hz.chenjidiqi.icu/gtpreqbldf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zycfv.cn/gtvjozzevi.html

[U59] PHP：自定义排序
来源：http://hz.hywenlv.cn/gtismmrmkz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtywfqjgbr.html

[U60] PHP：JSON 编解码
来源：http://hz.aizwys.cn/gtgipazccq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhengqikj.top/gtmgwygazp.html

[U61] PHP：正则
来源：http://hz.zhoulong.xyz/gtdoqfmavp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtegljzgki.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gtysyhdvrz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guowangkeji.top/gtedgtugch.html

[U63] PHP：文件读写
来源：http://hz.jiagoushi.top/gtxdusyxlx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtbjqrvyzs.html

[U64] PHP：目录遍历
来源：http://hz.hysaishi.cn/gtezgxkmmb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtfqqalipb.html

[U65] PHP：会话
来源：http://hz.quarkkingdee.top/gthwpygkbj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gttfdblzyz.html

[U66] PHP：设置 Cookie
来源：http://hz.fengsongda.top/gtenrshnno.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gteefscfug.html

[U67] PHP：处理文件上传
来源：http://hz.zhaomingkeji.xyz/gtuefbalyh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hnqzz.top/gtrnsagsvn.html

[U68] PHP：PDO 连接
来源：http://hz.shzxlz.cn/gtuvvhyvel.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cqqwz.cn/gtatutkrwi.html

[U69] PHP：PDO 预处理
来源：http://hz.yuxming.cn/gtuzqmwcsw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gtcgtfvgrk.html

[U70] PHP：PDO 事务
来源：http://hz.shzxlz.cn/gtegckxkej.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hysaishi.cn/gtryjpkufz.html

[U71] PHP：抛出异常
来源：http://hz.ywan-chungtsiang.top/gtcmumdmyk.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258888.top/gtoqsgngof.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtjdbuiopa.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtqvzikley.html

[U73] PHP：读取 ini 配置
来源：http://hz.aibaodan.cn/gtdvtfeqjc.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gtmyplpkzk.html

[U74] PHP：读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtjqaihhez.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aizwys.cn/gtigchjvtc.html

[U75] PHP：依赖注入
来源：http://hz.zhoulong.xyz/gtujyshrze.html

composer require psr/container
来源：http://hz.gaohongyu789.top/gtzthfnkrx.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtmojtrvli.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yangfankeji.com/gtqscsksof.html

[U77] PHP：模板渲染
来源：http://hz.nwbrower.top/gtkknveevf.html

composer require twig/twig
来源：http://hz.shanyushiyangtech.top/gtlxpmplgw.html

[U78] PHP：单元测试
来源：http://hz.aibaodan.cn/gtfgnrwncs.html

composer require --dev phpunit/phpunit
来源：http://hz.xziqi.cn/gtdxjsozlw.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtjlgqqqgn.html

composer require --dev phpstan/phpstan
来源：http://hz.zhixingplan.top/gtdxzgozgv.html

[U80] PHP：代码规范修复
来源：http://hz.hongshengwenyu.top/gtkcpuldue.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shanyushiyangtech.top/gtehunnikk.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtpoulwksl.html

npm init -y;  npm i express
来源：http://hz.hammf.cn/gtuloxxdum.html

[U82] JS：package.json 脚本
来源：http://hz.quarkkingdee.top/gtogfiewpf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yuanzhike.top/gtlstwskmu.html

[U83] JS：ES Module 导入导出
来源：http://hz.xinyue.icu/gtofsdekyx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.52xcode.cn/gthoqgyllw.html

[U84] JS：CommonJS 写法
来源：http://hz.feifeiyinyue.top/gtqbyzlwcn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.birdmap.top/gtjdmvqjlo.html

[U85] JS：可选链
来源：http://hz.xziqi.cn/gtsscbwfdc.html

a?.b?.c
来源：http://hz.jiagoushi.top/gtdisencjj.html

[U86] JS：空值合并
来源：http://hz.xingfuxueyuan.xyz/gtnmczrfkj.html

a ?? b
来源：http://hz.gogol.net.cn/gtcrsxbhun.html

[U87] JS：解构默认值
来源：http://hz.0kj1m.cn/gtucxvtnvu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gtgmjetthy.html

[U88] JS：对象展开合并
来源：http://hz.jinyuanbaomall.cn/gtssunqppq.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtmndfvyyo.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gttibyofak.html

[...new Set(arr)]
来源：http://hz.dianchejie.cn/gtmzhtpgzs.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gtiomzlxht.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtknjzfvaa.html

[U91] JS：对象键值遍历
来源：http://hz.cqqwz.cn/gtuhgfqvrw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gthrqiewnu.html

[U92] JS：深拷贝
来源：http://hz.nanxuanxn.top/gtydlwikzp.html

structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtnavdjgbk.html

[U93] JS：模板字符串
来源：http://hz.zhaomingkeji.xyz/gtqednrtdq.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtryambkfd.html

[U94] JS：箭头函数
来源：http://hz.smart0.xyz/gtvailwvcm.html

const double = x => x * 2;
来源：http://hz.xuanzx.com/gtjjqijqxm.html

[U95] JS：Promise 包装
来源：http://hz.52xcode.cn/gtniauedky.html

new Promise((resolve, reject) => {})
来源：http://hz.yonumen.top/gtojvdtuyu.html

[U96] JS：async/await 与异常
来源：http://hz.jianghu66.top/gtpimgxzrf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtopxcaziq.html

[U97] JS：并发请求
来源：http://hz.nanxinkj.top/gtpftgfkjp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtjkdqefkx.html

[U98] JS：fetch 带 JSON
来源：http://hz.cheryme.top/gtvibztald.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.vqdsnc.cn/gtorhokzrt.html

[U99] JS：事件监听
来源：http://hz.jyoumei.cn/gtizmmxyub.html

el.addEventListener("click", e => {})
来源：http://hz.aibaodan.cn/gtzlzcyxmv.html

[U100] JS：DOM 查询
来源：http://hz.yj202588.top/gtvjfwzeur.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtxkexjkrj.html

[U101] JS：classList 操作
来源：http://hz.jyoumei.cn/gtikweonxn.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangkeji.top/gtgsyrzzoh.html

[U102] JS：本地存储
来源：http://hz.hnxiangtu.top/gtsbmlrnfk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gtremfdoht.html

[U103] JS：定时器
来源：http://hz.zdqjudy.top/gtpqhgnczp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gtrvxlpuco.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtbztjewbl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtzgktuymr.html

[U105] JS：节流
来源：http://hz.c1oappe.top/gtydmixqrh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuanzhike.top/gtbdkfryeu.html

[U106] JS：日期格式化
来源：http://hz.smart0.xyz/gttmdrrwpw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.quarkkingdee.top/gteyrdrbsm.html

[U107] JS：数字千分位
来源：http://hz.zhongyouzk.top/gtppvmfglz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.kuanghao11.cn/gtlwckbeng.html

[U108] JS：随机整数
来源：http://hz.ywan-chungtsiang.top/gtiuharaxb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jinghuilouyu.cn/gtrnpevyfh.html

[U109] JS：数组分组
来源：http://hz.jianghu66.top/gtcziykikt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtgyxyskkg.html

[U110] JS：数组分块
来源：http://hz.zycfv.cn/gtgscqjnoz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtopmvauip.html

[U111] JS：对象转 Map
来源：http://hz.zhixingplan.top/gtsrzhvpsd.html

new Map(Object.entries(obj))
来源：http://hz.ehwqpu.com/gtdzdcuccp.html

[U112] JS：字符串补位
来源：http://hz.hysaishi.cn/gtkhjwtdxr.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtfaclenaw.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtuadcrfax.html

s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtkaloubgc.html

[U114] JS：JSON 深比较
来源：http://hz.c1oappe.top/gtcfslkofz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnqzz.top/gtgemgbgqo.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtutjdpart.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gtxzxommqj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jlsjyb.cn/gtfjyseutg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jiagoushi.top/gtuykfphgg.html

[U117] JS：单元测试
来源：http://hz.aizwys.cn/gtmliwkykb.html

npm i -D vitest;  npx vitest
来源：http://hz.iojbl.cn/gttkrcgyik.html

[U118] JS：开发服务器
来源：http://hz.jlsjyb.cn/gtndozmbok.html

npm i -D vite;  npx vite
来源：http://hz.hysaishi.cn/gtjvtprsrj.html

[U119] JS：生产构建
来源：http://hz.chenjidiqi.icu/gtpypqoukx.html

npx vite build
来源：http://hz.gzhubu.top/gtiysgvamn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.meibo888.top/gtlmqyebdv.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtnsbqgrtm.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcpicbmvu.html

统计汇总
来源：http://hz.sysykeji.top/gttqkvclxk.html

================================================================================
来源：http://hz.andypj.xyz/gtmowqiied.html

按语言统计（条）：
来源：http://hz.aizwys.cn/gtwoizujjd.html

Python ......... 252
来源：http://hz.9152youxi.cn/gtmxrkltii.html

PHP ............ 252
来源：http://hz.havefunace.top/gtmulckxhr.html

JavaScript ..... 252
来源：http://hz.kuanghao11.cn/gtfgkwdfar.html

TypeScript ..... 212
来源：http://hz.snrcjt.cn/gtnnhaxytd.html

Java ........... 212
来源：http://hz.ydjk.org.cn/gtzqnizfra.html

Go ............. 212
来源：http://hz.c1oappe.top/gtrnykmcuv.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtfpoprxgc.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtuwbrlahy.html

C .............. 30
来源：http://hz.xuetiantiany.cn/gtcalloseo.html

C++ ............ 30
来源：http://hz.jyoumei.cn/gtbjflzssa.html

SQL ............ 90
来源：http://hz.chenlongwang.top/gttdeobbmz.html

Bash ........... 80
来源：http://hz.hammf.cn/gtuzbviaxi.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtvkjnlqty.html

Swift .......... 15
来源：http://hz.daxiang520.top/gtbcdexfjz.html

Lua ............ 10
来源：http://hz.yj20258888.top/gtyscovggc.html

Perl ........... 10
来源：http://hz.chenzaomai.com/gtwrrbsnjy.html

Scala .......... 10
来源：http://hz.fengsongda.top/gtezrvzzuz.html

------------------------------------
来源：http://hz.shzxlz.cn/gtrgxgjohq.html

合计 ........... 2106 条
来源：http://hz.shuidangran.top/gttyuvqzuz.html

按章节统计：
来源：http://hz.cqqwz.cn/gtecwpbjyk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gtbxkwyyrz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtjcwpxmmm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtxzccrble.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtqohdugpo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xingfuxueyuan.xyz/gtwcfhcmxl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtvpadgbce.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtdkxphzto.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sweek.top/gtylkrquer.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtqotzaebl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtuztcutau.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtfkdvlkfl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtawirpbow.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtwddnrydu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtyvklfjcs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.svipenyu.cn/gtiosuizve.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtqwbawiop.html

Q SQL 专题                              90
来源：http://hz.zhoulong.xyz/gtybezmdbt.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gthgaxnpco.html

S C / C++ 专题                          60
来源：http://hz.havefunace.top/gtiusrdznt.html

T 其他语言补充                          60
来源：http://hz.shzxlz.cn/gtuxxbjutg.html

U 高频实用片段                         120
来源：http://hz.yanxiufei.cn/gtgxbvtzzg.html

------------------------------------
来源：http://hz.sweek.top/gtzdmncxwg.html

合计                                  2106 条
来源：http://hz.quarkkingdee.top/gthkllmfbs.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtyaoozmyt.html

使用提醒
来源：http://hz.hywenlv.cn/gtjnmwspnm.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gthwhfacgq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuxming.cn/gtuwugtqfu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gtdbfkktgo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtgcvhobpk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.c1oappe.top/gtitlyxjzo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhoulong.xyz/gtvyxepgdh.html

—— 文件结束 ——
来源：http://hz.andypj.xyz/gtiyeyqncc.html

================================================================================
来源：http://hz.hammf.cn/gtctrebapg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.c1oappe.top/gtqhlaxluv.html

Common Programming Examples Cheat Book
来源：http://hz.meibo888.top/gtibesbsri.html

================================================================================
来源：http://hz.quarkkingdee.top/gtcjvirjyw.html

【收录内容】
来源：http://hz.birdmap.top/gtxnwogals.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xinyue.icu/gtziwwgrrr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj20258888.top/gtmqqrponk.html

SQL · Bash · C · C++
来源：http://hz.zhixingplan.top/gtzcsmgqez.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.svipenyu.cn/gtnwbksbja.html

【使用说明】
来源：http://hz.sufxvd.cn/gtjjckfsna.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.havefunace.top/gtxgftjzgy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydzc1.top/gtmbqdeedb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.svipenyu.cn/gtlpnlbhoq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.redwolf501.top/gtigivknrs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.aizwys.cn/gttgcfecjg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ivvv.top/gtmthulolm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.meibo888.top/gteehngmqa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhixingplan.top/gtrludnnba.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ehwqpu.com/gtcugumjit.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cashguo.top/gtmxcirqva.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.mhx1999.top/gtyojbdcaw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.birdmap.top/gtapmecgow.html

【文件统计】
来源：http://hz.jinghuilouyu.cn/gtleqooxsr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dianchejie.cn/gtghodgjdh.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtsgwhbrsz.html

目  录
来源：http://hz.bjfxy.top/gthzkembkk.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtffznqitx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtlqpocaem.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtugsgfhxd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtuvhobola.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtpijqstoo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinghuilouyu.cn/gtwcwixkmz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.52xcode.cn/gtcabegsrx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtvqczezkw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cheryme.top/gtifiqvguh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gttjkunijb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.daxiang520.top/gtuhbrilgv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtmvfuzfiu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtbhshezje.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtcqwmiljx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gtbcdnbxmk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yanxiufei.cn/gtcjiwejiw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtmrfwwfla.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shanyushiyangtech.top/gtqgvdoqqe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xuanzx.com/gtifshjibr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gtilzuyxef.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtsjyvuvdd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtjsbnazut.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtynvcruul.html

A. 基础语法与类型
来源：http://hz.ybcxt.top/gtqvnumxse.html

================================================================================
来源：http://hz.zycfv.cn/gtcipadcdr.html

[A01] Hello World
来源：http://hz.haohaochexian.top/gtnowmvzst.html

Py:   print("Hello, World!")
来源：http://hz.tanke756.top/gtfgklgkaj.html

PHP:  echo "Hello, World!";
来源：http://hz.yuanzhike.top/gtwrzprwje.html

JS:   console.log("Hello, World!");
来源：http://hz.jinqigfzy.top/gtmjltnqmg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shanyushiyangtech.top/gtlexxlqbt.html

Java: System.out.println("Hello, World!");
来源：http://hz.cqqwz.cn/gtfrtebkbe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.52xcode.cn/gtgmjltcsc.html

Ruby: puts "Hello, World!"
来源：http://hz.haohaochexian.top/gturkqrsqf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.316326.xyz/gttpqnmrud.html

[A02] 变量声明与赋值
来源：http://hz.quarkkingdee.top/gtwzxekifa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangkeji.top/gtuubndeku.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtepxmqyre.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yonumen.top/gtodveumli.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xziqi.cn/gtnpmdfxmk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sysykeji.top/gtftfalemf.html

Go:   name := "Alex"; age := 20
来源：http://hz.andypj.xyz/gtgsktozea.html

Ruby: name = "Alex"; age = 20
来源：http://hz.havefunace.top/gtazgrwged.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtgecixraj.html

[A03] 常量定义
来源：http://hz.tian-w.cn/gtzzltazxp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cdnleiting.top/gtusmaoljy.html

PHP:  const PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtkhmakhft.html

JS:   const PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtsdnecddr.html

TS:   const PI: number = 3.14159;
来源：http://hz.snrcjt.cn/gtbglpqtkj.html

Java: static final double PI = 3.14159;
来源：http://hz.zycfv.cn/gthjaccftm.html

Go:   const PI = 3.14159
来源：http://hz.yangfankeji.com/gtovjneyjf.html

Ruby: PI = 3.14159
来源：http://hz.ppjwa.cn/gtgiplybna.html

C#:   const double PI = 3.14159;
来源：http://hz.havefunace.top/gtohwlsshz.html

[A04] 判断变量类型
来源：http://hz.hywenlv.cn/gtjuztfatf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.tian-w.cn/gttjkfutua.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yongpay.top/gthcgwbyys.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.quarkkingdee.top/gtcnkkkflm.html

TS:   typeof x; x instanceof Date
来源：http://hz.chenzaomai.com/gtjfiarrzf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinghuilouyu.cn/gtgvxwvcjy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xziqi.cn/gtfetqnfcp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hongshengwenyu.top/gtueirjutt.html

C#:   x.GetType().Name; x is int
来源：http://hz.shanyushiyangkeji.top/gtnezseuiw.html

[A05] 整数除法与取模
来源：http://hz.xinyue.icu/gtmwqfxmjy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.redwolf501.top/gtevqfgsuv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jqgfzy.top/gtxwougczi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shzxlz.cn/gtaxadtima.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtkfjoredp.html

Java: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtvhagusyn.html

Go:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtouzuaevf.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtdjgbzbbk.html

C#:   7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gtowxbsdae.html

[A06] 字符串转数字
来源：http://hz.hongshengwenyu.top/gtajfkiqkh.html

Py:   int("42"); float("3.14")
来源：http://hz.sweek.top/gtawvhhwvz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yuxming.cn/gttrtogicc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.vqdsnc.cn/gtmuicnqhm.html


<!-- 参考信息 -->