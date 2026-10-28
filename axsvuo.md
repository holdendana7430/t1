代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hz.aibaodan.cn/gtapltgdes.html

sys.stdout.isatty()
来源：http://hz.svipenyu.cn/gtzrqnokqv.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gtsszsjhks.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtlwdaxpif.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtjcecpjbt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.316326.xyz/gtdmkcebsb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtvwmedeig.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.bjfxy.top/gtutbzmiex.html

[U43] PHP：声明命名空间
来源：http://hz.yongpay.top/gthtfqpawo.html

namespace App\Http;
来源：http://hz.yj20258.top/gtfzhjvpwn.html

[U44] PHP：开启严格类型
来源：http://hz.hnxiangtu.top/gtrjksmfen.html

declare(strict_types=1);
来源：http://hz.shangyingyoupin.top/gteuguzmhp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.haohaochexian.top/gtjrxvmjqv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtbfnaozkr.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtfqjrixqb.html

?string $name = null
来源：http://hz.yuanzhike.top/gtkkzhqhlx.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtrssjqycg.html

int|string $id
来源：http://hz.dianchejie.cn/gtrgebhnqc.html

[U48] PHP：纯枚举
来源：http://hz.smart0.xyz/gtydlzmqsw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yonumen.top/gtonsmtwfx.html

[U49] PHP：只读属性
来源：http://hz.pengpengdd.cyou/gtjazjddpy.html

public readonly string $name
来源：http://hz.hammf.cn/gthksprgbs.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtyuuslzxp.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtdqiqwqkk.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtyejvyhwu.html

[$a, $b] = $arr;
来源：http://hz.xinyue.icu/gtpfwtecfa.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtqgzlyyrp.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtmsrdzetr.html

[U53] PHP：空合并运算符
来源：http://hz.ybcxt.top/gtyfknuscx.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtcjvrmcov.html

[U54] PHP：空安全调用
来源：http://hz.zycfv.cn/gtzxhiywir.html

$obj?->method()
来源：http://hz.hongshengwenyu.top/gtfediygrv.html

[U55] PHP：match 表达式
来源：http://hz.yanxiufei.cn/gtyfowjntv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.iojbl.cn/gtbgnthpdt.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gtdorgzydz.html

f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtoxfjebsj.html

[U57] PHP：字符串插值
来源：http://hz.ywan-chungtsiang.top/gttnkxjfie.html

"值: {$a}"
来源：http://hz.hnqzz.top/gttcwdwdkt.html

[U58] PHP：数组三件套
来源：http://hz.ywan-chungtsiang.top/gtzzzsname.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtpllylwma.html

[U59] PHP：自定义排序
来源：http://hz.ybcxt.top/gtukclcbkn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtyjsxorit.html

[U60] PHP：JSON 编解码
来源：http://hz.ppjwa.cn/gthjaoevva.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhoulong.xyz/gtfaoxzzep.html

[U61] PHP：正则
来源：http://hz.cheryme.top/gttznainbe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtijdrgjna.html

[U62] PHP：日期对象
来源：http://hz.mhx1999.top/gtzyzamwac.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.andypj.xyz/gtpyprolxa.html

[U63] PHP：文件读写
来源：http://hz.316326.xyz/gtpudgvtrr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yangfankeji.com/gtqtxczxlf.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtmhmpwlyn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydjk.org.cn/gteydujhkb.html

[U65] PHP：会话
来源：http://hz.hnqzz.top/gtfkvgudvp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhijiandao.cn/gturtnkiwp.html

[U66] PHP：设置 Cookie
来源：http://hz.chenlongwang.top/gtitweyunj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jlsjyb.cn/gtrzzpazsi.html

[U67] PHP：处理文件上传
来源：http://hz.sufxvd.cn/gtpmgelmuk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shzxlz.cn/gtjqhngema.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtqznayldh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jyoumei.cn/gtfslmttvm.html

[U69] PHP：PDO 预处理
来源：http://hz.zdqjudy.top/gtttypzxkt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yanxiufei.cn/gtoqfrkrlz.html

[U70] PHP：PDO 事务
来源：http://hz.chenlongwang.top/gtzqsqaocv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.tianlin.xyz/gtdbqmpruv.html

[U71] PHP：抛出异常
来源：http://hz.hfpthk.cn/gtltilferk.html

throw new RuntimeException("失败", 500);
来源：http://hz.andypj.xyz/gtsiznloix.html

[U72] PHP：写错误日志
来源：http://hz.havefunace.top/gtrmgxzubp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenzaomai.com/gtvuhuajby.html

[U73] PHP：读取 ini 配置
来源：http://hz.yueranfly.top/gtbamjipis.html

parse_ini_file("config.ini", true)
来源：http://hz.xylfe.cn/gtcvodpdqu.html

[U74] PHP：读取环境变量
来源：http://hz.shuidangran.top/gtnjegmxul.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinyuanbaomall.cn/gtqrulgbnd.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtgniszbai.html

composer require psr/container
来源：http://hz.daria6918.cn/gtwmhsglcb.html

[U76] PHP：简单路由
来源：http://hz.yonumen.top/gtsszryjbm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.redwolf501.top/gtubuxjslz.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gtinlqmyjv.html

composer require twig/twig
来源：http://hz.zhaomingkeji.xyz/gtfihpsqze.html

[U78] PHP：单元测试
来源：http://hz.sweek.top/gteodwetgi.html

composer require --dev phpunit/phpunit
来源：http://hz.yvedp.cn/gtaqkzxxhv.html

[U79] PHP：静态分析
来源：http://hz.haohaochexian.top/gtyngbkmyp.html

composer require --dev phpstan/phpstan
来源：http://hz.cqqwz.cn/gtweoidzsv.html

[U80] PHP：代码规范修复
来源：http://hz.jinghuilouyu.cn/gtzwgrgsbo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jqgfzy.top/gtgoxtoups.html

[U81] JS：初始化项目
来源：http://hz.zhiwuduotai.top/gtsvgtyutt.html

npm init -y;  npm i express
来源：http://hz.chenlongwang.top/gtkkofajer.html

[U82] JS：package.json 脚本
来源：http://hz.meibo888.top/gtdciaybaj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtbcckokis.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258.top/gtsuyzrmqg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yuanzhike.top/gtjnjtemon.html

[U84] JS：CommonJS 写法
来源：http://hz.xuetiantiany.cn/gtimzxhwnn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jqgfzy.top/gttfstlhze.html

[U85] JS：可选链
来源：http://hz.jqgufenzy.top/gtlmnqhmwb.html

a?.b?.c
来源：http://hz.guowangkeji.top/gtcgzqrqmu.html

[U86] JS：空值合并
来源：http://hz.xylfe.cn/gtghzhdzgg.html

a ?? b
来源：http://hz.jianghu66.top/gtkfnqmeth.html

[U87] JS：解构默认值
来源：http://hz.aibaodan.cn/gtdrrhuyrq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.aibaodan.cn/gtnjmgzlqs.html

[U88] JS：对象展开合并
来源：http://hz.ehwqpu.com/gtgknxddul.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtrvpawwwa.html

[U89] JS：数组去重
来源：http://hz.xziqi.cn/gtqfkebxng.html

[...new Set(arr)]
来源：http://hz.nanxinkj.top/gttjnzkjww.html

[U90] JS：数字数组排序
来源：http://hz.gaohongyu789.top/gttlgukphl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtaulxnxjn.html

[U91] JS：对象键值遍历
来源：http://hz.jqgufenzy.top/gtavpqsddn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cheryme.top/gtopmserej.html

[U92] JS：深拷贝
来源：http://hz.yongpay.top/gtpeeuzjho.html

structuredClone(obj)
来源：http://hz.havefunace.top/gtwhfsvvhm.html

[U93] JS：模板字符串
来源：http://hz.xuanzx.com/gtaxlyfxqf.html

`共 ${n} 条`
来源：http://hz.jinqigufen.top/gtsbzzhozh.html

[U94] JS：箭头函数
来源：http://hz.xinyue.icu/gtsuwfzwqc.html

const double = x => x * 2;
来源：http://hz.xuanzx.com/gttghtmbig.html

[U95] JS：Promise 包装
来源：http://hz.shangyingyoupin.top/gtjzbmanjf.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtakekirvn.html

[U96] JS：async/await 与异常
来源：http://hz.hfpthk.cn/gtfrqpycps.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtnkraexxm.html

[U97] JS：并发请求
来源：http://hz.nanxuanxn.top/gttrscjveg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtuxgbchpw.html

[U98] JS：fetch 带 JSON
来源：http://hz.yvedp.cn/gtxmxvljdf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.feifeiyinyue.top/gtocifagsu.html

[U99] JS：事件监听
来源：http://hz.chenzaomai.com/gtilhdnfpi.html

el.addEventListener("click", e => {})
来源：http://hz.nwbrower.top/gtitmkrxhv.html

[U100] JS：DOM 查询
来源：http://hz.hfpthk.cn/gttpjmpgle.html

document.querySelector(".item")
来源：http://hz.shangyingyoupin.top/gtlrlwjjrm.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtxemybjau.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtzcfifzvb.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtpgrepxmb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.pengpengdd.cyou/gtatayaamj.html

[U103] JS：定时器
来源：http://hz.guowangkeji.top/gtydjxdhle.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gotoacloud.top/gtrbiswymm.html

[U104] JS：防抖
来源：http://hz.jinqigfzy.top/gtsdyeursn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtxyalowzc.html

[U105] JS：节流
来源：http://hz.guannengcc.top/gthkgmairp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.52xcode.cn/gtxmahiokk.html

[U106] JS：日期格式化
来源：http://hz.yongpay.top/gtfxrdaltb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhongyouzk.top/gtrgfjowvi.html

[U107] JS：数字千分位
来源：http://hz.shuidangran.top/gtfiokuten.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yangfankeji.com/gtgkknfwdp.html

[U108] JS：随机整数
来源：http://hz.pengpengdd.cyou/gtxorbdvpc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jianghu66.top/gtpfhtaqsp.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtcueyhdvj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtjzzdssjt.html

[U110] JS：数组分块
来源：http://hz.hnxiangtu.top/gtoidpzaku.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.iojbl.cn/gtgamuhcun.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtnzgbiczw.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtvcooyitc.html

[U112] JS：字符串补位
来源：http://hz.chenjidiqi.icu/gttnmhvgjd.html

"7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtfvvlgtly.html

[U113] JS：正则替换全部
来源：http://hz.ppjwa.cn/gtdogsjfjs.html

s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtlondssrv.html

[U114] JS：JSON 深比较
来源：http://hz.kuanghao11.cn/gtvsizwxet.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtbpvuqekv.html

[U115] JS：生成 UUID
来源：http://hz.zhoulong.xyz/gtomukixok.html

crypto.randomUUID()
来源：http://hz.hnqzz.top/gtfcelpfsy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pycfn.com/gtbfvwsdkz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuanzhike.top/gtckkcygyx.html

[U117] JS：单元测试
来源：http://hz.smart0.xyz/gtrgldtuqo.html

npm i -D vitest;  npx vitest
来源：http://hz.yonumen.top/gtjuithzda.html

[U118] JS：开发服务器
来源：http://hz.hnqzz.top/gtrraxugct.html

npm i -D vite;  npx vite
来源：http://hz.birdmap.top/gtmdlnhymg.html

[U119] JS：生产构建
来源：http://hz.hywenlv.cn/gtsficczpa.html

npx vite build
来源：http://hz.kuanghao11.cn/gtbyjvrxxf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj202588.top/gtgueteulj.html

import.meta.env.VITE_API_URL
来源：http://hz.yj202588.top/gtoefoldmc.html

================================================================================
来源：http://hz.wangdashe.top/gtvotipapp.html

统计汇总
来源：http://hz.andypj.xyz/gtbmrafpzk.html

================================================================================
来源：http://hz.jinqigufen.top/gtnuumjrqt.html

按语言统计（条）：
来源：http://hz.cqqwz.cn/gtdycatgxm.html

Python ......... 252
来源：http://hz.xziqi.cn/gtivilbrez.html

PHP ............ 252
来源：http://hz.meibo888.top/gtmqsnvhni.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gthrupjvyr.html

TypeScript ..... 212
来源：http://hz.xinyue.icu/gtyisbvvzx.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtbkqwfvne.html

Go ............. 212
来源：http://hz.fengsongda.top/gtxgdjnuah.html

Ruby ........... 212
来源：http://hz.birdmap.top/gtobaaahvt.html

C# ............. 212
来源：http://hz.ydzc1.top/gtqqdvwefm.html

C .............. 30
来源：http://hz.hongshengwenyu.top/gtuejginna.html

C++ ............ 30
来源：http://hz.vqdsnc.cn/gtgxwkeygj.html

SQL ............ 90
来源：http://hz.52xcode.cn/gtofiozgdn.html

Bash ........... 80
来源：http://hz.cqqwz.cn/gtmvexmzav.html

Kotlin ......... 15
来源：http://hz.yj20258.top/gttmdqhunb.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtwdlaslcu.html

Lua ............ 10
来源：http://hz.aibaodan.cn/gtlwgzaqen.html

Perl ........... 10
来源：http://hz.xziqi.cn/gtbraakfcw.html

Scala .......... 10
来源：http://hz.hfpthk.cn/gtuxesaxua.html

------------------------------------
来源：http://hz.jinghuilouyu.cn/gtciyewryf.html

合计 ........... 2106 条
来源：http://hz.gotoacloud.top/gthztmwint.html

按章节统计：
来源：http://hz.jqgufenzy.top/gtrdjrjdts.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtdbtwqict.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtkcvaehzv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtpgdxhtbz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtgdbppynh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydjk.org.cn/gtvwnjcoky.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtilqmmwsz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtwazstnim.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtdjhihrmk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtmotdbxls.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nanxinkj.top/gtudaorbco.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtbsbswukt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtqtpktdlk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtbwcildxx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtahomgpwn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtjzjquttj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtnazmqdvz.html

Q SQL 专题                              90
来源：http://hz.ybcxt.top/gtssukkmmy.html

R Bash 专题                             80
来源：http://hz.xuetiantiany.cn/gtdayhcfkg.html

S C / C++ 专题                          60
来源：http://hz.shzxlz.cn/gtabpfxzcy.html

T 其他语言补充                          60
来源：http://hz.jinyuanbaomall.cn/gthrlsjmue.html

U 高频实用片段                         120
来源：http://hz.nanxuanxn.top/gtmwugexck.html

------------------------------------
来源：http://hz.0kj1m.cn/gtjsyqwuwy.html

合计                                  2106 条
来源：http://hz.wangdashe.top/gtqhetmqjl.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtuvmogcck.html

使用提醒
来源：http://hz.zycfv.cn/gtautqhuyr.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtxfemmmgr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258888.top/gtfqdexidt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnqzz.top/gtnfrcyeek.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.meibo888.top/gtyeiwzjvq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtxcsjftrv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fzhhl.top/gtepkcqsrr.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtulxkrhpf.html

================================================================================
来源：http://hz.ybcxt.top/gtvtvzefmr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zycfv.cn/gteeapchor.html

Common Programming Examples Cheat Book
来源：http://hz.yj20258888.top/gtwrqeifye.html

================================================================================
来源：http://hz.hfpthk.cn/gtbbevrkre.html

【收录内容】
来源：http://hz.ydjk.org.cn/gttebdfanl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yongpay.top/gtqtbsrptf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxuanxn.top/gtxxdfzexu.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gtfenvslyj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guannengcc.top/gtljpudmla.html

【使用说明】
来源：http://hz.kuanghao11.cn/gtxsdngavi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuanzhike.top/gtuwmdyzup.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258.top/gtdwlcvskg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hywenlv.cn/gtfnzbdxql.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tianlin.xyz/gtpqpipzrx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangtech.top/gtgpbwujcj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.daria6918.cn/gtlpzzlthb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xingfuxueyuan.xyz/gtvshydkkj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhengqikj.top/gtxskjgkqs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigfzy.top/gtivywmgie.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.haohaochexian.top/gtwkhvzwnn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.kuanghao11.cn/gtrwycofwj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ivvv.top/gtohdhkbrg.html

【文件统计】
来源：http://hz.hnqzz.top/gtuvxuornh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ydjk.org.cn/gtuhzzuhhw.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtyrswousp.html

目  录
来源：http://hz.jinyuanbaomall.cn/gtbaxzqaio.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtwattnpei.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtgecxmqfm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtjxtphdjn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtyhmxmjew.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtmmcoscdh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shuidangran.top/gtlkumphod.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gthnnrrfld.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtutvuutxj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.snrcjt.cn/gtulfegtby.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtlaxyvjza.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtlnfopxll.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gthzbvvjmn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtmwqrhoth.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtqktlicox.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.pengpengdd.cyou/gthfmnrhrp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yanxiufei.cn/gtczjdymlc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtuhtqddjw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtyjegrbrt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cucudq.cn/gtmzltswdw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtwriitkww.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gttkybybji.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtxdvmulbo.html

================================================================================
来源：http://hz.zycfv.cn/gtbwnopkpb.html

A. 基础语法与类型
来源：http://hz.nanxuanxn.top/gtjmynmhdz.html

================================================================================
来源：http://hz.316326.xyz/gtgixdkxxb.html

[A01] Hello World
来源：http://hz.birdmap.top/gtodsrwxoi.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtugjckuxu.html

PHP:  echo "Hello, World!";
来源：http://hz.shanyushiyangkeji.top/gteqyrpfxr.html

JS:   console.log("Hello, World!");
来源：http://hz.chenlongwang.top/gtoburhicd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtxhomhrsj.html

Java: System.out.println("Hello, World!");
来源：http://hz.yvedp.cn/gtkfycbeue.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gttbcrxzej.html

Ruby: puts "Hello, World!"
来源：http://hz.ivvv.top/gtnqrluxjm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sweek.top/gteozvwldu.html

[A02] 变量声明与赋值
来源：http://hz.cucudq.cn/gtwiwfputb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ybcxt.top/gtfmxsleps.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenlongwang.top/gtendredfo.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.kuanghao11.cn/gtplnjyeqw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sxryk.cn/gtnaggcynb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hywenlv.cn/gtpjpqtiep.html

Go:   name := "Alex"; age := 20
来源：http://hz.hongshengwenyu.top/gtfshagpqa.html

Ruby: name = "Alex"; age = 20
来源：http://hz.wangdashe.top/gtjbkycbif.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jqgfzy.top/gtzccleydk.html

[A03] 常量定义
来源：http://hz.tanke756.top/gtfvqmmwim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xingfuxueyuan.xyz/gtmfmdraiv.html

PHP:  const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtetewumov.html

JS:   const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gttqqlnzgb.html

TS:   const PI: number = 3.14159;
来源：http://hz.hysaishi.cn/gtvgnrmfnl.html

Java: static final double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtahxabhxt.html

Go:   const PI = 3.14159
来源：http://hz.yj20258.top/gtyzncicct.html

Ruby: PI = 3.14159
来源：http://hz.vqdsnc.cn/gtqverzyor.html

C#:   const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtqeehkton.html

[A04] 判断变量类型
来源：http://hz.sxryk.cn/gtjykucycr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gthqdiqoxn.html


<!-- 参考信息 -->