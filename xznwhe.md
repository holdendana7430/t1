代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtxhukxxjt.html

sys.stdout.isatty()
来源：http://hz.redwolf501.top/gtuataackh.html

[U40] Py：打印到标准错误
来源：http://hz.dianchejie.cn/gtnpyipjfv.html

print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtyvvoidyk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydzc1.top/gtvhemmcba.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tanke756.top/gtyvwbcbjn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhengqikj.top/gtwwsmgafo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtzggryepy.html

[U43] PHP：声明命名空间
来源：http://hz.yj20258.top/gtjropbxjm.html

namespace App\Http;
来源：http://hz.yj20258.top/gttvcowxbu.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtdnbsamun.html

declare(strict_types=1);
来源：http://hz.pengpengdd.cyou/gtwrsxadlc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj202588.top/gtzyfmfmly.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtppcyiydz.html

[U46] PHP：可空类型
来源：http://hz.hysaishi.cn/gtynoobkyh.html

?string $name = null
来源：http://hz.gaohongyu789.top/gtgubesklv.html

[U47] PHP：联合类型
来源：http://hz.xingfuxueyuan.xyz/gtovrbwers.html

int|string $id
来源：http://hz.cdnleiting.top/gtreerwmzn.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtretpsymz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yonumen.top/gtexoxjpyd.html

[U49] PHP：只读属性
来源：http://hz.xuanzx.com/gtuvvugqdo.html

public readonly string $name
来源：http://hz.yueranfly.top/gtjnmbrvej.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gtpldfcqie.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gtzylafpfk.html

[U51] PHP：数组解构
来源：http://hz.zhiwuduotai.top/gtsgqltneq.html

[$a, $b] = $arr;
来源：http://hz.pycfn.com/gtlmiaxqiy.html

[U52] PHP：箭头函数
来源：http://hz.c1oappe.top/gthmjruoyi.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtfmfslxwu.html

[U53] PHP：空合并运算符
来源：http://hz.gotoacloud.top/gtcgthwjqk.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gtlycxluyf.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtqkjlekvp.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtsfcjjrit.html

[U55] PHP：match 表达式
来源：http://hz.jianghu66.top/gtqcfljqqe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxuanxn.top/gtejjgujvb.html

[U56] PHP：命名参数
来源：http://hz.tian-w.cn/gtgqkxwzda.html

f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtelbskkru.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gtbcsfbhzw.html

"值: {$a}"
来源：http://hz.jlsjyb.cn/gtjukhukwl.html

[U58] PHP：数组三件套
来源：http://hz.svipenyu.cn/gtwycgqodf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.snrcjt.cn/gtujddshkz.html

[U59] PHP：自定义排序
来源：http://hz.yongpay.top/gtgcdhulac.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtlcekamil.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtbjxhyyqg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtmnlouyne.html

[U61] PHP：正则
来源：http://hz.cqqwz.cn/gtbaitqwqv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtqvsmeqcw.html

[U62] PHP：日期对象
来源：http://hz.ivvv.top/gtwqrvtecu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigufen.top/gtioyznknx.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtzwdlpskx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ivvv.top/gtazsurmyz.html

[U64] PHP：目录遍历
来源：http://hz.yuanzhike.top/gtyobzmlzv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuxming.cn/gtkrblbbgo.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtaeolffnz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtxrjsjuxp.html

[U66] PHP：设置 Cookie
来源：http://hz.yuxming.cn/gtcgohrozq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xingfuxueyuan.xyz/gtsftexzch.html

[U67] PHP：处理文件上传
来源：http://hz.pycfn.com/gtmadejuxh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hywenlv.cn/gtfqexpwvv.html

[U68] PHP：PDO 连接
来源：http://hz.jiagoushi.top/gtatyldhvr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtxxmspbcw.html

[U69] PHP：PDO 预处理
来源：http://hz.tianlin.xyz/gtvvxhxtxy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nwbrower.top/gtzspvrcrk.html

[U70] PHP：PDO 事务
来源：http://hz.nanxuanxn.top/gtjglheyfw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fengsongda.top/gtjxzgusmy.html

[U71] PHP：抛出异常
来源：http://hz.zhaomingkeji.xyz/gtdvojxcgt.html

throw new RuntimeException("失败", 500);
来源：http://hz.xziqi.cn/gtmlfqnglc.html

[U72] PHP：写错误日志
来源：http://hz.52xcode.cn/gtfqjtikib.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hysaishi.cn/gtevylnwko.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhixingplan.top/gtlcjdtfks.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtctziehgr.html

[U74] PHP：读取环境变量
来源：http://hz.shuidangran.top/gtqfainilr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtuhzzbgwj.html

[U75] PHP：依赖注入
来源：http://hz.daxiang520.top/gtzgctldtf.html

composer require psr/container
来源：http://hz.yanxiufei.cn/gtlrcbaknr.html

[U76] PHP：简单路由
来源：http://hz.jyoumei.cn/gthiozyzcq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.mhx1999.top/gtqguaegux.html

[U77] PHP：模板渲染
来源：http://hz.tanke756.top/gtueasrceu.html

composer require twig/twig
来源：http://hz.hammf.cn/gtcperhrpv.html

[U78] PHP：单元测试
来源：http://hz.cqqwz.cn/gtlnjggvzb.html

composer require --dev phpunit/phpunit
来源：http://hz.redwolf501.top/gtmbkcobqt.html

[U79] PHP：静态分析
来源：http://hz.hnxiangtu.top/gtdstnqokc.html

composer require --dev phpstan/phpstan
来源：http://hz.svipenyu.cn/gtqyciunlb.html

[U80] PHP：代码规范修复
来源：http://hz.dianchejie.cn/gthgbwmycj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gaohongyu789.top/gtieaonlyq.html

[U81] JS：初始化项目
来源：http://hz.pengpengdd.cyou/gtnnpgttci.html

npm init -y;  npm i express
来源：http://hz.havefunace.top/gtngfztflg.html

[U82] JS：package.json 脚本
来源：http://hz.chenjidiqi.icu/gtjkijlbyl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hfpthk.cn/gtwujsjmpn.html

[U83] JS：ES Module 导入导出
来源：http://hz.ivvv.top/gtavtlpwth.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.redwolf501.top/gtbvgjdwbr.html

[U84] JS：CommonJS 写法
来源：http://hz.52xcode.cn/gttzsmapgg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aizwys.cn/gtpzgoaydv.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gttozhrupn.html

a?.b?.c
来源：http://hz.bjfxy.top/gtcvrtahib.html

[U86] JS：空值合并
来源：http://hz.gaohongyu789.top/gtzaxxedmc.html

a ?? b
来源：http://hz.ehwqpu.com/gtzqizmujn.html

[U87] JS：解构默认值
来源：http://hz.jlsjyb.cn/gtdxbebmrs.html

const { a = 1, b = 2 } = obj;
来源：http://hz.iojbl.cn/gtmnijcrar.html

[U88] JS：对象展开合并
来源：http://hz.zycfv.cn/gtramzoafu.html

{ ...a, ...b }
来源：http://hz.nwbrower.top/gtfdijzbpc.html

[U89] JS：数组去重
来源：http://hz.daxiang520.top/gtquztuslq.html

[...new Set(arr)]
来源：http://hz.yj202588.top/gtqktnrjcs.html

[U90] JS：数字数组排序
来源：http://hz.jqgufenzy.top/gtdlffwgph.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtmvdpvooi.html

[U91] JS：对象键值遍历
来源：http://hz.dashuyun.cn/gtwdqkekyu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtiiakbugu.html

[U92] JS：深拷贝
来源：http://hz.hammf.cn/gtuxzkmlux.html

structuredClone(obj)
来源：http://hz.aizwys.cn/gtchyidevi.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtuvjbrbxb.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtztewcdbg.html

[U94] JS：箭头函数
来源：http://hz.shangyingyoupin.top/gtdxcmssun.html

const double = x => x * 2;
来源：http://hz.gotoacloud.top/gtmetunigz.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gtrnusbkqf.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtkabciczl.html

[U96] JS：async/await 与异常
来源：http://hz.xuetiantiany.cn/gtmwdjtioz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtilgqzawz.html

[U97] JS：并发请求
来源：http://hz.redwolf501.top/gtdkidvdbz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtrfecnwlx.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtouhlwmbh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nwbrower.top/gtutzulkkv.html

[U99] JS：事件监听
来源：http://hz.havefunace.top/gtybgqzibw.html

el.addEventListener("click", e => {})
来源：http://hz.yongpay.top/gtgusgosio.html

[U100] JS：DOM 查询
来源：http://hz.tanke756.top/gtamluvzrr.html

document.querySelector(".item")
来源：http://hz.yj20258888.top/gtkrutxuyv.html

[U101] JS：classList 操作
来源：http://hz.316326.xyz/gtaaidkekv.html

el.classList.toggle("active")
来源：http://hz.hywenlv.cn/gtevrzuaqb.html

[U102] JS：本地存储
来源：http://hz.vqdsnc.cn/gtawvsflio.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangdashe.top/gtptovcetb.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtxdnhpdrw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.smart0.xyz/gtuzjbxyqw.html

[U104] JS：防抖
来源：http://hz.haohaochexian.top/gtehelghym.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtuxpxwwyx.html

[U105] JS：节流
来源：http://hz.zhongyouzk.top/gtiwjtozby.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnxiangtu.top/gtlxpjqvif.html

[U106] JS：日期格式化
来源：http://hz.svipenyu.cn/gtbuhejieu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fzhhl.top/gthdajtmtk.html

[U107] JS：数字千分位
来源：http://hz.zhongyouzk.top/gtvyrlxudk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xylfe.cn/gtbcbarosn.html

[U108] JS：随机整数
来源：http://hz.jinghuilouyu.cn/gteripiyzi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.52xcode.cn/gtypgwebhc.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtakdwxohf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gttfrkrntg.html

[U110] JS：数组分块
来源：http://hz.shangyingyoupin.top/gtglqnsdxb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.52xcode.cn/gttrziuqeo.html

[U111] JS：对象转 Map
来源：http://hz.jinyuanbaomall.cn/gtzjuaaijm.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtshtrqqqa.html

[U112] JS：字符串补位
来源：http://hz.yuanzhike.top/gthvkwjhuw.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gttpdjfwrz.html

[U113] JS：正则替换全部
来源：http://hz.redwolf501.top/gtmduudtsw.html

s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtbsulvvqa.html

[U114] JS：JSON 深比较
来源：http://hz.c1oappe.top/gtdwypejhz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtvuixjipn.html

[U115] JS：生成 UUID
来源：http://hz.birdmap.top/gtyofyqqoa.html

crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtidtouegi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sweek.top/gtcwswxmig.html

/** @param {string} name */ function f(name) {}
来源：http://hz.quarkkingdee.top/gtdcisxuok.html

[U117] JS：单元测试
来源：http://hz.yj20258.top/gtliwmsnsa.html

npm i -D vitest;  npx vitest
来源：http://hz.hammf.cn/gtopcthaso.html

[U118] JS：开发服务器
来源：http://hz.hnqzz.top/gtbqhyilbq.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtrzvtjrqr.html

[U119] JS：生产构建
来源：http://hz.jinqigfzy.top/gttdiufnuu.html

npx vite build
来源：http://hz.xuetiantiany.cn/gtdmllorxp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuanzhike.top/gtjnrmielu.html

import.meta.env.VITE_API_URL
来源：http://hz.tianlin.xyz/gtehdmwvpv.html

================================================================================
来源：http://hz.ehwqpu.com/gtfnlaknub.html

统计汇总
来源：http://hz.jqgufenzy.top/gtadbjfeoe.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnomesxtd.html

按语言统计（条）：
来源：http://hz.yuanzhike.top/gtznlyyqdf.html

Python ......... 252
来源：http://hz.andypj.xyz/gtpivhdyqt.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtkcglabir.html

JavaScript ..... 252
来源：http://hz.kuanghao11.cn/gtabzzjwxk.html

TypeScript ..... 212
来源：http://hz.ivvv.top/gtzxpgxxmp.html

Java ........... 212
来源：http://hz.zhoulong.xyz/gtsjezesip.html

Go ............. 212
来源：http://hz.zhoulong.xyz/gtcfyjvhxo.html

Ruby ........... 212
来源：http://hz.zhoulong.xyz/gtuaceqpnl.html

C# ............. 212
来源：http://hz.sufxvd.cn/gtzxlabpas.html

C .............. 30
来源：http://hz.yueranfly.top/gtwraenwga.html

C++ ............ 30
来源：http://hz.zdqjudy.top/gtmnngyrlf.html

SQL ............ 90
来源：http://hz.hywenlv.cn/gtvulhdrst.html

Bash ........... 80
来源：http://hz.xingfuxueyuan.xyz/gtiwjjajzt.html

Kotlin ......... 15
来源：http://hz.nanxinkj.top/gtecyghscx.html

Swift .......... 15
来源：http://hz.wangdashe.top/gtvfkpfxrd.html

Lua ............ 10
来源：http://hz.316326.xyz/gtvvfvqorh.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtsxvxkmnc.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtbrmvweyl.html

------------------------------------
来源：http://hz.cucudq.cn/gtidcnieyx.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangkeji.top/gtgenwglpt.html

按章节统计：
来源：http://hz.vqdsnc.cn/gtophjlfke.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtumaguush.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtzaviebsl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtygnqkuxh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gteurvwrjl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sxryk.cn/gtnlhtnboi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtcvuzuzsx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtziygcxvd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jianghu66.top/gtgglnjhwy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtkytpnivh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtyyvmhjil.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtqbncsqtr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtozweilks.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtugrsnedr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtdynmsosh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangdashe.top/gtzjnvoxwr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtaslqtxzk.html

Q SQL 专题                              90
来源：http://hz.jyoumei.cn/gtfnolnepg.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gttktepzhi.html

S C / C++ 专题                          60
来源：http://hz.gotoacloud.top/gtfppogxgp.html

T 其他语言补充                          60
来源：http://hz.kuanghao11.cn/gtnuimiceo.html

U 高频实用片段                         120
来源：http://hz.zycfv.cn/gtnaaquzcj.html

------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtsbbbzndv.html

合计                                  2106 条
来源：http://hz.guannengcc.top/gtirrmipyj.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtvuzfpois.html

使用提醒
来源：http://hz.gaohongyu789.top/gtxbqhswhx.html

--------------------------------------------------------------------------------
来源：http://hz.yangfankeji.com/gtuvgqrytv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.andypj.xyz/gtzrvvccmb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj202588.top/gtcarxvfyc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhengqikj.top/gtnrwqaywm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtamvpacfi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gaohongyu789.top/gttykzkzkz.html

—— 文件结束 ——
来源：http://hz.yangfankeji.com/gtflgvqjxh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtypxkviks.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtaisnxndg.html

Common Programming Examples Cheat Book
来源：http://hz.hammf.cn/gtbxontuuu.html

================================================================================
来源：http://hz.guowangkeji.top/gtwowtadhw.html

【收录内容】
来源：http://hz.aizwys.cn/gtdvurmmfs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dashuyun.cn/gtermnppwm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinghuilouyu.cn/gtcbaxowvy.html

SQL · Bash · C · C++
来源：http://hz.yongpay.top/gtcobfuyoj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ppjwa.cn/gtjepkgycf.html

【使用说明】
来源：http://hz.sxryk.cn/gtwvscclry.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hongshengwenyu.top/gtxiwuqhqq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnqzz.top/gtsnuqhodj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtlfxpbqkd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ivvv.top/gtnkopblgv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.pycfn.com/gtojrnfzjr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xuanzx.com/gtdxgsswit.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnxiangtu.top/gtocsjqdrs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zdqjudy.top/gtqsnjmpwp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.havefunace.top/gtkmvxzarr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gzhubu.top/gthpwhcugs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtvcxswjzg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgfzy.top/gtdpxgjzkc.html

【文件统计】
来源：http://hz.guowangkeji.top/gtrtosogob.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.kuanghao11.cn/gtcbvxqawe.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtbcohemfc.html

目  录
来源：http://hz.chenlongwang.top/gtcjdhmscc.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtefqigtnw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtzxssrqdf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.bjfxy.top/gtajstwdgp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtiawjckqs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtxuzpfaav.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.redwolf501.top/gtljhearkx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yuxming.cn/gtyotnbtrd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtturtjfel.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.0kj1m.cn/gtrtbqxipy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtmkbcwctb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydzc1.top/gtscutikgt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtvaubdtas.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtkkwtvsph.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtndkvynkl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gtamempome.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hongshengwenyu.top/gtxrhkqgpd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtcvsuzlwt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nwbrower.top/gtjyhtbfpa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.mhx1999.top/gttdhnljag.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinqigfzy.top/gtfiwwayjr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtmmrensdw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hysaishi.cn/gtrkylediz.html

================================================================================
来源：http://hz.guowangkeji.top/gtsaqkjiyi.html

A. 基础语法与类型
来源：http://hz.cucudq.cn/gtcqccsmno.html

================================================================================
来源：http://hz.nanxinkj.top/gtjiexghzp.html

[A01] Hello World
来源：http://hz.zdqjudy.top/gtuscixddb.html

Py:   print("Hello, World!")
来源：http://hz.jianghu66.top/gtszbstxit.html

PHP:  echo "Hello, World!";
来源：http://hz.shanyushiyangtech.top/gtgqtnryju.html

JS:   console.log("Hello, World!");
来源：http://hz.hnqzz.top/gtypaqqwtg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.dashuyun.cn/gtrvuffawv.html

Java: System.out.println("Hello, World!");
来源：http://hz.fengsongda.top/gtfrtrclkb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jlsjyb.cn/gtktezuadj.html

Ruby: puts "Hello, World!"
来源：http://hz.hammf.cn/gtdvzgjqjd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhiwuduotai.top/gtvuodcfpc.html

[A02] 变量声明与赋值
来源：http://hz.yj20258.top/gtzupbtadu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.smart0.xyz/gtebqdmutn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinqigfzy.top/gtmnabqihv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.bjfxy.top/gtalqnxqzg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhaomingkeji.xyz/gtaddgelak.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yangfankeji.com/gtxcegxjpa.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhixingplan.top/gtcpewqgze.html

Ruby: name = "Alex"; age = 20
来源：http://hz.quarkkingdee.top/gtokuqtvxq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtvezcjyno.html

[A03] 常量定义
来源：http://hz.fengsongda.top/gtizphiyjy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenjidiqi.icu/gtyqppmoll.html

PHP:  const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtxmvcvqfa.html

JS:   const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtwkfxymew.html

TS:   const PI: number = 3.14159;
来源：http://hz.zdqjudy.top/gtxfxormyn.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtgglbceqh.html

Go:   const PI = 3.14159
来源：http://hz.xziqi.cn/gtlabrully.html

Ruby: PI = 3.14159
来源：http://hz.chenjidiqi.icu/gtrehhbzgu.html

C#:   const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtgdpnvpip.html

[A04] 判断变量类型
来源：http://hz.ehwqpu.com/gtddizebpz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinghuilouyu.cn/gtisvjodyf.html


<!-- 参考信息 -->