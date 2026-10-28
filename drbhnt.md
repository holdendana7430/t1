代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtquqjkvwh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtzinfghsr.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtaofnmxiy.html

?string $name = null
来源：http://hz.chenzaomai.com/gttfdxqbww.html

[U47] PHP：联合类型
来源：http://hz.sxryk.cn/gtilvzmkut.html

int|string $id
来源：http://hz.tianlin.xyz/gtletcnjlb.html

[U48] PHP：纯枚举
来源：http://hz.zycfv.cn/gtxzqvrupb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtazcciprt.html

[U49] PHP：只读属性
来源：http://hz.svipenyu.cn/gttblfgedt.html

public readonly string $name
来源：http://hz.0kj1m.cn/gtvkjtgkel.html

[U50] PHP：构造器属性提升
来源：http://hz.hysaishi.cn/gthglfmwch.html

public function __construct(private int $id) {}
来源：http://hz.pycfn.com/gtxkclqiwn.html

[U51] PHP：数组解构
来源：http://hz.jianghu66.top/gtjzicadoe.html

[$a, $b] = $arr;
来源：http://hz.yonumen.top/gtzjpobncy.html

[U52] PHP：箭头函数
来源：http://hz.jinghuilouyu.cn/gtjqwyargp.html

$double = fn($x) => $x * 2;
来源：http://hz.yvedp.cn/gtamemdavn.html

[U53] PHP：空合并运算符
来源：http://hz.feifeiyinyue.top/gteeyvuloz.html

$v = $a ?? $b ?? "default";
来源：http://hz.aizwys.cn/gtjyrtvxhx.html

[U54] PHP：空安全调用
来源：http://hz.hfpthk.cn/gtewivcvje.html

$obj?->method()
来源：http://hz.gzhubu.top/gtnpayzypv.html

[U55] PHP：match 表达式
来源：http://hz.cashguo.top/gtxkvtgctq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuanzx.com/gtmqbkdzcj.html

[U56] PHP：命名参数
来源：http://hz.yuxming.cn/gtwonyjnpu.html

f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtlshhqvgr.html

[U57] PHP：字符串插值
来源：http://hz.kuanghao11.cn/gtsfllhddw.html

"值: {$a}"
来源：http://hz.snrcjt.cn/gtmutylesw.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtgasjevvp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tian-w.cn/gtoqpiemya.html

[U59] PHP：自定义排序
来源：http://hz.52xcode.cn/gtgjxgfzpy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtmqwfagab.html

[U60] PHP：JSON 编解码
来源：http://hz.yanxiufei.cn/gtbvtwtpjm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.daxiang520.top/gtgydnodge.html

[U61] PHP：正则
来源：http://hz.yj20258888.top/gtmztieupu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtspfufuza.html

[U62] PHP：日期对象
来源：http://hz.tian-w.cn/gtqmbamnzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pycfn.com/gtxsdyxpqo.html

[U63] PHP：文件读写
来源：http://hz.nanxinkj.top/gtbhmzgais.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhengqikj.top/gtgaqatoar.html

[U64] PHP：目录遍历
来源：http://hz.zhixingplan.top/gthslltppz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.kuanghao11.cn/gtkyaqsrkd.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gtcuzmzcxe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.andypj.xyz/gtszimilgq.html

[U66] PHP：设置 Cookie
来源：http://hz.zdqjudy.top/gtvxmnzelq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhongyouzk.top/gtasglbljr.html

[U67] PHP：处理文件上传
来源：http://hz.gzhubu.top/gtjxmzscmp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinyuanbaomall.cn/gthrzqaday.html

[U68] PHP：PDO 连接
来源：http://hz.feifeiyinyue.top/gtddbszxrm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtpccpjhqa.html

[U69] PHP：PDO 预处理
来源：http://hz.jinyuanbaomall.cn/gtjkkfnoey.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tian-w.cn/gtgecqbohw.html

[U70] PHP：PDO 事务
来源：http://hz.xziqi.cn/gtdqsdibrp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtnrfbzleh.html

[U71] PHP：抛出异常
来源：http://hz.gaohongyu789.top/gthmlvhfui.html

throw new RuntimeException("失败", 500);
来源：http://hz.haohaochexian.top/gtealepgxb.html

[U72] PHP：写错误日志
来源：http://hz.feifeiyinyue.top/gtwhapcvew.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuanzx.com/gthfnfpflp.html

[U73] PHP：读取 ini 配置
来源：http://hz.shuidangran.top/gtelbrtptm.html

parse_ini_file("config.ini", true)
来源：http://hz.pycfn.com/gtejxjryyh.html

[U74] PHP：读取环境变量
来源：http://hz.52xcode.cn/gtchrmwmok.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shangyingyoupin.top/gtlmrnywrc.html

[U75] PHP：依赖注入
来源：http://hz.cqqwz.cn/gtgtnclsrj.html

composer require psr/container
来源：http://hz.hnqzz.top/gtuspfvdlw.html

[U76] PHP：简单路由
来源：http://hz.yj20258.top/gtmahrfauv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.316326.xyz/gtxxapukzo.html

[U77] PHP：模板渲染
来源：http://hz.mhx1999.top/gtejikqqca.html

composer require twig/twig
来源：http://hz.feifeiyinyue.top/gtfocnkjao.html

[U78] PHP：单元测试
来源：http://hz.9152youxi.cn/gtnweihwkt.html

composer require --dev phpunit/phpunit
来源：http://hz.zhixingplan.top/gtzytqhdnd.html

[U79] PHP：静态分析
来源：http://hz.sweek.top/gthxvvpshp.html

composer require --dev phpstan/phpstan
来源：http://hz.gzhubu.top/gthnxrueqe.html

[U80] PHP：代码规范修复
来源：http://hz.c1oappe.top/gtjmgviowh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ybcxt.top/gtxyvnnkos.html

[U81] JS：初始化项目
来源：http://hz.dianchejie.cn/gtexrxvtqq.html

npm init -y;  npm i express
来源：http://hz.iojbl.cn/gtgubcdkgl.html

[U82] JS：package.json 脚本
来源：http://hz.yueranfly.top/gtaebrldef.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shanyushiyangkeji.top/gtzuuuwthy.html

[U83] JS：ES Module 导入导出
来源：http://hz.hnqzz.top/gtbvtzlfoh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.mhx1999.top/gtuylsxiec.html

[U84] JS：CommonJS 写法
来源：http://hz.jlsjyb.cn/gteubvbisc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hammf.cn/gtfmgqlilw.html

[U85] JS：可选链
来源：http://hz.ivvv.top/gtlfdyipyk.html

a?.b?.c
来源：http://hz.iojbl.cn/gtcsgymqmx.html

[U86] JS：空值合并
来源：http://hz.dashuyun.cn/gtudxugxth.html

a ?? b
来源：http://hz.tian-w.cn/gtmyonobhj.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gtesoskhyr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gthhqtwtjf.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtkcdvyktg.html

{ ...a, ...b }
来源：http://hz.nanxuanxn.top/gtwqinznpt.html

[U89] JS：数组去重
来源：http://hz.ehwqpu.com/gtkdbymzzy.html

[...new Set(arr)]
来源：http://hz.gzhubu.top/gtyqyanohx.html

[U90] JS：数字数组排序
来源：http://hz.jinghuilouyu.cn/gtxtzwsbpn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtvrylsgnd.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258.top/gtexrpzcyf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.daria6918.cn/gtxyltirwg.html

[U92] JS：深拷贝
来源：http://hz.gotoacloud.top/gtceumfnsk.html

structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtyqdgekve.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtdljildqh.html

`共 ${n} 条`
来源：http://hz.nanxinkj.top/gtpxacgsqo.html

[U94] JS：箭头函数
来源：http://hz.yuanzhike.top/gtnwiqwjhp.html

const double = x => x * 2;
来源：http://hz.fzhhl.top/gtxcafhyct.html

[U95] JS：Promise 包装
来源：http://hz.ehwqpu.com/gtyqemxfna.html

new Promise((resolve, reject) => {})
来源：http://hz.xylfe.cn/gtytthrwzj.html

[U96] JS：async/await 与异常
来源：http://hz.hywenlv.cn/gtzmbmbpux.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtkzzzntgj.html

[U97] JS：并发请求
来源：http://hz.chenjidiqi.icu/gtxmnsvvkw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtdrdmmwig.html

[U98] JS：fetch 带 JSON
来源：http://hz.fzhhl.top/gtztlsdmrv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hongshengwenyu.top/gtljypjfgw.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtycegmmfx.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gtutpjonns.html

[U100] JS：DOM 查询
来源：http://hz.havefunace.top/gtsvbrxjvf.html

document.querySelector(".item")
来源：http://hz.316326.xyz/gtmifvcnxz.html

[U101] JS：classList 操作
来源：http://hz.yj202588.top/gtgggugksd.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtlhetdbqp.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtptwkhndz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xingfuxueyuan.xyz/gtwoxljwuq.html

[U103] JS：定时器
来源：http://hz.zhijiandao.cn/gtgxpzuivv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daria6918.cn/gteqjxewnn.html

[U104] JS：防抖
来源：http://hz.sweek.top/gtklbkccfp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtdcuzcevc.html

[U105] JS：节流
来源：http://hz.cdnleiting.top/gtbbkauktv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydzc1.top/gtblstsolt.html

[U106] JS：日期格式化
来源：http://hz.yuanzhike.top/gtqbevhfbg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnxiangtu.top/gtzjojfosi.html

[U107] JS：数字千分位
来源：http://hz.hammf.cn/gtahepjprl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gotoacloud.top/gtennizvld.html

[U108] JS：随机整数
来源：http://hz.xylfe.cn/gttnzhueki.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj202588.top/gtvsmvgpse.html

[U109] JS：数组分组
来源：http://hz.jqgfzy.top/gtzojlebqw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtdfzvabeq.html

[U110] JS：数组分块
来源：http://hz.feifeiyinyue.top/gtswgytard.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gogol.net.cn/gtpppgysvk.html

[U111] JS：对象转 Map
来源：http://hz.chenjidiqi.icu/gtjhopahwn.html

new Map(Object.entries(obj))
来源：http://hz.ivvv.top/gtgzxqcvtz.html

[U112] JS：字符串补位
来源：http://hz.316326.xyz/gtzlnsogec.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gthmqzyxot.html

[U113] JS：正则替换全部
来源：http://hz.jqgufenzy.top/gtetizxgse.html

s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtrkhyenyp.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gtbbhsbpmv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtiwuzjdha.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gtwnmevjkv.html

crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gthxyhpwau.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtqzknnfat.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtvrfhcyvp.html

[U117] JS：单元测试
来源：http://hz.dianchejie.cn/gtiuziscdm.html

npm i -D vitest;  npx vitest
来源：http://hz.hfpthk.cn/gtdltbxzhp.html

[U118] JS：开发服务器
来源：http://hz.c1oappe.top/gtdtijweyw.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtsbhfzawr.html

[U119] JS：生产构建
来源：http://hz.sufxvd.cn/gtupabbsok.html

npx vite build
来源：http://hz.guannengcc.top/gtxehyhntm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenzaomai.com/gtypsldvak.html

import.meta.env.VITE_API_URL
来源：http://hz.guowangkeji.top/gtugvbtlaj.html

================================================================================
来源：http://hz.aibaodan.cn/gtveonugar.html

统计汇总
来源：http://hz.gogol.net.cn/gtkvfxixrk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvdjenrcu.html

按语言统计（条）：
来源：http://hz.daxiang520.top/gtnpjyhcsu.html

Python ......... 252
来源：http://hz.jqgufenzy.top/gtvmfvnzkv.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtberpsbhd.html

JavaScript ..... 252
来源：http://hz.yuanzhike.top/gtmknejkbo.html

TypeScript ..... 212
来源：http://hz.nwbrower.top/gtpuziohyv.html

Java ........... 212
来源：http://hz.mhx1999.top/gtojwltvru.html

Go ............. 212
来源：http://hz.gogol.net.cn/gtpsdlhoso.html

Ruby ........... 212
来源：http://hz.xylfe.cn/gtkqwbdkef.html

C# ............. 212
来源：http://hz.aibaodan.cn/gtedtkdnaf.html

C .............. 30
来源：http://hz.ppjwa.cn/gtvcdnjpat.html

C++ ............ 30
来源：http://hz.gotoacloud.top/gtesniczmc.html

SQL ............ 90
来源：http://hz.zdqjudy.top/gtupjgtytr.html

Bash ........... 80
来源：http://hz.gaohongyu789.top/gtimrjeakz.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtfgszesmw.html

Swift .......... 15
来源：http://hz.yvedp.cn/gtyfhmsqgq.html

Lua ............ 10
来源：http://hz.pycfn.com/gtrusvxhjb.html

Perl ........... 10
来源：http://hz.gogol.net.cn/gtryynxkxn.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtnragyseu.html

------------------------------------
来源：http://hz.tian-w.cn/gtnuykderv.html

合计 ........... 2106 条
来源：http://hz.fengsongda.top/gtlgoxcooj.html

按章节统计：
来源：http://hz.hnqzz.top/gtdgkjreof.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtjibrilxy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtowiyrztt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtxruwfyct.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtjktxmnll.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuxming.cn/gtbagavote.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.havefunace.top/gtofvalwfg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gthallqoyc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtydjzyidc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtnpvowgkv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.iojbl.cn/gtsvbmkxji.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtwzhhtovn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtqkllwrty.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtcwznkjqh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yueranfly.top/gtztsixixl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtmswxiqce.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtoxhjbdsq.html

Q SQL 专题                              90
来源：http://hz.hongshengwenyu.top/gtvnccdppq.html

R Bash 专题                             80
来源：http://hz.ydzc1.top/gtgvdobmon.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtsrtgfgjh.html

T 其他语言补充                          60
来源：http://hz.52xcode.cn/gtzubuvjly.html

U 高频实用片段                         120
来源：http://hz.zhiwuduotai.top/gtxlvdzayx.html

------------------------------------
来源：http://hz.sufxvd.cn/gtakjmtzll.html

合计                                  2106 条
来源：http://hz.jianghu66.top/gtfnjmeevc.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtneybsoox.html

使用提醒
来源：http://hz.ydzc1.top/gtkwmlclez.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtgypgnivg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.316326.xyz/gtptbuctny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangtech.top/gtciykztmi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtkgabeecp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhaomingkeji.xyz/gtunndypzl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aizwys.cn/gtxcbmsggp.html

—— 文件结束 ——
来源：http://hz.yonumen.top/gtkcuaxwps.html

================================================================================
来源：http://hz.jianghu66.top/gtonnzhygq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aibaodan.cn/gtxjszcxnv.html

Common Programming Examples Cheat Book
来源：http://hz.yonumen.top/gtmljzgsqa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmqqiglgl.html

【收录内容】
来源：http://hz.kuanghao11.cn/gtambavqoq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shzxlz.cn/gtgihqpsrr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenlongwang.top/gtoaykuejq.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gtjcplspcq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.fengsongda.top/gtbyaysrpo.html

【使用说明】
来源：http://hz.chenlongwang.top/gtfcecgume.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.feifeiyinyue.top/gtwbbogmbx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zdqjudy.top/gthmjkcmic.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tianlin.xyz/gtvjwzjgcz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sysykeji.top/gtrtlohnik.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hysaishi.cn/gtaviuqosj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.andypj.xyz/gtkxihtclp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinqigufen.top/gteubvmsee.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tian-w.cn/gtdtogfnqg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.tianlin.xyz/gtrbmpsoly.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ybcxt.top/gtiaznvlbx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.9152youxi.cn/gtqpurynxt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.kuanghao11.cn/gtfkbtrqdj.html

【文件统计】
来源：http://hz.svipenyu.cn/gtcqhsimjp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hammf.cn/gtfsrttuiy.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtzvdifwwo.html

目  录
来源：http://hz.zhongyouzk.top/gtvnhqcwpl.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtrkyrwsud.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hnxiangtu.top/gtrwkhhnly.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtsigieqdd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtswyrltic.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtlfprwihc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.mhx1999.top/gtmxeotmyp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhaomingkeji.xyz/gtxtubsttv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtgnbktvaw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cqqwz.cn/gtjuabrate.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtqqftbzyp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhengqikj.top/gtfqxbqkfu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtubvxgnsz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtocduhgqk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtjwsipovi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.guannengcc.top/gtpdzuicst.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenjidiqi.icu/gtvqzuqmtk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtwaupmefe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.daria6918.cn/gtzfzajgrn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xziqi.cn/gtfphbjnqf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtliqogyxr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtshzzdois.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gttrcgicpf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkcdzmuwj.html

A. 基础语法与类型
来源：http://hz.andypj.xyz/gtyyocpqpr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtltclzvmd.html

[A01] Hello World
来源：http://hz.tian-w.cn/gtydfilyir.html

Py:   print("Hello, World!")
来源：http://hz.redwolf501.top/gtnetnljok.html

PHP:  echo "Hello, World!";
来源：http://hz.yanxiufei.cn/gtqgbbvxht.html

JS:   console.log("Hello, World!");
来源：http://hz.zdqjudy.top/gtpjmqnmil.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.nanxinkj.top/gtmqcjmnjz.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhaomingkeji.xyz/gtobiaotsh.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.redwolf501.top/gtjhxmdvia.html

Ruby: puts "Hello, World!"
来源：http://hz.hammf.cn/gtnxyuwkej.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yongpay.top/gtaclwbkqc.html

[A02] 变量声明与赋值
来源：http://hz.xuanzx.com/gtwokvnzge.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtvpboboja.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gthkhplyew.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jiagoushi.top/gteuknyxvg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj20258888.top/gtvcssbkjz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtmlhphsds.html

Go:   name := "Alex"; age := 20
来源：http://hz.jyoumei.cn/gtelqibnxh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.tianlin.xyz/gtslakzpln.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtolfratfb.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtzpvnivlt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.kuanghao11.cn/gtvkpwyukq.html

PHP:  const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gttrwqbvvl.html

JS:   const PI = 3.14159;
来源：http://hz.tianlin.xyz/gtopdxwihr.html

TS:   const PI: number = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtpxqukpgq.html

Java: static final double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtovydokep.html

Go:   const PI = 3.14159
来源：http://hz.hfpthk.cn/gtdistxtba.html

Ruby: PI = 3.14159
来源：http://hz.tianlin.xyz/gtbefnszxo.html

C#:   const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtlriyofky.html

[A04] 判断变量类型
来源：http://hz.chenlongwang.top/gttetjofiy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinyuanbaomall.cn/gtyaanwvko.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yangfankeji.com/gtvwdrgzpv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangdashe.top/gtulnmaavr.html

TS:   typeof x; x instanceof Date
来源：http://hz.bjfxy.top/gttmkfmqyx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jqgufenzy.top/gtjylsxzmr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.andypj.xyz/gtnupacdor.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gaohongyu789.top/gtkranwaml.html

C#:   x.GetType().Name; x is int
来源：http://hz.nanxuanxn.top/gtfxqohair.html

[A05] 整数除法与取模
来源：http://hz.hammf.cn/gtrnfglthf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ywan-chungtsiang.top/gtwwaxddgg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.fzhhl.top/gtjzmvrhxq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xylfe.cn/gtyuilylty.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxinkj.top/gtslomjafu.html


<!-- 参考信息 -->