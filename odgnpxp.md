代发 wailian999

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/geyudcfax.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gdbsedrkw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/ghxnclize.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gwtnaqykg.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/glbaprjep.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gzuhkbgip.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrmlwhw.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gleveimue.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/galxvjvkj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gdnitfdjd.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gjayzeueh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gcphhrkgo.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gmrrnbmta.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/grmptgluf.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gatemysyp.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gulfixhep.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/glocghgyu.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gcecvxaoc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gchhdywdc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gngfhmcpt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gsiciahwm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gegpjqxnb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gscexhekg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gzltkboge.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gdyapuude.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gxrnmvhhw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gmzrikwxz.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gjtxiyzog.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gbwuxtplf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gemywwlkr.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/geegxztbk.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gvnhrywac.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gpypbklig.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gsnqmajcb.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ggdwocebs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gflknvxhj.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gagpyfhzv.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gpmeofjgx.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/grrvmxtqr.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gpzyqxwgo.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gdiovsxwg.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gabpcjcak.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gjlucpurj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gyndrslip.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gqnxgrxie.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gzkjrkace.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gagvtzlmg.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gfkhfkaqj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwwuwjpzc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gnnwgoujo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqbivuihi.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gfseekiza.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdvsgozhh.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/glogznhkc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gxxiiablb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmxdkqsqh.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/guyyrlgwa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gqxnltkrk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/ghyjngddr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gduwixokg.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gewzgovcf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gdwrupppw.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gjytgyrla.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gukoidboa.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gaixxycvh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/ggrhjfiwa.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gcodxfxhg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gasalwmdp.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gtpklbnky.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdskizszq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gorzjtoau.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gendmjecm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gxelywizg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gyoeznwxn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gfzagegff.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmyiflx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gtyfsikhy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gzxljjqxt.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/grdoxfdej.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gfkdutxjq.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gyhzcpoou.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gyyyxonkd.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gjsgyujme.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gumoppelg.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gxdtrpjpb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gxcmxsnup.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfsbcmwsl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gvmnvwsht.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gggydjths.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwsoerfeu.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gpgvmymya.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gubxcgihk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gjalbotrr.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/goqdzmizx.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gumwhqkfg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gbijywkzk.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/glvdtyubd.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gxvjggyff.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/ggkxakfor.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ggllkvyhj.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gviwdzhuv.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gbafytsie.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gyjsbuwuv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gmbsgylfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gnbkhknlm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gufcrabzr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/glpgqdqwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gijzgqqmv.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gotvkswyc.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gvreukvny.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/ggiavevip.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gcnttpmis.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/groschkpo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gacutpisc.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gawnsqabo.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gypevogxe.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gcyttdgzu.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gguqyygqs.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gwpnrugyu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gpjjpedtu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghlfosjho.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gciatvqgc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gmdckkwus.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcnniztpi.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gvfmvrlef.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gkvqhzsrs.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gqaptyqsz.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gprmtgtyn.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gobzmmxnb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gbwetiooq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gmnzsvisc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/giacunzhv.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/geaegkzsj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gfdmajymo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gipyswpyd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gtpuvwxss.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkdrfiqdm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gpeoejxgx.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gtzuybbqa.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gijjesklq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gsqkdexwu.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gulsafdak.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gpmygfsej.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gildhwbbx.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gwiiwjcwh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gumbpnhsh.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/ggpzewlsa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gkqebiofn.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/grgjxzwtm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gkpifgezf.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gbvokauvq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gjwexnfou.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gusxzftid.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gqwjysdet.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gfxzrubhp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gafxxysdp.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gogjhaetk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnzdxowec.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/glziapgpk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/geqeyicqc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gdqfzwjce.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/grydivwmv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gqgugauqe.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/goufsthla.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gmtglmuls.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdqxxkfix.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gnfvbjasz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfmmddqqe.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gxwuoydph.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmgyyftqc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gtmyyzcnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gnzhcbenb.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gnftkezjo.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gwoyoynuf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/ggbmdgrqq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gljayfjxo.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gldculfvt.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gqryqfmuz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gmntuklze.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gmjxryqvk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggsvkhygb.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gccauxiok.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzhuqxkbm.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gfdjlymnw.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/grszxqsmr.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gltuiavgy.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/giezbikwm.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwneqll.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gjufnejsb.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/ghnyaqwxk.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/guuwdigoz.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gdcoccmza.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gqdflqnmo.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/ghrxpuykt.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gsywyvcim.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/ggdiuxfbu.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gbesjnrcw.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gpplmwrmx.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gpajwlqzo.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gkghkfbwi.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gpxldmsqd.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/guqucekbu.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gkmfqxvyz.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gjuuglkel.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gubducoee.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gxefgosly.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gwcrlcdtw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/ggfxqlcfh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gszjmxvij.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gczutboqj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gxyihpxvx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gshmwifwd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gsjvxjbjw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/ggvggzwuf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gdzthazlo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjllqctxn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gatftdicd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gmdxdmlic.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gtgyvlfpg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdtwbmmzg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gggchcpwk.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gtvnvptmm.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gzcluvorx.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gisplsoia.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gybocmjqi.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gynxqggnx.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/giuiolebd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjgwfuiai.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gfksgekdi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ggemkxpej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/glvqzunvt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gwbgganjb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/glbuyrlyb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gdnfvfjhv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/giietekud.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gfwmmmaav.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnkpozaux.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gpzhyllxt.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gmpskmgvv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcpntngle.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gkodqncan.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gvulmyxgn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gnzhvexcb.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gykokbnge.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gymmwcxui.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gvagapmrw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gbjunlbmd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/grbzreyae.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gjtxhlfin.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/ghnqahgtd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gclqreack.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gmphuiqaz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/ghuuszzjh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gyziistmf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gflwjsayn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gpoikmhro.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gqfauujso.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gpiglehyl.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gglosywey.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gpdnaqmxb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbhotdayr.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/grfpetvya.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gsaqaomxd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjawtywje.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/glnqfmlec.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gzhqqcqgh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gclwmzdoi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gtyufdxhg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/ggvndecaq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gqbdvlkjr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gvxpmlzrm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gsbnvjesc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/goecxygll.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ggiveovsg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnaeujrlx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gnuzdtgbs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gcixuefwm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/glbsrahyq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtkzxdcwn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gftpwwymu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gsgelplor.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gbgpplwaf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gartxfsmm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ghvouzbdk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotieiird.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gbacuhibq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghpzklvpf.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gmzygokym.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gaxpuvxdr.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gqktttxtp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gcpsmscim.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gaiaqmbtr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/genauekze.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gkciycopt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gxljgvujx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gdbccolgr.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gexgnmsks.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gmmszrrlh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gjdifgiit.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gdwyggwkh.sHtML


<!-- 参考信息 -->