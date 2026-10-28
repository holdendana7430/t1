代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.daxiang520.top/gtoavdrhxg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtmlnyaczw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gttgtcxgsm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gaohongyu789.top/gtdfxxjfjw.html

[U43] PHP：声明命名空间
来源：http://hz.ivvv.top/gtkzxwkwnq.html

namespace App\Http;
来源：http://hz.guowangkeji.top/gtqqfjwvlh.html

[U44] PHP：开启严格类型
来源：http://hz.cashguo.top/gtcsaquusc.html

declare(strict_types=1);
来源：http://hz.sxryk.cn/gtndguwqsd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.iojbl.cn/gtqdsjnwvt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtmqoeeyrz.html

[U46] PHP：可空类型
来源：http://hz.cqqwz.cn/gtnrcwfphx.html

?string $name = null
来源：http://hz.havefunace.top/gtmuvpcntp.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtvrizapum.html

int|string $id
来源：http://hz.redwolf501.top/gtyoupnmwk.html

[U48] PHP：纯枚举
来源：http://hz.52xcode.cn/gtxcywbtbg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangshuangyany.cn/gtbonysyvr.html

[U49] PHP：只读属性
来源：http://hz.zhoulong.xyz/gtvoasgxet.html

public readonly string $name
来源：http://hz.xinyue.icu/gtjbojqwhw.html

[U50] PHP：构造器属性提升
来源：http://hz.vqdsnc.cn/gteegjqtgf.html

public function __construct(private int $id) {}
来源：http://hz.tianlin.xyz/gtypmfheds.html

[U51] PHP：数组解构
来源：http://hz.zhoulong.xyz/gtoyihtxlu.html

[$a, $b] = $arr;
来源：http://hz.zhixingplan.top/gtfixdnscm.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtcmpgjgsr.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtfipcnflz.html

[U53] PHP：空合并运算符
来源：http://hz.tian-w.cn/gtsghskgvm.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtwkhgglzr.html

[U54] PHP：空安全调用
来源：http://hz.quarkkingdee.top/gtlxkscsxn.html

$obj?->method()
来源：http://hz.ybcxt.top/gtnpurhkyy.html

[U55] PHP：match 表达式
来源：http://hz.yangfankeji.com/gtgluhigqo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258.top/gtugfxtvjr.html

[U56] PHP：命名参数
来源：http://hz.snrcjt.cn/gtxnvytfbx.html

f(a: 1, b: 2)
来源：http://hz.dianchejie.cn/gtoslcraba.html

[U57] PHP：字符串插值
来源：http://hz.xuanzx.com/gttjondfpa.html

"值: {$a}"
来源：http://hz.daria6918.cn/gtofyhbodr.html

[U58] PHP：数组三件套
来源：http://hz.bjfxy.top/gtazcmzafr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnqzz.top/gtkmjxygvc.html

[U59] PHP：自定义排序
来源：http://hz.ywan-chungtsiang.top/gtxhmogkyb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtbttlbauq.html

[U60] PHP：JSON 编解码
来源：http://hz.jinghuilouyu.cn/gtzwftfrxf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.haohaochexian.top/gtvrssnvmz.html

[U61] PHP：正则
来源：http://hz.nanxinkj.top/gtsbefeyda.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtpptdajyb.html

[U62] PHP：日期对象
来源：http://hz.aibaodan.cn/gtjdrvtxll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.meibo888.top/gtmczdlcpi.html

[U63] PHP：文件读写
来源：http://hz.wangdashe.top/gtwijqzlza.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ybcxt.top/gtrevhjqsz.html

[U64] PHP：目录遍历
来源：http://hz.havefunace.top/gtxtjcpmvs.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtgtrdyynf.html

[U65] PHP：会话
来源：http://hz.birdmap.top/gthbkiicqa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.birdmap.top/gtldopybes.html

[U66] PHP：设置 Cookie
来源：http://hz.mhx1999.top/gteurtftuz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gtwruygeic.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtabquiwkn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtrnzqpoak.html

[U68] PHP：PDO 连接
来源：http://hz.xuanzx.com/gtfqsrhvjk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.smart0.xyz/gtomlaaekt.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtufunabzy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtudbdyymn.html

[U70] PHP：PDO 事务
来源：http://hz.shuidangran.top/gtzjehsqqi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhaomingkeji.xyz/gtexbvmpwz.html

[U71] PHP：抛出异常
来源：http://hz.cqqwz.cn/gtzsbukxxo.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangkeji.top/gtmrttndrx.html

[U72] PHP：写错误日志
来源：http://hz.yueranfly.top/gtuffrsjpy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jianghu66.top/gtlrhervmz.html

[U73] PHP：读取 ini 配置
来源：http://hz.iojbl.cn/gtyraqximr.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtjldfpbhh.html

[U74] PHP：读取环境变量
来源：http://hz.zhixingplan.top/gtyupywkmg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gotoacloud.top/gtwgtztbal.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gthpkfjmgg.html

composer require psr/container
来源：http://hz.quarkkingdee.top/gteqlprdxz.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtlqqltmja.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hfpthk.cn/gtcnyiftdc.html

[U77] PHP：模板渲染
来源：http://hz.hfpthk.cn/gtwwusibji.html

composer require twig/twig
来源：http://hz.mhx1999.top/gtbipjgody.html

[U78] PHP：单元测试
来源：http://hz.iojbl.cn/gtlmjfdont.html

composer require --dev phpunit/phpunit
来源：http://hz.jinghuilouyu.cn/gtmmgcpdzz.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtdodbysbl.html

composer require --dev phpstan/phpstan
来源：http://hz.wangshuangyany.cn/gtfdtditrc.html

[U80] PHP：代码规范修复
来源：http://hz.316326.xyz/gtnyqkuytf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigufen.top/gtdljdytfq.html

[U81] JS：初始化项目
来源：http://hz.nanxuanxn.top/gtxcholoog.html

npm init -y;  npm i express
来源：http://hz.sxryk.cn/gtjkrexoii.html

[U82] JS：package.json 脚本
来源：http://hz.wangdashe.top/gttrcsomep.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnxiangtu.top/gtgpcudhzw.html

[U83] JS：ES Module 导入导出
来源：http://hz.nwbrower.top/gtocpphrpr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258888.top/gtbaknvejb.html

[U84] JS：CommonJS 写法
来源：http://hz.jyoumei.cn/gtvzvzaczh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenlongwang.top/gthbwczzon.html

[U85] JS：可选链
来源：http://hz.zhaomingkeji.xyz/gttczsenev.html

a?.b?.c
来源：http://hz.jqgfzy.top/gtnvtpfnzk.html

[U86] JS：空值合并
来源：http://hz.fengsongda.top/gtbuhrhnpw.html

a ?? b
来源：http://hz.fengsongda.top/gtrmhccfdc.html

[U87] JS：解构默认值
来源：http://hz.sysykeji.top/gtudbtjooh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj20258888.top/gtzqifbydi.html

[U88] JS：对象展开合并
来源：http://hz.cqqwz.cn/gtpnobhamu.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gtgljfgfdo.html

[U89] JS：数组去重
来源：http://hz.nwbrower.top/gtbsmwvziv.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gthhwgsyaq.html

[U90] JS：数字数组排序
来源：http://hz.hongshengwenyu.top/gtjsbnffno.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtvevvrbnk.html

[U91] JS：对象键值遍历
来源：http://hz.nanxinkj.top/gtgpgaguhv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gtiwjjbhtr.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtdkraazfw.html

structuredClone(obj)
来源：http://hz.yonumen.top/gtrpqtzpjr.html

[U93] JS：模板字符串
来源：http://hz.zycfv.cn/gtueeynigi.html

`共 ${n} 条`
来源：http://hz.sufxvd.cn/gtzhvmxlhf.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtmnesaisb.html

const double = x => x * 2;
来源：http://hz.yj20258888.top/gtjkwhlfbm.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gtftucaaca.html

new Promise((resolve, reject) => {})
来源：http://hz.c1oappe.top/gtieacflgm.html

[U96] JS：async/await 与异常
来源：http://hz.daxiang520.top/gtebrflyxc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtyslqcfgk.html

[U97] JS：并发请求
来源：http://hz.ydzc1.top/gtpygivfop.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtdwqgvrre.html

[U98] JS：fetch 带 JSON
来源：http://hz.52xcode.cn/gtdlhgsxcr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gtckdtowhm.html

[U99] JS：事件监听
来源：http://hz.nwbrower.top/gthtfinjhw.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtdrmbkhrh.html

[U100] JS：DOM 查询
来源：http://hz.daxiang520.top/gtlgfrluzc.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtbqxxemfe.html

[U101] JS：classList 操作
来源：http://hz.jiagoushi.top/gtgjobfghq.html

el.classList.toggle("active")
来源：http://hz.snrcjt.cn/gtapzccylq.html

[U102] JS：本地存储
来源：http://hz.gzhubu.top/gtohueorml.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xziqi.cn/gttynhlnsp.html

[U103] JS：定时器
来源：http://hz.tanke756.top/gtrayufmiq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.havefunace.top/gtrgjxkkyr.html

[U104] JS：防抖
来源：http://hz.zycfv.cn/gtbrcfwsqi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtdbwptjfm.html

[U105] JS：节流
来源：http://hz.jianghu66.top/gthhxrifne.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj202588.top/gtlxoxbteg.html

[U106] JS：日期格式化
来源：http://hz.zhengqikj.top/gtzhsvwumm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuxming.cn/gtjqyxavrr.html

[U107] JS：数字千分位
来源：http://hz.jinqigufen.top/gtjkpmojfd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigfzy.top/gtuyhlfqqu.html

[U108] JS：随机整数
来源：http://hz.cdnleiting.top/gtbbeuixzt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sysykeji.top/gtgbqrmnev.html

[U109] JS：数组分组
来源：http://hz.yj20258.top/gtqiqbdjvl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtavmdsmtn.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtstzqvuje.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtmbveyadt.html

[U111] JS：对象转 Map
来源：http://hz.sxryk.cn/gtxqicpvle.html

new Map(Object.entries(obj))
来源：http://hz.gaohongyu789.top/gtywwcyfvj.html

[U112] JS：字符串补位
来源：http://hz.jiagoushi.top/gttbwwgupf.html

"7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtymvlqbkw.html

[U113] JS：正则替换全部
来源：http://hz.jinqigfzy.top/gtwrmngjzy.html

s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtcqbfaimr.html

[U114] JS：JSON 深比较
来源：http://hz.yangfankeji.com/gtjcifieue.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtehxneviz.html

[U115] JS：生成 UUID
来源：http://hz.meibo888.top/gtsurgjjbu.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtlcfkaijs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shanyushiyangtech.top/gtixffpsxf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.redwolf501.top/gtpqjqfstk.html

[U117] JS：单元测试
来源：http://hz.hfpthk.cn/gtyyuwjjaa.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigfzy.top/gtymeagexp.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtgfjbmauy.html

npm i -D vite;  npx vite
来源：http://hz.haohaochexian.top/gtmbtvwgxt.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangkeji.top/gtvgkvzatj.html

npx vite build
来源：http://hz.daria6918.cn/gtudcxvksh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnqzz.top/gtciukxomw.html

import.meta.env.VITE_API_URL
来源：http://hz.ydzc1.top/gtqpvjaahh.html

================================================================================
来源：http://hz.zdqjudy.top/gtojudrfdg.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtwiqkjovc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxgynhqgh.html

按语言统计（条）：
来源：http://hz.xziqi.cn/gtixmpfohd.html

Python ......... 252
来源：http://hz.shangyingyoupin.top/gtpjcijjbw.html

PHP ............ 252
来源：http://hz.9152youxi.cn/gtljqeypcq.html

JavaScript ..... 252
来源：http://hz.quarkkingdee.top/gtgdrqaexb.html

TypeScript ..... 212
来源：http://hz.shuidangran.top/gtwcqpdcxt.html

Java ........... 212
来源：http://hz.daria6918.cn/gtzfijnzao.html

Go ............. 212
来源：http://hz.yj20258.top/gtclmlhfkk.html

Ruby ........... 212
来源：http://hz.dianchejie.cn/gtdbmfhhnu.html

C# ............. 212
来源：http://hz.jiagoushi.top/gthgtljxvy.html

C .............. 30
来源：http://hz.svipenyu.cn/gtwgqnnjwa.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtvsoanxnw.html

SQL ............ 90
来源：http://hz.xuanzx.com/gtbnzqfwxu.html

Bash ........... 80
来源：http://hz.meibo888.top/gtxqjxelzt.html

Kotlin ......... 15
来源：http://hz.shanyushiyangtech.top/gtndmjdmdh.html

Swift .......... 15
来源：http://hz.gaohongyu789.top/gtoksqxmzh.html

Lua ............ 10
来源：http://hz.zhoulong.xyz/gtfmiksvdm.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gthhbvpsen.html

Scala .......... 10
来源：http://hz.sweek.top/gtuarbednz.html

------------------------------------
来源：http://hz.xziqi.cn/gtaxhwcdiq.html

合计 ........... 2106 条
来源：http://hz.hnqzz.top/gtmwiuffdg.html

按章节统计：
来源：http://hz.chenjidiqi.icu/gtivtwsjav.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gttaannjnm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtamwmcugr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.kuanghao11.cn/gtflebrbps.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtcvixxcib.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinqigufen.top/gtgmbijgyl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtuyqiqubu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtdwavzugj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yongpay.top/gtxxtszghb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtteawdeum.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.feifeiyinyue.top/gtdlmkxqqa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtsllcpnrz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtkusgxqqf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtvtykrjgy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gthdnrmarz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtvtzoeoxa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtncspxsvr.html

Q SQL 专题                              90
来源：http://hz.yvedp.cn/gtfsksavxe.html

R Bash 专题                             80
来源：http://hz.sxryk.cn/gtrlkwjwnp.html

S C / C++ 专题                          60
来源：http://hz.jlsjyb.cn/gtncmtcddd.html

T 其他语言补充                          60
来源：http://hz.yonumen.top/gthbhekinl.html

U 高频实用片段                         120
来源：http://hz.jyoumei.cn/gtriszkuno.html

------------------------------------
来源：http://hz.0kj1m.cn/gtdeywhmie.html

合计                                  2106 条
来源：http://hz.snrcjt.cn/gtwypuaawc.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtvgdqegof.html

使用提醒
来源：http://hz.yanxiufei.cn/gtwlryizcc.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtninxzfot.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xuanzx.com/gtddlrqdpy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gotoacloud.top/gtnlntlicb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nwbrower.top/gtqwalzmnc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxinkj.top/gtmhfiawct.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhixingplan.top/gtrzlthxzm.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtqmmyywrg.html

================================================================================
来源：http://hz.cdnleiting.top/gtyopcbzej.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sysykeji.top/gtjjlekeah.html

Common Programming Examples Cheat Book
来源：http://hz.ywan-chungtsiang.top/gtcclefqgk.html

================================================================================
来源：http://hz.havefunace.top/gtdinmyord.html

【收录内容】
来源：http://hz.pycfn.com/gtgkhzrmct.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daxiang520.top/gtcmsrufxe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinghuilouyu.cn/gtzdkfmyii.html

SQL · Bash · C · C++
来源：http://hz.havefunace.top/gtswybapat.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hfpthk.cn/gtgnefpcll.html

【使用说明】
来源：http://hz.9152youxi.cn/gteydmadfe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhijiandao.cn/gtwnkofpxd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ywan-chungtsiang.top/gtfflstpya.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.9152youxi.cn/gtmvpbkoqf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yueranfly.top/gtooighswd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sxryk.cn/gtylaegrbd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.0kj1m.cn/gtxgfaddsd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hysaishi.cn/gttznssdan.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.snrcjt.cn/gtqqqdwxmc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xuanzx.com/gtfbifeuwm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xylfe.cn/gtsfydqlbu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.haohaochexian.top/gtgcyssyrb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenjidiqi.icu/gtuhrlannt.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gtxrnfenlu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gaohongyu789.top/gtktshdaun.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtneudvuny.html

目  录
来源：http://hz.hysaishi.cn/gtmwnkajtp.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtpaocluah.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtxvzbxada.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangdashe.top/gtdwfuljxh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtohylmxvz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtodwhtpmc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xuetiantiany.cn/gtihgawglh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtcfaarthn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtvxysvthh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinyuanbaomall.cn/gtamornehp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtrzysmvtg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtcgbpmnhu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtgvqfkccv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtmnlzeebz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtcmummcwi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gttiqurbgf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhixingplan.top/gthwdighbo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtoiqmlizf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gaohongyu789.top/gtynvzwfgm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shzxlz.cn/gtgrdpxglt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxuanxn.top/gtqbjakmou.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gthtefuzgm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj202588.top/gtkbpmpplp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtleuohjrk.html

A. 基础语法与类型
来源：http://hz.xziqi.cn/gtyxwblmfd.html

================================================================================
来源：http://hz.xinyue.icu/gtwivltmdr.html

[A01] Hello World
来源：http://hz.cqqwz.cn/gtxwkstcgz.html

Py:   print("Hello, World!")
来源：http://hz.haohaochexian.top/gtdjnvpcrb.html

PHP:  echo "Hello, World!";
来源：http://hz.ydjk.org.cn/gtcplusnvs.html

JS:   console.log("Hello, World!");
来源：http://hz.ivvv.top/gtbmwytfpa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gaohongyu789.top/gtpygcnunk.html

Java: System.out.println("Hello, World!");
来源：http://hz.gaohongyu789.top/gthbmkayhm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangkeji.top/gtrpudfcqw.html

Ruby: puts "Hello, World!"
来源：http://hz.ydjk.org.cn/gtpgwfffzb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yj20258.top/gtwdfwpelg.html

[A02] 变量声明与赋值
来源：http://hz.shuidangran.top/gtbpwlcgmd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.316326.xyz/gteroiazmy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aizwys.cn/gtudhkkulx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.dashuyun.cn/gtljlvgaiv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guowangkeji.top/gtsxrjyexm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gtmhuweoao.html

Go:   name := "Alex"; age := 20
来源：http://hz.9152youxi.cn/gtabswylkb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sufxvd.cn/gtfgwrodxm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.wangshuangyany.cn/gtgedkmuzk.html

[A03] 常量定义
来源：http://hz.zhoulong.xyz/gtigfyxwfp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhixingplan.top/gtmmgacdis.html

PHP:  const PI = 3.14159;
来源：http://hz.svipenyu.cn/gtlgzlpbga.html

JS:   const PI = 3.14159;
来源：http://hz.xylfe.cn/gtvkkszsnu.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtszpwuath.html

Java: static final double PI = 3.14159;
来源：http://hz.smart0.xyz/gtkcpsxelg.html

Go:   const PI = 3.14159
来源：http://hz.havefunace.top/gtqprrzaig.html

Ruby: PI = 3.14159
来源：http://hz.yanxiufei.cn/gtcnrupdea.html

C#:   const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtswxvtqpb.html

[A04] 判断变量类型
来源：http://hz.sysykeji.top/gtcemtyqhw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gzhubu.top/gtcwkwfdhr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.snrcjt.cn/gtfxmgsqfz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtmeauaplt.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj202588.top/gttxaauklj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cucudq.cn/gtnqdsvtti.html


<!-- 参考信息 -->