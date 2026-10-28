代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.jyoumei.cn/gtuiyotiwe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtxmdyrigk.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gthpsdxydp.html

?string $name = null
来源：http://hz.redwolf501.top/gtahihcyzl.html

[U47] PHP：联合类型
来源：http://hz.hongshengwenyu.top/gtckgpbwqq.html

int|string $id
来源：http://hz.nwbrower.top/gtmtdxmers.html

[U48] PHP：纯枚举
来源：http://hz.gaohongyu789.top/gtdwgarfwj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zdqjudy.top/gtqyllbkyo.html

[U49] PHP：只读属性
来源：http://hz.cheryme.top/gtblvildvj.html

public readonly string $name
来源：http://hz.yj20258.top/gtljuxrgsl.html

[U50] PHP：构造器属性提升
来源：http://hz.hammf.cn/gttcweqtzg.html

public function __construct(private int $id) {}
来源：http://hz.sysykeji.top/gtfeiyrqeg.html

[U51] PHP：数组解构
来源：http://hz.ywan-chungtsiang.top/gtwkykeszk.html

[$a, $b] = $arr;
来源：http://hz.yuxming.cn/gtmscdjefc.html

[U52] PHP：箭头函数
来源：http://hz.fengsongda.top/gtyfmivdan.html

$double = fn($x) => $x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtomykrjad.html

[U53] PHP：空合并运算符
来源：http://hz.ywan-chungtsiang.top/gtrvsihesn.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydzc1.top/gtlsjhntem.html

[U54] PHP：空安全调用
来源：http://hz.ppjwa.cn/gtbtpwxtmn.html

$obj?->method()
来源：http://hz.feifeiyinyue.top/gtritutvqi.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtymxdtibk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxuanxn.top/gtjdkcdiqo.html

[U56] PHP：命名参数
来源：http://hz.haohaochexian.top/gtcumljslg.html

f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtutwezwbv.html

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtddentdsl.html

"值: {$a}"
来源：http://hz.shzxlz.cn/gtsueprcfz.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gtnufnqxqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xinyue.icu/gtyjfiunoa.html

[U59] PHP：自定义排序
来源：http://hz.jlsjyb.cn/gtpmqubvwi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gtcqxszsfj.html

[U60] PHP：JSON 编解码
来源：http://hz.iojbl.cn/gtqvzvldoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yonumen.top/gtoythpqtx.html

[U61] PHP：正则
来源：http://hz.yueranfly.top/gtocdamhcq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gtwasijnaa.html

[U62] PHP：日期对象
来源：http://hz.jianghu66.top/gthhhfyyub.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtyjqhkfug.html

[U63] PHP：文件读写
来源：http://hz.fengsongda.top/gtynuzmine.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.nanxinkj.top/gtfldasedq.html

[U64] PHP：目录遍历
来源：http://hz.cdnleiting.top/gtwdqrxpqx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cashguo.top/gtjidfhzva.html

[U65] PHP：会话
来源：http://hz.daxiang520.top/gtrzfsryly.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtjzvjfxwn.html

[U66] PHP：设置 Cookie
来源：http://hz.wangdashe.top/gtdqyichbs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gtyudywtks.html

[U67] PHP：处理文件上传
来源：http://hz.jlsjyb.cn/gtrrhnbyhw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gtxljbjevk.html

[U68] PHP：PDO 连接
来源：http://hz.yj202588.top/gtxjpnhtav.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gotoacloud.top/gtfrkonqcj.html

[U69] PHP：PDO 预处理
来源：http://hz.daxiang520.top/gtfbsovtyx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dianchejie.cn/gtnejxrjjh.html

[U70] PHP：PDO 事务
来源：http://hz.jianghu66.top/gttyqmmfjf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenzaomai.com/gtcsfykvoe.html

[U71] PHP：抛出异常
来源：http://hz.jinqigfzy.top/gtrvvuuzyq.html

throw new RuntimeException("失败", 500);
来源：http://hz.iojbl.cn/gtggwgfbwj.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtdvnhyrlt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxuanxn.top/gtavlbsdrm.html

[U73] PHP：读取 ini 配置
来源：http://hz.vqdsnc.cn/gtmxeavusq.html

parse_ini_file("config.ini", true)
来源：http://hz.hongshengwenyu.top/gtmydeqbcy.html

[U74] PHP：读取环境变量
来源：http://hz.shzxlz.cn/gtvpmmwhof.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cucudq.cn/gtxhzozxkv.html

[U75] PHP：依赖注入
来源：http://hz.tian-w.cn/gtknucavpu.html

composer require psr/container
来源：http://hz.fzhhl.top/gtxtzuhozt.html

[U76] PHP：简单路由
来源：http://hz.xuetiantiany.cn/gtklyukibj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xinyue.icu/gtpkhxuvru.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtqgyyjhzg.html

composer require twig/twig
来源：http://hz.andypj.xyz/gtsodqfzqp.html

[U78] PHP：单元测试
来源：http://hz.nwbrower.top/gtplrwnpby.html

composer require --dev phpunit/phpunit
来源：http://hz.chenlongwang.top/gthiejtcou.html

[U79] PHP：静态分析
来源：http://hz.shzxlz.cn/gtjravdfil.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtymeavcbd.html

[U80] PHP：代码规范修复
来源：http://hz.shangyingyoupin.top/gthpkmtknt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gtabjeowfp.html

[U81] JS：初始化项目
来源：http://hz.yuanzhike.top/gthvmbjzbd.html

npm init -y;  npm i express
来源：http://hz.svipenyu.cn/gtbizgcgqt.html

[U82] JS：package.json 脚本
来源：http://hz.yangfankeji.com/gthsseltkf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gogol.net.cn/gtublihrsp.html

[U83] JS：ES Module 导入导出
来源：http://hz.yvedp.cn/gtybkwfdqx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.mhx1999.top/gtivbraajd.html

[U84] JS：CommonJS 写法
来源：http://hz.zdqjudy.top/gtddaicitg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jyoumei.cn/gtfuxoxiqw.html

[U85] JS：可选链
来源：http://hz.xingfuxueyuan.xyz/gtnmadhpfq.html

a?.b?.c
来源：http://hz.yonumen.top/gtbbsgdpvi.html

[U86] JS：空值合并
来源：http://hz.vqdsnc.cn/gtlfcnmtqp.html

a ?? b
来源：http://hz.shanyushiyangkeji.top/gtxecntbxc.html

[U87] JS：解构默认值
来源：http://hz.ydzc1.top/gttvpnejlo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nwbrower.top/gtzqwsnjto.html

[U88] JS：对象展开合并
来源：http://hz.316326.xyz/gttatfbjxw.html

{ ...a, ...b }
来源：http://hz.pycfn.com/gtgnjnqvpk.html

[U89] JS：数组去重
来源：http://hz.ydjk.org.cn/gtqagkcrrg.html

[...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtupcvaiag.html

[U90] JS：数字数组排序
来源：http://hz.ehwqpu.com/gthrwlhirb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtotljwfqr.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gtpsghglfe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shangyingyoupin.top/gtkbcvuytd.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtzfjjzdza.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtqccqhonh.html

[U93] JS：模板字符串
来源：http://hz.guowangkeji.top/gtoqviqxgj.html

`共 ${n} 条`
来源：http://hz.pengpengdd.cyou/gtqqpxhdgm.html

[U94] JS：箭头函数
来源：http://hz.hongshengwenyu.top/gtimwczcfh.html

const double = x => x * 2;
来源：http://hz.ydjk.org.cn/gtgnklrmyx.html

[U95] JS：Promise 包装
来源：http://hz.52xcode.cn/gtrnwouisj.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtsaiappaf.html

[U96] JS：async/await 与异常
来源：http://hz.xylfe.cn/gtetgwtfqn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtoinougjd.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtuvlouodo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtwqudammo.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinqigfzy.top/gtpeszruqc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gtxjqzmipr.html

[U99] JS：事件监听
来源：http://hz.cqqwz.cn/gtuwadaxdx.html

el.addEventListener("click", e => {})
来源：http://hz.cucudq.cn/gtsfigqkim.html

[U100] JS：DOM 查询
来源：http://hz.jianghu66.top/gtdvhhqusk.html

document.querySelector(".item")
来源：http://hz.xuetiantiany.cn/gtypiipvcv.html

[U101] JS：classList 操作
来源：http://hz.jinyuanbaomall.cn/gtvgpskgee.html

el.classList.toggle("active")
来源：http://hz.guowangkeji.top/gttdkixxjh.html

[U102] JS：本地存储
来源：http://hz.quarkkingdee.top/gthhgpgdcm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydjk.org.cn/gtmrbbjaup.html

[U103] JS：定时器
来源：http://hz.jinqigfzy.top/gtcdvyxrlo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenlongwang.top/gtksjwrytm.html

[U104] JS：防抖
来源：http://hz.dianchejie.cn/gthxwxgrzo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtsdrpzpch.html

[U105] JS：节流
来源：http://hz.hnqzz.top/gtfczupvic.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jianghu66.top/gtlrxfdvgv.html

[U106] JS：日期格式化
来源：http://hz.chenzaomai.com/gtawwdxuwe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shangyingyoupin.top/gtlolgdcut.html

[U107] JS：数字千分位
来源：http://hz.ivvv.top/gtindetcyj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cqqwz.cn/gtpqqletom.html

[U108] JS：随机整数
来源：http://hz.guannengcc.top/gtoqhstkvg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hysaishi.cn/gtafffmorz.html

[U109] JS：数组分组
来源：http://hz.cashguo.top/gtavtnvqqu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxinkj.top/gttvdmhmsp.html

[U110] JS：数组分块
来源：http://hz.cheryme.top/gtbkeptgcy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yonumen.top/gtrbwdtgos.html

[U111] JS：对象转 Map
来源：http://hz.pengpengdd.cyou/gtbzcclnrm.html

new Map(Object.entries(obj))
来源：http://hz.gaohongyu789.top/gtdiitldud.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtdcqaxhkp.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtlwjysqkk.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gtachhveco.html

s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtmsdgctft.html

[U114] JS：JSON 深比较
来源：http://hz.yongpay.top/gtmsnjoccl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtitsnrtsn.html

[U115] JS：生成 UUID
来源：http://hz.yuxming.cn/gtmdzmtqgw.html

crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtipovqoeu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yanxiufei.cn/gtfvhhkqzv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtujjwoleo.html

[U117] JS：单元测试
来源：http://hz.ehwqpu.com/gtrrkospnw.html

npm i -D vitest;  npx vitest
来源：http://hz.tian-w.cn/gtelqyfyaa.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtcviyehtg.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gtixlcwqpa.html

[U119] JS：生产构建
来源：http://hz.jyoumei.cn/gtidngqhji.html

npx vite build
来源：http://hz.wangdashe.top/gtitecmunx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gaohongyu789.top/gtdvkmohtl.html

import.meta.env.VITE_API_URL
来源：http://hz.sxryk.cn/gtutsdmzyq.html

================================================================================
来源：http://hz.9152youxi.cn/gtlhxghubg.html

统计汇总
来源：http://hz.yangfankeji.com/gtkksitktq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlemtpjpv.html

按语言统计（条）：
来源：http://hz.jinyuanbaomall.cn/gtwythwhad.html

Python ......... 252
来源：http://hz.gzhubu.top/gtxfqifdew.html

PHP ............ 252
来源：http://hz.yuanzhike.top/gtamihytha.html

JavaScript ..... 252
来源：http://hz.jinghuilouyu.cn/gtwbcmzogf.html

TypeScript ..... 212
来源：http://hz.jqgufenzy.top/gtkvyleerw.html

Java ........... 212
来源：http://hz.shuidangran.top/gtagohovsk.html

Go ............. 212
来源：http://hz.hnxiangtu.top/gtnaesahpa.html

Ruby ........... 212
来源：http://hz.xuanzx.com/gtubcahkwp.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtieuawwmz.html

C .............. 30
来源：http://hz.daxiang520.top/gtfyfdbbxt.html

C++ ............ 30
来源：http://hz.cheryme.top/gtzfjukkoo.html

SQL ............ 90
来源：http://hz.daxiang520.top/gtuyjytkar.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtobenzgey.html

Kotlin ......... 15
来源：http://hz.ehwqpu.com/gtuovqoyiw.html

Swift .......... 15
来源：http://hz.jinqigfzy.top/gteumeaejy.html

Lua ............ 10
来源：http://hz.cashguo.top/gtknbcaoed.html

Perl ........... 10
来源：http://hz.fzhhl.top/gtyratztaz.html

Scala .......... 10
来源：http://hz.birdmap.top/gtttuzblzz.html

------------------------------------
来源：http://hz.sufxvd.cn/gtypcbufxc.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gtlmbhqpxu.html

按章节统计：
来源：http://hz.jinqigufen.top/gtockcbhan.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gtntfladda.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtytkguust.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtajhtuino.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gtrzndibrx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuanzhike.top/gtclbpejxw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtsbugcned.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtfytjjsre.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtvxpqxtqo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtxbsjkceb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtmnxahpye.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtmgjizcka.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtykwlzwuf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtbsximgkt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenlongwang.top/gtjeilnvca.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gtrcweqemj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtuukzrwwn.html

Q SQL 专题                              90
来源：http://hz.shzxlz.cn/gtjfrumjna.html

R Bash 专题                             80
来源：http://hz.haohaochexian.top/gtcksygdoc.html

S C / C++ 专题                          60
来源：http://hz.aibaodan.cn/gtqxdfifls.html

T 其他语言补充                          60
来源：http://hz.zhixingplan.top/gtivtivrcv.html

U 高频实用片段                         120
来源：http://hz.yuanzhike.top/gtmljjnojg.html

------------------------------------
来源：http://hz.yuxming.cn/gtjqtnxwhy.html

合计                                  2106 条
来源：http://hz.sufxvd.cn/gtlrlzagnp.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtohutcvit.html

使用提醒
来源：http://hz.jinqigufen.top/gtzjtvdwad.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtxichcebt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jiagoushi.top/gtiwotxcij.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenlongwang.top/gtjxqjwdre.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shanyushiyangkeji.top/gtwlhvuebj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.pengpengdd.cyou/gtgzjfpmed.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangshuangyany.cn/gtrptkvkmh.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gtscftxftz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkaoopujp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.haohaochexian.top/gtpgexssss.html

Common Programming Examples Cheat Book
来源：http://hz.zycfv.cn/gtjgagorgg.html

================================================================================
来源：http://hz.daria6918.cn/gtnhjrhwbc.html

【收录内容】
来源：http://hz.ppjwa.cn/gtqilcobgh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtxddzvkjy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gtgufbqajz.html

SQL · Bash · C · C++
来源：http://hz.mhx1999.top/gtevkbnawq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigufen.top/gttazrwnvc.html

【使用说明】
来源：http://hz.0kj1m.cn/gtqaclnmiw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cashguo.top/gtzlyfxfzv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shanyushiyangkeji.top/gteklpgrdv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xingfuxueyuan.xyz/gtnclaqeko.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cashguo.top/gtkwhkacqu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.feifeiyinyue.top/gtpdslxcft.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gotoacloud.top/gtmeavlbwv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hysaishi.cn/gttrmzkwsx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yuanzhike.top/gtiewnkjcg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnqzz.top/gtehnlaztg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtcaaxbirt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.meibo888.top/gtnszfcayv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenzaomai.com/gtzagvawpy.html

【文件统计】
来源：http://hz.cashguo.top/gtcxrxgaxr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shzxlz.cn/gtgrmvmvvp.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtauzvgjpb.html

目  录
来源：http://hz.iojbl.cn/gtpspittll.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gthnodnzlo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.haohaochexian.top/gtepxtepwf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gtccxsozfn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtfvqhaido.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yuxming.cn/gtwlyvybqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinqigfzy.top/gtabnxfwdr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.quarkkingdee.top/gtmxcsvxhg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtybclhbvi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.andypj.xyz/gthlleaavf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtjppmneaj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.0kj1m.cn/gtbwfoodlr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtboybamnz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtrfhnqwqw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtegoyzmrt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yueranfly.top/gtmhdcgcfh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daria6918.cn/gtwtpzsels.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtwrnhpkbo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtrivhasvh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxuanxn.top/gtatjeikav.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yuxming.cn/gtjlakznyt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtfwuxnavq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.dianchejie.cn/gtiyuydnsm.html

================================================================================
来源：http://hz.tianlin.xyz/gtibszkdhr.html

A. 基础语法与类型
来源：http://hz.ehwqpu.com/gtpjojhgvd.html

================================================================================
来源：http://hz.ivvv.top/gtczhwlkcp.html

[A01] Hello World
来源：http://hz.cucudq.cn/gtawyjovya.html

Py:   print("Hello, World!")
来源：http://hz.daxiang520.top/gtxaexwzaz.html

PHP:  echo "Hello, World!";
来源：http://hz.tianlin.xyz/gtxevfbctj.html

JS:   console.log("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtflvbiciw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.aizwys.cn/gtfvaxyxgg.html

Java: System.out.println("Hello, World!");
来源：http://hz.redwolf501.top/gtdjrmjekc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangdashe.top/gtkwasxqcf.html

Ruby: puts "Hello, World!"
来源：http://hz.cqqwz.cn/gtadxrshtx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.9152youxi.cn/gtflctsphg.html

[A02] 变量声明与赋值
来源：http://hz.c1oappe.top/gtmyxcvxiw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gtnfzkswbs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenlongwang.top/gtqhetfklm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.feifeiyinyue.top/gtsvizcsvs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ivvv.top/gtuqxcpcaf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtohpebdzg.html

Go:   name := "Alex"; age := 20
来源：http://hz.ehwqpu.com/gtwafsjxgs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.wangdashe.top/gtcpzropbl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtmbmbmbhn.html

[A03] 常量定义
来源：http://hz.hywenlv.cn/gtmrvtrjwp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhaomingkeji.xyz/gtpvoaldhs.html

PHP:  const PI = 3.14159;
来源：http://hz.bjfxy.top/gteloyghla.html

JS:   const PI = 3.14159;
来源：http://hz.fengsongda.top/gtetscwdry.html

TS:   const PI: number = 3.14159;
来源：http://hz.daria6918.cn/gtimzlarmb.html

Java: static final double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtndqnpvcy.html

Go:   const PI = 3.14159
来源：http://hz.yueranfly.top/gtstmabgsk.html

Ruby: PI = 3.14159
来源：http://hz.mhx1999.top/gtwdrjoaem.html

C#:   const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtfhmyaljx.html

[A04] 判断变量类型
来源：http://hz.9152youxi.cn/gtbnadcbow.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jianghu66.top/gtbtlvrchq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fengsongda.top/gtjvwwcqto.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ivvv.top/gtkptavglj.html

TS:   typeof x; x instanceof Date
来源：http://hz.cashguo.top/gtgicadkma.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yanxiufei.cn/gtlbhievod.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.quarkkingdee.top/gtusxvffws.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jyoumei.cn/gtzolneucv.html

C#:   x.GetType().Name; x is int
来源：http://hz.cheryme.top/gtzvlwttjk.html

[A05] 整数除法与取模
来源：http://hz.ppjwa.cn/gtzefgwfyy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj202588.top/gtchuapgwh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hysaishi.cn/gtthznguwf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hammf.cn/gtgwydjpbm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnxiangtu.top/gtvyrcqugg.html


<!-- 参考信息 -->