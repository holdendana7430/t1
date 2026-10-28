代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.jinghuilouyu.cn/gtxshdyqdw.html

namespace App\Http;
来源：http://hz.feifeiyinyue.top/gtgbranomu.html

[U44] PHP：开启严格类型
来源：http://hz.yanxiufei.cn/gthhxuiogl.html

declare(strict_types=1);
来源：http://hz.dianchejie.cn/gtbwlgzvys.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gtcavhbyyx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gthhlzdrgw.html

[U46] PHP：可空类型
来源：http://hz.jinqigufen.top/gtiwtstanm.html

?string $name = null
来源：http://hz.zhiwuduotai.top/gtrgfnywii.html

[U47] PHP：联合类型
来源：http://hz.sufxvd.cn/gtluqxqxpi.html

int|string $id
来源：http://hz.pycfn.com/gtyxdzivou.html

[U48] PHP：纯枚举
来源：http://hz.shangyingyoupin.top/gtdkxjbqku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.9152youxi.cn/gtkmgcpria.html

[U49] PHP：只读属性
来源：http://hz.ivvv.top/gthblnwjet.html

public readonly string $name
来源：http://hz.xuanzx.com/gtuloouskq.html

[U50] PHP：构造器属性提升
来源：http://hz.0kj1m.cn/gtqxiazscb.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangkeji.top/gtovpcqoih.html

[U51] PHP：数组解构
来源：http://hz.sufxvd.cn/gtgxfqchod.html

[$a, $b] = $arr;
来源：http://hz.cdnleiting.top/gtobccihxv.html

[U52] PHP：箭头函数
来源：http://hz.hysaishi.cn/gtpxuzwmgb.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgufenzy.top/gtpixktcds.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtkperldql.html

$v = $a ?? $b ?? "default";
来源：http://hz.iojbl.cn/gthztutvxr.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtknnrauoq.html

$obj?->method()
来源：http://hz.dashuyun.cn/gtxtckggqj.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtrafagawo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sysykeji.top/gtkijpxokr.html

[U56] PHP：命名参数
来源：http://hz.c1oappe.top/gtnpvnxngm.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtmbrbjfvp.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtyjczcnqo.html

"值: {$a}"
来源：http://hz.yuanzhike.top/gtttnzqbbj.html

[U58] PHP：数组三件套
来源：http://hz.gzhubu.top/gtkjocpgii.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hfpthk.cn/gtaakwuubn.html

[U59] PHP：自定义排序
来源：http://hz.jlsjyb.cn/gtafmmskod.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtfsovpotb.html

[U60] PHP：JSON 编解码
来源：http://hz.yuxming.cn/gtgtoqrsrf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.quarkkingdee.top/gtjepfcstt.html

[U61] PHP：正则
来源：http://hz.yueranfly.top/gtjegniwbu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtjqqvgehs.html

[U62] PHP：日期对象
来源：http://hz.smart0.xyz/gtepmrpzus.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xinyue.icu/gtjvtxlyem.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gtvwhoqgio.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gzhubu.top/gtsoxzheaj.html

[U64] PHP：目录遍历
来源：http://hz.yuanzhike.top/gtnxppfrjp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daxiang520.top/gtvwwrawlr.html

[U65] PHP：会话
来源：http://hz.shanyushiyangtech.top/gtqjqojxnp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gogol.net.cn/gtzssyslem.html

[U66] PHP：设置 Cookie
来源：http://hz.xylfe.cn/gtamslrbua.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtkiawwhrt.html

[U67] PHP：处理文件上传
来源：http://hz.guannengcc.top/gtvcysbgre.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.feifeiyinyue.top/gtsrbbivde.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtwiekdyaf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yangfankeji.com/gtcaltooxs.html

[U69] PHP：PDO 预处理
来源：http://hz.shzxlz.cn/gtwioscjnf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tianlin.xyz/gtkpsjewmh.html

[U70] PHP：PDO 事务
来源：http://hz.meibo888.top/gtcyhsghfu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtetbbdhvu.html

[U71] PHP：抛出异常
来源：http://hz.chenlongwang.top/gtruslrmgm.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhoulong.xyz/gtzujdzmwg.html

[U72] PHP：写错误日志
来源：http://hz.hywenlv.cn/gtkjeektiv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hnqzz.top/gtnyiqyobo.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtprbcdqoa.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtshkdvhtz.html

[U74] PHP：读取环境变量
来源：http://hz.pycfn.com/gtombappzq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cheryme.top/gtlyspvcyt.html

[U75] PHP：依赖注入
来源：http://hz.gaohongyu789.top/gtvnnnwjyx.html

composer require psr/container
来源：http://hz.meibo888.top/gtkcyhovce.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtgauuayos.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhixingplan.top/gthhwuelbu.html

[U77] PHP：模板渲染
来源：http://hz.meibo888.top/gtuylqzkbo.html

composer require twig/twig
来源：http://hz.316326.xyz/gtaafrnkkp.html

[U78] PHP：单元测试
来源：http://hz.zhiwuduotai.top/gtbakotlnn.html

composer require --dev phpunit/phpunit
来源：http://hz.zdqjudy.top/gtdegxvpyp.html

[U79] PHP：静态分析
来源：http://hz.aibaodan.cn/gtggmwpaim.html

composer require --dev phpstan/phpstan
来源：http://hz.xuanzx.com/gtclexzduw.html

[U80] PHP：代码规范修复
来源：http://hz.gotoacloud.top/gtxifwsmdj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zdqjudy.top/gtjlfdipdi.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtjemhkxik.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtimchxlht.html

[U82] JS：package.json 脚本
来源：http://hz.sweek.top/gtcywjditq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xinyue.icu/gtawjirrzt.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtrccjevpr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cqqwz.cn/gtkxjtwhoj.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtzrefmzua.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xuetiantiany.cn/gtlwlhlqpq.html

[U85] JS：可选链
来源：http://hz.mhx1999.top/gtmpvyecrn.html

a?.b?.c
来源：http://hz.jinyuanbaomall.cn/gtzvldjmjy.html

[U86] JS：空值合并
来源：http://hz.xziqi.cn/gtmhfzvjjt.html

a ?? b
来源：http://hz.shangyingyoupin.top/gtruebjztk.html

[U87] JS：解构默认值
来源：http://hz.daxiang520.top/gtubmnzulj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gtjbymjcel.html

[U88] JS：对象展开合并
来源：http://hz.zhixingplan.top/gtgtluzxfu.html

{ ...a, ...b }
来源：http://hz.chenzaomai.com/gtdmilaxfd.html

[U89] JS：数组去重
来源：http://hz.guowangkeji.top/gtlsjquwfg.html

[...new Set(arr)]
来源：http://hz.ppjwa.cn/gtbwhlmhpf.html

[U90] JS：数字数组排序
来源：http://hz.zhixingplan.top/gtakrhuffd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtessnxyhe.html

[U91] JS：对象键值遍历
来源：http://hz.cheryme.top/gtevgkownb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgfzy.top/gtfrfeuxuv.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtxhnqwpin.html

structuredClone(obj)
来源：http://hz.redwolf501.top/gtiowadccn.html

[U93] JS：模板字符串
来源：http://hz.zdqjudy.top/gtfkayrqxc.html

`共 ${n} 条`
来源：http://hz.bjfxy.top/gtxfyhavyx.html

[U94] JS：箭头函数
来源：http://hz.jianghu66.top/gtpbwvqrtt.html

const double = x => x * 2;
来源：http://hz.nanxuanxn.top/gtikrfoidf.html

[U95] JS：Promise 包装
来源：http://hz.yvedp.cn/gtqkbdsonr.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtmndcksvr.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtpcgaumva.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtyhfawahq.html

[U97] JS：并发请求
来源：http://hz.cheryme.top/gtahkoylzg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtlhqgcoos.html

[U98] JS：fetch 带 JSON
来源：http://hz.xingfuxueyuan.xyz/gteidpgagr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sxryk.cn/gtmlpjujfk.html

[U99] JS：事件监听
来源：http://hz.sufxvd.cn/gtsuowcusp.html

el.addEventListener("click", e => {})
来源：http://hz.cheryme.top/gtmesdezyj.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtkchgwxlj.html

document.querySelector(".item")
来源：http://hz.nanxinkj.top/gtgjomcnjv.html

[U101] JS：classList 操作
来源：http://hz.yueranfly.top/gtyqdrwijw.html

el.classList.toggle("active")
来源：http://hz.snrcjt.cn/gthtgtduuk.html

[U102] JS：本地存储
来源：http://hz.jinqigfzy.top/gtvwfcvvmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.52xcode.cn/gthoyoptmt.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gtytojqgpi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangkeji.top/gtxtibuwcq.html

[U104] JS：防抖
来源：http://hz.ywan-chungtsiang.top/gtsyotrhxo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtxuwsoijj.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtcahtljgp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gtvuexhyds.html

[U106] JS：日期格式化
来源：http://hz.hysaishi.cn/gterstxlea.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj202588.top/gtgykutyhm.html

[U107] JS：数字千分位
来源：http://hz.gaohongyu789.top/gtfyxkfiwm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuanzhike.top/gtnyxhshbi.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtglcmnjzb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.snrcjt.cn/gtzndzguvm.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtzwzvpdit.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gttyybsrhk.html

[U110] JS：数组分块
来源：http://hz.daria6918.cn/gtzxkzijfs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.meibo888.top/gtwxythgff.html

[U111] JS：对象转 Map
来源：http://hz.jqgufenzy.top/gtwocrttau.html

new Map(Object.entries(obj))
来源：http://hz.tian-w.cn/gtcwfkvspe.html

[U112] JS：字符串补位
来源：http://hz.52xcode.cn/gtrnbkctej.html

"7".padStart(3, "0")
来源：http://hz.yonumen.top/gtghtiaihv.html

[U113] JS：正则替换全部
来源：http://hz.fengsongda.top/gtqmkfnrxs.html

s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtdpdyosas.html

[U114] JS：JSON 深比较
来源：http://hz.yuanzhike.top/gtqwnydhnt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtfxzwbnkj.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtsllhbnuf.html

crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtgnqmlymt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtugidghec.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtdtvnllfy.html

[U117] JS：单元测试
来源：http://hz.kuanghao11.cn/gtfmxcezcx.html

npm i -D vitest;  npx vitest
来源：http://hz.ivvv.top/gtvwpixitn.html

[U118] JS：开发服务器
来源：http://hz.zhongyouzk.top/gtvskhzxov.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtjpeyuduy.html

[U119] JS：生产构建
来源：http://hz.shzxlz.cn/gtjjqufesh.html

npx vite build
来源：http://hz.xingfuxueyuan.xyz/gtmohnjpck.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gtzmowhfxv.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtkopnaomi.html

================================================================================
来源：http://hz.zhengqikj.top/gtulkkhnmo.html

统计汇总
来源：http://hz.nanxinkj.top/gtjiozzqpl.html

================================================================================
来源：http://hz.nwbrower.top/gtkuxxpwce.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtavihkriw.html

Python ......... 252
来源：http://hz.xuanzx.com/gtlrulprio.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gtdmgxvepa.html

JavaScript ..... 252
来源：http://hz.quarkkingdee.top/gtkfhoaiec.html

TypeScript ..... 212
来源：http://hz.jinghuilouyu.cn/gtfhqvlumi.html

Java ........... 212
来源：http://hz.gzhubu.top/gtwxjxjlua.html

Go ............. 212
来源：http://hz.yuxming.cn/gtksolyhhf.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gttquuiwoe.html

C# ............. 212
来源：http://hz.jinqigfzy.top/gtvvpwfvoc.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gtyjwsnsen.html

C++ ............ 30
来源：http://hz.hammf.cn/gtsfnrqucq.html

SQL ............ 90
来源：http://hz.wangdashe.top/gtvxstxsgd.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtbxvpexuf.html

Kotlin ......... 15
来源：http://hz.tianlin.xyz/gtdjffgbmn.html

Swift .......... 15
来源：http://hz.yj20258.top/gtpftroaef.html

Lua ............ 10
来源：http://hz.yongpay.top/gtdurkjtse.html

Perl ........... 10
来源：http://hz.yongpay.top/gtlssrtvsv.html

Scala .......... 10
来源：http://hz.mhx1999.top/gtagjspmyp.html

------------------------------------
来源：http://hz.jiagoushi.top/gtmippnrkr.html

合计 ........... 2106 条
来源：http://hz.sysykeji.top/gtwhzkvsqj.html

按章节统计：
来源：http://hz.jinqigufen.top/gtucscciob.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.svipenyu.cn/gtoitmlfqi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtubkdhlnp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ybcxt.top/gtwgpgdqnw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yuanzhike.top/gtspodvpsd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.haohaochexian.top/gtobkmtldj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtdhgkdhwl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtmjjncdoa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtrbtlsupv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtrwdxpybz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gttffcjjgh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtukqncyzh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gthiohriyg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtfighcrbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigfzy.top/gtzftljjyr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.svipenyu.cn/gtczhzwexz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gttjubskpr.html

Q SQL 专题                              90
来源：http://hz.fengsongda.top/gtzdbmbyeh.html

R Bash 专题                             80
来源：http://hz.cucudq.cn/gtmzgeirqp.html

S C / C++ 专题                          60
来源：http://hz.jqgufenzy.top/gtbxewojoo.html

T 其他语言补充                          60
来源：http://hz.nanxinkj.top/gtztlnjcqr.html

U 高频实用片段                         120
来源：http://hz.cdnleiting.top/gtbdmhpoqv.html

------------------------------------
来源：http://hz.wangdashe.top/gtwqriarhq.html

合计                                  2106 条
来源：http://hz.ehwqpu.com/gtplxfjgnu.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtafaotpej.html

使用提醒
来源：http://hz.zhongyouzk.top/gtmxeybglj.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtsjrbczsz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnxiangtu.top/gthevqhvuu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydzc1.top/gtiojlhnxe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.wangdashe.top/gtjgmkersx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.pengpengdd.cyou/gtfieunawm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dianchejie.cn/gtkeglxrki.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtiaxscdep.html

================================================================================
来源：http://hz.birdmap.top/gtqsiairwg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yangfankeji.com/gtdjagqdth.html

Common Programming Examples Cheat Book
来源：http://hz.jqgufenzy.top/gtmxmzofmz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtopqjybav.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gteiofjiwv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hammf.cn/gtkvowbocz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.bjfxy.top/gtlkcihvdj.html

SQL · Bash · C · C++
来源：http://hz.sxryk.cn/gtzcvwznst.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.fzhhl.top/gtuylhzucu.html

【使用说明】
来源：http://hz.jqgfzy.top/gtrkxpvtek.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.fengsongda.top/gtgynjitmb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.0kj1m.cn/gtfbiqppci.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.gzhubu.top/gtikgdrnip.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenjidiqi.icu/gtftrthyep.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.316326.xyz/gtzvppptrf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gaohongyu789.top/gtmfetpurz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenjidiqi.icu/gtuqfhxgnt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.nanxuanxn.top/gthhfraswz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.quarkkingdee.top/gtbhoqdhxj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.0kj1m.cn/gtjshydfpw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigfzy.top/gtiddlhytm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.dashuyun.cn/gtobppmner.html

【文件统计】
来源：http://hz.zycfv.cn/gtgelmlpsh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sufxvd.cn/gtkmhcennr.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtwkzghjet.html

目  录
来源：http://hz.cqqwz.cn/gtnyfvmioi.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gteikiglng.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxinkj.top/gtjlwbqvfk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtnolcgvum.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtzkrihaxz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtcwkoqwuj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jlsjyb.cn/gtsyssxjng.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtapiafwng.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinqigufen.top/gtomuqeofp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gaohongyu789.top/gtyfaygvmh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtaxelvyvn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.aizwys.cn/gtswebkypn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtbvwjefca.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtvsiusosh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtqvembsmr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtwwcgnqeq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ydjk.org.cn/gtbbnoqbxf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtwkcdcjlt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yvedp.cn/gtzjpruqev.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtzulhcyvf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhiwuduotai.top/gtjsnkqkfo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinghuilouyu.cn/gtrlzshvhb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtxhnqpgqb.html

================================================================================
来源：http://hz.jinqigufen.top/gtgtwqwboy.html

A. 基础语法与类型
来源：http://hz.jinqigufen.top/gtjlcdaefw.html

================================================================================
来源：http://hz.dianchejie.cn/gtdrwaxdrv.html

[A01] Hello World
来源：http://hz.cashguo.top/gtfyytwlyg.html

Py:   print("Hello, World!")
来源：http://hz.zhoulong.xyz/gtaxmjxxmb.html

PHP:  echo "Hello, World!";
来源：http://hz.sxryk.cn/gteclsqwxp.html

JS:   console.log("Hello, World!");
来源：http://hz.hnxiangtu.top/gtgwmtqqlu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.daria6918.cn/gtvkktlrxg.html

Java: System.out.println("Hello, World!");
来源：http://hz.c1oappe.top/gtgizkzzfk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinqigfzy.top/gtgymronya.html

Ruby: puts "Hello, World!"
来源：http://hz.xziqi.cn/gthipfored.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.smart0.xyz/gtwwutgkzo.html

[A02] 变量声明与赋值
来源：http://hz.cucudq.cn/gtnaztytph.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhiwuduotai.top/gtrpancbho.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nanxuanxn.top/gtbyyolxax.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gttlilfguy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.316326.xyz/gtvpnxzrdf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtajmtbzcy.html

Go:   name := "Alex"; age := 20
来源：http://hz.ivvv.top/gtgiexjirf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigfzy.top/gtssqfewtj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hywenlv.cn/gtdwjzriex.html

[A03] 常量定义
来源：http://hz.meibo888.top/gtdvekfngr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.c1oappe.top/gtyeyxhhju.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gtjdxzasrt.html

JS:   const PI = 3.14159;
来源：http://hz.jinqigufen.top/gtaoyxrhnp.html

TS:   const PI: number = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtsivsolmx.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtmsdpxtfx.html

Go:   const PI = 3.14159
来源：http://hz.gotoacloud.top/gttexmpqdi.html

Ruby: PI = 3.14159
来源：http://hz.tanke756.top/gticfxelty.html

C#:   const double PI = 3.14159;
来源：http://hz.yonumen.top/gtdokhifob.html

[A04] 判断变量类型
来源：http://hz.yanxiufei.cn/gtjbywzyje.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.cucudq.cn/gtyijtrpwx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yueranfly.top/gtwsapnafh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tanke756.top/gtgelxadiy.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhiwuduotai.top/gtrlghlbpv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.aibaodan.cn/gtjhtlmyep.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shanyushiyangtech.top/gtfyeqfgch.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.chenzaomai.com/gtlxzeyeqf.html

C#:   x.GetType().Name; x is int
来源：http://hz.ppjwa.cn/gtvvenezbt.html

[A05] 整数除法与取模
来源：http://hz.yuxming.cn/gtmngssunz.html


<!-- 参考信息 -->