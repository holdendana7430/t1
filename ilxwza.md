代发 wailian999

[U49] PHP：只读属性
来源：http://hz.zhoulong.xyz/gtxrlqhvpa.html

public readonly string $name
来源：http://hz.xylfe.cn/gtltdxkgrd.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gtfeszsjty.html

public function __construct(private int $id) {}
来源：http://hz.andypj.xyz/gtqfgvvitu.html

[U51] PHP：数组解构
来源：http://hz.sxryk.cn/gtvhcdydql.html

[$a, $b] = $arr;
来源：http://hz.quarkkingdee.top/gtmfkekwov.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtiyqlooib.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigfzy.top/gtkcoliqyw.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gtztledrlq.html

$v = $a ?? $b ?? "default";
来源：http://hz.tanke756.top/gtxzgijmeu.html

[U54] PHP：空安全调用
来源：http://hz.zhaomingkeji.xyz/gthicjuhpv.html

$obj?->method()
来源：http://hz.52xcode.cn/gtlwwhupjd.html

[U55] PHP：match 表达式
来源：http://hz.nanxinkj.top/gtdlgvxwtw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.quarkkingdee.top/gtdqzrwgqt.html

[U56] PHP：命名参数
来源：http://hz.cashguo.top/gtecthazis.html

f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtvengqlkl.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gtxrenbypw.html

"值: {$a}"
来源：http://hz.cdnleiting.top/gtvqhnaadu.html

[U58] PHP：数组三件套
来源：http://hz.pycfn.com/gtpmnfnqxp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.dianchejie.cn/gtmiwambdo.html

[U59] PHP：自定义排序
来源：http://hz.dashuyun.cn/gtqqwoadnh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtwsshorxj.html

[U60] PHP：JSON 编解码
来源：http://hz.yvedp.cn/gtcofodbnl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.dianchejie.cn/gtuphhrmhh.html

[U61] PHP：正则
来源：http://hz.yangfankeji.com/gtwwqjslwq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtljxqqxuu.html

[U62] PHP：日期对象
来源：http://hz.yuanzhike.top/gtzfcdgkoj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtjbwitptz.html

[U63] PHP：文件读写
来源：http://hz.ydzc1.top/gtetrizdln.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gtigfytvgy.html

[U64] PHP：目录遍历
来源：http://hz.xingfuxueyuan.xyz/gtyegnpfwt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgufenzy.top/gtywfdqgwg.html

[U65] PHP：会话
来源：http://hz.hnqzz.top/gtlsuqgguv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnxiangtu.top/gtoyusunjt.html

[U66] PHP：设置 Cookie
来源：http://hz.cqqwz.cn/gtoeuhsyru.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sweek.top/gtvmxcjpmt.html

[U67] PHP：处理文件上传
来源：http://hz.snrcjt.cn/gttghfdowv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.52xcode.cn/gtrjtgjgot.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtjhrecmeb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yueranfly.top/gtfkixyvnp.html

[U69] PHP：PDO 预处理
来源：http://hz.mhx1999.top/gtifbhesel.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sweek.top/gtqojkgofl.html

[U70] PHP：PDO 事务
来源：http://hz.daria6918.cn/gtiywoqxmx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yueranfly.top/gttdtnymhx.html

[U71] PHP：抛出异常
来源：http://hz.hammf.cn/gtbjhqauno.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangtech.top/gtvqmdcxdb.html

[U72] PHP：写错误日志
来源：http://hz.chenjidiqi.icu/gtxdacmqgd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.52xcode.cn/gtxhdmnlir.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gtmwhnpqjl.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtwbwrdelp.html

[U74] PHP：读取环境变量
来源：http://hz.guannengcc.top/gtmtclfvln.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xingfuxueyuan.xyz/gtvbcoobgf.html

[U75] PHP：依赖注入
来源：http://hz.hammf.cn/gtoezywtyc.html

composer require psr/container
来源：http://hz.meibo888.top/gtkqfvluvq.html

[U76] PHP：简单路由
来源：http://hz.haohaochexian.top/gtazxcbegr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jlsjyb.cn/gtrsezpsnw.html

[U77] PHP：模板渲染
来源：http://hz.sufxvd.cn/gtzzjxtzns.html

composer require twig/twig
来源：http://hz.xziqi.cn/gtbydhvqfh.html

[U78] PHP：单元测试
来源：http://hz.yonumen.top/gtblfqonri.html

composer require --dev phpunit/phpunit
来源：http://hz.xingfuxueyuan.xyz/gthdklrrnp.html

[U79] PHP：静态分析
来源：http://hz.shuidangran.top/gtfikzaord.html

composer require --dev phpstan/phpstan
来源：http://hz.chenzaomai.com/gtpjomgdkr.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gtvkeleicr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jyoumei.cn/gtyqnccyhk.html

[U81] JS：初始化项目
来源：http://hz.zhaomingkeji.xyz/gtsxuhdtzb.html

npm init -y;  npm i express
来源：http://hz.vqdsnc.cn/gtbathjkmv.html

[U82] JS：package.json 脚本
来源：http://hz.zycfv.cn/gtdxbrgegk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jianghu66.top/gtgtaswhdl.html

[U83] JS：ES Module 导入导出
来源：http://hz.smart0.xyz/gtzvgkptqd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.daxiang520.top/gtxpekgaxs.html

[U84] JS：CommonJS 写法
来源：http://hz.316326.xyz/gticvemnvn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gtqqjahmdo.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtqmhacabw.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtxwdwgltg.html

[U86] JS：空值合并
来源：http://hz.cdnleiting.top/gttrkijwso.html

a ?? b
来源：http://hz.xziqi.cn/gtjmnrvzrq.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtqlcdawlb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.52xcode.cn/gtmptrqnez.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtkwhfydue.html

{ ...a, ...b }
来源：http://hz.zhoulong.xyz/gtyuntyevl.html

[U89] JS：数组去重
来源：http://hz.52xcode.cn/gtqbivokqs.html

[...new Set(arr)]
来源：http://hz.fzhhl.top/gtdugircow.html

[U90] JS：数字数组排序
来源：http://hz.jqgufenzy.top/gtnajpliaf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtltbbroxg.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangkeji.top/gttyyzutil.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shuidangran.top/gtoobyfkqt.html

[U92] JS：深拷贝
来源：http://hz.zhengqikj.top/gtzybsscif.html

structuredClone(obj)
来源：http://hz.cdnleiting.top/gthslonhpj.html

[U93] JS：模板字符串
来源：http://hz.xingfuxueyuan.xyz/gtaloeebuh.html

`共 ${n} 条`
来源：http://hz.yuanzhike.top/gtbzeqvbrd.html

[U94] JS：箭头函数
来源：http://hz.jinyuanbaomall.cn/gtjffbgxtn.html

const double = x => x * 2;
来源：http://hz.yvedp.cn/gtxawyvjxw.html

[U95] JS：Promise 包装
来源：http://hz.xuanzx.com/gtycbgkmrm.html

new Promise((resolve, reject) => {})
来源：http://hz.shangyingyoupin.top/gtypkghxvf.html

[U96] JS：async/await 与异常
来源：http://hz.jyoumei.cn/gtvebyugor.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gteeishkio.html

[U97] JS：并发请求
来源：http://hz.bjfxy.top/gtpavusnvq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtvpxmxpul.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhijiandao.cn/gtrhvtbpeu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtfdtbksne.html

[U99] JS：事件监听
来源：http://hz.hammf.cn/gtogsayhdu.html

el.addEventListener("click", e => {})
来源：http://hz.sweek.top/gtjdxcabyw.html

[U100] JS：DOM 查询
来源：http://hz.daria6918.cn/gttsqyqujq.html

document.querySelector(".item")
来源：http://hz.mhx1999.top/gtprrmxyca.html

[U101] JS：classList 操作
来源：http://hz.cashguo.top/gtcbzniten.html

el.classList.toggle("active")
来源：http://hz.ivvv.top/gtncvapuvg.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gtiyhwsjql.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gzhubu.top/gtwzkarwdv.html

[U103] JS：定时器
来源：http://hz.bjfxy.top/gtqjqgzfrn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hongshengwenyu.top/gttowcgocb.html

[U104] JS：防抖
来源：http://hz.cucudq.cn/gtejaubfje.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gttlphvpnu.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtlzrbcbvj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtlxgrncat.html

[U106] JS：日期格式化
来源：http://hz.meibo888.top/gtsdcbpgsc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.52xcode.cn/gtvodghorj.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gttoualbng.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gturjcdgkw.html

[U108] JS：随机整数
来源：http://hz.yongpay.top/gtrsleuznn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtdfvmyrvw.html

[U109] JS：数组分组
来源：http://hz.zhoulong.xyz/gtnzzywzde.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gtmpbtwrgo.html

[U110] JS：数组分块
来源：http://hz.cucudq.cn/gtujyfbxtl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangdashe.top/gtpnjwinpz.html

[U111] JS：对象转 Map
来源：http://hz.jinqigfzy.top/gtgiqczoys.html

new Map(Object.entries(obj))
来源：http://hz.jinqigfzy.top/gtlnshkzbt.html

[U112] JS：字符串补位
来源：http://hz.jlsjyb.cn/gtjxlxfzgg.html

"7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtyxjixvud.html

[U113] JS：正则替换全部
来源：http://hz.ywan-chungtsiang.top/gtltgizjkk.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtcitytgkv.html

[U114] JS：JSON 深比较
来源：http://hz.sysykeji.top/gtgjfupfoi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtxpcscgli.html

[U115] JS：生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtrefclorx.html

crypto.randomUUID()
来源：http://hz.birdmap.top/gthecmiwqr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shuidangran.top/gtdiuutbqs.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuetiantiany.cn/gtiuwslfnq.html

[U117] JS：单元测试
来源：http://hz.tianlin.xyz/gtxnaskqmm.html

npm i -D vitest;  npx vitest
来源：http://hz.hongshengwenyu.top/gtdfbplagj.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtshlvpcox.html

npm i -D vite;  npx vite
来源：http://hz.svipenyu.cn/gtxhxijupz.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtbsyemzok.html

npx vite build
来源：http://hz.fzhhl.top/gtjjcljnvk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jiagoushi.top/gthwmqpuxu.html

import.meta.env.VITE_API_URL
来源：http://hz.jianghu66.top/gtgntafuuq.html

================================================================================
来源：http://hz.shzxlz.cn/gtimnnrmop.html

统计汇总
来源：http://hz.zhiwuduotai.top/gtwbokmcet.html

================================================================================
来源：http://hz.yueranfly.top/gthdmabblw.html

按语言统计（条）：
来源：http://hz.xylfe.cn/gtdpjhzuja.html

Python ......... 252
来源：http://hz.jinghuilouyu.cn/gtzimbbpoc.html

PHP ............ 252
来源：http://hz.haohaochexian.top/gtlgaebubt.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gtnhahjzwu.html

TypeScript ..... 212
来源：http://hz.jianghu66.top/gtfcjcnqss.html

Java ........... 212
来源：http://hz.zhijiandao.cn/gtmdsjpyxl.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtzqspnkys.html

Ruby ........... 212
来源：http://hz.zhengqikj.top/gtonxsbwgb.html

C# ............. 212
来源：http://hz.birdmap.top/gtxnrafyxz.html

C .............. 30
来源：http://hz.xuetiantiany.cn/gtvbtqynrw.html

C++ ............ 30
来源：http://hz.kuanghao11.cn/gtnhcaxlfr.html

SQL ............ 90
来源：http://hz.shanyushiyangkeji.top/gtzadlyhuv.html

Bash ........... 80
来源：http://hz.jianghu66.top/gtdsdakubi.html

Kotlin ......... 15
来源：http://hz.chenzaomai.com/gtnolkaujc.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gtwtuymvrd.html

Lua ............ 10
来源：http://hz.jinghuilouyu.cn/gtezyezmcs.html

Perl ........... 10
来源：http://hz.ybcxt.top/gtsbrrpoja.html

Scala .......... 10
来源：http://hz.shanyushiyangtech.top/gtirnwefig.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtaatiwjnd.html

合计 ........... 2106 条
来源：http://hz.vqdsnc.cn/gtpwezbobm.html

按章节统计：
来源：http://hz.gaohongyu789.top/gtrnwfpjxv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtwbusegkw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtpyjgvuav.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtetvngevd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtzeyfcdma.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydzc1.top/gtnwwepqsc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtkhehpepz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtejdytctm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pycfn.com/gtnqkksmkf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtlzxnbpdq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jianghu66.top/gtoholnulg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtiogppfsj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtdkkrgdel.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gthrhbnwlc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtvoxtksvm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gtpynwjxpq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtgufzcnft.html

Q SQL 专题                              90
来源：http://hz.hnqzz.top/gttektpqrx.html

R Bash 专题                             80
来源：http://hz.yvedp.cn/gtluaqldhn.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtmvikomwu.html

T 其他语言补充                          60
来源：http://hz.haohaochexian.top/gtcviaczdq.html

U 高频实用片段                         120
来源：http://hz.wangdashe.top/gtyvnzfjli.html

------------------------------------
来源：http://hz.zhixingplan.top/gtrvvksuwh.html

合计                                  2106 条
来源：http://hz.ydzc1.top/gtucjivabo.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtcuvcsqkb.html

使用提醒
来源：http://hz.cashguo.top/gtkcrxlguf.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtwvzkohxd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shzxlz.cn/gtrftfyzqz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cucudq.cn/gtmyuwjwbq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258.top/gtyicrzycq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cheryme.top/gtpcaluofr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtcdgkwulj.html

—— 文件结束 ——
来源：http://hz.shuidangran.top/gtyvolucam.html

================================================================================
来源：http://hz.cashguo.top/gtiqizfvif.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cucudq.cn/gtbgwfcbtw.html

Common Programming Examples Cheat Book
来源：http://hz.ehwqpu.com/gtffhjcpvv.html

================================================================================
来源：http://hz.dashuyun.cn/gtterlpahu.html

【收录内容】
来源：http://hz.smart0.xyz/gtrpethmxl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhiwuduotai.top/gtikknpcjg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sysykeji.top/gtekrqohlj.html

SQL · Bash · C · C++
来源：http://hz.nanxinkj.top/gtuwdguqns.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangshuangyany.cn/gtnpxmkied.html

【使用说明】
来源：http://hz.jqgfzy.top/gtcauyvnla.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangtech.top/gtacfohuub.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.mhx1999.top/gtuxagmicp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ehwqpu.com/gtmmzvtmar.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.svipenyu.cn/gtszpcdtxg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtqegliacu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuanzhike.top/gtuvgxzzxd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinyuanbaomall.cn/gtwttwfcqq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fengsongda.top/gtcjfbhckq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.52xcode.cn/gtwonkeert.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shanyushiyangkeji.top/gtemsdtnit.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gtobriqlao.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yvedp.cn/gtcriksprk.html

【文件统计】
来源：http://hz.yongpay.top/gtuqadejlg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuetiantiany.cn/gtxmalfccc.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtkmhejvdl.html

目  录
来源：http://hz.yueranfly.top/gtqcflheio.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtxfegvtlx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.gzhubu.top/gtsurbyxhz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtilrahnmq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtpwzwrwof.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daria6918.cn/gtuqxehhjk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tanke756.top/gtmwcfzjfv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gtupgtoael.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtuodlbksi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sweek.top/gtrdcoynxh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtsdflpccq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cqqwz.cn/gtsadmeeyb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtjwqjdkmp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtxbrubrqr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gthghlghzk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cheryme.top/gtsqzomuqt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sxryk.cn/gtfxxpaesy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtnanbseqd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hammf.cn/gtdmvvfyuc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.wangshuangyany.cn/gtndfdpywm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.feifeiyinyue.top/gtuojodocr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtznjtpwqc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gtiqosjngz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgongfcjb.html

A. 基础语法与类型
来源：http://hz.yueranfly.top/gthnyngmip.html

================================================================================
来源：http://hz.316326.xyz/gtyudysgof.html

[A01] Hello World
来源：http://hz.guannengcc.top/gtgnlejpar.html

Py:   print("Hello, World!")
来源：http://hz.zycfv.cn/gtobnqmung.html

PHP:  echo "Hello, World!";
来源：http://hz.hnqzz.top/gtoefsxgqc.html

JS:   console.log("Hello, World!");
来源：http://hz.sysykeji.top/gtbfeaqrod.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cdnleiting.top/gtorswaxym.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtkgjgzftm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.9152youxi.cn/gtyrjbsioi.html

Ruby: puts "Hello, World!"
来源：http://hz.smart0.xyz/gtvrndpmqc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yueranfly.top/gtoyfeikqs.html

[A02] 变量声明与赋值
来源：http://hz.sweek.top/gtpokihnpf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangtech.top/gtasgcpkpd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.meibo888.top/gtufmnecji.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.svipenyu.cn/gtwvlgmcxd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yongpay.top/gtsyafgwzm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jiagoushi.top/gtulebtuen.html

Go:   name := "Alex"; age := 20
来源：http://hz.nwbrower.top/gtfdgppqju.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jiagoushi.top/gtdejidvzc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cheryme.top/gtsprhaglg.html

[A03] 常量定义
来源：http://hz.cucudq.cn/gtumnauwrt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yangfankeji.com/gtcmjyffwv.html

PHP:  const PI = 3.14159;
来源：http://hz.xinyue.icu/gtsihjtkeh.html

JS:   const PI = 3.14159;
来源：http://hz.ivvv.top/gtimvjgxsu.html

TS:   const PI: number = 3.14159;
来源：http://hz.52xcode.cn/gthtrzhlsw.html

Java: static final double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtjjuxabig.html

Go:   const PI = 3.14159
来源：http://hz.yonumen.top/gtdfyomkvr.html

Ruby: PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtpomufzhc.html

C#:   const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtmjktmwmf.html

[A04] 判断变量类型
来源：http://hz.meibo888.top/gtdcgiadke.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.daxiang520.top/gtdhbgtpwq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.52xcode.cn/gtgbqawusx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nwbrower.top/gtejtwmheo.html

TS:   typeof x; x instanceof Date
来源：http://hz.yangfankeji.com/gtfxsbgdpl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xinyue.icu/gtglhbzwmg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xinyue.icu/gtdsezbolq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinyuanbaomall.cn/gtgplahpsk.html

C#:   x.GetType().Name; x is int
来源：http://hz.316326.xyz/gtmyjrepmp.html

[A05] 整数除法与取模
来源：http://hz.jiagoushi.top/gtcriktzpt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhiwuduotai.top/gtgykqmndk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtpcoqxoic.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guowangkeji.top/gtftcpxvbf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuxming.cn/gtnssgjqaa.html

Java: 7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtmlqphifr.html

Go:   7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtfwjuzwwj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtswfvpcyl.html

C#:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtmpknuyyb.html

[A06] 字符串转数字
来源：http://hz.yanxiufei.cn/gtomrbdedd.html

Py:   int("42"); float("3.14")
来源：http://hz.yanxiufei.cn/gtyvduboru.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cucudq.cn/gtpaebuamd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xingfuxueyuan.xyz/gtgkldpvhv.html


<!-- 参考信息 -->