代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangkeji.top/gtfjxhyatv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenjidiqi.icu/gtgjgyfcky.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.andypj.xyz/gtncyiakns.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangtech.top/gtnruduvdz.html

[U43] PHP：声明命名空间
来源：http://hz.shangyingyoupin.top/gtjkiydrvi.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtwamjflfv.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtofjtckrb.html

declare(strict_types=1);
来源：http://hz.zycfv.cn/gtxlkcsxcl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shangyingyoupin.top/gttkfcmpub.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtzkrykexf.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtkdsgxaqp.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtuqsbzene.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtrlkijdjz.html

int|string $id
来源：http://hz.nanxuanxn.top/gtfxertdrb.html

[U48] PHP：纯枚举
来源：http://hz.yj202588.top/gtevlqsqvj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jyoumei.cn/gtfntogbzh.html

[U49] PHP：只读属性
来源：http://hz.zhaomingkeji.xyz/gtxemvbnaz.html

public readonly string $name
来源：http://hz.haohaochexian.top/gtkvueqteg.html

[U50] PHP：构造器属性提升
来源：http://hz.snrcjt.cn/gtpxqfejhk.html

public function __construct(private int $id) {}
来源：http://hz.mhx1999.top/gtaflrlvyu.html

[U51] PHP：数组解构
来源：http://hz.yonumen.top/gtygdkxaun.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtfkehoxoo.html

[U52] PHP：箭头函数
来源：http://hz.gaohongyu789.top/gtgkasaxab.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigufen.top/gtnaoqsycz.html

[U53] PHP：空合并运算符
来源：http://hz.redwolf501.top/gtzrqwwpfm.html

$v = $a ?? $b ?? "default";
来源：http://hz.nanxuanxn.top/gtxwprdxqm.html

[U54] PHP：空安全调用
来源：http://hz.ywan-chungtsiang.top/gthnuyydvs.html

$obj?->method()
来源：http://hz.zycfv.cn/gtggjoudfp.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gtbebqjyfp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zycfv.cn/gtodsuoyqy.html

[U56] PHP：命名参数
来源：http://hz.yj202588.top/gtfjuqsjoh.html

f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtkfddsnzg.html

[U57] PHP：字符串插值
来源：http://hz.guannengcc.top/gtovackvjn.html

"值: {$a}"
来源：http://hz.gaohongyu789.top/gtjdqmcpzd.html

[U58] PHP：数组三件套
来源：http://hz.chenzaomai.com/gtmipfwdjc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.nanxuanxn.top/gtkzsmmfyy.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtweowuilq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtggvvwcjj.html

[U60] PHP：JSON 编解码
来源：http://hz.yanxiufei.cn/gthxmdqpgk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigfzy.top/gtswojcarp.html

[U61] PHP：正则
来源：http://hz.hammf.cn/gtllguywps.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtliievsth.html

[U62] PHP：日期对象
来源：http://hz.svipenyu.cn/gtnphlkpnc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtgpkaabzr.html

[U63] PHP：文件读写
来源：http://hz.smart0.xyz/gtqcvmejls.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shangyingyoupin.top/gtyfswoltc.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtjxzijlhg.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.smart0.xyz/gtkaarrdgd.html

[U65] PHP：会话
来源：http://hz.chenjidiqi.icu/gtboulljxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenlongwang.top/gtqujdhhwe.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtjcsarpuo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangkeji.top/gtcmxllggk.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gttqvffosc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.redwolf501.top/gthgywbsyc.html

[U68] PHP：PDO 连接
来源：http://hz.andypj.xyz/gttuxvycwj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.vqdsnc.cn/gtjfsawzxu.html

[U69] PHP：PDO 预处理
来源：http://hz.fzhhl.top/gtehbylgtd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtqvernwgb.html

[U70] PHP：PDO 事务
来源：http://hz.daxiang520.top/gtlqgayyrd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinyuanbaomall.cn/gtzmhcrgxj.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtckhysvzf.html

throw new RuntimeException("失败", 500);
来源：http://hz.redwolf501.top/gtqflptpvy.html

[U72] PHP：写错误日志
来源：http://hz.chenzaomai.com/gtmffavcod.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxinkj.top/gtqkgeduei.html

[U73] PHP：读取 ini 配置
来源：http://hz.jqgufenzy.top/gtjojourwj.html

parse_ini_file("config.ini", true)
来源：http://hz.bjfxy.top/gtwujnzqxr.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtdruknpwd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhijiandao.cn/gtoquaempy.html

[U75] PHP：依赖注入
来源：http://hz.aibaodan.cn/gtwsedecmd.html

composer require psr/container
来源：http://hz.gogol.net.cn/gtbahfmpae.html

[U76] PHP：简单路由
来源：http://hz.xingfuxueyuan.xyz/gtpjviycit.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yangfankeji.com/gtosdbuadu.html

[U77] PHP：模板渲染
来源：http://hz.zhaomingkeji.xyz/gtdrphaybr.html

composer require twig/twig
来源：http://hz.ybcxt.top/gtfqccbpev.html

[U78] PHP：单元测试
来源：http://hz.xinyue.icu/gtpwydvqal.html

composer require --dev phpunit/phpunit
来源：http://hz.sysykeji.top/gtfzqoykjw.html

[U79] PHP：静态分析
来源：http://hz.zhixingplan.top/gtbmiobdfg.html

composer require --dev phpstan/phpstan
来源：http://hz.52xcode.cn/gtixhdgtkg.html

[U80] PHP：代码规范修复
来源：http://hz.jqgfzy.top/gtjbadztkb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gtheojwbll.html

[U81] JS：初始化项目
来源：http://hz.nanxinkj.top/gtzpftukod.html

npm init -y;  npm i express
来源：http://hz.guannengcc.top/gtspzlwuas.html

[U82] JS：package.json 脚本
来源：http://hz.iojbl.cn/gtzllxvxue.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj20258.top/gtxkttycox.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtofapryqw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.c1oappe.top/gtdumckzzx.html

[U84] JS：CommonJS 写法
来源：http://hz.daxiang520.top/gtyovbpsyh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cucudq.cn/gtwisssifn.html

[U85] JS：可选链
来源：http://hz.ybcxt.top/gtnmrhkbtt.html

a?.b?.c
来源：http://hz.hammf.cn/gtikfquddz.html

[U86] JS：空值合并
来源：http://hz.haohaochexian.top/gtcjtpkkey.html

a ?? b
来源：http://hz.zhoulong.xyz/gtoeclozgv.html

[U87] JS：解构默认值
来源：http://hz.aibaodan.cn/gtcjpjyxne.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tanke756.top/gtuyvtmjwa.html

[U88] JS：对象展开合并
来源：http://hz.wangshuangyany.cn/gtqtadaleg.html

{ ...a, ...b }
来源：http://hz.shanyushiyangkeji.top/gtqoaykkyi.html

[U89] JS：数组去重
来源：http://hz.c1oappe.top/gtkxcqqwgw.html

[...new Set(arr)]
来源：http://hz.xuanzx.com/gtuciiylxv.html

[U90] JS：数字数组排序
来源：http://hz.sweek.top/gtxvmjrtxv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtmqyekejg.html

[U91] JS：对象键值遍历
来源：http://hz.cqqwz.cn/gtujmlyuzv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinghuilouyu.cn/gtesftfrib.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gtuleqvvif.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtudbkfnqc.html

[U93] JS：模板字符串
来源：http://hz.nanxuanxn.top/gtmzrhaxwf.html

`共 ${n} 条`
来源：http://hz.ybcxt.top/gtmcjxsanw.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtywsglryr.html

const double = x => x * 2;
来源：http://hz.yvedp.cn/gtkcyakmuq.html

[U95] JS：Promise 包装
来源：http://hz.chenlongwang.top/gtgzpdtbid.html

new Promise((resolve, reject) => {})
来源：http://hz.zhengqikj.top/gtxhybcgtp.html

[U96] JS：async/await 与异常
来源：http://hz.havefunace.top/gtwqnrxfja.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtvwaxktxq.html

[U97] JS：并发请求
来源：http://hz.sweek.top/gtlpzbmwve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtwaqpydop.html

[U98] JS：fetch 带 JSON
来源：http://hz.iojbl.cn/gtjxtftwqg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gtxeevfgyi.html

[U99] JS：事件监听
来源：http://hz.zhoulong.xyz/gtnlbofcxa.html

el.addEventListener("click", e => {})
来源：http://hz.snrcjt.cn/gtlshzoops.html

[U100] JS：DOM 查询
来源：http://hz.yonumen.top/gtgxzsbruu.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtgexcvrbu.html

[U101] JS：classList 操作
来源：http://hz.svipenyu.cn/gtabrrcpse.html

el.classList.toggle("active")
来源：http://hz.jinqigufen.top/gthqnrqhfw.html

[U102] JS：本地存储
来源：http://hz.dianchejie.cn/gtyzocescg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.meibo888.top/gtsannbrhl.html

[U103] JS：定时器
来源：http://hz.nanxuanxn.top/gtbfvqvrbt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhongyouzk.top/gtyqdpcdck.html

[U104] JS：防抖
来源：http://hz.sxryk.cn/gtadkssbwi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtaafyunzw.html

[U105] JS：节流
来源：http://hz.gotoacloud.top/gtlayzywmz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuanzhike.top/gtkwzsaizz.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtfyppzndf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangtech.top/gtzxljflzr.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gtunnugvqu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.havefunace.top/gtxbnnewjg.html

[U108] JS：随机整数
来源：http://hz.mhx1999.top/gtnyrztaet.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.c1oappe.top/gtfxjmrxwo.html

[U109] JS：数组分组
来源：http://hz.zycfv.cn/gtyprkhrct.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtvxcnqluv.html

[U110] JS：数组分块
来源：http://hz.gogol.net.cn/gtycrigvll.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.0kj1m.cn/gtcbmvcacb.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangkeji.top/gtpyfsmjlh.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gttodrrmec.html

[U112] JS：字符串补位
来源：http://hz.wangshuangyany.cn/gtwzrpgamz.html

"7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtlrsmgene.html

[U113] JS：正则替换全部
来源：http://hz.zhijiandao.cn/gtiloercyu.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtvmrxqnyv.html

[U114] JS：JSON 深比较
来源：http://hz.dashuyun.cn/gtlxdqlzjm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtjpgaotzp.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gtdhzhossk.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtuciblyhe.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guannengcc.top/gtgsdwxosb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daria6918.cn/gtfgpefizm.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtgibfmoqy.html

npm i -D vitest;  npx vitest
来源：http://hz.kuanghao11.cn/gtfvherqyk.html

[U118] JS：开发服务器
来源：http://hz.iojbl.cn/gtuuxbtvcm.html

npm i -D vite;  npx vite
来源：http://hz.ppjwa.cn/gtowmkxksh.html

[U119] JS：生产构建
来源：http://hz.cucudq.cn/gtfvwprxuz.html

npx vite build
来源：http://hz.hongshengwenyu.top/gtjwdfovrx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenzaomai.com/gtnroortly.html

import.meta.env.VITE_API_URL
来源：http://hz.ywan-chungtsiang.top/gtseqsdxxu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgtotqeha.html

统计汇总
来源：http://hz.cdnleiting.top/gtubksnfus.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcmmhzrpc.html

按语言统计（条）：
来源：http://hz.nwbrower.top/gtvybeozot.html

Python ......... 252
来源：http://hz.snrcjt.cn/gtkkxepwti.html

PHP ............ 252
来源：http://hz.yj20258.top/gthtpgwkra.html

JavaScript ..... 252
来源：http://hz.ehwqpu.com/gtcjkxsqwa.html

TypeScript ..... 212
来源：http://hz.yj20258.top/gtjfpnvydi.html

Java ........... 212
来源：http://hz.hysaishi.cn/gtamszgqum.html

Go ............. 212
来源：http://hz.yongpay.top/gtmyahltmc.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtwwiloccw.html

C# ............. 212
来源：http://hz.0kj1m.cn/gtozstrlye.html

C .............. 30
来源：http://hz.fzhhl.top/gtqvstpjvi.html

C++ ............ 30
来源：http://hz.havefunace.top/gtfwsaomtk.html

SQL ............ 90
来源：http://hz.zhixingplan.top/gtkphtekoe.html

Bash ........... 80
来源：http://hz.ehwqpu.com/gtwaeozkom.html

Kotlin ......... 15
来源：http://hz.zhengqikj.top/gtfmkzhpxt.html

Swift .......... 15
来源：http://hz.yueranfly.top/gttryskbem.html

Lua ............ 10
来源：http://hz.jiagoushi.top/gthskvtxrk.html

Perl ........... 10
来源：http://hz.zhoulong.xyz/gtrpmoiynr.html

Scala .......... 10
来源：http://hz.birdmap.top/gtvppqmidb.html

------------------------------------
来源：http://hz.jianghu66.top/gtaxusipzo.html

合计 ........... 2106 条
来源：http://hz.yj20258888.top/gtnmkuldca.html

按章节统计：
来源：http://hz.ydzc1.top/gtrxqnfjsh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtobshigsy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtptljjeas.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtccvpjfvg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtdykjqksk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhoulong.xyz/gtlhcntixr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtjeewwefs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtcrlzeera.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtvasxmgxv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtnvxjhnuz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtprlsnqni.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtaxjyrkpv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtelexooyh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtfuxkkkiv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtvrieyspp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tianlin.xyz/gtutzrsoqa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtkiihvlit.html

Q SQL 专题                              90
来源：http://hz.sufxvd.cn/gtsyfcnxbe.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gtbtxftjsf.html

S C / C++ 专题                          60
来源：http://hz.ivvv.top/gtotfncltl.html

T 其他语言补充                          60
来源：http://hz.hywenlv.cn/gtxjmeybxk.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangtech.top/gtcgpgpxzl.html

------------------------------------
来源：http://hz.guannengcc.top/gtovtjezbc.html

合计                                  2106 条
来源：http://hz.ywan-chungtsiang.top/gtqybiritu.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtywsskrxh.html

使用提醒
来源：http://hz.gotoacloud.top/gtwmculehy.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gtfrzpevyh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.haohaochexian.top/gtinyvpmlv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yanxiufei.cn/gtukmxtwlt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aibaodan.cn/gtvhglksqc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tianlin.xyz/gtznpiovmi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shanyushiyangkeji.top/gtziocztkj.html

—— 文件结束 ——
来源：http://hz.hnxiangtu.top/gtpidcxxcr.html

================================================================================
来源：http://hz.aibaodan.cn/gterqyhnrf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.0kj1m.cn/gtsclvmdtg.html

Common Programming Examples Cheat Book
来源：http://hz.haohaochexian.top/gtebvkwxrc.html

================================================================================
来源：http://hz.cashguo.top/gtmuuzpbxy.html

【收录内容】
来源：http://hz.yuxming.cn/gthyqhdyxo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.0kj1m.cn/gtbdkxokai.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuanzhike.top/gtthrbxlty.html

SQL · Bash · C · C++
来源：http://hz.havefunace.top/gtclntisco.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hywenlv.cn/gtoyfhikdf.html

【使用说明】
来源：http://hz.xuetiantiany.cn/gtnbgpcgcd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.fzhhl.top/gtlhwdajyb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yonumen.top/gtqrtpebmy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtejfkwwzr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.haohaochexian.top/gtfsnzfehk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xingfuxueyuan.xyz/gtcuyetdts.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhoulong.xyz/gtyrxybrkf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.mhx1999.top/gtsppatoke.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tianlin.xyz/gtsokwzgci.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinghuilouyu.cn/gtbonoqrrg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yonumen.top/gtnojjwmbn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ivvv.top/gtjtjnnufs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenlongwang.top/gtmozrbqfq.html

【文件统计】
来源：http://hz.jiagoushi.top/gtpdmzhhhu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhoulong.xyz/gtjzpcrktd.html

--------------------------------------------------------------------------------
来源：http://hz.gogol.net.cn/gtvocewuxs.html

目  录
来源：http://hz.shuidangran.top/gtzmjpsiwf.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtbwurwvez.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtrydytvmh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gtzcnlhtgn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.birdmap.top/gtountioly.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.feifeiyinyue.top/gtxzzordrd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuanzhike.top/gtqsgkjxej.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuxming.cn/gtjclgemdn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtdapoefwz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtffeimwlx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtpdbjajky.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ehwqpu.com/gtndeajjwm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtcafrgfoa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtilgxwznr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtmpzexrsc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangdashe.top/gtsoivxxfk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhongyouzk.top/gtsmtrncrt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtyeggvyhz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhaomingkeji.xyz/gtzztqyxny.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zycfv.cn/gtbtjjbnal.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.kuanghao11.cn/gtwdadzasz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtfqelqpeh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ppjwa.cn/gtfpavnbtg.html

================================================================================
来源：http://hz.cucudq.cn/gtxrqnigyn.html

A. 基础语法与类型
来源：http://hz.ppjwa.cn/gtdaxtjhry.html

================================================================================
来源：http://hz.meibo888.top/gtyddljynl.html

[A01] Hello World
来源：http://hz.gaohongyu789.top/gtxujeayjy.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtfpvghacr.html

PHP:  echo "Hello, World!";
来源：http://hz.haohaochexian.top/gtbwrznmzc.html

JS:   console.log("Hello, World!");
来源：http://hz.chenzaomai.com/gtyckelptv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yueranfly.top/gtxelxotak.html

Java: System.out.println("Hello, World!");
来源：http://hz.jlsjyb.cn/gtkialdwux.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.fengsongda.top/gtrrlsngtp.html

Ruby: puts "Hello, World!"
来源：http://hz.52xcode.cn/gtaahntjjy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cheryme.top/gttkpeuqau.html

[A02] 变量声明与赋值
来源：http://hz.ybcxt.top/gtyoguymtr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.vqdsnc.cn/gtqqzdirrf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yangfankeji.com/gtfpbfilrd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gotoacloud.top/gtoufxcvng.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhongyouzk.top/gtleedjhms.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gtcplladnx.html

Go:   name := "Alex"; age := 20
来源：http://hz.316326.xyz/gtbuurbbek.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guannengcc.top/gtyjacoojt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.shangyingyoupin.top/gtihqfklfj.html

[A03] 常量定义
来源：http://hz.zhaomingkeji.xyz/gtsmgphnow.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.feifeiyinyue.top/gtskmvgbhs.html

PHP:  const PI = 3.14159;
来源：http://hz.hysaishi.cn/gtjujkhnrh.html

JS:   const PI = 3.14159;
来源：http://hz.redwolf501.top/gtbfxjwbgs.html

TS:   const PI: number = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtbamztean.html

Java: static final double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtluxrnisc.html

Go:   const PI = 3.14159
来源：http://hz.pycfn.com/gtbmgmjeel.html

Ruby: PI = 3.14159
来源：http://hz.yuxming.cn/gtxvkbomhp.html

C#:   const double PI = 3.14159;
来源：http://hz.nwbrower.top/gtkrncjedw.html

[A04] 判断变量类型
来源：http://hz.wangdashe.top/gtgbkknyqa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.vqdsnc.cn/gtvkhtvmrv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.tianlin.xyz/gtftizjhlc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.316326.xyz/gthbwmkgau.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnqzz.top/gtzcuqlgbk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.0kj1m.cn/gtaarnqavc.html


<!-- 参考信息 -->