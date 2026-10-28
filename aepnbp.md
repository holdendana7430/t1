代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.yvedp.cn/gtfwwkdvsk.html

namespace App\Http;
来源：http://hz.ehwqpu.com/gtxhzgyivk.html

[U44] PHP：开启严格类型
来源：http://hz.dashuyun.cn/gtfswlnpup.html

declare(strict_types=1);
来源：http://hz.nanxuanxn.top/gtmombgfad.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtcptenizo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtdepseyeb.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtctanpeyg.html

?string $name = null
来源：http://hz.9152youxi.cn/gtjwgxkmrj.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtvpgtxgzi.html

int|string $id
来源：http://hz.cucudq.cn/gtfpfnnpsq.html

[U48] PHP：纯枚举
来源：http://hz.ivvv.top/gtyhjzrpns.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.snrcjt.cn/gtcirztemv.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtytvstrti.html

public readonly string $name
来源：http://hz.hywenlv.cn/gtpuhrplcw.html

[U50] PHP：构造器属性提升
来源：http://hz.aibaodan.cn/gtvracdvir.html

public function __construct(private int $id) {}
来源：http://hz.yj202588.top/gthkkdvlds.html

[U51] PHP：数组解构
来源：http://hz.shangyingyoupin.top/gtxdhoawar.html

[$a, $b] = $arr;
来源：http://hz.gzhubu.top/gtrcfglndh.html

[U52] PHP：箭头函数
来源：http://hz.yuanzhike.top/gtmfzsaexh.html

$double = fn($x) => $x * 2;
来源：http://hz.yanxiufei.cn/gtlahpdqbc.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtwxlvtsgm.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtvqulmbcf.html

[U54] PHP：空安全调用
来源：http://hz.haohaochexian.top/gtbgigtuqc.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gtrgvzklkj.html

[U55] PHP：match 表达式
来源：http://hz.fzhhl.top/gtexndkhdu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuanzx.com/gtzmeimljb.html

[U56] PHP：命名参数
来源：http://hz.haohaochexian.top/gtqyndugtx.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtbnhoewxp.html

[U57] PHP：字符串插值
来源：http://hz.mhx1999.top/gtczrronjn.html

"值: {$a}"
来源：http://hz.9152youxi.cn/gtewetxzpf.html

[U58] PHP：数组三件套
来源：http://hz.tian-w.cn/gtxknfukhl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gtlcnrcoex.html

[U59] PHP：自定义排序
来源：http://hz.zhixingplan.top/gtfcymgqqh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gtusfprcyl.html

[U60] PHP：JSON 编解码
来源：http://hz.aizwys.cn/gtsaqlqxsu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtklghmaua.html

[U61] PHP：正则
来源：http://hz.pycfn.com/gtlzareurk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtapaotaaa.html

[U62] PHP：日期对象
来源：http://hz.jqgfzy.top/gtdifacehr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ehwqpu.com/gtsuahwtee.html

[U63] PHP：文件读写
来源：http://hz.ydzc1.top/gtjfhiseqa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yanxiufei.cn/gtmehchbae.html

[U64] PHP：目录遍历
来源：http://hz.shuidangran.top/gtzsyoayhd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cashguo.top/gtjxiiiwil.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtplvmhcoa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yonumen.top/gttucrqtin.html

[U66] PHP：设置 Cookie
来源：http://hz.ywan-chungtsiang.top/gtyjzubbqh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tian-w.cn/gtwypcmvqb.html

[U67] PHP：处理文件上传
来源：http://hz.daria6918.cn/gtmvbisztr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinqigfzy.top/gtilfclbgo.html

[U68] PHP：PDO 连接
来源：http://hz.yongpay.top/gtmbxonmdd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cheryme.top/gtbcsdneqj.html

[U69] PHP：PDO 预处理
来源：http://hz.xuanzx.com/gtbnkfupxr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.9152youxi.cn/gtsuiojxni.html

[U70] PHP：PDO 事务
来源：http://hz.chenjidiqi.icu/gtigpvgsyp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ivvv.top/gtdlwvvrrf.html

[U71] PHP：抛出异常
来源：http://hz.andypj.xyz/gtwhmcccfh.html

throw new RuntimeException("失败", 500);
来源：http://hz.shuidangran.top/gtgxavwygz.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gtgtzhqymk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtqvrtgvci.html

[U73] PHP：读取 ini 配置
来源：http://hz.jqgufenzy.top/gtxhcqzmka.html

parse_ini_file("config.ini", true)
来源：http://hz.ydjk.org.cn/gtqzorropk.html

[U74] PHP：读取环境变量
来源：http://hz.shuidangran.top/gtlnnapyep.html

getenv("APP_ENV") ?: "production"
来源：http://hz.kuanghao11.cn/gtqcpqwmde.html

[U75] PHP：依赖注入
来源：http://hz.hfpthk.cn/gtxsrbrykg.html

composer require psr/container
来源：http://hz.jqgfzy.top/gtmeespngd.html

[U76] PHP：简单路由
来源：http://hz.fengsongda.top/gtzjsmerdt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cashguo.top/gtdjpoejhc.html

[U77] PHP：模板渲染
来源：http://hz.xinyue.icu/gtssfqjiak.html

composer require twig/twig
来源：http://hz.tanke756.top/gtghutibaj.html

[U78] PHP：单元测试
来源：http://hz.xuetiantiany.cn/gtgyptsomz.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gtonvjpszb.html

[U79] PHP：静态分析
来源：http://hz.jinghuilouyu.cn/gtystolrhs.html

composer require --dev phpstan/phpstan
来源：http://hz.hnxiangtu.top/gtvqrzerrm.html

[U80] PHP：代码规范修复
来源：http://hz.dashuyun.cn/gtcyrtknxh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.redwolf501.top/gttddokygg.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gtahjhkuoe.html

npm init -y;  npm i express
来源：http://hz.tianlin.xyz/gtavxurpui.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtdhnecryr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cashguo.top/gtyqwumkjo.html

[U83] JS：ES Module 导入导出
来源：http://hz.cheryme.top/gtnelparfk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.birdmap.top/gtsqijgkyc.html

[U84] JS：CommonJS 写法
来源：http://hz.wangshuangyany.cn/gtmnuzkpcl.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj202588.top/gtmavkarov.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtbaqonsbt.html

a?.b?.c
来源：http://hz.zhongyouzk.top/gtvcwmunwk.html

[U86] JS：空值合并
来源：http://hz.wangshuangyany.cn/gtlqlhezqm.html

a ?? b
来源：http://hz.yueranfly.top/gtjigxjefx.html

[U87] JS：解构默认值
来源：http://hz.yuanzhike.top/gtfggmcrgm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fzhhl.top/gtvypcyeqv.html

[U88] JS：对象展开合并
来源：http://hz.jinyuanbaomall.cn/gtfjxiykac.html

{ ...a, ...b }
来源：http://hz.yj202588.top/gtwckwlqyx.html

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtlzfuyebq.html

[...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtbcqxgauf.html

[U90] JS：数字数组排序
来源：http://hz.daxiang520.top/gtttgdxvrq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtjsjphvgt.html

[U91] JS：对象键值遍历
来源：http://hz.tian-w.cn/gtdnitunpp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenzaomai.com/gttyigvjsd.html

[U92] JS：深拷贝
来源：http://hz.316326.xyz/gtvtsixjns.html

structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtvosntrid.html

[U93] JS：模板字符串
来源：http://hz.pengpengdd.cyou/gthaqucvns.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtpdkkhhux.html

[U94] JS：箭头函数
来源：http://hz.jinyuanbaomall.cn/gtsfkpzhqb.html

const double = x => x * 2;
来源：http://hz.ywan-chungtsiang.top/gtnarrszsw.html

[U95] JS：Promise 包装
来源：http://hz.redwolf501.top/gtwkhtkqzv.html

new Promise((resolve, reject) => {})
来源：http://hz.sweek.top/gtefdvrmaq.html

[U96] JS：async/await 与异常
来源：http://hz.zhengqikj.top/gtiguzrous.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtenxprqek.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtilvhbnnb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtiwvzhoha.html

[U98] JS：fetch 带 JSON
来源：http://hz.jlsjyb.cn/gtybhbtwot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jiagoushi.top/gtjnuwagaz.html

[U99] JS：事件监听
来源：http://hz.yueranfly.top/gtxkdjjpmh.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gthydlyfjh.html

[U100] JS：DOM 查询
来源：http://hz.yonumen.top/gtpkhvjgsc.html

document.querySelector(".item")
来源：http://hz.316326.xyz/gtwybolequ.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gttprwmmkz.html

el.classList.toggle("active")
来源：http://hz.daria6918.cn/gtjevcecxs.html

[U102] JS：本地存储
来源：http://hz.tanke756.top/gtzbnykjiw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhixingplan.top/gtwkltxhce.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtiywvagrd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.snrcjt.cn/gtncyytyxf.html

[U104] JS：防抖
来源：http://hz.hywenlv.cn/gtovjotkui.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtxaxysxbn.html

[U105] JS：节流
来源：http://hz.ydzc1.top/gtdioyyrix.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gtwwgatnxa.html

[U106] JS：日期格式化
来源：http://hz.yuxming.cn/gtsicbrycx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jiagoushi.top/gtosqmlqbm.html

[U107] JS：数字千分位
来源：http://hz.fengsongda.top/gtmklwagrr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jiagoushi.top/gttrixpbfk.html

[U108] JS：随机整数
来源：http://hz.shangyingyoupin.top/gtuefsdmds.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.meibo888.top/gtphdkdnik.html

[U109] JS：数组分组
来源：http://hz.nanxuanxn.top/gtpiamhppr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gtnyguehzl.html

[U110] JS：数组分块
来源：http://hz.jinqigufen.top/gtsvahqhrx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hywenlv.cn/gtqbduxfny.html

[U111] JS：对象转 Map
来源：http://hz.fzhhl.top/gtzdjydzrs.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtwbljdzmc.html

[U112] JS：字符串补位
来源：http://hz.daria6918.cn/gticqvwhsh.html

"7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtqlwqptey.html

[U113] JS：正则替换全部
来源：http://hz.cucudq.cn/gtyswyurvv.html

s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtpembubyz.html

[U114] JS：JSON 深比较
来源：http://hz.smart0.xyz/gtehivnzag.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtzdvtmlrz.html

[U115] JS：生成 UUID
来源：http://hz.guowangkeji.top/gtrywjoaoj.html

crypto.randomUUID()
来源：http://hz.yongpay.top/gtwwrxbwkw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ydjk.org.cn/gtbkjjmvxt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydzc1.top/gtetafkxew.html

[U117] JS：单元测试
来源：http://hz.zhaomingkeji.xyz/gtqouuzotq.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gtmsuvykwx.html

[U118] JS：开发服务器
来源：http://hz.shzxlz.cn/gtpbclpcjr.html

npm i -D vite;  npx vite
来源：http://hz.svipenyu.cn/gtotwudpkj.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtxszccbst.html

npx vite build
来源：http://hz.fzhhl.top/gthndctndx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zdqjudy.top/gttoynqhmh.html

import.meta.env.VITE_API_URL
来源：http://hz.aibaodan.cn/gtazutfbpi.html

================================================================================
来源：http://hz.iojbl.cn/gtrtmvpmsc.html

统计汇总
来源：http://hz.shanyushiyangtech.top/gtoknjvnyh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjorengew.html

按语言统计（条）：
来源：http://hz.shuidangran.top/gtxymeucbe.html

Python ......... 252
来源：http://hz.gzhubu.top/gtrygkoczk.html

PHP ............ 252
来源：http://hz.gaohongyu789.top/gttuufdbdu.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtmbtnkqwx.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gthjcqxyfp.html

Java ........... 212
来源：http://hz.nanxinkj.top/gtuzcjelpd.html

Go ............. 212
来源：http://hz.iojbl.cn/gtydgmtapn.html

Ruby ........... 212
来源：http://hz.tian-w.cn/gtnarbnftu.html

C# ............. 212
来源：http://hz.kuanghao11.cn/gtukihnfhw.html

C .............. 30
来源：http://hz.feifeiyinyue.top/gtogxduxmg.html

C++ ............ 30
来源：http://hz.c1oappe.top/gtmbcqfgiv.html

SQL ............ 90
来源：http://hz.wangdashe.top/gtxtjtixxm.html

Bash ........... 80
来源：http://hz.kuanghao11.cn/gtfasaxlod.html

Kotlin ......... 15
来源：http://hz.tianlin.xyz/gtmpteiuly.html

Swift .......... 15
来源：http://hz.yangfankeji.com/gtdhqookcw.html

Lua ............ 10
来源：http://hz.yongpay.top/gtsurgokuv.html

Perl ........... 10
来源：http://hz.shzxlz.cn/gtuykiygtw.html

Scala .......... 10
来源：http://hz.jqgufenzy.top/gtqmsncmin.html

------------------------------------
来源：http://hz.aizwys.cn/gtwzvsmkhl.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtxalqbuah.html

按章节统计：
来源：http://hz.9152youxi.cn/gtwpoujirk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gtofxfxsir.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtcsrtiloo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtzfonbrmq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.svipenyu.cn/gtdzupevms.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.daxiang520.top/gtylwdooyh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtstduwryb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtknyemwzg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtcubyltkl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtjydblkxc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtmknehdyr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtaelanfyl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtnwofccty.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtvnjbtvsr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gttglvdjfs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cdnleiting.top/gtjqvnooay.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtbusltdhs.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtyasjjeij.html

R Bash 专题                             80
来源：http://hz.hongshengwenyu.top/gtjuievgey.html

S C / C++ 专题                          60
来源：http://hz.yongpay.top/gtprumjomv.html

T 其他语言补充                          60
来源：http://hz.nwbrower.top/gtipwmgwab.html

U 高频实用片段                         120
来源：http://hz.jlsjyb.cn/gtknghsutl.html

------------------------------------
来源：http://hz.hfpthk.cn/gtuygokdwr.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtkugztwei.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gttfzloeta.html

使用提醒
来源：http://hz.xingfuxueyuan.xyz/gtgkxqqxhm.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtqnvrlhzm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtoxddjmms.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jyoumei.cn/gtqejpgkkr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.pengpengdd.cyou/gtggynqowe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhiwuduotai.top/gtwfvzpxbo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jiagoushi.top/gtgtqifhja.html

—— 文件结束 ——
来源：http://hz.iojbl.cn/gtxbzuaplf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmakiluvw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gotoacloud.top/gtzjzueywe.html

Common Programming Examples Cheat Book
来源：http://hz.iojbl.cn/gtkxysxorr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwsiprwnk.html

【收录内容】
来源：http://hz.dashuyun.cn/gtnkxnzqxi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.svipenyu.cn/gtgnuhupap.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.wangdashe.top/gtlxjvycvf.html

SQL · Bash · C · C++
来源：http://hz.yj202588.top/gtmslpjsdu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nwbrower.top/gtmdydoeux.html

【使用说明】
来源：http://hz.meibo888.top/gtqdbivtmz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daxiang520.top/gtnarydblc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jiagoushi.top/gtzgvcxtvs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.iojbl.cn/gtrihkjvwx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.redwolf501.top/gtzazhvuvi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cdnleiting.top/gtvnajczfy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cashguo.top/gtkrkkzmza.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenzaomai.com/gttsolayyn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ppjwa.cn/gtsigqhqcp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xuetiantiany.cn/gtvbncrgew.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gzhubu.top/gtqotkacpe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtytknqupg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtmtwyzfcw.html

【文件统计】
来源：http://hz.gzhubu.top/gttgqkmqsl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtkyotewtm.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtqpufamhr.html

目  录
来源：http://hz.yj202588.top/gttjtxokhp.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtpdahmbnn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gttyszftqf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cdnleiting.top/gtflblkfox.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gtisiolyer.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gtigksbvar.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.mhx1999.top/gtpngqildp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cdnleiting.top/gtecpdoocp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtalevbjtv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtustetxif.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtstvytjcr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.guowangkeji.top/gtuownlrqy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtdlfdykrf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gttxpcukwm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtglvcioya.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gteukfiggo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aizwys.cn/gtdyasioit.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtebsdjzit.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yanxiufei.cn/gtcbimrlki.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangkeji.top/gtcjmrjpck.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shuidangran.top/gtaednoitt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtokgkpece.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtrspgmvgx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtciyjhakq.html

A. 基础语法与类型
来源：http://hz.jinqigufen.top/gtmkxxcqun.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtljrawztg.html

[A01] Hello World
来源：http://hz.shanyushiyangkeji.top/gtgljwkwhp.html

Py:   print("Hello, World!")
来源：http://hz.ehwqpu.com/gtpikdjhhp.html

PHP:  echo "Hello, World!";
来源：http://hz.yj20258.top/gtismmbhyv.html

JS:   console.log("Hello, World!");
来源：http://hz.haohaochexian.top/gtwbwdmmwm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ehwqpu.com/gtgotfhnxp.html

Java: System.out.println("Hello, World!");
来源：http://hz.jyoumei.cn/gtzpiigaxe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hnqzz.top/gtfqkgxolj.html

Ruby: puts "Hello, World!"
来源：http://hz.wangdashe.top/gtgbbnhfnu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.fzhhl.top/gtjubsfexe.html

[A02] 变量声明与赋值
来源：http://hz.birdmap.top/gtvurwxutv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.daxiang520.top/gtcspiaagk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yongpay.top/gtimcpxmui.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtluifaztm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.redwolf501.top/gtfjuehwhp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtgjcrjnqs.html

Go:   name := "Alex"; age := 20
来源：http://hz.jiagoushi.top/gtbyroqcdi.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daxiang520.top/gtfosiyguw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtckqysbgu.html

[A03] 常量定义
来源：http://hz.daxiang520.top/gtskkiilad.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinqigufen.top/gtmdomidgq.html

PHP:  const PI = 3.14159;
来源：http://hz.c1oappe.top/gthfemtiih.html

JS:   const PI = 3.14159;
来源：http://hz.aizwys.cn/gtnpihuczb.html

TS:   const PI: number = 3.14159;
来源：http://hz.xuetiantiany.cn/gtiwmnxmlw.html

Java: static final double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtwzhmipek.html

Go:   const PI = 3.14159
来源：http://hz.fengsongda.top/gtoijlkogq.html

Ruby: PI = 3.14159
来源：http://hz.dashuyun.cn/gtcfzaarnr.html

C#:   const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtztdjfiiy.html

[A04] 判断变量类型
来源：http://hz.zhaomingkeji.xyz/gtozhpliwi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ybcxt.top/gttqvpzdcm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xingfuxueyuan.xyz/gtujtqlumk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aizwys.cn/gtkkhernlb.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangdashe.top/gthgzdxwfs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jqgfzy.top/gtewmwanol.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhixingplan.top/gtrmlfwbav.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gzhubu.top/gtykzptwyq.html

C#:   x.GetType().Name; x is int
来源：http://hz.sweek.top/gtwmeewbic.html

[A05] 整数除法与取模
来源：http://hz.nanxinkj.top/gtpeimnwrd.html


<!-- 参考信息 -->