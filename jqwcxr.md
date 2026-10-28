代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.hfpthk.cn/gtykjjvdhq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtvfxtjvku.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtqmdlzskk.html

?string $name = null
来源：http://hz.jqgfzy.top/gtnesrxtqw.html

[U47] PHP：联合类型
来源：http://hz.aibaodan.cn/gtnzqscbez.html

int|string $id
来源：http://hz.yj20258888.top/gtnduslbtq.html

[U48] PHP：纯枚举
来源：http://hz.bjfxy.top/gtdfvcgmhj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yongpay.top/gtvnerogwy.html

[U49] PHP：只读属性
来源：http://hz.mhx1999.top/gtvnuahsge.html

public readonly string $name
来源：http://hz.ybcxt.top/gtnsxyfkim.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtzrkvxtfa.html

public function __construct(private int $id) {}
来源：http://hz.haohaochexian.top/gtreebfqqx.html

[U51] PHP：数组解构
来源：http://hz.ehwqpu.com/gtrydjitpu.html

[$a, $b] = $arr;
来源：http://hz.cheryme.top/gtfalmlque.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtjwevlybm.html

$double = fn($x) => $x * 2;
来源：http://hz.yangfankeji.com/gtcbucyeoa.html

[U53] PHP：空合并运算符
来源：http://hz.cashguo.top/gtbzbkdttp.html

$v = $a ?? $b ?? "default";
来源：http://hz.xylfe.cn/gtcigorxmg.html

[U54] PHP：空安全调用
来源：http://hz.cheryme.top/gtdioobptj.html

$obj?->method()
来源：http://hz.daxiang520.top/gtlcuvmuqr.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gtmhdbeecs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.birdmap.top/gtvxypvcfg.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gthztuhnyg.html

f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtrswlynkf.html

[U57] PHP：字符串插值
来源：http://hz.shzxlz.cn/gtbyexzilb.html

"值: {$a}"
来源：http://hz.yvedp.cn/gthqrrzedc.html

[U58] PHP：数组三件套
来源：http://hz.zhaomingkeji.xyz/gtdeeecgdp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.bjfxy.top/gtlambopzr.html

[U59] PHP：自定义排序
来源：http://hz.jinqigfzy.top/gthmupuqqd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtmuvzbcdc.html

[U60] PHP：JSON 编解码
来源：http://hz.ybcxt.top/gtoofzaqbt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.birdmap.top/gtrkynhcsg.html

[U61] PHP：正则
来源：http://hz.yj202588.top/gtlvyeedvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtmermoydd.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtlenxlivz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtkbabhwji.html

[U63] PHP：文件读写
来源：http://hz.birdmap.top/gtwunxynyw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtxksfnaal.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtekxkpmbn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gaohongyu789.top/gthivcunra.html

[U65] PHP：会话
来源：http://hz.dianchejie.cn/gtlutdvnqp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shanyushiyangtech.top/gtrgtwreee.html

[U66] PHP：设置 Cookie
来源：http://hz.ppjwa.cn/gtutqznisk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.daria6918.cn/gtelebxnuc.html

[U67] PHP：处理文件上传
来源：http://hz.nanxuanxn.top/gtirwwguqn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hnqzz.top/gtguqocsmo.html

[U68] PHP：PDO 连接
来源：http://hz.hfpthk.cn/gtjddyxfhv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhiwuduotai.top/gtwmnjzrlo.html

[U69] PHP：PDO 预处理
来源：http://hz.kuanghao11.cn/gtwhlgzgnw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtzoqruhzd.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gtkijsevip.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhixingplan.top/gttexgbbtk.html

[U71] PHP：抛出异常
来源：http://hz.zhixingplan.top/gtfpwgeliz.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtjqorqubq.html

[U72] PHP：写错误日志
来源：http://hz.zhaomingkeji.xyz/gtuhjvcaov.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daria6918.cn/gttuqtjyuf.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhixingplan.top/gtnzpwnelz.html

parse_ini_file("config.ini", true)
来源：http://hz.xinyue.icu/gtrdlvuhtw.html

[U74] PHP：读取环境变量
来源：http://hz.jyoumei.cn/gtlbdalqji.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cucudq.cn/gtejgwjzbo.html

[U75] PHP：依赖注入
来源：http://hz.gotoacloud.top/gtivfbgglx.html

composer require psr/container
来源：http://hz.yuanzhike.top/gtfexrdxjo.html

[U76] PHP：简单路由
来源：http://hz.xinyue.icu/gtfksrwtur.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.svipenyu.cn/gtjxhkwsqc.html

[U77] PHP：模板渲染
来源：http://hz.daxiang520.top/gtcrmmlzha.html

composer require twig/twig
来源：http://hz.pengpengdd.cyou/gtmivnvhhy.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangkeji.top/gtjyaxrkyg.html

composer require --dev phpunit/phpunit
来源：http://hz.0kj1m.cn/gtclpykymg.html

[U79] PHP：静态分析
来源：http://hz.smart0.xyz/gtxmaduned.html

composer require --dev phpstan/phpstan
来源：http://hz.hywenlv.cn/gtoolqkkny.html

[U80] PHP：代码规范修复
来源：http://hz.zhengqikj.top/gtrrrqxhli.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zycfv.cn/gtxqantayf.html

[U81] JS：初始化项目
来源：http://hz.yueranfly.top/gtxnihjrah.html

npm init -y;  npm i express
来源：http://hz.jinqigfzy.top/gthgtqqior.html

[U82] JS：package.json 脚本
来源：http://hz.xuetiantiany.cn/gtxqgvkgvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gtnuujacvs.html

[U83] JS：ES Module 导入导出
来源：http://hz.hammf.cn/gtpaczyint.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cheryme.top/gtdwtyqgep.html

[U84] JS：CommonJS 写法
来源：http://hz.0kj1m.cn/gtzbapmcvi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.316326.xyz/gtcixejfym.html

[U85] JS：可选链
来源：http://hz.hongshengwenyu.top/gtcsiarweo.html

a?.b?.c
来源：http://hz.chenjidiqi.icu/gtochdggdr.html

[U86] JS：空值合并
来源：http://hz.jianghu66.top/gtuurzrnsv.html

a ?? b
来源：http://hz.meibo888.top/gtlwycddsk.html

[U87] JS：解构默认值
来源：http://hz.feifeiyinyue.top/gtymbidpfd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.c1oappe.top/gtteqwktjv.html

[U88] JS：对象展开合并
来源：http://hz.zhaomingkeji.xyz/gtoqwshnlk.html

{ ...a, ...b }
来源：http://hz.jinqigfzy.top/gtngkgbcnb.html

[U89] JS：数组去重
来源：http://hz.daria6918.cn/gtwwhtevdu.html

[...new Set(arr)]
来源：http://hz.gotoacloud.top/gtwjufqxye.html

[U90] JS：数字数组排序
来源：http://hz.jlsjyb.cn/gtluctzrah.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtrewciymt.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gtdcmdmvpb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shangyingyoupin.top/gtnkftnibc.html

[U92] JS：深拷贝
来源：http://hz.cheryme.top/gtjtombivp.html

structuredClone(obj)
来源：http://hz.dashuyun.cn/gtitlihlsq.html

[U93] JS：模板字符串
来源：http://hz.tanke756.top/gtvvdbsjkp.html

`共 ${n} 条`
来源：http://hz.mhx1999.top/gtougskmbt.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gttykwxcfm.html

const double = x => x * 2;
来源：http://hz.daria6918.cn/gtobhzjjxh.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtbloikefx.html

new Promise((resolve, reject) => {})
来源：http://hz.vqdsnc.cn/gtdmqquwqm.html

[U96] JS：async/await 与异常
来源：http://hz.ppjwa.cn/gtdwvtwgsq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtuzhccrgr.html

[U97] JS：并发请求
来源：http://hz.yonumen.top/gtyduxnqqy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtzdilugrr.html

[U98] JS：fetch 带 JSON
来源：http://hz.sweek.top/gtvwuqjazp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shanyushiyangtech.top/gtchocvraq.html

[U99] JS：事件监听
来源：http://hz.jlsjyb.cn/gtuihhzcaa.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtytujdckc.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtrvglmmfv.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gttmzwttdz.html

[U101] JS：classList 操作
来源：http://hz.hongshengwenyu.top/gthlbpqwvu.html

el.classList.toggle("active")
来源：http://hz.fzhhl.top/gtymywlzif.html

[U102] JS：本地存储
来源：http://hz.0kj1m.cn/gtoezmydxa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.pengpengdd.cyou/gttbmeexpv.html

[U103] JS：定时器
来源：http://hz.daxiang520.top/gtwvfnagqk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.bjfxy.top/gtbkdpsivj.html

[U104] JS：防抖
来源：http://hz.cdnleiting.top/gtvaiyoqnx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtkwwqodzi.html

[U105] JS：节流
来源：http://hz.havefunace.top/gtaixpkwlr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daxiang520.top/gtazkkrrot.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtyuamuoeh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gttlkvmcpb.html

[U107] JS：数字千分位
来源：http://hz.chenzaomai.com/gtciofvynb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shangyingyoupin.top/gtnmhemjxm.html

[U108] JS：随机整数
来源：http://hz.nwbrower.top/gtlydtdofw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cheryme.top/gtfzatqfrv.html

[U109] JS：数组分组
来源：http://hz.chenzaomai.com/gtvntqegxh.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtffprbmxr.html

[U110] JS：数组分块
来源：http://hz.zhengqikj.top/gtflodhtsy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gttzcxtwjp.html

[U111] JS：对象转 Map
来源：http://hz.daxiang520.top/gtccugmixy.html

new Map(Object.entries(obj))
来源：http://hz.yj20258.top/gttbfrakjj.html

[U112] JS：字符串补位
来源：http://hz.chenzaomai.com/gtufritapl.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gthawvavkj.html

[U113] JS：正则替换全部
来源：http://hz.jianghu66.top/gtbofswsjo.html

s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtkzkgkjxe.html

[U114] JS：JSON 深比较
来源：http://hz.chenjidiqi.icu/gtjmweftjq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydzc1.top/gtsronibgx.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtixitvtko.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtzwtucfjq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.vqdsnc.cn/gtjtrspzvd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj202588.top/gtccorxfxt.html

[U117] JS：单元测试
来源：http://hz.zycfv.cn/gtpynyypeh.html

npm i -D vitest;  npx vitest
来源：http://hz.svipenyu.cn/gtppwwdwvg.html

[U118] JS：开发服务器
来源：http://hz.zhijiandao.cn/gtkozsfdxj.html

npm i -D vite;  npx vite
来源：http://hz.feifeiyinyue.top/gtnvgjbvdf.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gtenvwceey.html

npx vite build
来源：http://hz.cqqwz.cn/gtvgmslqde.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.guowangkeji.top/gtsuwppohk.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtoehwapta.html

================================================================================
来源：http://hz.hnqzz.top/gtpzswtlqd.html

统计汇总
来源：http://hz.tianlin.xyz/gtgztotwyj.html

================================================================================
来源：http://hz.gogol.net.cn/gtlwgtktnr.html

按语言统计（条）：
来源：http://hz.c1oappe.top/gtcnihaaua.html

Python ......... 252
来源：http://hz.kuanghao11.cn/gtizmymsxf.html

PHP ............ 252
来源：http://hz.yuanzhike.top/gtpniksjee.html

JavaScript ..... 252
来源：http://hz.jyoumei.cn/gtdlrinriq.html

TypeScript ..... 212
来源：http://hz.yj20258.top/gtjlxzuhzf.html

Java ........... 212
来源：http://hz.gzhubu.top/gtgwfivvps.html

Go ............. 212
来源：http://hz.andypj.xyz/gtkxggfuhb.html

Ruby ........... 212
来源：http://hz.yanxiufei.cn/gtjgdjbrhv.html

C# ............. 212
来源：http://hz.quarkkingdee.top/gtrminzvas.html

C .............. 30
来源：http://hz.yj20258888.top/gtzcwiaysv.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtrmnyoabv.html

SQL ............ 90
来源：http://hz.birdmap.top/gtsheepasj.html

Bash ........... 80
来源：http://hz.tian-w.cn/gtlskuelzy.html

Kotlin ......... 15
来源：http://hz.hammf.cn/gtbqweradg.html

Swift .......... 15
来源：http://hz.havefunace.top/gtsiyrpjjv.html

Lua ............ 10
来源：http://hz.cdnleiting.top/gtperkrmtx.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gthofwlftj.html

Scala .......... 10
来源：http://hz.svipenyu.cn/gtqawnygkb.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtldqqzusf.html

合计 ........... 2106 条
来源：http://hz.yuanzhike.top/gtqocvybev.html

按章节统计：
来源：http://hz.hongshengwenyu.top/gtwadhpdyi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtsikdfgll.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gthgsorsla.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtbzbcyvdq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.birdmap.top/gtlhsvqsfr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhengqikj.top/gtgnplczpz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtmpyhwzlw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtvogsansf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtghdhlzvc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtydmolnln.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtbmqitohy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtyxnnhjus.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtpkvteock.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtcgmigyff.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hfpthk.cn/gtfapxrsqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuetiantiany.cn/gtdvopnpws.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtvagqbqku.html

Q SQL 专题                              90
来源：http://hz.xuetiantiany.cn/gtgxmvpldf.html

R Bash 专题                             80
来源：http://hz.vqdsnc.cn/gtdbrgorky.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtjlqizijr.html

T 其他语言补充                          60
来源：http://hz.ppjwa.cn/gtcrdgoxak.html

U 高频实用片段                         120
来源：http://hz.ywan-chungtsiang.top/gtmptwenci.html

------------------------------------
来源：http://hz.havefunace.top/gtfhdymetm.html

合计                                  2106 条
来源：http://hz.yj202588.top/gtnededvjv.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtotkooudf.html

使用提醒
来源：http://hz.shanyushiyangkeji.top/gtbdpcrkoe.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtiriytoab.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtkyetobqn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jqgfzy.top/gtkpgwlsiv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jyoumei.cn/gtrtebknqs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj20258888.top/gtigrfxboq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tanke756.top/gtxcnqwqmx.html

—— 文件结束 ——
来源：http://hz.daxiang520.top/gtomnkbktb.html

================================================================================
来源：http://hz.kuanghao11.cn/gtopyyfjhd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shanyushiyangkeji.top/gtmqgyecdx.html

Common Programming Examples Cheat Book
来源：http://hz.yongpay.top/gtsvjxpreo.html

================================================================================
来源：http://hz.cheryme.top/gtkmotlats.html

【收录内容】
来源：http://hz.yongpay.top/gtioaxctvx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xuetiantiany.cn/gtdxytybgu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhongyouzk.top/gtpbijfnrq.html

SQL · Bash · C · C++
来源：http://hz.jyoumei.cn/gthjrpmkxy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ppjwa.cn/gtidlhljhl.html

【使用说明】
来源：http://hz.chenlongwang.top/gtyjurcmst.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gttmlnegli.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ppjwa.cn/gtihryfoze.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jlsjyb.cn/gtuwwoeowj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hongshengwenyu.top/gtgoragquk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xinyue.icu/gtwzedpvbp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.mhx1999.top/gtcxufgpys.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtgvjnjret.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hywenlv.cn/gthbzqxati.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hywenlv.cn/gtbexgqqcp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zdqjudy.top/gtmqkaqkgn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.guannengcc.top/gthxwyxfio.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinghuilouyu.cn/gtkjgymawp.html

【文件统计】
来源：http://hz.zycfv.cn/gtegwuauwm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pycfn.com/gtvmnjlunh.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gttayzphmr.html

目  录
来源：http://hz.52xcode.cn/gtatwqkjkr.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtwymwjmsx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.kuanghao11.cn/gtqflstnon.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtwjzsrlyk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gtvvnosjky.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtmkjeaywf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xziqi.cn/gtnysjnkox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtngqfejqn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtpztwrikn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.andypj.xyz/gtbhivbrpu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtelejhlux.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.316326.xyz/gtlfamzlqk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gteuxwtgvw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtzlfkcqdf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtiwcjifsd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hfpthk.cn/gtrrlsuyrs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dashuyun.cn/gtylezqwvr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtacjkpjvk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.9152youxi.cn/gtuvkchzwa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hysaishi.cn/gtdlxpuyfk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gthnbqgidi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtqzevvvjz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.feifeiyinyue.top/gtjiyrssgh.html

================================================================================
来源：http://hz.tian-w.cn/gtacuttgra.html

A. 基础语法与类型
来源：http://hz.shanyushiyangkeji.top/gtboblrlks.html

================================================================================
来源：http://hz.ydjk.org.cn/gtsrhqvlbq.html

[A01] Hello World
来源：http://hz.aizwys.cn/gtzfbrhgad.html

Py:   print("Hello, World!")
来源：http://hz.fengsongda.top/gthsmjewmu.html

PHP:  echo "Hello, World!";
来源：http://hz.hysaishi.cn/gtirmtrush.html

JS:   console.log("Hello, World!");
来源：http://hz.tianlin.xyz/gthtyezxzj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhiwuduotai.top/gtmbdzogmt.html

Java: System.out.println("Hello, World!");
来源：http://hz.cucudq.cn/gtwyfmqufc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.kuanghao11.cn/gtrtseymfv.html

Ruby: puts "Hello, World!"
来源：http://hz.yj20258888.top/gtnlfhhoek.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hywenlv.cn/gtxiukadrz.html

[A02] 变量声明与赋值
来源：http://hz.zhoulong.xyz/gtlmwylktu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.mhx1999.top/gtwehtmvam.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tianlin.xyz/gtgsambzvn.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sweek.top/gtfucoxzwp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydjk.org.cn/gtqtisornn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenlongwang.top/gtbjqxjmwm.html

Go:   name := "Alex"; age := 20
来源：http://hz.yangfankeji.com/gtvaklqjby.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgfzy.top/gtyztcbyjg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cdnleiting.top/gtbhgqlyvc.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtnoeenzzu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinghuilouyu.cn/gtlvggpmkm.html

PHP:  const PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtouhqcrgf.html

JS:   const PI = 3.14159;
来源：http://hz.ivvv.top/gtixpxmadr.html

TS:   const PI: number = 3.14159;
来源：http://hz.gaohongyu789.top/gthdlrdhtj.html

Java: static final double PI = 3.14159;
来源：http://hz.sweek.top/gtvohiltmv.html

Go:   const PI = 3.14159
来源：http://hz.fzhhl.top/gtpqkzpogr.html

Ruby: PI = 3.14159
来源：http://hz.yongpay.top/gtrcbvouwr.html

C#:   const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtnlfggucy.html

[A04] 判断变量类型
来源：http://hz.xingfuxueyuan.xyz/gtzabtzvwu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ybcxt.top/gtxkxbyayd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.nanxuanxn.top/gtdrqxihgs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.feifeiyinyue.top/gtajhqnhad.html

TS:   typeof x; x instanceof Date
来源：http://hz.hfpthk.cn/gtfwekyssx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.bjfxy.top/gtqtrtqubz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xuetiantiany.cn/gtdfdzdybi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gogol.net.cn/gtobpuwzwa.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtmqsvmhbs.html

[A05] 整数除法与取模
来源：http://hz.gotoacloud.top/gtptifyons.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.guannengcc.top/gtrtibfdkf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yanxiufei.cn/gtsnccwckv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sysykeji.top/gtvcybpitr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tianlin.xyz/gtwmgxmabp.html


<!-- 参考信息 -->