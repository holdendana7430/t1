代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.wangshuangyany.cn/gthlqrgcbj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtwmahsbjf.html

[U46] PHP：可空类型
来源：http://hz.jyoumei.cn/gtljgnzhla.html

?string $name = null
来源：http://hz.chenlongwang.top/gtjuwkgjqs.html

[U47] PHP：联合类型
来源：http://hz.yj202588.top/gttdmfmyeb.html

int|string $id
来源：http://hz.jinyuanbaomall.cn/gtmxwudggt.html

[U48] PHP：纯枚举
来源：http://hz.aizwys.cn/gtakngbomg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuetiantiany.cn/gtnarqxgix.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangtech.top/gtdedqzerq.html

public readonly string $name
来源：http://hz.ehwqpu.com/gtbykldiko.html

[U50] PHP：构造器属性提升
来源：http://hz.xuetiantiany.cn/gtbnygytwf.html

public function __construct(private int $id) {}
来源：http://hz.xuanzx.com/gtjcnaploo.html

[U51] PHP：数组解构
来源：http://hz.chenzaomai.com/gteivegukh.html

[$a, $b] = $arr;
来源：http://hz.quarkkingdee.top/gtkrkcarlb.html

[U52] PHP：箭头函数
来源：http://hz.svipenyu.cn/gtbdgxbkrc.html

$double = fn($x) => $x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtveaodhes.html

[U53] PHP：空合并运算符
来源：http://hz.cdnleiting.top/gtdvkezjiv.html

$v = $a ?? $b ?? "default";
来源：http://hz.jqgufenzy.top/gtyvqnmuus.html

[U54] PHP：空安全调用
来源：http://hz.jqgufenzy.top/gtipsrrpgn.html

$obj?->method()
来源：http://hz.nwbrower.top/gtaxbpisxk.html

[U55] PHP：match 表达式
来源：http://hz.0kj1m.cn/gtpfqeyegq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sxryk.cn/gtcndfwhmd.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtxdggopui.html

f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtmvzxpdzm.html

[U57] PHP：字符串插值
来源：http://hz.guannengcc.top/gtseyjcdzk.html

"值: {$a}"
来源：http://hz.fzhhl.top/gtnqwmzhqs.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gtzuikxslr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigufen.top/gtkitujnji.html

[U59] PHP：自定义排序
来源：http://hz.zhijiandao.cn/gtlpfktskp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtatjjtnak.html

[U60] PHP：JSON 编解码
来源：http://hz.52xcode.cn/gtqsfxrdsh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.wangshuangyany.cn/gtqncaytqw.html

[U61] PHP：正则
来源：http://hz.hammf.cn/gtoqutquua.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtizpqmzgi.html

[U62] PHP：日期对象
来源：http://hz.quarkkingdee.top/gtntusjykh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhengqikj.top/gtebydgoqc.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtpmeppgli.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pengpengdd.cyou/gtxkacoplt.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtwrtsroff.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhaomingkeji.xyz/gtbrhmzgfv.html

[U65] PHP：会话
来源：http://hz.ydjk.org.cn/gtywvtpuid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhijiandao.cn/gttxgnydew.html

[U66] PHP：设置 Cookie
来源：http://hz.yj202588.top/gtnvptbapm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.316326.xyz/gtoixofeis.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gttetxxxwj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gzhubu.top/gtxinfaqnn.html

[U68] PHP：PDO 连接
来源：http://hz.feifeiyinyue.top/gthkegoitm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yuxming.cn/gtqwxvhzqy.html

[U69] PHP：PDO 预处理
来源：http://hz.hysaishi.cn/gtmqqqgibu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.aibaodan.cn/gtuvispzgn.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258.top/gtwpjrxlbb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hysaishi.cn/gtgtclprps.html

[U71] PHP：抛出异常
来源：http://hz.9152youxi.cn/gtspehnmxq.html

throw new RuntimeException("失败", 500);
来源：http://hz.jianghu66.top/gtejbeslxc.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gtxapyyozx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.redwolf501.top/gtwbzngbdz.html

[U73] PHP：读取 ini 配置
来源：http://hz.52xcode.cn/gtuqyhwmas.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtasafbuiu.html

[U74] PHP：读取环境变量
来源：http://hz.jinqigufen.top/gtpjoerzsq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtkppufjrv.html

[U75] PHP：依赖注入
来源：http://hz.sufxvd.cn/gtjnypdauc.html

composer require psr/container
来源：http://hz.zhongyouzk.top/gtjjsuztcj.html

[U76] PHP：简单路由
来源：http://hz.tian-w.cn/gtujqwaqzm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.wangdashe.top/gtqteplhhf.html

[U77] PHP：模板渲染
来源：http://hz.wangdashe.top/gtavlkfclw.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtciiwddqk.html

[U78] PHP：单元测试
来源：http://hz.hysaishi.cn/gtuvxtpemn.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gthlciydjl.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtarsodueg.html

composer require --dev phpstan/phpstan
来源：http://hz.wangdashe.top/gtxdguvrnx.html

[U80] PHP：代码规范修复
来源：http://hz.hywenlv.cn/gtsbuzhleb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yonumen.top/gtyluvrvzt.html

[U81] JS：初始化项目
来源：http://hz.cqqwz.cn/gtyirydbxx.html

npm init -y;  npm i express
来源：http://hz.pycfn.com/gtfqwdarhz.html

[U82] JS：package.json 脚本
来源：http://hz.yvedp.cn/gtpzjsjsci.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhixingplan.top/gthnrdwdjb.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gtkzclpipn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtnkhvfgbg.html

[U84] JS：CommonJS 写法
来源：http://hz.redwolf501.top/gtldwribtd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gttanlggqr.html

[U85] JS：可选链
来源：http://hz.gaohongyu789.top/gtvbywhtok.html

a?.b?.c
来源：http://hz.tanke756.top/gtkonrghxq.html

[U86] JS：空值合并
来源：http://hz.daxiang520.top/gtmjgvfpvb.html

a ?? b
来源：http://hz.jyoumei.cn/gtgbicrurv.html

[U87] JS：解构默认值
来源：http://hz.daxiang520.top/gtomrkerdg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhaomingkeji.xyz/gtxzsnmrtf.html

[U88] JS：对象展开合并
来源：http://hz.jqgufenzy.top/gtfxowirvd.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtjkexfmwb.html

[U89] JS：数组去重
来源：http://hz.jinghuilouyu.cn/gtefreoppd.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gttzmqosgs.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangtech.top/gtbqjdwpka.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtvltuhzsb.html

[U91] JS：对象键值遍历
来源：http://hz.nanxuanxn.top/gtvakgurea.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhengqikj.top/gticuetoal.html

[U92] JS：深拷贝
来源：http://hz.yuanzhike.top/gtcmztjszz.html

structuredClone(obj)
来源：http://hz.tanke756.top/gtnekazyty.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtcxxynvsw.html

`共 ${n} 条`
来源：http://hz.yueranfly.top/gtojgvrwpi.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtnchaezhk.html

const double = x => x * 2;
来源：http://hz.guowangkeji.top/gtcpwxcnmm.html

[U95] JS：Promise 包装
来源：http://hz.redwolf501.top/gtftmppoaa.html

new Promise((resolve, reject) => {})
来源：http://hz.cashguo.top/gtzslmhuad.html

[U96] JS：async/await 与异常
来源：http://hz.xziqi.cn/gtwbqjznez.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtcrqbgbup.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gthmwutvet.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtbtdhvuki.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuanzx.com/gthoackamk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xingfuxueyuan.xyz/gttpegiokg.html

[U99] JS：事件监听
来源：http://hz.sufxvd.cn/gtbmhzvmjv.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtygmgdggc.html

[U100] JS：DOM 查询
来源：http://hz.wangdashe.top/gtrulingua.html

document.querySelector(".item")
来源：http://hz.52xcode.cn/gtipjrpksc.html

[U101] JS：classList 操作
来源：http://hz.yangfankeji.com/gtdjtziqfv.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gttdecbfpu.html

[U102] JS：本地存储
来源：http://hz.ppjwa.cn/gtcjaqozjm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.aizwys.cn/gtovqonnkf.html

[U103] JS：定时器
来源：http://hz.yongpay.top/gtpucjhlxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtfkhvzixt.html

[U104] JS：防抖
来源：http://hz.fzhhl.top/gtycsrryly.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtdgvxivwo.html

[U105] JS：节流
来源：http://hz.cucudq.cn/gtlsbjepgp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gttsfblhcf.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtzhkaupof.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtnflrxhiv.html

[U107] JS：数字千分位
来源：http://hz.chenjidiqi.icu/gtogoeoyac.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sxryk.cn/gtcgvfqoap.html

[U108] JS：随机整数
来源：http://hz.svipenyu.cn/gtajudcbbs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aizwys.cn/gtwvgoskkf.html

[U109] JS：数组分组
来源：http://hz.shangyingyoupin.top/gthlbtrlch.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtuybislsv.html

[U110] JS：数组分块
来源：http://hz.fengsongda.top/gtnwjnybeo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xziqi.cn/gtsfxkftiz.html

[U111] JS：对象转 Map
来源：http://hz.cqqwz.cn/gtrijrnovs.html

new Map(Object.entries(obj))
来源：http://hz.snrcjt.cn/gtvehstosg.html

[U112] JS：字符串补位
来源：http://hz.ivvv.top/gtbfklnxhx.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtcybhizel.html

[U113] JS：正则替换全部
来源：http://hz.bjfxy.top/gttpgpnpss.html

s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtrckdifzd.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtcjfoaxqb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtogskzcpj.html

[U115] JS：生成 UUID
来源：http://hz.smart0.xyz/gtexpcslwn.html

crypto.randomUUID()
来源：http://hz.mhx1999.top/gtcpfffwgp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.316326.xyz/gtfhdhwzbi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.c1oappe.top/gtcmcvifys.html

[U117] JS：单元测试
来源：http://hz.xuetiantiany.cn/gthtctnlji.html

npm i -D vitest;  npx vitest
来源：http://hz.0kj1m.cn/gtljxicjvj.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangkeji.top/gtfojfniag.html

npm i -D vite;  npx vite
来源：http://hz.havefunace.top/gtszgbwhuc.html

[U119] JS：生产构建
来源：http://hz.nwbrower.top/gtaugnvomp.html

npx vite build
来源：http://hz.chenzaomai.com/gtmniacvdr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnxiangtu.top/gtmxbbiaye.html

import.meta.env.VITE_API_URL
来源：http://hz.zhixingplan.top/gtojwpkntv.html

================================================================================
来源：http://hz.gotoacloud.top/gtghulcopx.html

统计汇总
来源：http://hz.zhaomingkeji.xyz/gtwmilaxtx.html

================================================================================
来源：http://hz.shuidangran.top/gtsijrmxyq.html

按语言统计（条）：
来源：http://hz.tianlin.xyz/gtrigufreu.html

Python ......... 252
来源：http://hz.daria6918.cn/gtzdetklju.html

PHP ............ 252
来源：http://hz.yj20258.top/gtwmnzsgti.html

JavaScript ..... 252
来源：http://hz.vqdsnc.cn/gtxltpmbpd.html

TypeScript ..... 212
来源：http://hz.shangyingyoupin.top/gtjdvnjebw.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtkcyuiwfc.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtfabztogl.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtymevyqcl.html

C# ............. 212
来源：http://hz.wangdashe.top/gtheikbfoj.html

C .............. 30
来源：http://hz.guowangkeji.top/gtjuelyebz.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtiwxkciel.html

SQL ............ 90
来源：http://hz.fengsongda.top/gtkwzkeexa.html

Bash ........... 80
来源：http://hz.mhx1999.top/gtvlwqubnz.html

Kotlin ......... 15
来源：http://hz.tianlin.xyz/gtbahvhsbm.html

Swift .......... 15
来源：http://hz.shanyushiyangkeji.top/gtrxxjccxr.html

Lua ............ 10
来源：http://hz.sxryk.cn/gtqvvnicgd.html

Perl ........... 10
来源：http://hz.shanyushiyangtech.top/gtssrnmbzb.html

Scala .......... 10
来源：http://hz.ydjk.org.cn/gtzkxevogv.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtwovlhjgr.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gtwyqoajut.html

按章节统计：
来源：http://hz.dianchejie.cn/gtuwtvezhf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gtxxeuinmu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtalxurcfg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtceeugamk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtovdbgvbc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnqzz.top/gtmxtyvlou.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gttjhuglaj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtdolsoykf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtofskuobs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtcroholaz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gtjejetdhj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtdfprjkga.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtvybhcnzm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtbsakifnr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtwsnayobr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.feifeiyinyue.top/gtdgngzpgd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtcrxxedwf.html

Q SQL 专题                              90
来源：http://hz.dianchejie.cn/gtbjzpjkpj.html

R Bash 专题                             80
来源：http://hz.yuanzhike.top/gtjesnxdny.html

S C / C++ 专题                          60
来源：http://hz.9152youxi.cn/gtgrvgrccw.html

T 其他语言补充                          60
来源：http://hz.yangfankeji.com/gtwcdrezct.html

U 高频实用片段                         120
来源：http://hz.hywenlv.cn/gtgmbbsarq.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtbfwktscv.html

合计                                  2106 条
来源：http://hz.ydzc1.top/gtntsyniio.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtsnrlxtzq.html

使用提醒
来源：http://hz.hfpthk.cn/gtsvhkepgi.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gthuiisydo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yongpay.top/gtimqfufrf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nwbrower.top/gtykjbofib.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtvjgbvhkf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yanxiufei.cn/gtprqdbahn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hnxiangtu.top/gtmezwwhpw.html

—— 文件结束 ——
来源：http://hz.zhixingplan.top/gtrotfhwnk.html

================================================================================
来源：http://hz.ybcxt.top/gtrsjdmthb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.snrcjt.cn/gtenbxgswa.html

Common Programming Examples Cheat Book
来源：http://hz.yj20258888.top/gtkkudqsdp.html

================================================================================
来源：http://hz.yuxming.cn/gtoetkaqrb.html

【收录内容】
来源：http://hz.cheryme.top/gtbwdrrfiz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinqigfzy.top/gtrrswyvbn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj20258.top/gtwvedlixv.html

SQL · Bash · C · C++
来源：http://hz.daxiang520.top/gturoalrmx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ivvv.top/gtfgpawjzg.html

【使用说明】
来源：http://hz.chenjidiqi.icu/gtgxwnzxjb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gtlocnxalt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.dianchejie.cn/gtofgaorgs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zdqjudy.top/gtcgnswqvq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gtnmvqgljy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangdashe.top/gtkibekedt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtjzujwevz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.svipenyu.cn/gtlgsnncas.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.quarkkingdee.top/gtynkadnqc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxuanxn.top/gtsulynmdb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.daria6918.cn/gtrfhanpfo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenlongwang.top/gtjmkpwidg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinyuanbaomall.cn/gtrvskilka.html

【文件统计】
来源：http://hz.xylfe.cn/gtnvvtlwqt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.wangshuangyany.cn/gtluszaawi.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtvikwfpox.html

目  录
来源：http://hz.dashuyun.cn/gtfrmjdapf.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtvtzlhhpn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gtuglwkwgk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtphackcfb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtjznzfkqa.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hfpthk.cn/gtrtnmfppo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.9152youxi.cn/gtdqldrtii.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnqzz.top/gtsmhrrwhf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtxdwexgwm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nwbrower.top/gtsypxkbbz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtpqcfpwkb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtmtqrflds.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtoaoinfor.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtspgcrdez.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtqqvuxwuk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtkqzlrdjs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ydzc1.top/gtuqpuoiaj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtplnzffvs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.tianlin.xyz/gtswycqwxn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zdqjudy.top/gtmwswkzgc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhaomingkeji.xyz/gtowcbdmyy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtwwurklxj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtordgnzqs.html

================================================================================
来源：http://hz.0kj1m.cn/gtblqhvrko.html

A. 基础语法与类型
来源：http://hz.yangfankeji.com/gtgwxueuxy.html

================================================================================
来源：http://hz.bjfxy.top/gttdhwzidk.html

[A01] Hello World
来源：http://hz.zhoulong.xyz/gtuhasuxqc.html

Py:   print("Hello, World!")
来源：http://hz.sweek.top/gtdgnckjha.html

PHP:  echo "Hello, World!";
来源：http://hz.yj20258.top/gtwufdpsya.html

JS:   console.log("Hello, World!");
来源：http://hz.sweek.top/gtzragliqn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ehwqpu.com/gtgazgbzmf.html

Java: System.out.println("Hello, World!");
来源：http://hz.gaohongyu789.top/gtgguwzjgm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.mhx1999.top/gtseutqwqd.html

Ruby: puts "Hello, World!"
来源：http://hz.c1oappe.top/gtitjrhefl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shzxlz.cn/gteahfsjlg.html

[A02] 变量声明与赋值
来源：http://hz.zhongyouzk.top/gtqwddknph.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.316326.xyz/gtijwiwbgq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.feifeiyinyue.top/gtmoullqwr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhiwuduotai.top/gtxgvkbnlm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jyoumei.cn/gtbchhifsq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daria6918.cn/gtpbbkahyw.html

Go:   name := "Alex"; age := 20
来源：http://hz.tianlin.xyz/gtbkvbtwuf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtmmsuatnl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.kuanghao11.cn/gtkiqiolrl.html

[A03] 常量定义
来源：http://hz.tanke756.top/gtkhfkcsqx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.vqdsnc.cn/gttdidkyue.html

PHP:  const PI = 3.14159;
来源：http://hz.hywenlv.cn/gtndalezmg.html

JS:   const PI = 3.14159;
来源：http://hz.birdmap.top/gtqalrhygq.html

TS:   const PI: number = 3.14159;
来源：http://hz.cdnleiting.top/gtgszdfaau.html

Java: static final double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtkfkolycb.html

Go:   const PI = 3.14159
来源：http://hz.hongshengwenyu.top/gtmgupzlat.html

Ruby: PI = 3.14159
来源：http://hz.cashguo.top/gtbgnnxtio.html

C#:   const double PI = 3.14159;
来源：http://hz.316326.xyz/gtkjldpyym.html

[A04] 判断变量类型
来源：http://hz.jinqigfzy.top/gtkjoimhho.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zdqjudy.top/gtkytfqkbl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yongpay.top/gthpdchwlr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangtech.top/gtxhnsncnh.html

TS:   typeof x; x instanceof Date
来源：http://hz.cdnleiting.top/gtfsxbjuzr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hfpthk.cn/gtocchvxvx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gogol.net.cn/gtziwtbhbu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shanyushiyangtech.top/gtrsjcwfnv.html

C#:   x.GetType().Name; x is int
来源：http://hz.gaohongyu789.top/gtaqldvdms.html

[A05] 整数除法与取模
来源：http://hz.yvedp.cn/gtvxmcgdmn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.dianchejie.cn/gtqyfxeokv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.c1oappe.top/gtqbmvhwek.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.c1oappe.top/gtvaruvltz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenjidiqi.icu/gtormwfxub.html


<!-- 参考信息 -->