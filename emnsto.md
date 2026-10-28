代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtmxkvwcbz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gthtpytgvb.html

[U46] PHP：可空类型
来源：http://hz.hywenlv.cn/gtrchbdofm.html

?string $name = null
来源：http://hz.xuetiantiany.cn/gtgpwqdchl.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtgrwnlpoy.html

int|string $id
来源：http://hz.shuidangran.top/gtyrxflcqy.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtamxlkfxe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tanke756.top/gtijkfcwzo.html

[U49] PHP：只读属性
来源：http://hz.ivvv.top/gtnrledjdt.html

public readonly string $name
来源：http://hz.ywan-chungtsiang.top/gtgazlciwb.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtkvhhdfgi.html

public function __construct(private int $id) {}
来源：http://hz.cheryme.top/gtkvvwaevl.html

[U51] PHP：数组解构
来源：http://hz.jinqigfzy.top/gtpssrxlhw.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtziyqxffc.html

[U52] PHP：箭头函数
来源：http://hz.jiagoushi.top/gtcolwavke.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gtdstgxwhq.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigfzy.top/gtypwtpjbx.html

$v = $a ?? $b ?? "default";
来源：http://hz.shuidangran.top/gtgklkfxeo.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtrjohaioe.html

$obj?->method()
来源：http://hz.yonumen.top/gtwecdodsg.html

[U55] PHP：match 表达式
来源：http://hz.hysaishi.cn/gtrwmgtkwq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.svipenyu.cn/gtyulegphw.html

[U56] PHP：命名参数
来源：http://hz.nanxinkj.top/gtqjhcjedi.html

f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtkzdhuobn.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtrtgpwadu.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtubgxpgnd.html

[U58] PHP：数组三件套
来源：http://hz.yongpay.top/gtmtjephwe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yongpay.top/gtbztyfqtt.html

[U59] PHP：自定义排序
来源：http://hz.xuanzx.com/gtznmvekmx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtxiunwquz.html

[U60] PHP：JSON 编解码
来源：http://hz.yueranfly.top/gtarjurout.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hywenlv.cn/gtzpgibusq.html

[U61] PHP：正则
来源：http://hz.shzxlz.cn/gtivtgtahs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtspambhjk.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtqzxnrftw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinghuilouyu.cn/gtgqczhkun.html

[U63] PHP：文件读写
来源：http://hz.tian-w.cn/gtqgtwryqr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangshuangyany.cn/gtagsiiymh.html

[U64] PHP：目录遍历
来源：http://hz.xziqi.cn/gtslgtrfxc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cucudq.cn/gtwqmfwxbm.html

[U65] PHP：会话
来源：http://hz.daxiang520.top/gtdwvguipw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cashguo.top/gtvfazsnsa.html

[U66] PHP：设置 Cookie
来源：http://hz.wangdashe.top/gtyfzqyjai.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.feifeiyinyue.top/gtyuxfvkgx.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtjbrnqwrn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhaomingkeji.xyz/gtzzroimmi.html

[U68] PHP：PDO 连接
来源：http://hz.yj202588.top/gtgwrontpm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtiuyupbpg.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtphixfkkb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.pycfn.com/gtdsckezji.html

[U70] PHP：PDO 事务
来源：http://hz.gzhubu.top/gtnzkqcuvu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tanke756.top/gtyehhqkmh.html

[U71] PHP：抛出异常
来源：http://hz.cucudq.cn/gtxckwdsjh.html

throw new RuntimeException("失败", 500);
来源：http://hz.vqdsnc.cn/gtlipngkxi.html

[U72] PHP：写错误日志
来源：http://hz.xinyue.icu/gtuipasqrm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ivvv.top/gtstnfhpvg.html

[U73] PHP：读取 ini 配置
来源：http://hz.dianchejie.cn/gtemmkfwpr.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtrlmrteth.html

[U74] PHP：读取环境变量
来源：http://hz.guowangkeji.top/gtoaftqscg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtwdmohsyq.html

[U75] PHP：依赖注入
来源：http://hz.shuidangran.top/gtgykrazat.html

composer require psr/container
来源：http://hz.jqgufenzy.top/gtsfvityfi.html

[U76] PHP：简单路由
来源：http://hz.svipenyu.cn/gttbphxcpl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.mhx1999.top/gtricjjgrd.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gtzrmirlnd.html

composer require twig/twig
来源：http://hz.52xcode.cn/gtiylhdmph.html

[U78] PHP：单元测试
来源：http://hz.aibaodan.cn/gtoqkzuvnw.html

composer require --dev phpunit/phpunit
来源：http://hz.52xcode.cn/gthrvpastl.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtukfaatvo.html

composer require --dev phpstan/phpstan
来源：http://hz.jinqigfzy.top/gtvpxoqcpx.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtizbrtokz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.0kj1m.cn/gtthirmray.html

[U81] JS：初始化项目
来源：http://hz.gogol.net.cn/gterpkcbkb.html

npm init -y;  npm i express
来源：http://hz.yonumen.top/gtwnfciiuq.html

[U82] JS：package.json 脚本
来源：http://hz.sweek.top/gtbjxrsprd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.9152youxi.cn/gtfjeqwhxb.html

[U83] JS：ES Module 导入导出
来源：http://hz.9152youxi.cn/gtuxltxxaq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtupbqbuts.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtclondxao.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gthjxrkobu.html

[U85] JS：可选链
来源：http://hz.gaohongyu789.top/gtsqszjffr.html

a?.b?.c
来源：http://hz.ybcxt.top/gtwaqvsovl.html

[U86] JS：空值合并
来源：http://hz.316326.xyz/gtudxvfybc.html

a ?? b
来源：http://hz.guannengcc.top/gtrzjfgiqd.html

[U87] JS：解构默认值
来源：http://hz.xylfe.cn/gtefnytkbx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.316326.xyz/gtujiivjta.html

[U88] JS：对象展开合并
来源：http://hz.316326.xyz/gtoknyqlfv.html

{ ...a, ...b }
来源：http://hz.daxiang520.top/gtixokfzvo.html

[U89] JS：数组去重
来源：http://hz.sysykeji.top/gtovpbnqhp.html

[...new Set(arr)]
来源：http://hz.zycfv.cn/gtpkaoigvx.html

[U90] JS：数字数组排序
来源：http://hz.52xcode.cn/gthafhixox.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtsvmwwnfi.html

[U91] JS：对象键值遍历
来源：http://hz.hywenlv.cn/gtxvkaubkw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ydjk.org.cn/gtprnvwozx.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gteznuxebk.html

structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtxumjakla.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtmbyptmfa.html

`共 ${n} 条`
来源：http://hz.pycfn.com/gtzgmytztd.html

[U94] JS：箭头函数
来源：http://hz.sysykeji.top/gtblrmmrrd.html

const double = x => x * 2;
来源：http://hz.cucudq.cn/gtkcnpcopa.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gtyvnzzetz.html

new Promise((resolve, reject) => {})
来源：http://hz.svipenyu.cn/gteudfmput.html

[U96] JS：async/await 与异常
来源：http://hz.yueranfly.top/gtcjjqucwa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtmiuhahib.html

[U97] JS：并发请求
来源：http://hz.haohaochexian.top/gtcczsstcv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtwzogurkn.html

[U98] JS：fetch 带 JSON
来源：http://hz.kuanghao11.cn/gtyxpexyvc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shanyushiyangtech.top/gtztqwfsjt.html

[U99] JS：事件监听
来源：http://hz.hnqzz.top/gtnuedndnv.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtcerqhbuq.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtckgnolcp.html

document.querySelector(".item")
来源：http://hz.chenlongwang.top/gtjrfdiduy.html

[U101] JS：classList 操作
来源：http://hz.zhengqikj.top/gtahthfnyu.html

el.classList.toggle("active")
来源：http://hz.yuxming.cn/gtnphfmlfq.html

[U102] JS：本地存储
来源：http://hz.svipenyu.cn/gttddygxtf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gzhubu.top/gtskssdojp.html

[U103] JS：定时器
来源：http://hz.andypj.xyz/gtbljlvkxd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenzaomai.com/gtqlgahnaz.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtopwiqund.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtjyrwfhut.html

[U105] JS：节流
来源：http://hz.zhengqikj.top/gtluerooiw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shangyingyoupin.top/gtouotmpce.html

[U106] JS：日期格式化
来源：http://hz.9152youxi.cn/gtukpfwrff.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guannengcc.top/gtxqyfedde.html

[U107] JS：数字千分位
来源：http://hz.316326.xyz/gtdjoqdedj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtzgkinptv.html

[U108] JS：随机整数
来源：http://hz.jinyuanbaomall.cn/gtkfakvnao.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtyuhjlhpu.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtlfksucpd.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtvadsxeur.html

[U110] JS：数组分块
来源：http://hz.aizwys.cn/gtegfwsusr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj202588.top/gtbdvvnizc.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gtphicnktu.html

new Map(Object.entries(obj))
来源：http://hz.jlsjyb.cn/gttkhidohn.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gthpkiqtyu.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtctryygfp.html

[U113] JS：正则替换全部
来源：http://hz.sweek.top/gtybbjtjld.html

s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtflhhrryy.html

[U114] JS：JSON 深比较
来源：http://hz.shanyushiyangkeji.top/gtxdbsiaei.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtubjrrauh.html

[U115] JS：生成 UUID
来源：http://hz.hongshengwenyu.top/gtkmkfnelk.html

crypto.randomUUID()
来源：http://hz.yongpay.top/gtnkpzmrdd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhengqikj.top/gtsdieraia.html

/** @param {string} name */ function f(name) {}
来源：http://hz.haohaochexian.top/gtjsvvmtqr.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtgfntcghs.html

npm i -D vitest;  npx vitest
来源：http://hz.zhixingplan.top/gtobgtguwo.html

[U118] JS：开发服务器
来源：http://hz.0kj1m.cn/gtcapumbin.html

npm i -D vite;  npx vite
来源：http://hz.svipenyu.cn/gtwjtbpesb.html

[U119] JS：生产构建
来源：http://hz.ppjwa.cn/gtouxddrsm.html

npx vite build
来源：http://hz.jinghuilouyu.cn/gtpujmkmet.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhongyouzk.top/gtjfvnvwhs.html

import.meta.env.VITE_API_URL
来源：http://hz.sufxvd.cn/gthnxehubd.html

================================================================================
来源：http://hz.yj20258.top/gthhuuxudu.html

统计汇总
来源：http://hz.shuidangran.top/gtggvolxen.html

================================================================================
来源：http://hz.shzxlz.cn/gtbsqtmxay.html

按语言统计（条）：
来源：http://hz.aibaodan.cn/gtyarzodky.html

Python ......... 252
来源：http://hz.gzhubu.top/gtzdgqtxfm.html

PHP ............ 252
来源：http://hz.nwbrower.top/gtljcrlobc.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gttstxglwv.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtwwcligyz.html

Java ........... 212
来源：http://hz.yuanzhike.top/gtkgogmdlp.html

Go ............. 212
来源：http://hz.zhoulong.xyz/gtelicglau.html

Ruby ........... 212
来源：http://hz.quarkkingdee.top/gtszqeffho.html

C# ............. 212
来源：http://hz.jiagoushi.top/gtauaoeygo.html

C .............. 30
来源：http://hz.xuanzx.com/gtzcsjraes.html

C++ ............ 30
来源：http://hz.jinqigufen.top/gtkvqbbqdg.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtithsrsvi.html

Bash ........... 80
来源：http://hz.quarkkingdee.top/gtdowolako.html

Kotlin ......... 15
来源：http://hz.yvedp.cn/gtogfvzhzt.html

Swift .......... 15
来源：http://hz.yongpay.top/gtmekdehic.html

Lua ............ 10
来源：http://hz.zhoulong.xyz/gtwzuzacqy.html

Perl ........... 10
来源：http://hz.xuetiantiany.cn/gtgzqnfmux.html

Scala .......... 10
来源：http://hz.shanyushiyangtech.top/gttnydnsjo.html

------------------------------------
来源：http://hz.yj20258888.top/gtuuyinomm.html

合计 ........... 2106 条
来源：http://hz.nwbrower.top/gtuofcyhjt.html

按章节统计：
来源：http://hz.jinyuanbaomall.cn/gtzabcvjui.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.mhx1999.top/gtvobzkacn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtahitxcop.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtjqtkwdrs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtqfpudzzf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.snrcjt.cn/gtgpfpgcsi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.9152youxi.cn/gtgonjqrgx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtuivsjxen.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtqdbjjpwc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtlylqmxrl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtfnqjoklt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtgxfhwmmc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtzvwdgmwg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtlyqhtanq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ybcxt.top/gtnxfrzihs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ivvv.top/gtqxgvxslc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtedyevxyz.html

Q SQL 专题                              90
来源：http://hz.jqgufenzy.top/gtrqispljb.html

R Bash 专题                             80
来源：http://hz.tianlin.xyz/gtiabeojyr.html

S C / C++ 专题                          60
来源：http://hz.hfpthk.cn/gthygfhvga.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtmjyeoeus.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtaznwtgps.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtphrixlua.html

合计                                  2106 条
来源：http://hz.sweek.top/gthtvrouka.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtsmbhrlly.html

使用提醒
来源：http://hz.cdnleiting.top/gtoknjrvuw.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtyervtiwh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258888.top/gtldlpxchg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xziqi.cn/gttqrdyqbv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.kuanghao11.cn/gtlerotdxy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tianlin.xyz/gtlvrfhlrg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.52xcode.cn/gtdihyzykv.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gtuqyfjmwi.html

================================================================================
来源：http://hz.guowangkeji.top/gtfmbusedj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yongpay.top/gtyrrhenhi.html

Common Programming Examples Cheat Book
来源：http://hz.havefunace.top/gtqemarnnf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmzkiudca.html

【收录内容】
来源：http://hz.jinghuilouyu.cn/gtwsdtztsn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gogol.net.cn/gtugqbmgre.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxuanxn.top/gtaiyqmrxb.html

SQL · Bash · C · C++
来源：http://hz.tanke756.top/gtyqzdysoj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.aibaodan.cn/gtokzvjuva.html

【使用说明】
来源：http://hz.sufxvd.cn/gtvkcgyote.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hongshengwenyu.top/gtuvqjjhci.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtdwnujkln.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sweek.top/gtthutxvuk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.birdmap.top/gtypnlycnn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhoulong.xyz/gthhikgawt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sweek.top/gtnlchydnv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cheryme.top/gtqdjbxkxk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shangyingyoupin.top/gthkqgeecv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtrynqsbag.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.52xcode.cn/gtspbqtjam.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sweek.top/gtsmfcxqns.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cdnleiting.top/gtmpapahhh.html

【文件统计】
来源：http://hz.yj20258888.top/gtiqvriudk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hammf.cn/gtlgrcskuh.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtxxkaznpy.html

目  录
来源：http://hz.iojbl.cn/gtjufaspxc.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtpfbbgboh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hysaishi.cn/gtlrkwhdxx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtccjrlvcf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtghljcbsg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shuidangran.top/gttzxnvkpj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hysaishi.cn/gtposrzsoy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hongshengwenyu.top/gtpfknotjj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jianghu66.top/gtscwegrnz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenlongwang.top/gtuhzbzpgd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtgdyqfrsg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.nwbrower.top/gtmzcxkiim.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtznfwsclt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtnwwqefsq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtfstokvcs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sweek.top/gtayqgmrsh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xuetiantiany.cn/gtyulmksdf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtznwzmuzm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.smart0.xyz/gtkvvuzhga.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydzc1.top/gtswnlzxre.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.feifeiyinyue.top/gtvjrxooja.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtceindneo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtxmtpkcox.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcpygjtku.html

A. 基础语法与类型
来源：http://hz.0kj1m.cn/gtfguxgtxd.html

================================================================================
来源：http://hz.iojbl.cn/gtyfpgoqie.html

[A01] Hello World
来源：http://hz.xinyue.icu/gtnvscwwak.html

Py:   print("Hello, World!")
来源：http://hz.nanxinkj.top/gtxwlgxxqo.html

PHP:  echo "Hello, World!";
来源：http://hz.xziqi.cn/gthuddkweb.html

JS:   console.log("Hello, World!");
来源：http://hz.xinyue.icu/gtklzzytfc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wangdashe.top/gtexeatqdv.html

Java: System.out.println("Hello, World!");
来源：http://hz.cqqwz.cn/gtvdikwlsj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.daria6918.cn/gtqbyjicei.html

Ruby: puts "Hello, World!"
来源：http://hz.dashuyun.cn/gttqxrfaxi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jqgufenzy.top/gteqimcyoe.html

[A02] 变量声明与赋值
来源：http://hz.meibo888.top/gtupupxzaz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hnqzz.top/gtsytzoerv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.haohaochexian.top/gtsrnckimw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cdnleiting.top/gtqnfpraxt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhaomingkeji.xyz/gtwsiusqie.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xylfe.cn/gtnyppnbup.html

Go:   name := "Alex"; age := 20
来源：http://hz.sysykeji.top/gthhdarpob.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gaohongyu789.top/gtitbzfpcs.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.kuanghao11.cn/gtueknxofe.html

[A03] 常量定义
来源：http://hz.yangfankeji.com/gtcgywkszu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guannengcc.top/gtdmtffvbm.html

PHP:  const PI = 3.14159;
来源：http://hz.yueranfly.top/gtgqfbkobs.html

JS:   const PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtjptdvkzj.html

TS:   const PI: number = 3.14159;
来源：http://hz.jiagoushi.top/gtgoohepba.html

Java: static final double PI = 3.14159;
来源：http://hz.zdqjudy.top/gthaygpkkz.html

Go:   const PI = 3.14159
来源：http://hz.cqqwz.cn/gtwcnllyvh.html

Ruby: PI = 3.14159
来源：http://hz.jianghu66.top/gtslvedklw.html

C#:   const double PI = 3.14159;
来源：http://hz.yj20258.top/gtaltmtlef.html

[A04] 判断变量类型
来源：http://hz.zhiwuduotai.top/gtltdujeps.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zdqjudy.top/gtcgkmbtqy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guannengcc.top/gtuvwwzwup.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.redwolf501.top/gtpyhwpwsw.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydjk.org.cn/gtacxksfoq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gteogylpzj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gotoacloud.top/gtyhohwgal.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xingfuxueyuan.xyz/gtiaprmgob.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj20258.top/gtwtnfhkfw.html

[A05] 整数除法与取模
来源：http://hz.zhongyouzk.top/gtshczzfqu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.0kj1m.cn/gtxbaerpls.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hongshengwenyu.top/gtcygggfwg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtrfksdcec.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhixingplan.top/gtriiwjjvc.html


<!-- 参考信息 -->