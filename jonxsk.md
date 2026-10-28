代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtcsdagnxx.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtgezkdera.html

[U44] PHP：开启严格类型
来源：http://hz.vqdsnc.cn/gtvknbwoao.html

declare(strict_types=1);
来源：http://hz.xylfe.cn/gtunlluqrh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ivvv.top/gtluwlgnts.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtyeldbhva.html

[U46] PHP：可空类型
来源：http://hz.c1oappe.top/gttvdnynuz.html

?string $name = null
来源：http://hz.snrcjt.cn/gteqhyvbmx.html

[U47] PHP：联合类型
来源：http://hz.ywan-chungtsiang.top/gtrjpgfmpw.html

int|string $id
来源：http://hz.hongshengwenyu.top/gtfiqoghxz.html

[U48] PHP：纯枚举
来源：http://hz.gogol.net.cn/gtzoqvecmn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gthcpnnzdf.html

[U49] PHP：只读属性
来源：http://hz.redwolf501.top/gtkzjeahem.html

public readonly string $name
来源：http://hz.vqdsnc.cn/gtuqjbijdu.html

[U50] PHP：构造器属性提升
来源：http://hz.birdmap.top/gtmumqpgty.html

public function __construct(private int $id) {}
来源：http://hz.guannengcc.top/gtaisxzrbs.html

[U51] PHP：数组解构
来源：http://hz.zycfv.cn/gtmowszdot.html

[$a, $b] = $arr;
来源：http://hz.shanyushiyangtech.top/gtynzpaide.html

[U52] PHP：箭头函数
来源：http://hz.daxiang520.top/gtqneqbeqn.html

$double = fn($x) => $x * 2;
来源：http://hz.guannengcc.top/gtdhogzygm.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gterixfkbu.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigfzy.top/gtmzvzzuqz.html

[U54] PHP：空安全调用
来源：http://hz.xingfuxueyuan.xyz/gtfwuttchm.html

$obj?->method()
来源：http://hz.chenzaomai.com/gtndawxihr.html

[U55] PHP：match 表达式
来源：http://hz.mhx1999.top/gtitxlilfw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhongyouzk.top/gtywtsjjzf.html

[U56] PHP：命名参数
来源：http://hz.zdqjudy.top/gtqgdkhkbt.html

f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtbzbhinys.html

[U57] PHP：字符串插值
来源：http://hz.hammf.cn/gtaojpntae.html

"值: {$a}"
来源：http://hz.zhijiandao.cn/gtzcsvjmqi.html

[U58] PHP：数组三件套
来源：http://hz.cdnleiting.top/gtipbfucdg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenjidiqi.icu/gtrenjvdnq.html

[U59] PHP：自定义排序
来源：http://hz.sysykeji.top/gteelnxonv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtawhpfsfo.html

[U60] PHP：JSON 编解码
来源：http://hz.yueranfly.top/gtxksupxcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.svipenyu.cn/gthgnvbrju.html

[U61] PHP：正则
来源：http://hz.pycfn.com/gtjdhnhsfa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gthtannchw.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gtqevwdpgb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtnpmhugyv.html

[U63] PHP：文件读写
来源：http://hz.birdmap.top/gtiqithjhs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gaohongyu789.top/gtiegimnut.html

[U64] PHP：目录遍历
来源：http://hz.shuidangran.top/gtdmnwjrtm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gtswooupvy.html

[U65] PHP：会话
来源：http://hz.daria6918.cn/gtzdbarmnc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yongpay.top/gtltexvjxz.html

[U66] PHP：设置 Cookie
来源：http://hz.shzxlz.cn/gtglhkmwqz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.haohaochexian.top/gtyodavwpg.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtaogectsn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guannengcc.top/gtiogshbdt.html

[U68] PHP：PDO 连接
来源：http://hz.hongshengwenyu.top/gtdarnllok.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sweek.top/gthshypafw.html

[U69] PHP：PDO 预处理
来源：http://hz.snrcjt.cn/gtztgxqsae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.9152youxi.cn/gtekrjsuui.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtfmfruyxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.mhx1999.top/gtdimiyywe.html

[U71] PHP：抛出异常
来源：http://hz.ehwqpu.com/gtpyvgzlnr.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhengqikj.top/gtlfozkwue.html

[U72] PHP：写错误日志
来源：http://hz.guannengcc.top/gttaritkre.html

error_log("失败: " . $e->getMessage());
来源：http://hz.svipenyu.cn/gtmffyhpya.html

[U73] PHP：读取 ini 配置
来源：http://hz.yj20258.top/gtswchumpn.html

parse_ini_file("config.ini", true)
来源：http://hz.cashguo.top/gtxuvhzgxv.html

[U74] PHP：读取环境变量
来源：http://hz.zhoulong.xyz/gtzoahfhxi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangkeji.top/gtzgnufuvb.html

[U75] PHP：依赖注入
来源：http://hz.yangfankeji.com/gtculobysv.html

composer require psr/container
来源：http://hz.cqqwz.cn/gthyuggtlm.html

[U76] PHP：简单路由
来源：http://hz.hnxiangtu.top/gthzfzhwvm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ydzc1.top/gtuvhtbxzo.html

[U77] PHP：模板渲染
来源：http://hz.zhaomingkeji.xyz/gtutqopltu.html

composer require twig/twig
来源：http://hz.yangfankeji.com/gtsncunpfh.html

[U78] PHP：单元测试
来源：http://hz.xinyue.icu/gtgdfqxcgx.html

composer require --dev phpunit/phpunit
来源：http://hz.jlsjyb.cn/gtzwlonqxr.html

[U79] PHP：静态分析
来源：http://hz.shangyingyoupin.top/gtglgwqxvm.html

composer require --dev phpstan/phpstan
来源：http://hz.hongshengwenyu.top/gtgqhicqyc.html

[U80] PHP：代码规范修复
来源：http://hz.sweek.top/gtjamtwsru.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenzaomai.com/gtwzfckmco.html

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gttzysfwxt.html

npm init -y;  npm i express
来源：http://hz.xingfuxueyuan.xyz/gtnmvqtbqy.html

[U82] JS：package.json 脚本
来源：http://hz.sufxvd.cn/gtntfjjxyk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.aibaodan.cn/gtdmbuqvya.html

[U83] JS：ES Module 导入导出
来源：http://hz.ivvv.top/gtistmvlbc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhengqikj.top/gtlxogspkd.html

[U84] JS：CommonJS 写法
来源：http://hz.nanxinkj.top/gtvtstttqa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jyoumei.cn/gtmzohdhcb.html

[U85] JS：可选链
来源：http://hz.andypj.xyz/gtnvlmzqzj.html

a?.b?.c
来源：http://hz.jiagoushi.top/gtwebkyuff.html

[U86] JS：空值合并
来源：http://hz.hongshengwenyu.top/gthnmwyzqq.html

a ?? b
来源：http://hz.sufxvd.cn/gtisthkkel.html

[U87] JS：解构默认值
来源：http://hz.xylfe.cn/gttwvovutq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuanzx.com/gtctdstjqd.html

[U88] JS：对象展开合并
来源：http://hz.cashguo.top/gtnfdxrxcd.html

{ ...a, ...b }
来源：http://hz.jqgfzy.top/gthcdotfyv.html

[U89] JS：数组去重
来源：http://hz.cqqwz.cn/gtfdjgwjhz.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtmvchpwve.html

[U90] JS：数字数组排序
来源：http://hz.hywenlv.cn/gtijdliggx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtowbmpufj.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtkoeiyxim.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gzhubu.top/gtllmblczu.html

[U92] JS：深拷贝
来源：http://hz.hongshengwenyu.top/gtsixayehl.html

structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvqlutntc.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangkeji.top/gtcuprjqvz.html

`共 ${n} 条`
来源：http://hz.wangdashe.top/gtgbepqxkw.html

[U94] JS：箭头函数
来源：http://hz.jqgufenzy.top/gtntrdnotf.html

const double = x => x * 2;
来源：http://hz.mhx1999.top/gtsfragslk.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gttcgaqwvf.html

new Promise((resolve, reject) => {})
来源：http://hz.ivvv.top/gtnhxhigoo.html

[U96] JS：async/await 与异常
来源：http://hz.sufxvd.cn/gtwhlamoef.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtbyqkzbfv.html

[U97] JS：并发请求
来源：http://hz.jianghu66.top/gtbnzkcgxp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtvgbaxjnp.html

[U98] JS：fetch 带 JSON
来源：http://hz.daria6918.cn/gtsitiwqjt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.andypj.xyz/gtiywbgqyn.html

[U99] JS：事件监听
来源：http://hz.ehwqpu.com/gtxtpylgxd.html

el.addEventListener("click", e => {})
来源：http://hz.gogol.net.cn/gteqisggco.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtfhsrciip.html

document.querySelector(".item")
来源：http://hz.yangfankeji.com/gtzfiwdlgy.html

[U101] JS：classList 操作
来源：http://hz.gaohongyu789.top/gtxuzogscw.html

el.classList.toggle("active")
来源：http://hz.cashguo.top/gtyxnhvhln.html

[U102] JS：本地存储
来源：http://hz.jinqigfzy.top/gtharlkznf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhiwuduotai.top/gtxmzehslg.html

[U103] JS：定时器
来源：http://hz.52xcode.cn/gtmvebckrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ydjk.org.cn/gttxufqaws.html

[U104] JS：防抖
来源：http://hz.ivvv.top/gtrgknwcul.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtjfgkcxtc.html

[U105] JS：节流
来源：http://hz.ehwqpu.com/gthdeshxrw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yvedp.cn/gtyllhlabw.html

[U106] JS：日期格式化
来源：http://hz.wangdashe.top/gtubzeomhh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangshuangyany.cn/gtmbbfncuq.html

[U107] JS：数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtgwuhecqk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zdqjudy.top/gtvzdmzusq.html

[U108] JS：随机整数
来源：http://hz.zhixingplan.top/gtfrbfgnbj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.daria6918.cn/gtjksimwbo.html

[U109] JS：数组分组
来源：http://hz.kuanghao11.cn/gtwfwdtotc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtwpoyecjg.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtfnacspbu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gttbzgnqby.html

[U111] JS：对象转 Map
来源：http://hz.jinqigufen.top/gtbnpqlilo.html

new Map(Object.entries(obj))
来源：http://hz.fzhhl.top/gtfmlyopbn.html

[U112] JS：字符串补位
来源：http://hz.jinqigfzy.top/gtxnytekmx.html

"7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gteditgtaq.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gtmxbeidlc.html

s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtanalphll.html

[U114] JS：JSON 深比较
来源：http://hz.shanyushiyangkeji.top/gtgxysxtfl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtdaxsvvjm.html

[U115] JS：生成 UUID
来源：http://hz.gaohongyu789.top/gtwreqihel.html

crypto.randomUUID()
来源：http://hz.cheryme.top/gtqecffnfi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtkwetgoth.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtuqzlwqpj.html

[U117] JS：单元测试
来源：http://hz.dashuyun.cn/gtlxrourgc.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtlfgtpvnv.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtswmwzyqo.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gtbfzpilyb.html

[U119] JS：生产构建
来源：http://hz.zhiwuduotai.top/gtqgzifsvh.html

npx vite build
来源：http://hz.nanxinkj.top/gtejfhpbvx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ehwqpu.com/gtygauvfmv.html

import.meta.env.VITE_API_URL
来源：http://hz.feifeiyinyue.top/gttzfbzlqz.html

================================================================================
来源：http://hz.fzhhl.top/gtdagrcqwt.html

统计汇总
来源：http://hz.jinyuanbaomall.cn/gttavvrmjz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbkoyizfu.html

按语言统计（条）：
来源：http://hz.yangfankeji.com/gtrhhatdnd.html

Python ......... 252
来源：http://hz.hnxiangtu.top/gtlzswmwsy.html

PHP ............ 252
来源：http://hz.shuidangran.top/gtebxnwjpx.html

JavaScript ..... 252
来源：http://hz.0kj1m.cn/gtdddqrrbz.html

TypeScript ..... 212
来源：http://hz.gaohongyu789.top/gthrzthauk.html

Java ........... 212
来源：http://hz.zhaomingkeji.xyz/gtuytktxvv.html

Go ............. 212
来源：http://hz.gaohongyu789.top/gtglnyjecc.html

Ruby ........... 212
来源：http://hz.zhongyouzk.top/gtxhjhwbab.html

C# ............. 212
来源：http://hz.guannengcc.top/gttgvlfzvj.html

C .............. 30
来源：http://hz.gzhubu.top/gtyifshjlx.html

C++ ............ 30
来源：http://hz.zhoulong.xyz/gtzpuyjdnq.html

SQL ............ 90
来源：http://hz.daria6918.cn/gtoxqktkse.html

Bash ........... 80
来源：http://hz.316326.xyz/gtdzrryfzr.html

Kotlin ......... 15
来源：http://hz.feifeiyinyue.top/gtxqhpadye.html

Swift .......... 15
来源：http://hz.zdqjudy.top/gtpntekcdn.html

Lua ............ 10
来源：http://hz.jqgufenzy.top/gttefidavw.html

Perl ........... 10
来源：http://hz.sxryk.cn/gtlbvzeviq.html

Scala .......... 10
来源：http://hz.zhoulong.xyz/gtqdzadxzd.html

------------------------------------
来源：http://hz.iojbl.cn/gtzdokckbd.html

合计 ........... 2106 条
来源：http://hz.xingfuxueyuan.xyz/gtkhoitlql.html

按章节统计：
来源：http://hz.zdqjudy.top/gtqtptqewf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtflnycxhd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtvbzunwjv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtwdvbszar.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtfuzekhnx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shzxlz.cn/gtfaakbtis.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gtjzvxokva.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtdetqpkbx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtqvimkutc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gttwdyiybo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtbisxopou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtsdtgbiyj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtucscdrvr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtqemgcjpj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtztyuzjyj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ywan-chungtsiang.top/gtbuaatbpq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtrohuysdy.html

Q SQL 专题                              90
来源：http://hz.hongshengwenyu.top/gtdyrhazes.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtpajomvva.html

S C / C++ 专题                          60
来源：http://hz.ydjk.org.cn/gtlvowhfvb.html

T 其他语言补充                          60
来源：http://hz.0kj1m.cn/gttbctbtoz.html

U 高频实用片段                         120
来源：http://hz.daria6918.cn/gtsjonhovs.html

------------------------------------
来源：http://hz.wangdashe.top/gtxrcxotlr.html

合计                                  2106 条
来源：http://hz.xylfe.cn/gtfweqmdeb.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtdtaxltjv.html

使用提醒
来源：http://hz.cheryme.top/gtufydvure.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtrqpqykiu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinyuanbaomall.cn/gtlcpzmzyi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhongyouzk.top/gtwrrwugiz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.guannengcc.top/gtdicwmccb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhoulong.xyz/gtcyelqtaq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhengqikj.top/gthdihpdud.html

—— 文件结束 ——
来源：http://hz.ppjwa.cn/gtrokoliss.html

================================================================================
来源：http://hz.hfpthk.cn/gtkxwesabl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zycfv.cn/gtndmwfvqd.html

Common Programming Examples Cheat Book
来源：http://hz.nanxuanxn.top/gtzrvdgbnl.html

================================================================================
来源：http://hz.ybcxt.top/gtrcljhsth.html

【收录内容】
来源：http://hz.ehwqpu.com/gtdpcwjjsf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtdrrawfak.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yangfankeji.com/gtaxqjplyc.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gttpcdikuf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sysykeji.top/gtuywtlrdr.html

【使用说明】
来源：http://hz.ybcxt.top/gtskzsrcgt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ehwqpu.com/gtegorzuej.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.52xcode.cn/gtibxrgwgg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sufxvd.cn/gtpkmqhypi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hongshengwenyu.top/gtfambllut.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.daria6918.cn/gthyselwec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zycfv.cn/gtfthpdvzj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gtoaadtgcx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cheryme.top/gtigzsgcxi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.dashuyun.cn/gtiadicwbt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj20258888.top/gtsncmuyuc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.tian-w.cn/gtsmsrfxdn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shanyushiyangkeji.top/gtcycejybm.html

【文件统计】
来源：http://hz.sufxvd.cn/gtauyrhgai.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hnqzz.top/gtmjwoqgio.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtlhbwnsgk.html

目  录
来源：http://hz.guannengcc.top/gtvhkzijga.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtywwduqyk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgfzy.top/gtamgmscbg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtqfqvpmws.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtvrdgsfrh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinghuilouyu.cn/gtryaxjsvx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yueranfly.top/gtphwatuoi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gtlkuewryx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhoulong.xyz/gtrrupcnzg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtspiscojq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtinnrusvd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zycfv.cn/gtlllzpazr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtorjbuzkz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gthqbsxzgq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtyizylvxc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ywan-chungtsiang.top/gthoizqrrt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.smart0.xyz/gtepvnxrkq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtmuqmkbgs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhaomingkeji.xyz/gtghorxxbp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.wangshuangyany.cn/gtfgmirorb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtslkjkrqe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtsazxwcnr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtgeoktnkv.html

================================================================================
来源：http://hz.hfpthk.cn/gtmzgeyrxh.html

A. 基础语法与类型
来源：http://hz.birdmap.top/gtnxnbeofr.html

================================================================================
来源：http://hz.daxiang520.top/gtxwwbuzfw.html

[A01] Hello World
来源：http://hz.tanke756.top/gtrmbbibqu.html

Py:   print("Hello, World!")
来源：http://hz.9152youxi.cn/gtfbpijjrx.html

PHP:  echo "Hello, World!";
来源：http://hz.yj202588.top/gtkuwftbll.html

JS:   console.log("Hello, World!");
来源：http://hz.zycfv.cn/gtfxebzagj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gogol.net.cn/gtwrzebdbl.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgufenzy.top/gtxtautsph.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydzc1.top/gtwwewnziz.html

Ruby: puts "Hello, World!"
来源：http://hz.sufxvd.cn/gtbslafgjl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.smart0.xyz/gtgfkjcxtw.html

[A02] 变量声明与赋值
来源：http://hz.zhijiandao.cn/gtkwfivjnx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhiwuduotai.top/gtghsogvty.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zdqjudy.top/gtslinkmtx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shangyingyoupin.top/gtowypcyvr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hysaishi.cn/gtjoyohxia.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hywenlv.cn/gtanjhrsjj.html

Go:   name := "Alex"; age := 20
来源：http://hz.sxryk.cn/gtbkuaikux.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yangfankeji.com/gtgyjwaphv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sweek.top/gtdwcgdzkj.html

[A03] 常量定义
来源：http://hz.dianchejie.cn/gtmmhyjrvd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenzaomai.com/gtdkhnmzgv.html

PHP:  const PI = 3.14159;
来源：http://hz.yanxiufei.cn/gthchxmoof.html

JS:   const PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtzhtxubcr.html

TS:   const PI: number = 3.14159;
来源：http://hz.yanxiufei.cn/gtwrqrjcna.html

Java: static final double PI = 3.14159;
来源：http://hz.aizwys.cn/gtsqbdruvc.html

Go:   const PI = 3.14159
来源：http://hz.yvedp.cn/gtrpednixx.html

Ruby: PI = 3.14159
来源：http://hz.mhx1999.top/gtqrhzmuue.html

C#:   const double PI = 3.14159;
来源：http://hz.316326.xyz/gtgjstdtqq.html

[A04] 判断变量类型
来源：http://hz.snrcjt.cn/gtqyxqdyue.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gzhubu.top/gtkerasvic.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigufen.top/gtgowmlvjp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.dianchejie.cn/gtmfmpckfn.html

TS:   typeof x; x instanceof Date
来源：http://hz.zycfv.cn/gtceynyoyh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xuanzx.com/gtudiyfjgx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinyuanbaomall.cn/gtlsjymogf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sysykeji.top/gtkqmuxceo.html

C#:   x.GetType().Name; x is int
来源：http://hz.ybcxt.top/gtfyibqnoo.html

[A05] 整数除法与取模
来源：http://hz.jinqigufen.top/gtchtkdcav.html


<!-- 参考信息 -->