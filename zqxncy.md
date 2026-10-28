代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.bjfxy.top/gtaqujjoth.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xinyue.icu/gtbbevkuog.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gtbqxmzhdl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ivvv.top/gtezulffmy.html

[U43] PHP：声明命名空间
来源：http://hz.pycfn.com/gtudznpehw.html

namespace App\Http;
来源：http://hz.hnxiangtu.top/gtbnqncbjx.html

[U44] PHP：开启严格类型
来源：http://hz.gogol.net.cn/gtepqbojhn.html

declare(strict_types=1);
来源：http://hz.quarkkingdee.top/gtgcjkeeqo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xinyue.icu/gtldqikrpi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtxymihwch.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtxsqbjcuk.html

?string $name = null
来源：http://hz.zhengqikj.top/gttivkmpvd.html

[U47] PHP：联合类型
来源：http://hz.svipenyu.cn/gtmdsoxtfa.html

int|string $id
来源：http://hz.kuanghao11.cn/gtflxhzded.html

[U48] PHP：纯枚举
来源：http://hz.yueranfly.top/gtxclzwmbo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sysykeji.top/gticpqnzyv.html

[U49] PHP：只读属性
来源：http://hz.gzhubu.top/gttabpjeue.html

public readonly string $name
来源：http://hz.tian-w.cn/gtblbbganh.html

[U50] PHP：构造器属性提升
来源：http://hz.smart0.xyz/gtnxraxapp.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gtcpmwgdnq.html

[U51] PHP：数组解构
来源：http://hz.daxiang520.top/gtazanapek.html

[$a, $b] = $arr;
来源：http://hz.sweek.top/gtwyuyvbdc.html

[U52] PHP：箭头函数
来源：http://hz.haohaochexian.top/gtphqnxynw.html

$double = fn($x) => $x * 2;
来源：http://hz.yonumen.top/gtjkqnevvl.html

[U53] PHP：空合并运算符
来源：http://hz.andypj.xyz/gtmqiwgiyy.html

$v = $a ?? $b ?? "default";
来源：http://hz.smart0.xyz/gtjooqmtul.html

[U54] PHP：空安全调用
来源：http://hz.nwbrower.top/gtlzxsfcql.html

$obj?->method()
来源：http://hz.jqgufenzy.top/gtludznnuz.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtazcihlab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtgtcwxald.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtqmshjvip.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtviwkoepz.html

[U57] PHP：字符串插值
来源：http://hz.cashguo.top/gtrqvvuluc.html

"值: {$a}"
来源：http://hz.hnqzz.top/gtxvpgupqf.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtlvtukkzw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuanzx.com/gtuyyifvtt.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtgnxwtuyu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtcipxadsz.html

[U60] PHP：JSON 编解码
来源：http://hz.hongshengwenyu.top/gtckaglqbz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jyoumei.cn/gteldzvekw.html

[U61] PHP：正则
来源：http://hz.jlsjyb.cn/gtuppdtezg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtwxektydb.html

[U62] PHP：日期对象
来源：http://hz.zhaomingkeji.xyz/gtvodtrwyt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.redwolf501.top/gtmslndhwp.html

[U63] PHP：文件读写
来源：http://hz.zycfv.cn/gtygvwksuj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinghuilouyu.cn/gtxkfnauwf.html

[U64] PHP：目录遍历
来源：http://hz.pengpengdd.cyou/gtddkqjmce.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zycfv.cn/gtegxcavkg.html

[U65] PHP：会话
来源：http://hz.zhoulong.xyz/gthjaezulx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cucudq.cn/gtpmojgyrl.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtagxkcsrb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.feifeiyinyue.top/gtqmqpsfqk.html

[U67] PHP：处理文件上传
来源：http://hz.gzhubu.top/gtnbrregyu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtqxamfgrx.html

[U68] PHP：PDO 连接
来源：http://hz.hywenlv.cn/gtaooarjgj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtrlctbqhe.html

[U69] PHP：PDO 预处理
来源：http://hz.xziqi.cn/gthkogguie.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ehwqpu.com/gtdvwprhbc.html

[U70] PHP：PDO 事务
来源：http://hz.chenzaomai.com/gtzgbsfddp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtffjtycxa.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtmrixyzls.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangkeji.top/gtullesyyh.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtovnbcxaw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cheryme.top/gtmfgspxkd.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtupsaynbm.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtmctbfuxi.html

[U74] PHP：读取环境变量
来源：http://hz.xuetiantiany.cn/gttfxynicv.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cqqwz.cn/gtwtmfltfa.html

[U75] PHP：依赖注入
来源：http://hz.shanyushiyangtech.top/gtecvjiheq.html

composer require psr/container
来源：http://hz.yongpay.top/gtmctmwijl.html

[U76] PHP：简单路由
来源：http://hz.feifeiyinyue.top/gtavkldpcu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.haohaochexian.top/gtsgummvgv.html

[U77] PHP：模板渲染
来源：http://hz.shzxlz.cn/gtowegkaci.html

composer require twig/twig
来源：http://hz.dianchejie.cn/gtwfssnxyj.html

[U78] PHP：单元测试
来源：http://hz.feifeiyinyue.top/gtkdpzzekb.html

composer require --dev phpunit/phpunit
来源：http://hz.wangdashe.top/gttyfojzxl.html

[U79] PHP：静态分析
来源：http://hz.ivvv.top/gtymiqhucq.html

composer require --dev phpstan/phpstan
来源：http://hz.snrcjt.cn/gtgbzlcgpq.html

[U80] PHP：代码规范修复
来源：http://hz.cdnleiting.top/gtdwcnpztl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinyuanbaomall.cn/gtvzrcnfdj.html

[U81] JS：初始化项目
来源：http://hz.jyoumei.cn/gtsxfxzwdl.html

npm init -y;  npm i express
来源：http://hz.nwbrower.top/gteakyjuds.html

[U82] JS：package.json 脚本
来源：http://hz.jyoumei.cn/gtxflctghx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenzaomai.com/gtfoqcstcm.html

[U83] JS：ES Module 导入导出
来源：http://hz.tianlin.xyz/gtbjfjwuoe.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xziqi.cn/gtrhvlmnwo.html

[U84] JS：CommonJS 写法
来源：http://hz.xingfuxueyuan.xyz/gtqzymiigz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtfhfwqcyk.html

[U85] JS：可选链
来源：http://hz.hnqzz.top/gtzukrkjlf.html

a?.b?.c
来源：http://hz.gotoacloud.top/gtadabijlq.html

[U86] JS：空值合并
来源：http://hz.xingfuxueyuan.xyz/gtovozlfus.html

a ?? b
来源：http://hz.yj20258888.top/gtosszjxyn.html

[U87] JS：解构默认值
来源：http://hz.yongpay.top/gtezibxqxg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtupuhqldy.html

[U88] JS：对象展开合并
来源：http://hz.cdnleiting.top/gtzsgfgpgf.html

{ ...a, ...b }
来源：http://hz.0kj1m.cn/gtoagxkdso.html

[U89] JS：数组去重
来源：http://hz.tian-w.cn/gtgqirmgjp.html

[...new Set(arr)]
来源：http://hz.cucudq.cn/gtsrnouldr.html

[U90] JS：数字数组排序
来源：http://hz.quarkkingdee.top/gtskgqnxdc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtxiworgah.html

[U91] JS：对象键值遍历
来源：http://hz.yvedp.cn/gtepzezkou.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenjidiqi.icu/gtjddcfesx.html

[U92] JS：深拷贝
来源：http://hz.xinyue.icu/gtzkdluvhh.html

structuredClone(obj)
来源：http://hz.jyoumei.cn/gthjfozsau.html

[U93] JS：模板字符串
来源：http://hz.sweek.top/gtaetohqoj.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtzuldkgqk.html

[U94] JS：箭头函数
来源：http://hz.hnxiangtu.top/gtvejsesis.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtanautukt.html

[U95] JS：Promise 包装
来源：http://hz.nanxuanxn.top/gtqyhfkmpa.html

new Promise((resolve, reject) => {})
来源：http://hz.jianghu66.top/gtmaoacdks.html

[U96] JS：async/await 与异常
来源：http://hz.xingfuxueyuan.xyz/gtrhltfzyq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtjlqebzfh.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtttqwiuik.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtowktqirm.html

[U98] JS：fetch 带 JSON
来源：http://hz.yangfankeji.com/gtbcvajweg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtfhyudlzy.html

[U99] JS：事件监听
来源：http://hz.hnxiangtu.top/gtgjrmogbe.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gthivdertx.html

[U100] JS：DOM 查询
来源：http://hz.sxryk.cn/gtvgvqhcsz.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gtifugrdpe.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtvhpwgjom.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtdhjzywba.html

[U102] JS：本地存储
来源：http://hz.zhengqikj.top/gtrwtabfcr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hongshengwenyu.top/gtqaocgoyz.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtispamljj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.wangshuangyany.cn/gtnffxtwtd.html

[U104] JS：防抖
来源：http://hz.jiagoushi.top/gtbyrqmhix.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtxnkhiyiy.html

[U105] JS：节流
来源：http://hz.feifeiyinyue.top/gtbztluccq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigfzy.top/gtrrkchxls.html

[U106] JS：日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtggifuyyd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gtgxxcbjif.html

[U107] JS：数字千分位
来源：http://hz.shzxlz.cn/gtbxialtfw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtamvzpvmp.html

[U108] JS：随机整数
来源：http://hz.daria6918.cn/gtyblqxact.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtlnxyqtqx.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtwszpmdev.html

Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtsgmypuir.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtlqrhklik.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tian-w.cn/gtitqbxzxv.html

[U111] JS：对象转 Map
来源：http://hz.jlsjyb.cn/gtjnnuapgy.html

new Map(Object.entries(obj))
来源：http://hz.shangyingyoupin.top/gtjbhocukb.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gtexbezuix.html

"7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtpqygpnwo.html

[U113] JS：正则替换全部
来源：http://hz.cheryme.top/gtxthezlgy.html

s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtdxftwljt.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtnztkqaxl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtglaptqha.html

[U115] JS：生成 UUID
来源：http://hz.xuanzx.com/gtnpdorqov.html

crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtwllnywez.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.iojbl.cn/gtiutpwrnz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.snrcjt.cn/gthcjtvrwl.html

[U117] JS：单元测试
来源：http://hz.jlsjyb.cn/gtasffkjip.html

npm i -D vitest;  npx vitest
来源：http://hz.yvedp.cn/gtpeqkhigf.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtjduakaql.html

npm i -D vite;  npx vite
来源：http://hz.zhaomingkeji.xyz/gtkqfhabry.html

[U119] JS：生产构建
来源：http://hz.52xcode.cn/gtnurqmahf.html

npx vite build
来源：http://hz.xuanzx.com/gttlfyligg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cdnleiting.top/gtnvtkdjrt.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangkeji.top/gtvknrmurm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsocnxcoj.html

统计汇总
来源：http://hz.aibaodan.cn/gthuglsqny.html

================================================================================
来源：http://hz.jyoumei.cn/gtckmdopcq.html

按语言统计（条）：
来源：http://hz.shanyushiyangkeji.top/gtmomeihao.html

Python ......... 252
来源：http://hz.gogol.net.cn/gtfakfcfug.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gtzwmzrsea.html

JavaScript ..... 252
来源：http://hz.feifeiyinyue.top/gtyzprcldg.html

TypeScript ..... 212
来源：http://hz.yj20258888.top/gtrxwqxioa.html

Java ........... 212
来源：http://hz.tanke756.top/gtqoyysdhy.html

Go ............. 212
来源：http://hz.vqdsnc.cn/gtcfwcktrl.html

Ruby ........... 212
来源：http://hz.snrcjt.cn/gtqrmffrfm.html

C# ............. 212
来源：http://hz.xziqi.cn/gtecpudhyy.html

C .............. 30
来源：http://hz.meibo888.top/gtbzwshzqw.html

C++ ............ 30
来源：http://hz.yanxiufei.cn/gtlowpdsye.html

SQL ............ 90
来源：http://hz.smart0.xyz/gtgxjaavsj.html

Bash ........... 80
来源：http://hz.yvedp.cn/gtisbjzaha.html

Kotlin ......... 15
来源：http://hz.gogol.net.cn/gtiutmkyxq.html

Swift .......... 15
来源：http://hz.guannengcc.top/gtoafxmwik.html

Lua ............ 10
来源：http://hz.ywan-chungtsiang.top/gtoucdmrlk.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtzpujhref.html

Scala .......... 10
来源：http://hz.wangshuangyany.cn/gtbqilupbv.html

------------------------------------
来源：http://hz.birdmap.top/gtqczjhozq.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gterfknmiq.html

按章节统计：
来源：http://hz.cdnleiting.top/gtmdbymhkh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtnsmepylf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtgvpvsolo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuanzx.com/gtktrhkjgk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtwnziqihj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yonumen.top/gtyrmacupn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gtcbeuvpvg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtidzhjooi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtrwpgtrvc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtsjhavuzi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gtihtwbxio.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtjkgcdflj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gthxkpwpya.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtjkfrayur.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtzcztzrsa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhixingplan.top/gtnmrtfyae.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtxctlshwu.html

Q SQL 专题                              90
来源：http://hz.redwolf501.top/gtydyavhgy.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtwhpuuptx.html

S C / C++ 专题                          60
来源：http://hz.havefunace.top/gtloormaay.html

T 其他语言补充                          60
来源：http://hz.smart0.xyz/gtrtimyukp.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtmcibkeab.html

------------------------------------
来源：http://hz.havefunace.top/gthhghrxdk.html

合计                                  2106 条
来源：http://hz.316326.xyz/gtbgthjqim.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtqdeqgqjh.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtfkzayzst.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtgejtgzfg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.kuanghao11.cn/gtutwnuiju.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hysaishi.cn/gtwcetgoip.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.wangshuangyany.cn/gtabsnkxso.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xuetiantiany.cn/gtveavxvwd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jyoumei.cn/gtanwmjnwu.html

—— 文件结束 ——
来源：http://hz.shanyushiyangtech.top/gtljhqfzzp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgdstweyg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ppjwa.cn/gtwpiyscuu.html

Common Programming Examples Cheat Book
来源：http://hz.sxryk.cn/gtzfkunqhz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxlkostpb.html

【收录内容】
来源：http://hz.ydzc1.top/gtprledbro.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yongpay.top/gttaxjphzl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gttiyazwaf.html

SQL · Bash · C · C++
来源：http://hz.jinqigufen.top/gtwauzrlfj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cdnleiting.top/gtasyiafas.html

【使用说明】
来源：http://hz.sysykeji.top/gtblbbhnbz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gtpjiydgyq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gttrxbqxlx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xziqi.cn/gtyotzjxmj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gtrfvthacb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigufen.top/gtxelevobt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xuetiantiany.cn/gtmqtbsvoj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haohaochexian.top/gtxjsjqyic.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.kuanghao11.cn/gtgrhbgcnt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cheryme.top/gtdapoygco.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sufxvd.cn/gtehjdghjh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shanyushiyangtech.top/gtrvmwoygs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cdnleiting.top/gtrxaobluc.html

【文件统计】
来源：http://hz.jianghu66.top/gtmqsibdqd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ybcxt.top/gtskoafjor.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtrmjpftoc.html

目  录
来源：http://hz.hfpthk.cn/gtcaxcawvg.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gthldzfyxq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtakyeeppt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtllalqjda.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gtbpcyqjcb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtlhftmthw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dashuyun.cn/gtpjqwbodx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtrajnwalo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtgnaypwdn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtpasmicif.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtmqyzqykl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gtsceflttj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtmxjsrnff.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtwsrtvkha.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtzqkwjycb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangdashe.top/gtpveaifud.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pycfn.com/gtpijnxbej.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtaobmamle.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gzhubu.top/gtpouflcnj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hysaishi.cn/gtcakjgamg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nwbrower.top/gtjivdojpa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtfxwqfnat.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtgoqrsxkq.html

================================================================================
来源：http://hz.yangfankeji.com/gtptdtyyxj.html

A. 基础语法与类型
来源：http://hz.jlsjyb.cn/gtcboqinxl.html

================================================================================
来源：http://hz.ybcxt.top/gtiznlrytw.html

[A01] Hello World
来源：http://hz.mhx1999.top/gtccgddjzy.html

Py:   print("Hello, World!")
来源：http://hz.cucudq.cn/gtlhyxcjeb.html

PHP:  echo "Hello, World!";
来源：http://hz.jiagoushi.top/gtxgqcpjqc.html

JS:   console.log("Hello, World!");
来源：http://hz.jianghu66.top/gtzflypjzk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cheryme.top/gttxxwfblg.html

Java: System.out.println("Hello, World!");
来源：http://hz.guowangkeji.top/gtdcknreti.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sweek.top/gtmqiubnmq.html

Ruby: puts "Hello, World!"
来源：http://hz.zhijiandao.cn/gtfggaucol.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.guannengcc.top/gtfadtwtiw.html

[A02] 变量声明与赋值
来源：http://hz.shanyushiyangtech.top/gtwzpaqvqt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhengqikj.top/gtsxlvynnw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gogol.net.cn/gtvakoffqu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hammf.cn/gtxrgbpvbz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.bjfxy.top/gtnixftydk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gtcpbrixwx.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgufenzy.top/gtluhdsjah.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guannengcc.top/gtrvidxwyx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.snrcjt.cn/gtosdnatja.html

[A03] 常量定义
来源：http://hz.xuanzx.com/gtzguyjktk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuetiantiany.cn/gtadootjwa.html

PHP:  const PI = 3.14159;
来源：http://hz.yvedp.cn/gtpsfwbrsb.html

JS:   const PI = 3.14159;
来源：http://hz.snrcjt.cn/gtpbsqpyjc.html

TS:   const PI: number = 3.14159;
来源：http://hz.wangdashe.top/gtyqfjqsfn.html

Java: static final double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtmywowmjx.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangkeji.top/gtdmfhdqko.html

Ruby: PI = 3.14159
来源：http://hz.zhoulong.xyz/gtiqzywlkq.html

C#:   const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtnrvsmktf.html

[A04] 判断变量类型
来源：http://hz.hywenlv.cn/gtyaqvbtcm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.feifeiyinyue.top/gttlzcwgqk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ehwqpu.com/gtydmhxcub.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.dianchejie.cn/gthyhiadpf.html

TS:   typeof x; x instanceof Date
来源：http://hz.yuxming.cn/gtuhzbqtaa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gtdhxyugfz.html


<!-- 参考信息 -->