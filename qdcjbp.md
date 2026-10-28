代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.jiagoushi.top/gtvpcdwbtq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtvounhlnm.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtqasqbtyl.html

?string $name = null
来源：http://hz.hnxiangtu.top/gtruglglgt.html

[U47] PHP：联合类型
来源：http://hz.cdnleiting.top/gtkbhgvvlh.html

int|string $id
来源：http://hz.nanxuanxn.top/gtkcdrlvpl.html

[U48] PHP：纯枚举
来源：http://hz.xziqi.cn/gtinzcwpse.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtojyexnry.html

[U49] PHP：只读属性
来源：http://hz.ppjwa.cn/gtbfuukocb.html

public readonly string $name
来源：http://hz.guannengcc.top/gticrotuve.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgfzy.top/gtrlvwvefa.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gticziynfd.html

[U51] PHP：数组解构
来源：http://hz.yj202588.top/gtzondyszr.html

[$a, $b] = $arr;
来源：http://hz.vqdsnc.cn/gtibxynhtf.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtsopywrdz.html

$double = fn($x) => $x * 2;
来源：http://hz.jinyuanbaomall.cn/gtgbkitdcb.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtusphpqoq.html

$v = $a ?? $b ?? "default";
来源：http://hz.aizwys.cn/gtkgpcgunc.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangtech.top/gtpdaelutf.html

$obj?->method()
来源：http://hz.jiagoushi.top/gtmvhmmimk.html

[U55] PHP：match 表达式
来源：http://hz.nanxinkj.top/gtbyaulgyk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.vqdsnc.cn/gtxcllwkir.html

[U56] PHP：命名参数
来源：http://hz.xylfe.cn/gtylwxwcja.html

f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtkfifpbdz.html

[U57] PHP：字符串插值
来源：http://hz.shzxlz.cn/gteduegvlt.html

"值: {$a}"
来源：http://hz.quarkkingdee.top/gtdcetsawl.html

[U58] PHP：数组三件套
来源：http://hz.fzhhl.top/gtyoswfvdn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenlongwang.top/gtlvlpozvn.html

[U59] PHP：自定义排序
来源：http://hz.jqgfzy.top/gtebljcrew.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtsurmqugf.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangtech.top/gtceiosmad.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigfzy.top/gtnxquflyp.html

[U61] PHP：正则
来源：http://hz.quarkkingdee.top/gtmqpwmboz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtmggxtero.html

[U62] PHP：日期对象
来源：http://hz.smart0.xyz/gtcnjgjmfx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sweek.top/gtbtrhiqmz.html

[U63] PHP：文件读写
来源：http://hz.guowangkeji.top/gtbjltifif.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydzc1.top/gtjldsocde.html

[U64] PHP：目录遍历
来源：http://hz.gzhubu.top/gtfcxjbzad.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj20258.top/gtspyfgvte.html

[U65] PHP：会话
来源：http://hz.zhaomingkeji.xyz/gtuaomcnwq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhongyouzk.top/gtfyotgfsx.html

[U66] PHP：设置 Cookie
来源：http://hz.yvedp.cn/gturqirnyf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangtech.top/gtugjxmkle.html

[U67] PHP：处理文件上传
来源：http://hz.ybcxt.top/gtvmvcdpoo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtjrafjaxd.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gthpbgccbs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangtech.top/gtezeijbfa.html

[U69] PHP：PDO 预处理
来源：http://hz.ivvv.top/gtghyenwrd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nwbrower.top/gteellgbnb.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtfttygyqq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jianghu66.top/gtgbadtvfz.html

[U71] PHP：抛出异常
来源：http://hz.guannengcc.top/gtzsakhbrn.html

throw new RuntimeException("失败", 500);
来源：http://hz.pycfn.com/gtbrpjethb.html

[U72] PHP：写错误日志
来源：http://hz.hammf.cn/gtizzfokqf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuetiantiany.cn/gtclkqbtuh.html

[U73] PHP：读取 ini 配置
来源：http://hz.cucudq.cn/gtatccuzvh.html

parse_ini_file("config.ini", true)
来源：http://hz.ybcxt.top/gtyiosmkzc.html

[U74] PHP：读取环境变量
来源：http://hz.ivvv.top/gtlufsvxuz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shangyingyoupin.top/gtpnxenyxs.html

[U75] PHP：依赖注入
来源：http://hz.hysaishi.cn/gtfcseyrus.html

composer require psr/container
来源：http://hz.hnxiangtu.top/gtlgfohtzl.html

[U76] PHP：简单路由
来源：http://hz.shzxlz.cn/gtstugoebg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sxryk.cn/gtoavighae.html

[U77] PHP：模板渲染
来源：http://hz.jqgfzy.top/gtqhngccqf.html

composer require twig/twig
来源：http://hz.jqgufenzy.top/gtajevjujy.html

[U78] PHP：单元测试
来源：http://hz.yuxming.cn/gtyopllzfg.html

composer require --dev phpunit/phpunit
来源：http://hz.zhixingplan.top/gtrlmlejep.html

[U79] PHP：静态分析
来源：http://hz.daxiang520.top/gtobxzxovn.html

composer require --dev phpstan/phpstan
来源：http://hz.yj202588.top/gtulqiwulx.html

[U80] PHP：代码规范修复
来源：http://hz.shzxlz.cn/gtvrxwqpsp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigfzy.top/gthegjjjbb.html

[U81] JS：初始化项目
来源：http://hz.yangfankeji.com/gtmbobcbul.html

npm init -y;  npm i express
来源：http://hz.fzhhl.top/gttlfutfes.html

[U82] JS：package.json 脚本
来源：http://hz.yuxming.cn/gtqgbtzxyd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yangfankeji.com/gterazamrt.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuanzhike.top/gtfqnuqpin.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258.top/gtiqppydxm.html

[U84] JS：CommonJS 写法
来源：http://hz.daria6918.cn/gtzssfqdab.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydjk.org.cn/gtxfcipclz.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtcnqowfss.html

a?.b?.c
来源：http://hz.dashuyun.cn/gtkkmgqpem.html

[U86] JS：空值合并
来源：http://hz.quarkkingdee.top/gtsgqetpif.html

a ?? b
来源：http://hz.zdqjudy.top/gtanvbshev.html

[U87] JS：解构默认值
来源：http://hz.daria6918.cn/gthdaytsid.html

const { a = 1, b = 2 } = obj;
来源：http://hz.52xcode.cn/gtpopjinmm.html

[U88] JS：对象展开合并
来源：http://hz.xinyue.icu/gtxjreorom.html

{ ...a, ...b }
来源：http://hz.ehwqpu.com/gteoqgekmg.html

[U89] JS：数组去重
来源：http://hz.guannengcc.top/gtsbkofblz.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gttordjkni.html

[U90] JS：数字数组排序
来源：http://hz.guannengcc.top/gtmnlejqsg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtqaqswtvg.html

[U91] JS：对象键值遍历
来源：http://hz.pengpengdd.cyou/gtiesaueuy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.bjfxy.top/gtsuledqxm.html

[U92] JS：深拷贝
来源：http://hz.gaohongyu789.top/gtuqobjwrn.html

structuredClone(obj)
来源：http://hz.nwbrower.top/gtploktzxb.html

[U93] JS：模板字符串
来源：http://hz.bjfxy.top/gtwrvkyazr.html

`共 ${n} 条`
来源：http://hz.ybcxt.top/gtuklfgxsv.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gthxsvomca.html

const double = x => x * 2;
来源：http://hz.zhiwuduotai.top/gtluafsrdt.html

[U95] JS：Promise 包装
来源：http://hz.pengpengdd.cyou/gtjdmrpzpj.html

new Promise((resolve, reject) => {})
来源：http://hz.havefunace.top/gtqtbyuykd.html

[U96] JS：async/await 与异常
来源：http://hz.shzxlz.cn/gtdlksddxl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtyerggjve.html

[U97] JS：并发请求
来源：http://hz.cucudq.cn/gtjcaknupc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtswzrrowm.html

[U98] JS：fetch 带 JSON
来源：http://hz.yangfankeji.com/gtfwaxgzfx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ppjwa.cn/gtszwsmgqx.html

[U99] JS：事件监听
来源：http://hz.shanyushiyangtech.top/gtuczfxztg.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtjliqdgdx.html

[U100] JS：DOM 查询
来源：http://hz.yueranfly.top/gtvvsczwmh.html

document.querySelector(".item")
来源：http://hz.hammf.cn/gtaeimkuzl.html

[U101] JS：classList 操作
来源：http://hz.yvedp.cn/gtjvvcuinx.html

el.classList.toggle("active")
来源：http://hz.9152youxi.cn/gtbnliyxem.html

[U102] JS：本地存储
来源：http://hz.aibaodan.cn/gtrkkwksbn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hywenlv.cn/gtdbwooobp.html

[U103] JS：定时器
来源：http://hz.bjfxy.top/gtuvfewcva.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gtomokqxpb.html

[U104] JS：防抖
来源：http://hz.xziqi.cn/gtcxzqatft.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtjwhqpdpi.html

[U105] JS：节流
来源：http://hz.fengsongda.top/gttbtqjboj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.guowangkeji.top/gtfvctrkql.html

[U106] JS：日期格式化
来源：http://hz.haohaochexian.top/gthjfxxkhk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guowangkeji.top/gtrsdmowts.html

[U107] JS：数字千分位
来源：http://hz.ybcxt.top/gtzokqjzsm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.c1oappe.top/gtyrxbavjp.html

[U108] JS：随机整数
来源：http://hz.shuidangran.top/gtmbjqjrcv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtazkzifie.html

[U109] JS：数组分组
来源：http://hz.0kj1m.cn/gtdpljadtn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtiifjfqbh.html

[U110] JS：数组分块
来源：http://hz.yvedp.cn/gtvmhzpomc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.quarkkingdee.top/gtngqlzrpu.html

[U111] JS：对象转 Map
来源：http://hz.yvedp.cn/gtgnvsujlc.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtlchiqxtg.html

[U112] JS：字符串补位
来源：http://hz.c1oappe.top/gtgdopelbt.html

"7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtqrqrugpg.html

[U113] JS：正则替换全部
来源：http://hz.yj20258.top/gtzwqjsagr.html

s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtygclgcrl.html

[U114] JS：JSON 深比较
来源：http://hz.shangyingyoupin.top/gtfsdbludx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtrirljtyv.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gtyqakyktc.html

crypto.randomUUID()
来源：http://hz.sxryk.cn/gtuwhtpjwy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtoezyxsot.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gtmovmjnqj.html

[U117] JS：单元测试
来源：http://hz.0kj1m.cn/gtuooihbqc.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gtuhhlfwha.html

[U118] JS：开发服务器
来源：http://hz.jlsjyb.cn/gtseukqkpn.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtanlmxtfn.html

[U119] JS：生产构建
来源：http://hz.yj202588.top/gtstgawrow.html

npx vite build
来源：http://hz.ydzc1.top/gtjqtjuvty.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.fzhhl.top/gtvviztapq.html

import.meta.env.VITE_API_URL
来源：http://hz.guowangkeji.top/gtdjzehlpt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gticktdrpp.html

统计汇总
来源：http://hz.jinghuilouyu.cn/gttoeluiwp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteuzjveyz.html

按语言统计（条）：
来源：http://hz.nwbrower.top/gtwxyiuaec.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtekyydspt.html

PHP ............ 252
来源：http://hz.shzxlz.cn/gtwpmqjznb.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtoyayupcu.html

TypeScript ..... 212
来源：http://hz.zhixingplan.top/gtljfuxiea.html

Java ........... 212
来源：http://hz.yuxming.cn/gtxfisffhx.html

Go ............. 212
来源：http://hz.aibaodan.cn/gtkfuigdbt.html

Ruby ........... 212
来源：http://hz.gotoacloud.top/gtvvekzaxu.html

C# ............. 212
来源：http://hz.birdmap.top/gtxtafiekd.html

C .............. 30
来源：http://hz.xziqi.cn/gtsvfphijh.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gthrgsoxzo.html

SQL ............ 90
来源：http://hz.zdqjudy.top/gtdwexkcik.html

Bash ........... 80
来源：http://hz.chenzaomai.com/gtgjzyfcre.html

Kotlin ......... 15
来源：http://hz.dianchejie.cn/gtqwytziyt.html

Swift .......... 15
来源：http://hz.iojbl.cn/gthogpakvt.html

Lua ............ 10
来源：http://hz.xziqi.cn/gtwuhlvtmx.html

Perl ........... 10
来源：http://hz.xylfe.cn/gthpxsxpnk.html

Scala .......... 10
来源：http://hz.9152youxi.cn/gththctjpf.html

------------------------------------
来源：http://hz.yueranfly.top/gtxaxooaez.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gtwtexcoxu.html

按章节统计：
来源：http://hz.c1oappe.top/gtvxjmyook.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhixingplan.top/gtbumjlooq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtqfwqavve.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtxhqqcavm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.guannengcc.top/gtifpspqno.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenjidiqi.icu/gtneuqtzxz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sxryk.cn/gtoyzsuzrr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gttcngwsnd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtnwtqjqpn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtgqeztbws.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtwkphyukr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtqlsrwpob.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtysiueirl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtksjaumbw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtwcjbfpgc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhixingplan.top/gteovgmqct.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtvpiadpxc.html

Q SQL 专题                              90
来源：http://hz.svipenyu.cn/gtasyeevms.html

R Bash 专题                             80
来源：http://hz.xziqi.cn/gtbrogdyqs.html

S C / C++ 专题                          60
来源：http://hz.yanxiufei.cn/gtrvhvkdpx.html

T 其他语言补充                          60
来源：http://hz.quarkkingdee.top/gtamlqngqz.html

U 高频实用片段                         120
来源：http://hz.cashguo.top/gtkrkctvyh.html

------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtdkezhmwe.html

合计                                  2106 条
来源：http://hz.fzhhl.top/gtckahhwhm.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtwnljkeyw.html

使用提醒
来源：http://hz.wangshuangyany.cn/gtoltaxcnh.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtdypfyuoe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cashguo.top/gtntstvfmp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sxryk.cn/gtmskxfgze.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenzaomai.com/gtgqtublxb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cashguo.top/gtqjqucxbz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jianghu66.top/gtfslbcvkz.html

—— 文件结束 ——
来源：http://hz.zhixingplan.top/gtsjbaceib.html

================================================================================
来源：http://hz.shzxlz.cn/gtpdnjkshi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cashguo.top/gtrbjsbyfc.html

Common Programming Examples Cheat Book
来源：http://hz.ivvv.top/gtppfibgnf.html

================================================================================
来源：http://hz.yuanzhike.top/gtvlnqlpxq.html

【收录内容】
来源：http://hz.zhoulong.xyz/gtpjamzawb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xziqi.cn/gteblbboua.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tianlin.xyz/gteztwnhpl.html

SQL · Bash · C · C++
来源：http://hz.mhx1999.top/gtkvxfowch.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ppjwa.cn/gtpnigwnzo.html

【使用说明】
来源：http://hz.tianlin.xyz/gtsdunrqmd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daria6918.cn/gteqeuybfc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.svipenyu.cn/gtayjxvdxf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jqgfzy.top/gtwwjawrin.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhongyouzk.top/gtrrvybqtw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yanxiufei.cn/gtrvqinmhw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gtdnbwezac.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.bjfxy.top/gtcuxemjso.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cucudq.cn/gtthkmdikx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinyuanbaomall.cn/gtoyznzozb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gogol.net.cn/gtqvpukybx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.svipenyu.cn/gttqpvdasv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shangyingyoupin.top/gtuoiywieh.html

【文件统计】
来源：http://hz.xingfuxueyuan.xyz/gtwphqttrg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yongpay.top/gtblpajeji.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtfhuuebmn.html

目  录
来源：http://hz.ydzc1.top/gtqfysynfl.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtvnysidun.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ybcxt.top/gtkietllgy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtfdkvyxxt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gteubkivlj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gtjtpzztgx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.chenjidiqi.icu/gtulnpztdn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hywenlv.cn/gtsxwgawsu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gthtnrqfax.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nanxinkj.top/gthbgqxjxo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtqqfgnjsy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gzhubu.top/gtqmqkczyw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtotymrfms.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtykroutxz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtmzanfokm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.fzhhl.top/gtmqeymunx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dashuyun.cn/gtvegzyisa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtqrobffor.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jinyuanbaomall.cn/gtnyescssx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sweek.top/gtdoteljwv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.haohaochexian.top/gtocdfhbxr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtqpmiykjy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.dianchejie.cn/gtiyqkplge.html

================================================================================
来源：http://hz.gzhubu.top/gtausvofom.html

A. 基础语法与类型
来源：http://hz.chenlongwang.top/gtnyuwgjgq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrgugkonc.html

[A01] Hello World
来源：http://hz.fzhhl.top/gtofewibqq.html

Py:   print("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtyfxhcosf.html

PHP:  echo "Hello, World!";
来源：http://hz.smart0.xyz/gtatqytmxk.html

JS:   console.log("Hello, World!");
来源：http://hz.shzxlz.cn/gteahlqdxb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hywenlv.cn/gtkcdockcg.html

Java: System.out.println("Hello, World!");
来源：http://hz.cucudq.cn/gtpfuunycn.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtqhjzqvrn.html

Ruby: puts "Hello, World!"
来源：http://hz.jyoumei.cn/gtdwdaxtgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.havefunace.top/gthndjnumb.html

[A02] 变量声明与赋值
来源：http://hz.xylfe.cn/gtpvlrjsdy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.smart0.xyz/gtqktfbnpb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yj20258.top/gtobddblek.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hnxiangtu.top/gtadookowl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.mhx1999.top/gtcxivmjbb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtvdcdfdap.html

Go:   name := "Alex"; age := 20
来源：http://hz.dashuyun.cn/gtksojlbtb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtfeudiwna.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.tianlin.xyz/gtbclycufu.html

[A03] 常量定义
来源：http://hz.gotoacloud.top/gtkmfvomzw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj202588.top/gtheuxdmkm.html

PHP:  const PI = 3.14159;
来源：http://hz.jinqigufen.top/gtppzdjwja.html

JS:   const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtgsuafpog.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhoulong.xyz/gtkpvqwsbm.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtydmzanat.html

Go:   const PI = 3.14159
来源：http://hz.gzhubu.top/gthipnhjeb.html

Ruby: PI = 3.14159
来源：http://hz.jiagoushi.top/gtwpfkkvzn.html

C#:   const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtrlqfdaai.html

[A04] 判断变量类型
来源：http://hz.wangdashe.top/gtmiteobqq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.meibo888.top/gtenvjjtwv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sweek.top/gtrfbestks.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.daxiang520.top/gtlasofxue.html

TS:   typeof x; x instanceof Date
来源：http://hz.jqgufenzy.top/gtmnoorgrl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yongpay.top/gtpqjyvufx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gtjlivvvvz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gtuotzikuz.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtcmaftqsy.html

[A05] 整数除法与取模
来源：http://hz.havefunace.top/gttpxecmdn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhixingplan.top/gtflcmiuqq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.haohaochexian.top/gtgvlivowj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.haohaochexian.top/gtvmjlbhgk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zycfv.cn/gthkkhsyoa.html


<!-- 参考信息 -->