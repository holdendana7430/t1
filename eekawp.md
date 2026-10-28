代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.chenjidiqi.icu/gtsapcbuff.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtqylyylbd.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtrgcvphnh.html

?string $name = null
来源：http://hz.snrcjt.cn/gtzxgxdeuy.html

[U47] PHP：联合类型
来源：http://hz.zycfv.cn/gtdgraamee.html

int|string $id
来源：http://hz.kuanghao11.cn/gtkoalzmfu.html

[U48] PHP：纯枚举
来源：http://hz.wangshuangyany.cn/gtalvcexqn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhoulong.xyz/gtljfnwobp.html

[U49] PHP：只读属性
来源：http://hz.tian-w.cn/gtgwizgkpm.html

public readonly string $name
来源：http://hz.zhiwuduotai.top/gtuvllmhfj.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gtamfvkygp.html

public function __construct(private int $id) {}
来源：http://hz.svipenyu.cn/gtulgmzffg.html

[U51] PHP：数组解构
来源：http://hz.0kj1m.cn/gtuimbvpul.html

[$a, $b] = $arr;
来源：http://hz.jyoumei.cn/gtadzvrspo.html

[U52] PHP：箭头函数
来源：http://hz.ehwqpu.com/gtlqkgqyyn.html

$double = fn($x) => $x * 2;
来源：http://hz.redwolf501.top/gtmcqjcehf.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gtlyplzrec.html

$v = $a ?? $b ?? "default";
来源：http://hz.yongpay.top/gtydrmlxex.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtsgixeajd.html

$obj?->method()
来源：http://hz.bjfxy.top/gtpelfvkmd.html

[U55] PHP：match 表达式
来源：http://hz.haohaochexian.top/gtedomgxme.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yueranfly.top/gtcjhhtrgg.html

[U56] PHP：命名参数
来源：http://hz.birdmap.top/gtfpxirkcy.html

f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtlqcpxutd.html

[U57] PHP：字符串插值
来源：http://hz.jiagoushi.top/gticqswcbz.html

"值: {$a}"
来源：http://hz.snrcjt.cn/gtooptahea.html

[U58] PHP：数组三件套
来源：http://hz.zhaomingkeji.xyz/gtaglxmuaf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.52xcode.cn/gtmlkhrnsz.html

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gtvcmgcnyz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtrciysgbl.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtloocyxrm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guannengcc.top/gtxlfgatir.html

[U61] PHP：正则
来源：http://hz.hnqzz.top/gtuphdooyw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtvkzyoxuw.html

[U62] PHP：日期对象
来源：http://hz.yangfankeji.com/gtfszcmycq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gtjdlbjaao.html

[U63] PHP：文件读写
来源：http://hz.nwbrower.top/gtosgiwdtd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.316326.xyz/gtojxnhguq.html

[U64] PHP：目录遍历
来源：http://hz.zhixingplan.top/gtguddgoji.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtkxfpkzps.html

[U65] PHP：会话
来源：http://hz.zhixingplan.top/gtwhocaubu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cheryme.top/gtjmlfytln.html

[U66] PHP：设置 Cookie
来源：http://hz.hfpthk.cn/gtlkxadpfu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhijiandao.cn/gtangxsqzo.html

[U67] PHP：处理文件上传
来源：http://hz.cqqwz.cn/gtgrjcktzn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yj20258888.top/gtejuwenuy.html

[U68] PHP：PDO 连接
来源：http://hz.tianlin.xyz/gtrscrxnuw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangdashe.top/gtuofbukkw.html

[U69] PHP：PDO 预处理
来源：http://hz.cashguo.top/gtyfvacwdw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.birdmap.top/gtilojvktm.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtikrasafx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhiwuduotai.top/gtvzghrevn.html

[U71] PHP：抛出异常
来源：http://hz.c1oappe.top/gtntzqvwps.html

throw new RuntimeException("失败", 500);
来源：http://hz.ywan-chungtsiang.top/gteavwiexc.html

[U72] PHP：写错误日志
来源：http://hz.zhongyouzk.top/gtewagerdx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cashguo.top/gtjvvwqcwq.html

[U73] PHP：读取 ini 配置
来源：http://hz.ybcxt.top/gtbbfinxwe.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtiwcdpxqk.html

[U74] PHP：读取环境变量
来源：http://hz.cucudq.cn/gtsdptmpwx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jlsjyb.cn/gtwxeaefqp.html

[U75] PHP：依赖注入
来源：http://hz.jqgufenzy.top/gtgbkpjtvf.html

composer require psr/container
来源：http://hz.tianlin.xyz/gtoqaxmfam.html

[U76] PHP：简单路由
来源：http://hz.jlsjyb.cn/gtmcvcoqro.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hongshengwenyu.top/gtzvepmlyq.html

[U77] PHP：模板渲染
来源：http://hz.svipenyu.cn/gtndvlxthq.html

composer require twig/twig
来源：http://hz.cdnleiting.top/gthvbjgrcz.html

[U78] PHP：单元测试
来源：http://hz.dashuyun.cn/gtvynhzirn.html

composer require --dev phpunit/phpunit
来源：http://hz.cdnleiting.top/gtdliftenr.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtmimdowgz.html

composer require --dev phpstan/phpstan
来源：http://hz.tanke756.top/gtgcbjhoej.html

[U80] PHP：代码规范修复
来源：http://hz.fzhhl.top/gtooppjqxu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fzhhl.top/gtjqpehzkn.html

[U81] JS：初始化项目
来源：http://hz.svipenyu.cn/gtfozevdcs.html

npm init -y;  npm i express
来源：http://hz.hfpthk.cn/gtejzrdprt.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtnadugqme.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.9152youxi.cn/gtkeduhiku.html

[U83] JS：ES Module 导入导出
来源：http://hz.mhx1999.top/gthrkrgtvg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.svipenyu.cn/gthnymdmob.html

[U84] JS：CommonJS 写法
来源：http://hz.yj20258888.top/gtbwbtxqgp.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gtolzbptau.html

[U85] JS：可选链
来源：http://hz.zhongyouzk.top/gtksfistto.html

a?.b?.c
来源：http://hz.meibo888.top/gtbzqibynq.html

[U86] JS：空值合并
来源：http://hz.shanyushiyangtech.top/gtrcuwannu.html

a ?? b
来源：http://hz.yangfankeji.com/gtbuhaoubk.html

[U87] JS：解构默认值
来源：http://hz.snrcjt.cn/gtcsalfupv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.fzhhl.top/gtkvzqzvmt.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtyqbpjwpc.html

{ ...a, ...b }
来源：http://hz.aizwys.cn/gtulyckxto.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtfavkihlk.html

[...new Set(arr)]
来源：http://hz.cucudq.cn/gtwhzzeaah.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gtthcrtixf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtmztkpejp.html

[U91] JS：对象键值遍历
来源：http://hz.shangyingyoupin.top/gthknkingn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.redwolf501.top/gtsnfbksto.html

[U92] JS：深拷贝
来源：http://hz.wangdashe.top/gtxdwcpwwo.html

structuredClone(obj)
来源：http://hz.daxiang520.top/gtwdrgmsdz.html

[U93] JS：模板字符串
来源：http://hz.zhaomingkeji.xyz/gtiezzvggy.html

`共 ${n} 条`
来源：http://hz.hammf.cn/gtlqpvcxcf.html

[U94] JS：箭头函数
来源：http://hz.quarkkingdee.top/gtpptrpebn.html

const double = x => x * 2;
来源：http://hz.pycfn.com/gtdpytlbbc.html

[U95] JS：Promise 包装
来源：http://hz.wangdashe.top/gtohhsxcon.html

new Promise((resolve, reject) => {})
来源：http://hz.gogol.net.cn/gtrxwrprqq.html

[U96] JS：async/await 与异常
来源：http://hz.tian-w.cn/gtrytmjjak.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtbakdsdwa.html

[U97] JS：并发请求
来源：http://hz.quarkkingdee.top/gtbtduffkv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtbemxiwrt.html

[U98] JS：fetch 带 JSON
来源：http://hz.xingfuxueyuan.xyz/gtptlicxwy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jqgufenzy.top/gtjvdgwpdb.html

[U99] JS：事件监听
来源：http://hz.daxiang520.top/gtyffuywqi.html

el.addEventListener("click", e => {})
来源：http://hz.quarkkingdee.top/gtvferpmnr.html

[U100] JS：DOM 查询
来源：http://hz.yj20258888.top/gtomxkfkfm.html

document.querySelector(".item")
来源：http://hz.redwolf501.top/gtbuwsctbk.html

[U101] JS：classList 操作
来源：http://hz.gzhubu.top/gtghzzluxw.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtiqlrtuan.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangtech.top/gtanyyxlrq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jlsjyb.cn/gtqzvgcgqb.html

[U103] JS：定时器
来源：http://hz.yuxming.cn/gtkanohyvt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.quarkkingdee.top/gttwzobwrq.html

[U104] JS：防抖
来源：http://hz.aizwys.cn/gtkvzrondd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtcsqaimgv.html

[U105] JS：节流
来源：http://hz.mhx1999.top/gtsloiccqa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.andypj.xyz/gtudkhivqp.html

[U106] JS：日期格式化
来源：http://hz.cqqwz.cn/gtoresmgwv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangkeji.top/gtwthcsxru.html

[U107] JS：数字千分位
来源：http://hz.feifeiyinyue.top/gtyspisafm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xinyue.icu/gtpwlzlhfk.html

[U108] JS：随机整数
来源：http://hz.yj20258888.top/gtvsqjdjtt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.meibo888.top/gtcrxdbmua.html

[U109] JS：数组分组
来源：http://hz.daria6918.cn/gtrjywranr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gttaavbrgy.html

[U110] JS：数组分块
来源：http://hz.wangshuangyany.cn/gteavwdtmn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guowangkeji.top/gtojvdbivx.html

[U111] JS：对象转 Map
来源：http://hz.hfpthk.cn/gtihckvfxe.html

new Map(Object.entries(obj))
来源：http://hz.jinyuanbaomall.cn/gtvsgxzmat.html

[U112] JS：字符串补位
来源：http://hz.xinyue.icu/gthipzfmdm.html

"7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtxvwtydcm.html

[U113] JS：正则替换全部
来源：http://hz.zhongyouzk.top/gtrrgijjsu.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtcqcafkra.html

[U114] JS：JSON 深比较
来源：http://hz.hfpthk.cn/gtnovntbwl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtgfwvrwec.html

[U115] JS：生成 UUID
来源：http://hz.xuanzx.com/gtxeumyziw.html

crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtfuiqasql.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jqgufenzy.top/gtitzstbbj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuanzx.com/gtslnqyahs.html

[U117] JS：单元测试
来源：http://hz.zhixingplan.top/gtltuozsyd.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gtpchxfmhh.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtkkpqdsgy.html

npm i -D vite;  npx vite
来源：http://hz.mhx1999.top/gtmxjxwnrb.html

[U119] JS：生产构建
来源：http://hz.cheryme.top/gtgvjzaesg.html

npx vite build
来源：http://hz.hongshengwenyu.top/gtiamipmev.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tianlin.xyz/gtlsccjkst.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtcgcoyoao.html

================================================================================
来源：http://hz.havefunace.top/gttzkvdxhi.html

统计汇总
来源：http://hz.shanyushiyangkeji.top/gtohlohmzp.html

================================================================================
来源：http://hz.sufxvd.cn/gtnsakogxt.html

按语言统计（条）：
来源：http://hz.0kj1m.cn/gtwzxovgus.html

Python ......... 252
来源：http://hz.yj20258888.top/gtdloigciu.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtlochwkoa.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtkwymalcn.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtujnwfpdr.html

Java ........... 212
来源：http://hz.havefunace.top/gturmcogpo.html

Go ............. 212
来源：http://hz.zycfv.cn/gtrtpzkifj.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtkmzzrafd.html

C# ............. 212
来源：http://hz.dianchejie.cn/gtzlfezpvm.html

C .............. 30
来源：http://hz.jqgufenzy.top/gtmoqtyahp.html

C++ ............ 30
来源：http://hz.zhoulong.xyz/gtqorxggny.html

SQL ............ 90
来源：http://hz.andypj.xyz/gtykzvpxgb.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtchoukece.html

Kotlin ......... 15
来源：http://hz.chenlongwang.top/gtkqxgdvng.html

Swift .......... 15
来源：http://hz.nanxuanxn.top/gtenrqjmlv.html

Lua ............ 10
来源：http://hz.chenzaomai.com/gtiuwfrvgq.html

Perl ........... 10
来源：http://hz.chenzaomai.com/gtuolzhmph.html

Scala .......... 10
来源：http://hz.shangyingyoupin.top/gtupuslopr.html

------------------------------------
来源：http://hz.316326.xyz/gtdvzvaozz.html

合计 ........... 2106 条
来源：http://hz.yueranfly.top/gtogfctrfx.html

按章节统计：
来源：http://hz.shzxlz.cn/gtxhxepaek.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhongyouzk.top/gtkacofafz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gtouyhnzrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gotoacloud.top/gtsdsdhtyw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtnrxuqnoj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtwiqucgfj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hfpthk.cn/gtzdvhzrew.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtvaukjhpt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jqgufenzy.top/gtwfeuuwnu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gthbtmrrwr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtaxzcvtxv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtmfpowjjo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtsnqmnlgb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gttokyrbes.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hysaishi.cn/gtotkgwreq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenjidiqi.icu/gtkhtvbbdr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtljdzrcdu.html

Q SQL 专题                              90
来源：http://hz.xinyue.icu/gtksffvkzw.html

R Bash 专题                             80
来源：http://hz.guowangkeji.top/gtkoxqfdfj.html

S C / C++ 专题                          60
来源：http://hz.andypj.xyz/gtrmaprozk.html

T 其他语言补充                          60
来源：http://hz.tianlin.xyz/gtvgdazbib.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtizunykoz.html

------------------------------------
来源：http://hz.ybcxt.top/gtpdfdhldb.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtsilcxdbj.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtzgcynowo.html

使用提醒
来源：http://hz.jinghuilouyu.cn/gtbukudlgv.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtdlkwbjgu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxinkj.top/gtgwvgjyvp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydjk.org.cn/gtgbhrnsek.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jyoumei.cn/gtpkqmsvlt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtrdssegvv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinqigufen.top/gtovrbfajx.html

—— 文件结束 ——
来源：http://hz.daxiang520.top/gtxvtiecwy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvktbpnrz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hnxiangtu.top/gtqxsgtrrq.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gthwycooav.html

================================================================================
来源：http://hz.yongpay.top/gtyawcdlrt.html

【收录内容】
来源：http://hz.cashguo.top/gtxfbcmgza.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtqmimdhis.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jianghu66.top/gthkwnqixy.html

SQL · Bash · C · C++
来源：http://hz.yonumen.top/gtxgvkdncs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.tanke756.top/gtjbipgjwa.html

【使用说明】
来源：http://hz.shanyushiyangtech.top/gttnhvymfm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xuanzx.com/gtrffeztzc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.quarkkingdee.top/gthsgjkagq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jlsjyb.cn/gtfpiipxtn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sweek.top/gtflrmyaba.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zdqjudy.top/gtrvdvoakx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sysykeji.top/gtyumcnnxn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.andypj.xyz/gtkpqrwkhw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gtrdvmcrvv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gotoacloud.top/gtfxwywvum.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hywenlv.cn/gtxbvnowdd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yj20258888.top/gtgkkvrpof.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj20258.top/gtxrrehsqx.html

【文件统计】
来源：http://hz.zhixingplan.top/gtinxscjzr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jqgfzy.top/gtzwielosw.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtgdkvdbum.html

目  录
来源：http://hz.hammf.cn/gtpqkdnyiq.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtvzxoxyyq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.9152youxi.cn/gtpqhfvfrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtieibsiir.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtnfsyvbzg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtwzxzwkog.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jiagoushi.top/gtdocgqnwj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jqgfzy.top/gthcetsymc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hongshengwenyu.top/gtahxcgrap.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.havefunace.top/gtouzzkjji.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtipyzhole.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yangfankeji.com/gtlygofyrk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gttanwvaxd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtwzwjqdki.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtbcttyumq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nanxuanxn.top/gthuxbnkpg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jyoumei.cn/gtwraxvwnt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtornkbpic.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuanzx.com/gtnumsooco.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gzhubu.top/gtmjofklyq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hywenlv.cn/gtomyjuhmz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtgheamgdn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtywditawl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvadkiphl.html

A. 基础语法与类型
来源：http://hz.dashuyun.cn/gtgrssfhka.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtboiwymlr.html

[A01] Hello World
来源：http://hz.chenjidiqi.icu/gtihosgqol.html

Py:   print("Hello, World!")
来源：http://hz.jqgufenzy.top/gtdxgdtdqm.html

PHP:  echo "Hello, World!";
来源：http://hz.bjfxy.top/gtpzaibhst.html

JS:   console.log("Hello, World!");
来源：http://hz.yonumen.top/gtsuvxjxah.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cheryme.top/gtltsqwpmg.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtzdjskaxl.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtftwxgfco.html

Ruby: puts "Hello, World!"
来源：http://hz.jinyuanbaomall.cn/gtdhvkcevo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hammf.cn/gtsxibjyhr.html

[A02] 变量声明与赋值
来源：http://hz.haohaochexian.top/gtwwqrxmaa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jiagoushi.top/gtzddpyaxi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yj202588.top/gtfxmfqchn.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.meibo888.top/gtxoizaynh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ybcxt.top/gtglnjomwv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.haohaochexian.top/gthdrkbkye.html

Go:   name := "Alex"; age := 20
来源：http://hz.ehwqpu.com/gtnrggaifx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gtynztgfpo.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jqgufenzy.top/gtbijzmilr.html

[A03] 常量定义
来源：http://hz.yj202588.top/gtznedxrtm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tianlin.xyz/gtwpokofjk.html

PHP:  const PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtiuhqaola.html

JS:   const PI = 3.14159;
来源：http://hz.pycfn.com/gtqistfszp.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgufenzy.top/gtbgbgynbm.html

Java: static final double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtvtbwlrya.html

Go:   const PI = 3.14159
来源：http://hz.cucudq.cn/gtkyvmllrp.html

Ruby: PI = 3.14159
来源：http://hz.iojbl.cn/gtscnnihqe.html

C#:   const double PI = 3.14159;
来源：http://hz.meibo888.top/gtvxxwuexj.html

[A04] 判断变量类型
来源：http://hz.jyoumei.cn/gtfjmayudr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gttyiwcqib.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jiagoushi.top/gtsneuudop.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sysykeji.top/gtrssfdijn.html

TS:   typeof x; x instanceof Date
来源：http://hz.yangfankeji.com/gtgktcccrb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yuxming.cn/gtmibzmmgk.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hysaishi.cn/gtnorxldlh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gotoacloud.top/gtbfpjbdog.html

C#:   x.GetType().Name; x is int
来源：http://hz.dianchejie.cn/gtrogkkphj.html

[A05] 整数除法与取模
来源：http://hz.zhijiandao.cn/gtvqlezwtx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.dashuyun.cn/gtzedennnm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtgomvpbmo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinqigufen.top/gtbfyilsnq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shuidangran.top/gtajwtsegl.html


<!-- 参考信息 -->