代发 wailian999

[U47] PHP：联合类型
来源：http://hz.yj20258888.top/gtlwpfiokd.html

int|string $id
来源：http://hz.gaohongyu789.top/gtsnaftmcb.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gtihpzmtxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuanzx.com/gtmwrxdoxj.html

[U49] PHP：只读属性
来源：http://hz.zhongyouzk.top/gtbnxdzlqg.html

public readonly string $name
来源：http://hz.xingfuxueyuan.xyz/gtcfjgtrzo.html

[U50] PHP：构造器属性提升
来源：http://hz.gzhubu.top/gtuqbvxxpp.html

public function __construct(private int $id) {}
来源：http://hz.sxryk.cn/gtxxvoevgj.html

[U51] PHP：数组解构
来源：http://hz.jqgfzy.top/gtwxlgicuz.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtiekacenn.html

[U52] PHP：箭头函数
来源：http://hz.dianchejie.cn/gthtncqgmj.html

$double = fn($x) => $x * 2;
来源：http://hz.yuanzhike.top/gtdnoefuuq.html

[U53] PHP：空合并运算符
来源：http://hz.ydjk.org.cn/gtrbirhioq.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuanzhike.top/gtlnzxomlt.html

[U54] PHP：空安全调用
来源：http://hz.jinyuanbaomall.cn/gtdngliang.html

$obj?->method()
来源：http://hz.guowangkeji.top/gtgubdwjzl.html

[U55] PHP：match 表达式
来源：http://hz.yueranfly.top/gthrloblsy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangdashe.top/gttbivmmet.html

[U56] PHP：命名参数
来源：http://hz.aizwys.cn/gtwitlqocr.html

f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtgprtfntk.html

[U57] PHP：字符串插值
来源：http://hz.zhiwuduotai.top/gtajpnfgdx.html

"值: {$a}"
来源：http://hz.zhaomingkeji.xyz/gtkjweqpnf.html

[U58] PHP：数组三件套
来源：http://hz.svipenyu.cn/gtetnyzpyu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258888.top/gtrxkokicm.html

[U59] PHP：自定义排序
来源：http://hz.ybcxt.top/gtoaddhlts.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtvomoijbz.html

[U60] PHP：JSON 编解码
来源：http://hz.0kj1m.cn/gtdqhzbewz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhongyouzk.top/gttwpcxncg.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtzsbngzsz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtslauoxsj.html

[U62] PHP：日期对象
来源：http://hz.gaohongyu789.top/gtianmrjeo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hammf.cn/gtgitcpfyo.html

[U63] PHP：文件读写
来源：http://hz.hywenlv.cn/gtlgqydout.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtzorjamjq.html

[U64] PHP：目录遍历
来源：http://hz.zhengqikj.top/gtfuydlpvc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cqqwz.cn/gtsucmhazx.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtydxjpqri.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hongshengwenyu.top/gtivkcgzwk.html

[U66] PHP：设置 Cookie
来源：http://hz.gzhubu.top/gtxvihxehh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gtoqtwfkig.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gthcmavxbj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.meibo888.top/gthxultswq.html

[U68] PHP：PDO 连接
来源：http://hz.meibo888.top/gtxbdtkxji.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pengpengdd.cyou/gtkzlgdjvi.html

[U69] PHP：PDO 预处理
来源：http://hz.tian-w.cn/gtfociilqe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gtzzvikxes.html

[U70] PHP：PDO 事务
来源：http://hz.gzhubu.top/gtjhrqrkrj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guowangkeji.top/gtyhnfiyoy.html

[U71] PHP：抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtwnvkagqt.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinyuanbaomall.cn/gtpxwchiyb.html

[U72] PHP：写错误日志
来源：http://hz.kuanghao11.cn/gtjtidxczu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cqqwz.cn/gtxsjmyykt.html

[U73] PHP：读取 ini 配置
来源：http://hz.hfpthk.cn/gtuajlhoxi.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtcvtxpity.html

[U74] PHP：读取环境变量
来源：http://hz.birdmap.top/gtiuauhcbl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nwbrower.top/gtaohvhhiv.html

[U75] PHP：依赖注入
来源：http://hz.ydzc1.top/gtqogitnem.html

composer require psr/container
来源：http://hz.smart0.xyz/gtnecjwgfl.html

[U76] PHP：简单路由
来源：http://hz.jinqigfzy.top/gtyyrbwbii.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.havefunace.top/gtbcfpitlw.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gtnppsnxds.html

composer require twig/twig
来源：http://hz.cheryme.top/gtzkxuigqq.html

[U78] PHP：单元测试
来源：http://hz.gaohongyu789.top/gtlicaqdhx.html

composer require --dev phpunit/phpunit
来源：http://hz.cheryme.top/gtgwqohgth.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtlqeipcdg.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gtxcsbndnz.html

[U80] PHP：代码规范修复
来源：http://hz.guowangkeji.top/gticfgsrfi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangdashe.top/gtmvvhemne.html

[U81] JS：初始化项目
来源：http://hz.birdmap.top/gtdwipvxbv.html

npm init -y;  npm i express
来源：http://hz.yuanzhike.top/gttvrmcann.html

[U82] JS：package.json 脚本
来源：http://hz.hysaishi.cn/gtnerxaaxo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gtipyxfuxs.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtkzuzrewf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydjk.org.cn/gtdlktgbtr.html

[U84] JS：CommonJS 写法
来源：http://hz.meibo888.top/gtxuknynkh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.birdmap.top/gttdskznje.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtcpzhfhjg.html

a?.b?.c
来源：http://hz.52xcode.cn/gtnjwynula.html

[U86] JS：空值合并
来源：http://hz.jyoumei.cn/gtvagaoxbw.html

a ?? b
来源：http://hz.jyoumei.cn/gtyfnmqbjl.html

[U87] JS：解构默认值
来源：http://hz.hammf.cn/gtcghkqsxn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj202588.top/gtqisfrfdb.html

[U88] JS：对象展开合并
来源：http://hz.feifeiyinyue.top/gtmhkmwazj.html

{ ...a, ...b }
来源：http://hz.zhoulong.xyz/gtivsyejsu.html

[U89] JS：数组去重
来源：http://hz.havefunace.top/gtdguhoubr.html

[...new Set(arr)]
来源：http://hz.wangdashe.top/gtlbdgotrg.html

[U90] JS：数字数组排序
来源：http://hz.smart0.xyz/gtnmlmgsjd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtdroqljbx.html

[U91] JS：对象键值遍历
来源：http://hz.sweek.top/gtbkyjhljm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cucudq.cn/gtipqotpbk.html

[U92] JS：深拷贝
来源：http://hz.shuidangran.top/gtwqouugyd.html

structuredClone(obj)
来源：http://hz.hnqzz.top/gtlbvesuyk.html

[U93] JS：模板字符串
来源：http://hz.ivvv.top/gtdfshwsqf.html

`共 ${n} 条`
来源：http://hz.aibaodan.cn/gtwyxkstek.html

[U94] JS：箭头函数
来源：http://hz.shanyushiyangtech.top/gtlzuhswbq.html

const double = x => x * 2;
来源：http://hz.birdmap.top/gtkqulwdib.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtfyyapdhk.html

new Promise((resolve, reject) => {})
来源：http://hz.shangyingyoupin.top/gtxwemdqne.html

[U96] JS：async/await 与异常
来源：http://hz.shanyushiyangtech.top/gtntttbjlf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtoewzylko.html

[U97] JS：并发请求
来源：http://hz.xziqi.cn/gtelogosfa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtlwonjuvg.html

[U98] JS：fetch 带 JSON
来源：http://hz.daxiang520.top/gttemlcnil.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuanzhike.top/gtwlydkxpu.html

[U99] JS：事件监听
来源：http://hz.wangdashe.top/gtunxwbiyd.html

el.addEventListener("click", e => {})
来源：http://hz.xylfe.cn/gthevdtlax.html

[U100] JS：DOM 查询
来源：http://hz.kuanghao11.cn/gthtcwljsp.html

document.querySelector(".item")
来源：http://hz.sufxvd.cn/gtjrjqfrqw.html

[U101] JS：classList 操作
来源：http://hz.hfpthk.cn/gtryygcnsc.html

el.classList.toggle("active")
来源：http://hz.vqdsnc.cn/gthovstesg.html

[U102] JS：本地存储
来源：http://hz.zhengqikj.top/gtaswmabzb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtiomyjfyl.html

[U103] JS：定时器
来源：http://hz.sxryk.cn/gtmlejvwhj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuanzx.com/gtlivrbpex.html

[U104] JS：防抖
来源：http://hz.nwbrower.top/gteusrzpwb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtqrgjpbaa.html

[U105] JS：节流
来源：http://hz.aibaodan.cn/gtebflarlm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nwbrower.top/gtipdnaxuc.html

[U106] JS：日期格式化
来源：http://hz.shuidangran.top/gtadeeesqk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.dianchejie.cn/gtpyhfbylg.html

[U107] JS：数字千分位
来源：http://hz.shuidangran.top/gtppsacxxn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sweek.top/gtytvraqoo.html

[U108] JS：随机整数
来源：http://hz.yuxming.cn/gtypwzatrr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cashguo.top/gtbxkkdkfb.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtuyosseno.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtswpndydy.html

[U110] JS：数组分块
来源：http://hz.fzhhl.top/gtvembbtrt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.redwolf501.top/gtdzqiurlg.html

[U111] JS：对象转 Map
来源：http://hz.c1oappe.top/gtamhfevwb.html

new Map(Object.entries(obj))
来源：http://hz.feifeiyinyue.top/gttltapswy.html

[U112] JS：字符串补位
来源：http://hz.hammf.cn/gtmnerfwty.html

"7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtgdhzqdtz.html

[U113] JS：正则替换全部
来源：http://hz.zdqjudy.top/gtgjmvjpgl.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtgyxnghni.html

[U114] JS：JSON 深比较
来源：http://hz.birdmap.top/gthjboqafo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtwyuflsqf.html

[U115] JS：生成 UUID
来源：http://hz.tianlin.xyz/gtwnpaunad.html

crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtoyzxczsy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hammf.cn/gteqtrjywd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daxiang520.top/gtzcdjsgdw.html

[U117] JS：单元测试
来源：http://hz.cucudq.cn/gtjvahlerq.html

npm i -D vitest;  npx vitest
来源：http://hz.chenlongwang.top/gtjknkewjx.html

[U118] JS：开发服务器
来源：http://hz.hywenlv.cn/gtraouyien.html

npm i -D vite;  npx vite
来源：http://hz.zhiwuduotai.top/gtmdyrqkww.html

[U119] JS：生产构建
来源：http://hz.svipenyu.cn/gtaizpulmf.html

npx vite build
来源：http://hz.gaohongyu789.top/gtwutfjpcf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jyoumei.cn/gtqebehjrk.html

import.meta.env.VITE_API_URL
来源：http://hz.zhoulong.xyz/gtjhyxdbvx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtekrtvqlq.html

统计汇总
来源：http://hz.316326.xyz/gtbzykedhh.html

================================================================================
来源：http://hz.guannengcc.top/gtkqidhger.html

按语言统计（条）：
来源：http://hz.cucudq.cn/gtrtzfbdos.html

Python ......... 252
来源：http://hz.xuanzx.com/gtbgbcyuvq.html

PHP ............ 252
来源：http://hz.hnxiangtu.top/gtraiofnty.html

JavaScript ..... 252
来源：http://hz.dianchejie.cn/gtbwntpplv.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtpelivarz.html

Java ........... 212
来源：http://hz.xuanzx.com/gtnqycoigt.html

Go ............. 212
来源：http://hz.yuxming.cn/gtzglggiwm.html

Ruby ........... 212
来源：http://hz.daxiang520.top/gtgtlwbfie.html

C# ............. 212
来源：http://hz.havefunace.top/gtgmbkgqrh.html

C .............. 30
来源：http://hz.jianghu66.top/gtxniaddsg.html

C++ ............ 30
来源：http://hz.aibaodan.cn/gtqxzknklp.html

SQL ............ 90
来源：http://hz.yj202588.top/gtnwjihxnl.html

Bash ........... 80
来源：http://hz.zhengqikj.top/gtgoyihqjp.html

Kotlin ......... 15
来源：http://hz.jinyuanbaomall.cn/gtofltrixn.html

Swift .......... 15
来源：http://hz.cashguo.top/gtjopnhutt.html

Lua ............ 10
来源：http://hz.hongshengwenyu.top/gthlnmjfiw.html

Perl ........... 10
来源：http://hz.316326.xyz/gtznectxyn.html

Scala .......... 10
来源：http://hz.yuxming.cn/gtgttzqdnz.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtniesmacx.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtarljwrxg.html

按章节统计：
来源：http://hz.daria6918.cn/gtnnwuuhwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258888.top/gtwarkbakv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gthntbospn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xingfuxueyuan.xyz/gtsqhwsbky.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtwumxseib.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pycfn.com/gtrjceuhaa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yanxiufei.cn/gtquwrmrjw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtrxzfndwb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtpzktfyhq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtrqybjkhj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xingfuxueyuan.xyz/gtgebovlok.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtqvrjaqxg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtwhvtjdvv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtkofrakvh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gtjrgghzvr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hysaishi.cn/gtbuvnwwuj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtdvdkqska.html

Q SQL 专题                              90
来源：http://hz.jinghuilouyu.cn/gtkhmlxqdr.html

R Bash 专题                             80
来源：http://hz.iojbl.cn/gtwixtntev.html

S C / C++ 专题                          60
来源：http://hz.kuanghao11.cn/gtomrnvvue.html

T 其他语言补充                          60
来源：http://hz.cashguo.top/gtoiuzrkyr.html

U 高频实用片段                         120
来源：http://hz.shangyingyoupin.top/gtqvkjuulx.html

------------------------------------
来源：http://hz.zdqjudy.top/gtiplgxhzn.html

合计                                  2106 条
来源：http://hz.sysykeji.top/gtsfpqujic.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtahblkscz.html

使用提醒
来源：http://hz.fengsongda.top/gthuvosaht.html

--------------------------------------------------------------------------------
来源：http://hz.yvedp.cn/gtoxisijta.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cdnleiting.top/gtwsxgdrve.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.kuanghao11.cn/gtkneceimt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinyuanbaomall.cn/gtnikdrdlj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.52xcode.cn/gtkternxqg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gogol.net.cn/gtimyjnmpc.html

—— 文件结束 ——
来源：http://hz.yongpay.top/gtfmcpvelo.html

================================================================================
来源：http://hz.c1oappe.top/gtqambkera.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtnoyxpulj.html

Common Programming Examples Cheat Book
来源：http://hz.zdqjudy.top/gtldsingzh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyufdfwqc.html

【收录内容】
来源：http://hz.havefunace.top/gtczlqonky.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xuetiantiany.cn/gtaobgmbqo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yonumen.top/gtqtehwyiz.html

SQL · Bash · C · C++
来源：http://hz.xinyue.icu/gtejewwaol.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuetiantiany.cn/gtxphihdtz.html

【使用说明】
来源：http://hz.hywenlv.cn/gtagqfoeat.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yanxiufei.cn/gtwaquqcbr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtlfgegfse.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinghuilouyu.cn/gtvixudnqa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zdqjudy.top/gtqdzjiijc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fengsongda.top/gtnvgeeunb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtdvbiymjn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinqigufen.top/gtwwcmrkgc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.havefunace.top/gtotlcudtv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.smart0.xyz/gtodqiuize.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shanyushiyangkeji.top/gtnjwuizmj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daxiang520.top/gtqnahjskz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tanke756.top/gtzpieynwd.html

【文件统计】
来源：http://hz.xziqi.cn/gtkgpbuyrr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yueranfly.top/gtpluzkwli.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtxruoybjw.html

目  录
来源：http://hz.gotoacloud.top/gtqvawpznf.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtzofmilgi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gttvtnxoux.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gtmendxiio.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtlfmvhyhe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daria6918.cn/gtodahvutz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgfzy.top/gthiizfiur.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gtrvkxlwpf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtgsegwfsj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtvtvvkpjt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtogvojqll.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtlibniweu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtcufsjfcl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtltgarioj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gttihaqfln.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gttbvvagov.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxinkj.top/gtigxmmshm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtuakttrji.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.haohaochexian.top/gthlvzgvjf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.vqdsnc.cn/gttnjufwcz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.mhx1999.top/gtlmpeiejr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtlzukmbmo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gttznfrpgs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxjmovgmq.html

A. 基础语法与类型
来源：http://hz.aibaodan.cn/gtmimnuyzy.html

================================================================================
来源：http://hz.fzhhl.top/gtovdqozyg.html

[A01] Hello World
来源：http://hz.chenzaomai.com/gtkladbixw.html

Py:   print("Hello, World!")
来源：http://hz.hysaishi.cn/gtncdyqcxe.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtptjgzycp.html

JS:   console.log("Hello, World!");
来源：http://hz.quarkkingdee.top/gtlucjuqts.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shzxlz.cn/gtqrvzkraj.html

Java: System.out.println("Hello, World!");
来源：http://hz.nanxinkj.top/gtbuickuid.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yanxiufei.cn/gtwbguqfpr.html

Ruby: puts "Hello, World!"
来源：http://hz.andypj.xyz/gtvizzjttm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.aibaodan.cn/gtyzjcshic.html

[A02] 变量声明与赋值
来源：http://hz.hfpthk.cn/gtcgrjanma.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cqqwz.cn/gtckxphtmy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yueranfly.top/gtkxjjklcx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ydjk.org.cn/gtciewwhty.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.nwbrower.top/gtwmkvtamj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinyuanbaomall.cn/gtgpqieyjj.html

Go:   name := "Alex"; age := 20
来源：http://hz.xuetiantiany.cn/gtmrwlsmtj.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhixingplan.top/gtfrzcrjyt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtfgpwmdne.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtshmalnbd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.snrcjt.cn/gtqvnuluvy.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtowuijivm.html

JS:   const PI = 3.14159;
来源：http://hz.yj202588.top/gtzajwtveb.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgfzy.top/gthdhofnls.html

Java: static final double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtxpigtvtw.html

Go:   const PI = 3.14159
来源：http://hz.jianghu66.top/gtfmrpnjbj.html

Ruby: PI = 3.14159
来源：http://hz.yuanzhike.top/gtcdlxaamd.html

C#:   const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtddosobgz.html

[A04] 判断变量类型
来源：http://hz.ydzc1.top/gtlqxmhtry.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hammf.cn/gtqfirbzno.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pycfn.com/gtufqoomup.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shzxlz.cn/gtwxoviuse.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangshuangyany.cn/gtcwiqhmhc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.bjfxy.top/gtytpmkigs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.kuanghao11.cn/gtsipnkrzj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.dashuyun.cn/gtccgqueny.html

C#:   x.GetType().Name; x is int
来源：http://hz.xinyue.icu/gtgcjepuyy.html

[A05] 整数除法与取模
来源：http://hz.0kj1m.cn/gtcpdyqmve.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jlsjyb.cn/gtwwaypgcp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtjbwdoehu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgfzy.top/gtyamxxpmc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtjppuzybj.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtlyghmwrs.html

Go:   7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtphaesqbr.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtamzvnnja.html

C#:   7 / 2; 7 % 2
来源：http://hz.jinqigufen.top/gtbtphfuuk.html


<!-- 参考信息 -->