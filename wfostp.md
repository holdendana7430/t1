代发 wailian999

[U47] PHP：联合类型
来源：http://hz.yvedp.cn/gtlymclhml.html

int|string $id
来源：http://hz.andypj.xyz/gtkkscdkej.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtcfumhmyh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigfzy.top/gtrvnqxvev.html

[U49] PHP：只读属性
来源：http://hz.zycfv.cn/gtssijvnxk.html

public readonly string $name
来源：http://hz.yonumen.top/gtuihnxxca.html

[U50] PHP：构造器属性提升
来源：http://hz.fzhhl.top/gtmpjpcvou.html

public function __construct(private int $id) {}
来源：http://hz.sufxvd.cn/gtsathjevj.html

[U51] PHP：数组解构
来源：http://hz.yangfankeji.com/gtrkcovigf.html

[$a, $b] = $arr;
来源：http://hz.cheryme.top/gtzyeoqxxy.html

[U52] PHP：箭头函数
来源：http://hz.xylfe.cn/gtfegvkjpd.html

$double = fn($x) => $x * 2;
来源：http://hz.hnqzz.top/gtzlkikmar.html

[U53] PHP：空合并运算符
来源：http://hz.nanxuanxn.top/gtqvzzdlkj.html

$v = $a ?? $b ?? "default";
来源：http://hz.dashuyun.cn/gtznddpsst.html

[U54] PHP：空安全调用
来源：http://hz.yongpay.top/gtfgwpkipm.html

$obj?->method()
来源：http://hz.yongpay.top/gtbyaleqgn.html

[U55] PHP：match 表达式
来源：http://hz.chenlongwang.top/gteldtejzs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.meibo888.top/gtkykekfbt.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtshwuvarv.html

f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtawkjnsvd.html

[U57] PHP：字符串插值
来源：http://hz.jqgufenzy.top/gtactufqwq.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtuijhlibj.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtrovpwwnn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gzhubu.top/gtuprpipsy.html

[U59] PHP：自定义排序
来源：http://hz.jinghuilouyu.cn/gtqlhuzfvm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtbawngdtr.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtrlrfpvha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jyoumei.cn/gtaucbqkgl.html

[U61] PHP：正则
来源：http://hz.smart0.xyz/gtupkkbhzz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtnmwxkukp.html

[U62] PHP：日期对象
来源：http://hz.jyoumei.cn/gtnqvsldlh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtjbvnivvo.html

[U63] PHP：文件读写
来源：http://hz.kuanghao11.cn/gtygghocqo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtgrqdaqae.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtprpjqfwr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yanxiufei.cn/gtxdqtaysl.html

[U65] PHP：会话
来源：http://hz.meibo888.top/gtdyqpjbla.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhiwuduotai.top/gtbekfmqda.html

[U66] PHP：设置 Cookie
来源：http://hz.ivvv.top/gthzayqtwn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtfwidcqlv.html

[U67] PHP：处理文件上传
来源：http://hz.zhaomingkeji.xyz/gtsljhlqbl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.0kj1m.cn/gthpfptcmv.html

[U68] PHP：PDO 连接
来源：http://hz.yueranfly.top/gtggywikfu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhoulong.xyz/gttvosblxe.html

[U69] PHP：PDO 预处理
来源：http://hz.zhijiandao.cn/gtjobesjlr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ydzc1.top/gtppwjuogx.html

[U70] PHP：PDO 事务
来源：http://hz.fengsongda.top/gtzceatifr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.smart0.xyz/gtmkqjjbrl.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gthzsbastd.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenlongwang.top/gtelyonpam.html

[U72] PHP：写错误日志
来源：http://hz.zhiwuduotai.top/gttsbextjh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hysaishi.cn/gtugtdutdo.html

[U73] PHP：读取 ini 配置
来源：http://hz.havefunace.top/gtpscrcepx.html

parse_ini_file("config.ini", true)
来源：http://hz.havefunace.top/gtxrtgqoue.html

[U74] PHP：读取环境变量
来源：http://hz.ehwqpu.com/gtyyfftsjf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhongyouzk.top/gteiujwqdz.html

[U75] PHP：依赖注入
来源：http://hz.hongshengwenyu.top/gtveitrvyd.html

composer require psr/container
来源：http://hz.cashguo.top/gttzdavkfm.html

[U76] PHP：简单路由
来源：http://hz.jqgfzy.top/gtovgwqtio.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtkpwvjyga.html

[U77] PHP：模板渲染
来源：http://hz.hywenlv.cn/gtiaftkahi.html

composer require twig/twig
来源：http://hz.jlsjyb.cn/gtzduafnxq.html

[U78] PHP：单元测试
来源：http://hz.shanyushiyangtech.top/gtlldpplaj.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtmbiyofom.html

[U79] PHP：静态分析
来源：http://hz.zhijiandao.cn/gtngoiuoly.html

composer require --dev phpstan/phpstan
来源：http://hz.hysaishi.cn/gttzqryutc.html

[U80] PHP：代码规范修复
来源：http://hz.nanxuanxn.top/gtgeqcdivp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daria6918.cn/gtkkrylgan.html

[U81] JS：初始化项目
来源：http://hz.guowangkeji.top/gtjevvoxsc.html

npm init -y;  npm i express
来源：http://hz.vqdsnc.cn/gtabkbfsgh.html

[U82] JS：package.json 脚本
来源：http://hz.xuetiantiany.cn/gtneprsium.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gtrnrsiail.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhongyouzk.top/gtkkouulyp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.pengpengdd.cyou/gtslbqgtad.html

[U84] JS：CommonJS 写法
来源：http://hz.xingfuxueyuan.xyz/gtfdujyoqy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hammf.cn/gtysedmozu.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtqqhhegzj.html

a?.b?.c
来源：http://hz.gzhubu.top/gtrkpepnyz.html

[U86] JS：空值合并
来源：http://hz.meibo888.top/gthhgplnxm.html

a ?? b
来源：http://hz.jinqigfzy.top/gtroxcdfbx.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gttzhghmcn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gttxsomjxk.html

[U88] JS：对象展开合并
来源：http://hz.zhiwuduotai.top/gtuslzapub.html

{ ...a, ...b }
来源：http://hz.snrcjt.cn/gtjyzgfach.html

[U89] JS：数组去重
来源：http://hz.cheryme.top/gtcyklrbhn.html

[...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtmaliilgt.html

[U90] JS：数字数组排序
来源：http://hz.nanxinkj.top/gtqlkusodo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtclfmawqa.html

[U91] JS：对象键值遍历
来源：http://hz.jlsjyb.cn/gtageoagmu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.haohaochexian.top/gtsovjvjar.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gtpomnhbel.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtieyynspn.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtfaanoyvw.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtlwknxubn.html

[U94] JS：箭头函数
来源：http://hz.chenzaomai.com/gtdxcalxqh.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gtmejxqdau.html

[U95] JS：Promise 包装
来源：http://hz.pengpengdd.cyou/gtdoedyvyb.html

new Promise((resolve, reject) => {})
来源：http://hz.chenlongwang.top/gtxfhvxdlk.html

[U96] JS：async/await 与异常
来源：http://hz.zhijiandao.cn/gteshsagdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtdlyajmdc.html

[U97] JS：并发请求
来源：http://hz.cqqwz.cn/gtevfezmko.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtojzlnowl.html

[U98] JS：fetch 带 JSON
来源：http://hz.9152youxi.cn/gtjvjsiblz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yangfankeji.com/gtuwefbzvf.html

[U99] JS：事件监听
来源：http://hz.chenzaomai.com/gtngkzxufp.html

el.addEventListener("click", e => {})
来源：http://hz.bjfxy.top/gtgypzpirv.html

[U100] JS：DOM 查询
来源：http://hz.chenjidiqi.icu/gtqrwtirdu.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtxslqxmvm.html

[U101] JS：classList 操作
来源：http://hz.yvedp.cn/gtovwnovsl.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtticcnher.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtsgotgivi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.316326.xyz/gtgjopupqm.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtfwvvrzcq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yueranfly.top/gtjebzcpne.html

[U104] JS：防抖
来源：http://hz.iojbl.cn/gtuxatqlwy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gttzumbcjc.html

[U105] JS：节流
来源：http://hz.tanke756.top/gtuohlclep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinghuilouyu.cn/gtltvtrjeo.html

[U106] JS：日期格式化
来源：http://hz.birdmap.top/gtvtdrrwvc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhijiandao.cn/gtqpfsxblv.html

[U107] JS：数字千分位
来源：http://hz.shangyingyoupin.top/gtadqfkbvk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtgythzjyv.html

[U108] JS：随机整数
来源：http://hz.cqqwz.cn/gtwxnxykex.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtjrfvrazn.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtbypklbae.html

Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gteiwkoqak.html

[U110] JS：数组分块
来源：http://hz.aibaodan.cn/gtacsijayn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhengqikj.top/gtastqwtel.html

[U111] JS：对象转 Map
来源：http://hz.hywenlv.cn/gtvtwgtlpt.html

new Map(Object.entries(obj))
来源：http://hz.guowangkeji.top/gtcznplrqx.html

[U112] JS：字符串补位
来源：http://hz.redwolf501.top/gtktdfnjfm.html

"7".padStart(3, "0")
来源：http://hz.hammf.cn/gtcsonkvgp.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gtiuymrqaz.html

s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtcwctwczt.html

[U114] JS：JSON 深比较
来源：http://hz.daria6918.cn/gtptllpwcd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhoulong.xyz/gtdodkyegp.html

[U115] JS：生成 UUID
来源：http://hz.ybcxt.top/gtcycsqrty.html

crypto.randomUUID()
来源：http://hz.yongpay.top/gtglivsmhk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gtoqjvahvr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtxhlbbzny.html

[U117] JS：单元测试
来源：http://hz.zhixingplan.top/gtveixoprs.html

npm i -D vitest;  npx vitest
来源：http://hz.hfpthk.cn/gtofrjadgu.html

[U118] JS：开发服务器
来源：http://hz.ppjwa.cn/gttnmfxhqn.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtrqpghsdo.html

[U119] JS：生产构建
来源：http://hz.kuanghao11.cn/gtbrnyjncq.html

npx vite build
来源：http://hz.cucudq.cn/gtgijsmmjd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtkissqfwd.html

import.meta.env.VITE_API_URL
来源：http://hz.jinyuanbaomall.cn/gtekbgcxvj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtajodkfst.html

统计汇总
来源：http://hz.tanke756.top/gtiinqmcfm.html

================================================================================
来源：http://hz.cashguo.top/gtofmkaxsz.html

按语言统计（条）：
来源：http://hz.jinqigfzy.top/gtjrrzawxg.html

Python ......... 252
来源：http://hz.jinyuanbaomall.cn/gtfjxqpgcv.html

PHP ............ 252
来源：http://hz.zhoulong.xyz/gtxvwffqyk.html

JavaScript ..... 252
来源：http://hz.fzhhl.top/gtrkpbsati.html

TypeScript ..... 212
来源：http://hz.xinyue.icu/gtxhwebefx.html

Java ........... 212
来源：http://hz.xuanzx.com/gtpoetrjne.html

Go ............. 212
来源：http://hz.zhaomingkeji.xyz/gtrqgcyizh.html

Ruby ........... 212
来源：http://hz.jqgufenzy.top/gtqfxegihs.html

C# ............. 212
来源：http://hz.ydjk.org.cn/gtraeuleyc.html

C .............. 30
来源：http://hz.yj202588.top/gtjrwhljcx.html

C++ ............ 30
来源：http://hz.zycfv.cn/gtwhythgim.html

SQL ............ 90
来源：http://hz.aibaodan.cn/gtvjeqnmas.html

Bash ........... 80
来源：http://hz.birdmap.top/gtpndmcnlk.html

Kotlin ......... 15
来源：http://hz.cqqwz.cn/gtgwlwltkb.html

Swift .......... 15
来源：http://hz.chenzaomai.com/gtblhlybkb.html

Lua ............ 10
来源：http://hz.52xcode.cn/gtconwufvh.html

Perl ........... 10
来源：http://hz.fengsongda.top/gtoontzjvj.html

Scala .......... 10
来源：http://hz.sweek.top/gttpxwcmpj.html

------------------------------------
来源：http://hz.svipenyu.cn/gtcczsqwup.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtusfjqowb.html

按章节统计：
来源：http://hz.hywenlv.cn/gtoetgjgtv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tian-w.cn/gtydgcqkkw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtkexoxsub.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtywcncjea.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtoggcfppc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jiagoushi.top/gtfhihssoi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtxejogkai.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtpnjtdxpv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cdnleiting.top/gtfcfrebgn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtwzojhhfj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jqgufenzy.top/gtgqezskgk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtyurznhqp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtkigohito.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtshcqzysv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtpclusoga.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtesxgyeqq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtlldvwned.html

Q SQL 专题                              90
来源：http://hz.52xcode.cn/gtcbuvqlru.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtccoipsip.html

S C / C++ 专题                          60
来源：http://hz.shzxlz.cn/gtmzwbnyxj.html

T 其他语言补充                          60
来源：http://hz.sysykeji.top/gtddiqtvpx.html

U 高频实用片段                         120
来源：http://hz.svipenyu.cn/gttzszdyaq.html

------------------------------------
来源：http://hz.jiagoushi.top/gtlbryhgph.html

合计                                  2106 条
来源：http://hz.kuanghao11.cn/gtiydnadjx.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtliuszxzw.html

使用提醒
来源：http://hz.fzhhl.top/gthresedte.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gthqolrsuq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhixingplan.top/gtssmjjiiu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.pengpengdd.cyou/gtkmtjqwyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hysaishi.cn/gtznytdxdg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhoulong.xyz/gtfnmsnhtd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.0kj1m.cn/gtrwmsbyim.html

—— 文件结束 ——
来源：http://hz.pengpengdd.cyou/gtwzsijery.html

================================================================================
来源：http://hz.tanke756.top/gtacrranli.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuxming.cn/gtsuvisbia.html

Common Programming Examples Cheat Book
来源：http://hz.zdqjudy.top/gtjrmaeksl.html

================================================================================
来源：http://hz.zhijiandao.cn/gtsqhaxruf.html

【收录内容】
来源：http://hz.gotoacloud.top/gtwyjyfsyo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guowangkeji.top/gtzjtfmrsn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gotoacloud.top/gttedxrbsw.html

SQL · Bash · C · C++
来源：http://hz.yj20258888.top/gtxzjmgshr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigfzy.top/gthexcqqts.html

【使用说明】
来源：http://hz.cucudq.cn/gtfmglprvr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangshuangyany.cn/gtydteowfm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ehwqpu.com/gtrtkcrmcu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinghuilouyu.cn/gtfwggpkyl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dashuyun.cn/gtapsebbqy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dashuyun.cn/gtgxmfaomw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtobjzayjr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinqigfzy.top/gthsylpfzh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ehwqpu.com/gtythyjppe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuxming.cn/gtzutzgeiw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.0kj1m.cn/gtbtvyodan.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenjidiqi.icu/gtepnpxgbz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.havefunace.top/gtybacoret.html

【文件统计】
来源：http://hz.xinyue.icu/gtbmnuqdwp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hongshengwenyu.top/gtbvpapcij.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtshrdxwsr.html

目  录
来源：http://hz.jlsjyb.cn/gthgfhcptr.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtyidmkbzx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtexznndon.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtgxvbthte.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtteloqkvd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtmhxuacki.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ppjwa.cn/gtnvyrjlbj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtbgpehhle.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtewbpujop.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.316326.xyz/gtaimxinun.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtporydwhq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jlsjyb.cn/gteazpbwlx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtzlsdlsxw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtsvpavfsy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtimveqtqd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yj20258888.top/gtrzzkwkyh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.redwolf501.top/gtywsaaxff.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtpopuvjcb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gaohongyu789.top/gtuzbxedvc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cheryme.top/gtroifdowm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shangyingyoupin.top/gtjjwjkhrc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtpfvjafts.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtgluiiutl.html

================================================================================
来源：http://hz.iojbl.cn/gtuinuswap.html

A. 基础语法与类型
来源：http://hz.hongshengwenyu.top/gtnxjqrikb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdzmtllie.html

[A01] Hello World
来源：http://hz.chenzaomai.com/gtoulnefsp.html

Py:   print("Hello, World!")
来源：http://hz.0kj1m.cn/gtpbfasjhr.html

PHP:  echo "Hello, World!";
来源：http://hz.xziqi.cn/gthdmbneqk.html

JS:   console.log("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtnbcdhurd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gogol.net.cn/gturpcnviw.html

Java: System.out.println("Hello, World!");
来源：http://hz.c1oappe.top/gttuhnthzo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangdashe.top/gtywpdlwkb.html

Ruby: puts "Hello, World!"
来源：http://hz.wangshuangyany.cn/gtfcmgvrzb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gzhubu.top/gtjcznyagc.html

[A02] 变量声明与赋值
来源：http://hz.yangfankeji.com/gtiorvtcdr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.feifeiyinyue.top/gtwakznkkp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shangyingyoupin.top/gtzkzjwvyy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jiagoushi.top/gtclaotfzy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.dashuyun.cn/gtnljfmrws.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gtimtgcyux.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangshuangyany.cn/gtmrsqltkq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daria6918.cn/gtnwjtbytn.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtcsqamvbf.html

[A03] 常量定义
来源：http://hz.yangfankeji.com/gtapevhznc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.vqdsnc.cn/gtxkidmwqj.html

PHP:  const PI = 3.14159;
来源：http://hz.dianchejie.cn/gthwuufuuj.html

JS:   const PI = 3.14159;
来源：http://hz.aibaodan.cn/gtpranqxhm.html

TS:   const PI: number = 3.14159;
来源：http://hz.ybcxt.top/gtnmiggidv.html

Java: static final double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtkucxurkt.html

Go:   const PI = 3.14159
来源：http://hz.guowangkeji.top/gtfapgyqhk.html

Ruby: PI = 3.14159
来源：http://hz.zdqjudy.top/gtzhttakdl.html

C#:   const double PI = 3.14159;
来源：http://hz.316326.xyz/gtexsykpbr.html

[A04] 判断变量类型
来源：http://hz.yj20258888.top/gtleahwcwq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gttdhvqqfe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yangfankeji.com/gtoyxddnqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zdqjudy.top/gtuacjswlr.html

TS:   typeof x; x instanceof Date
来源：http://hz.quarkkingdee.top/gtrxcretzn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.bjfxy.top/gtncrdaghx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gtcqmkidmr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ywan-chungtsiang.top/gtejvnrojy.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydzc1.top/gtrkkklikx.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangkeji.top/gtncyhnkzg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.smart0.xyz/gtrixvjhqc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yonumen.top/gtsvxatkeg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yvedp.cn/gtlglqcvrv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtqrbctrje.html

Java: 7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gtpqtskvfn.html

Go:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtldhuvlpr.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtixxurcmw.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtfzblctdr.html


<!-- 参考信息 -->