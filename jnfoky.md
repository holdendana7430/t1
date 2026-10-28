代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gtkxqzszae.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tianlin.xyz/gtkqdorveg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.0kj1m.cn/gtuwjjzoir.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yongpay.top/gtddlxsvhs.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gtmrqsbrwg.html

namespace App\Http;
来源：http://hz.gogol.net.cn/gtcqtbnjfg.html

[U44] PHP：开启严格类型
来源：http://hz.vqdsnc.cn/gtuuswsvgx.html

declare(strict_types=1);
来源：http://hz.xziqi.cn/gtdcwhlwlz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gtmmodnwgc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtfmbrwdky.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtkmncpvur.html

?string $name = null
来源：http://hz.havefunace.top/gtjwqdrmlq.html

[U47] PHP：联合类型
来源：http://hz.haohaochexian.top/gtvddlcnoy.html

int|string $id
来源：http://hz.dashuyun.cn/gtkdkqtptl.html

[U48] PHP：纯枚举
来源：http://hz.nwbrower.top/gtfgeactqy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.andypj.xyz/gtmzbrxgcc.html

[U49] PHP：只读属性
来源：http://hz.zhijiandao.cn/gtdkdvhzsc.html

public readonly string $name
来源：http://hz.0kj1m.cn/gtlrhkuepm.html

[U50] PHP：构造器属性提升
来源：http://hz.gotoacloud.top/gtpqktzmol.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gteveosroc.html

[U51] PHP：数组解构
来源：http://hz.bjfxy.top/gtpzcorknr.html

[$a, $b] = $arr;
来源：http://hz.sysykeji.top/gtjwbmaaiz.html

[U52] PHP：箭头函数
来源：http://hz.yuxming.cn/gtifvnxwdf.html

$double = fn($x) => $x * 2;
来源：http://hz.tianlin.xyz/gtvysicsnu.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtpuzvuyni.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenjidiqi.icu/gtkxhykayl.html

[U54] PHP：空安全调用
来源：http://hz.fzhhl.top/gtesnvohfm.html

$obj?->method()
来源：http://hz.hammf.cn/gtfyzueosu.html

[U55] PHP：match 表达式
来源：http://hz.xingfuxueyuan.xyz/gtsobiygwi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuanzx.com/gtwnoroiuv.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtvawaitaq.html

f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtvxdapwat.html

[U57] PHP：字符串插值
来源：http://hz.birdmap.top/gtqsqbbjeo.html

"值: {$a}"
来源：http://hz.yvedp.cn/gttynwzrie.html

[U58] PHP：数组三件套
来源：http://hz.bjfxy.top/gtignxoizh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sufxvd.cn/gttlrjfgdy.html

[U59] PHP：自定义排序
来源：http://hz.xinyue.icu/gtvslrmkzf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtynsmwaez.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgufenzy.top/gtrpqgkjyw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gtszauefqc.html

[U61] PHP：正则
来源：http://hz.9152youxi.cn/gttqldrpcr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtnlkrifhk.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangkeji.top/gtptlsejhx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.0kj1m.cn/gttawwupiu.html

[U63] PHP：文件读写
来源：http://hz.jyoumei.cn/gtamjoswlm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuxming.cn/gtsgaaowci.html

[U64] PHP：目录遍历
来源：http://hz.cheryme.top/gtkvrdqyin.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hammf.cn/gtabvzkvcf.html

[U65] PHP：会话
来源：http://hz.cheryme.top/gtscgikudp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtknbqtymn.html

[U66] PHP：设置 Cookie
来源：http://hz.shanyushiyangtech.top/gtaqldixan.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gtcjuxyces.html

[U67] PHP：处理文件上传
来源：http://hz.jiagoushi.top/gtcntfelvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.snrcjt.cn/gtbjdedgnu.html

[U68] PHP：PDO 连接
来源：http://hz.yj202588.top/gtpcyiihfj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.316326.xyz/gtbxckegdu.html

[U69] PHP：PDO 预处理
来源：http://hz.aibaodan.cn/gtbanoartg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cashguo.top/gttmfnvctg.html

[U70] PHP：PDO 事务
来源：http://hz.yueranfly.top/gtvafavvau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.kuanghao11.cn/gtjctrhnxr.html

[U71] PHP：抛出异常
来源：http://hz.tianlin.xyz/gtvtnepqiq.html

throw new RuntimeException("失败", 500);
来源：http://hz.andypj.xyz/gtnvhdtgzf.html

[U72] PHP：写错误日志
来源：http://hz.tianlin.xyz/gtvevsemdo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxuanxn.top/gthvtwqfmr.html

[U73] PHP：读取 ini 配置
来源：http://hz.sysykeji.top/gttfjazygi.html

parse_ini_file("config.ini", true)
来源：http://hz.pengpengdd.cyou/gtqlvbueaa.html

[U74] PHP：读取环境变量
来源：http://hz.pycfn.com/gtdzddtyju.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xingfuxueyuan.xyz/gtcdpltdat.html

[U75] PHP：依赖注入
来源：http://hz.ivvv.top/gtjcqsrgcj.html

composer require psr/container
来源：http://hz.jyoumei.cn/gtwpbqfizi.html

[U76] PHP：简单路由
来源：http://hz.cashguo.top/gthqckqsyq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangkeji.top/gtcmpzorjq.html

[U77] PHP：模板渲染
来源：http://hz.redwolf501.top/gtiuxndwdw.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtcfisytjb.html

[U78] PHP：单元测试
来源：http://hz.hfpthk.cn/gtbueamgip.html

composer require --dev phpunit/phpunit
来源：http://hz.gotoacloud.top/gtpgeamnhs.html

[U79] PHP：静态分析
来源：http://hz.hammf.cn/gtfpxrosdh.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtdzyeapgs.html

[U80] PHP：代码规范修复
来源：http://hz.cucudq.cn/gtfpvlurdr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jyoumei.cn/gtmxnvfmkj.html

[U81] JS：初始化项目
来源：http://hz.yj20258888.top/gtrrjdwzum.html

npm init -y;  npm i express
来源：http://hz.chenjidiqi.icu/gtxftoqfys.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtfgrytrnf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cashguo.top/gtueodejrs.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinyuanbaomall.cn/gtibqyfoow.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tianlin.xyz/gtypheedoc.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtmddmniro.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtyvxcykkx.html

[U85] JS：可选链
来源：http://hz.haohaochexian.top/gteluemsfb.html

a?.b?.c
来源：http://hz.cheryme.top/gtgqeotbmp.html

[U86] JS：空值合并
来源：http://hz.ivvv.top/gtqnmxnubk.html

a ?? b
来源：http://hz.nanxuanxn.top/gtanhimoqo.html

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtjzmfcatw.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zdqjudy.top/gtjhssqema.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangtech.top/gtdysdprxd.html

{ ...a, ...b }
来源：http://hz.fzhhl.top/gtrbaftjet.html

[U89] JS：数组去重
来源：http://hz.shuidangran.top/gthlqndook.html

[...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtwpqyvwug.html

[U90] JS：数字数组排序
来源：http://hz.tian-w.cn/gtldombqej.html

[...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtppicwetg.html

[U91] JS：对象键值遍历
来源：http://hz.sxryk.cn/gtqfvxnefg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zdqjudy.top/gtupciicja.html

[U92] JS：深拷贝
来源：http://hz.guowangkeji.top/gtyxytixit.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gtvahnryzj.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtxepthhzh.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtxfnlqiqp.html

[U94] JS：箭头函数
来源：http://hz.chenzaomai.com/gtdnakqffl.html

const double = x => x * 2;
来源：http://hz.snrcjt.cn/gtkogtucqw.html

[U95] JS：Promise 包装
来源：http://hz.jlsjyb.cn/gtqqsuerzh.html

new Promise((resolve, reject) => {})
来源：http://hz.daria6918.cn/gtmjsqqlla.html

[U96] JS：async/await 与异常
来源：http://hz.chenzaomai.com/gtxpxgbwhg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtsotdznpm.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtwztbstsf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtqrafdwct.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenzaomai.com/gtswhcowmr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtywzqcdpx.html

[U99] JS：事件监听
来源：http://hz.yuxming.cn/gtwltwntnr.html

el.addEventListener("click", e => {})
来源：http://hz.cdnleiting.top/gthujijbqm.html

[U100] JS：DOM 查询
来源：http://hz.jinghuilouyu.cn/gtkankawog.html

document.querySelector(".item")
来源：http://hz.bjfxy.top/gtrutpdixt.html

[U101] JS：classList 操作
来源：http://hz.c1oappe.top/gtrwtynwnm.html

el.classList.toggle("active")
来源：http://hz.cashguo.top/gtyqqouxzi.html

[U102] JS：本地存储
来源：http://hz.jqgfzy.top/gtciipxpov.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sxryk.cn/gtabqggbuv.html

[U103] JS：定时器
来源：http://hz.mhx1999.top/gtsponozsm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtbqvoddmk.html

[U104] JS：防抖
来源：http://hz.dashuyun.cn/gtgkwvhspa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtxqpxynnv.html

[U105] JS：节流
来源：http://hz.hywenlv.cn/gtjxnaqile.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.haohaochexian.top/gtnqaszcxy.html

[U106] JS：日期格式化
来源：http://hz.dianchejie.cn/gtudgnocly.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhoulong.xyz/gtiogeplrq.html

[U107] JS：数字千分位
来源：http://hz.hfpthk.cn/gtsszxgbfu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ppjwa.cn/gtqoeepkyh.html

[U108] JS：随机整数
来源：http://hz.0kj1m.cn/gteqcswbuk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.316326.xyz/gterrzohap.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtdmqkihla.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtxbraounh.html

[U110] JS：数组分块
来源：http://hz.jinghuilouyu.cn/gtnhrehilk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhoulong.xyz/gtlcovxkts.html

[U111] JS：对象转 Map
来源：http://hz.yuxming.cn/gtjgtkejny.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtxziyoflf.html

[U112] JS：字符串补位
来源：http://hz.guannengcc.top/gtmwjjzrhf.html

"7".padStart(3, "0")
来源：http://hz.yonumen.top/gtvdqqayzc.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtvzhkjjte.html

s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtwsdbhivx.html

[U114] JS：JSON 深比较
来源：http://hz.xylfe.cn/gtluhnxuzi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtugbinojz.html

[U115] JS：生成 UUID
来源：http://hz.hywenlv.cn/gtunwhbmur.html

crypto.randomUUID()
来源：http://hz.ivvv.top/gtuyhudcnj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sysykeji.top/gtglupfseq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sufxvd.cn/gtnhsxwcxo.html

[U117] JS：单元测试
来源：http://hz.hywenlv.cn/gtvtadoytl.html

npm i -D vitest;  npx vitest
来源：http://hz.kuanghao11.cn/gtglbsnwdg.html

[U118] JS：开发服务器
来源：http://hz.tanke756.top/gtqlfvmiwc.html

npm i -D vite;  npx vite
来源：http://hz.fzhhl.top/gtswgsazls.html

[U119] JS：生产构建
来源：http://hz.cdnleiting.top/gtztajqiyy.html

npx vite build
来源：http://hz.xylfe.cn/gtxfwzpvpk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sufxvd.cn/gtmpsqlmso.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtmdmpbkhh.html

================================================================================
来源：http://hz.meibo888.top/gtpvhrvfnw.html

统计汇总
来源：http://hz.redwolf501.top/gtptsabtyu.html

================================================================================
来源：http://hz.tianlin.xyz/gtwietccnp.html

按语言统计（条）：
来源：http://hz.hysaishi.cn/gtjdvfjtxb.html

Python ......... 252
来源：http://hz.jlsjyb.cn/gtatrwoxka.html

PHP ............ 252
来源：http://hz.guannengcc.top/gtpgkogcue.html

JavaScript ..... 252
来源：http://hz.jinghuilouyu.cn/gtbajxtzmk.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtstqeshrf.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtfyjhzjpv.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtanlsydze.html

Ruby ........... 212
来源：http://hz.jianghu66.top/gtfjvfpagi.html

C# ............. 212
来源：http://hz.mhx1999.top/gtakjkqjpa.html

C .............. 30
来源：http://hz.pengpengdd.cyou/gtkbeynope.html

C++ ............ 30
来源：http://hz.cheryme.top/gtvahguyxn.html

SQL ............ 90
来源：http://hz.jinyuanbaomall.cn/gtaluvnvbr.html

Bash ........... 80
来源：http://hz.gaohongyu789.top/gtgukmdyew.html

Kotlin ......... 15
来源：http://hz.xuetiantiany.cn/gtbshjppwo.html

Swift .......... 15
来源：http://hz.0kj1m.cn/gtfheulvgn.html

Lua ............ 10
来源：http://hz.jinyuanbaomall.cn/gtblonypkb.html

Perl ........... 10
来源：http://hz.tian-w.cn/gtyxbujghv.html

Scala .......... 10
来源：http://hz.yangfankeji.com/gtiqbwzwep.html

------------------------------------
来源：http://hz.yangfankeji.com/gtdqwjdqgy.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gttjfisbqo.html

按章节统计：
来源：http://hz.ppjwa.cn/gtymggoovy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtfjkgfmta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtubfzbefj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhengqikj.top/gtmmhavssx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtoljdylej.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hfpthk.cn/gtedrrapbe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtkrxuhbdz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtwdaravxy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtnsuknpxb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtfftovtsy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtlrurybcg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtasyepney.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gttjnvjhmp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtbvrobalt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtxgcbnwwu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yuanzhike.top/gtpvockftk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtrvgdgevv.html

Q SQL 专题                              90
来源：http://hz.jlsjyb.cn/gtpvaqipmx.html

R Bash 专题                             80
来源：http://hz.zycfv.cn/gtajpvmogk.html

S C / C++ 专题                          60
来源：http://hz.zycfv.cn/gtbiucegaf.html

T 其他语言补充                          60
来源：http://hz.yongpay.top/gtunstnsfb.html

U 高频实用片段                         120
来源：http://hz.bjfxy.top/gtibxxmnjv.html

------------------------------------
来源：http://hz.yvedp.cn/gtyolipdwz.html

合计                                  2106 条
来源：http://hz.hammf.cn/gttzphyqum.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gthmeezxpv.html

使用提醒
来源：http://hz.ydjk.org.cn/gtmtfkhjcq.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtbboicoud.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258888.top/gtrnlneadr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gotoacloud.top/gtvquhyioo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.kuanghao11.cn/gthrgrxkuo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydjk.org.cn/gtsyyjopnz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.birdmap.top/gtwjigbtlz.html

—— 文件结束 ——
来源：http://hz.ehwqpu.com/gtidiqdzgf.html

================================================================================
来源：http://hz.jiagoushi.top/gtllhizncw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ybcxt.top/gtghwammao.html

Common Programming Examples Cheat Book
来源：http://hz.aizwys.cn/gtnnlztqlr.html

================================================================================
来源：http://hz.jinqigufen.top/gtsvtdyina.html

【收录内容】
来源：http://hz.cdnleiting.top/gtbrjaqhzx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnqzz.top/gtjkpntodn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ehwqpu.com/gtrmyryujf.html

SQL · Bash · C · C++
来源：http://hz.hongshengwenyu.top/gtwjhyfsmv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydjk.org.cn/gtqzendwzj.html

【使用说明】
来源：http://hz.jinqigfzy.top/gthlkditga.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.0kj1m.cn/gtlknngdqh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.quarkkingdee.top/gtokdshqyg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinghuilouyu.cn/gtfmvvdpkp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tianlin.xyz/gtijbqabuh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ivvv.top/gtujnbqhxr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.haohaochexian.top/gtkipgzqil.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zdqjudy.top/gtsahmqoxb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hysaishi.cn/gtrtlmslcq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhengqikj.top/gtzpdscijb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgfzy.top/gtnkntafih.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.9152youxi.cn/gtnsffgmai.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zycfv.cn/gtizwzeqna.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtroxhrdrp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sysykeji.top/gtzpmooiey.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtwhzeiuml.html

目  录
来源：http://hz.jlsjyb.cn/gthvxqyqpf.html

--------------------------------------------------------------------------------
来源：http://hz.xuetiantiany.cn/gtrameneam.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtbsmrzqeg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtfyfsppco.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtxloatxjz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gtbnhzpqwm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.feifeiyinyue.top/gtvnyjebzu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jyoumei.cn/gtjuvidvle.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.bjfxy.top/gtebyphmtf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.fzhhl.top/gtdnvjqycr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gttaexcgmx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sysykeji.top/gtwcbklyct.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtlkpywvef.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtccrdejvo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtqayigzgu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtrzjsftxv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxuanxn.top/gtgxbtjakf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtmurnpsxo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.snrcjt.cn/gtzzngvacf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jlsjyb.cn/gtzbrmccza.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yuanzhike.top/gtyiddeebz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gtdorbhjmj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtuhjtleat.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrcqxbocl.html

A. 基础语法与类型
来源：http://hz.birdmap.top/gtidtilnct.html

================================================================================
来源：http://hz.haohaochexian.top/gthesrcnrc.html

[A01] Hello World
来源：http://hz.nanxuanxn.top/gtlxumshou.html

Py:   print("Hello, World!")
来源：http://hz.ehwqpu.com/gtxoytgutm.html

PHP:  echo "Hello, World!";
来源：http://hz.nwbrower.top/gtzykagxze.html

JS:   console.log("Hello, World!");
来源：http://hz.yj202588.top/gtidaocczj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinghuilouyu.cn/gtvabppfsu.html

Java: System.out.println("Hello, World!");
来源：http://hz.kuanghao11.cn/gtlcxvkfme.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.tanke756.top/gtqgwqwhnh.html

Ruby: puts "Hello, World!"
来源：http://hz.quarkkingdee.top/gtvlkwvdtj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhoulong.xyz/gtljlhimbv.html

[A02] 变量声明与赋值
来源：http://hz.fengsongda.top/gtqujvdyjy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yanxiufei.cn/gttcpefiry.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nanxuanxn.top/gtwssbuapy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sysykeji.top/gtswkyhwuo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.chenzaomai.com/gtisqdztfi.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtlpeublxd.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenjidiqi.icu/gtxlfmjrlg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daxiang520.top/gtcijbypfo.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtrfodisjc.html

[A03] 常量定义
来源：http://hz.jqgfzy.top/gtcgicidrb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aizwys.cn/gtvfvaulpb.html

PHP:  const PI = 3.14159;
来源：http://hz.52xcode.cn/gtdvrxcgsn.html

JS:   const PI = 3.14159;
来源：http://hz.smart0.xyz/gtzavvjtln.html

TS:   const PI: number = 3.14159;
来源：http://hz.jyoumei.cn/gtxvyxcuxq.html

Java: static final double PI = 3.14159;
来源：http://hz.52xcode.cn/gtuohunwnk.html

Go:   const PI = 3.14159
来源：http://hz.haohaochexian.top/gtxoquzmvy.html

Ruby: PI = 3.14159
来源：http://hz.birdmap.top/gtbbtyinki.html

C#:   const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gthumpashf.html

[A04] 判断变量类型
来源：http://hz.sysykeji.top/gtjohfbimn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.daria6918.cn/gthssobqbc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sysykeji.top/gtjpouocoy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangshuangyany.cn/gtavuxhvhr.html

TS:   typeof x; x instanceof Date
来源：http://hz.yvedp.cn/gtokgwwcib.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.vqdsnc.cn/gtgqasvpxn.html


<!-- 参考信息 -->