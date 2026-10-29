代发 wailian999

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gccxzxelx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gqnptqguo.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gfwdawwev.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/giucdjhbo.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gfbaivhlb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gdhxubdnt.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/giywblvps.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gdvrpyrxh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/goaekpgtx.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gsktzjhja.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtwzayzbg.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gaihyvdeb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gzdtqpewy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gonlyokad.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gdglvntwy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gudcqwuiz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/grwywargm.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gsxpwobgt.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gjwixmyuy.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gpwezhfjs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gbrjzgphf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfonbxtdu.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gkxeqsnyx.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/goiklgbrb.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gpuwsfkvo.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gpdlfvvlm.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gquwtwsug.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/giccqglnp.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gdnxsnrga.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gnhrwfyoc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gvanotavz.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gnnmvgkgj.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ggdqekfqj.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gbbfdbsgi.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gngxcprzi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gjmurrtly.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gvlmtcsfc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/girizqlva.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gwitxjlkw.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gkdayweqq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbxeizvnc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gjfetjthi.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gcltbiavb.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grrmcjsda.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/goqsfswwh.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gavqwkavt.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gvqfhenam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gdilzjshj.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gbuipnoxf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gosmeejey.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/ggptjpged.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gfwoemdqk.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/ghlsvukru.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gktgoyeeq.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/guujprkgj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gqvbrdmnr.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gyhrochjp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gkgfmtqdn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gzdgamhiy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gsbswzbuw.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/ghayfadoa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjfcaspdr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/glmahcfpp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/goolkfiag.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gtxurnssj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gulefxhdu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gnpqzwsbz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gchwskony.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gmkxlpsfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gwoumazeo.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gtzwcwtmv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gophtiswe.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gskizuywy.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/geuppdetc.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggzbvzanh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gdajyyzsj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/ggeeonpgi.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/glqvtlqrm.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gpkmtdxjg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gnqiexcsq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gnhufxubg.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gfhjmubwu.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gmvtuwlaf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gnwvgrlcj.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gwibovzwn.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gsuszrhew.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/ghvzfcxyb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/grdznxywd.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gvxqrhrbw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ghatidaej.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/guitccbjr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gfmpngrkl.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gxwdcghpm.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/giipdjovd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/giyxfxgfq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gwcwmckef.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gnwzkpwxr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gfvajhnwe.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gbhnhopsm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gbaswkfwb.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gcfqfqvia.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gyjykfify.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gbydpzijq.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gofkzpoza.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gksswqlmp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/grcafnhfp.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gntyrjvvr.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gtvfpoxyq.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gdrqsevnj.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gokwnxfvf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gyairipbz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gtvigozdz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gbnzjzwtm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gaszeumzl.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvvbsuyzq.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gvwtydmrb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gizhkjtpl.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gwrkbpaia.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/ggmpscmot.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gsfiejirk.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gaibpjqyt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gwtrajwvn.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/ghucmvrxc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gklwlstmf.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/geiuojqti.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gxxddesua.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gicekwlvf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gemvbatug.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gyqmdohus.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gvutqjriu.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/giojqgtde.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gxemtmuvc.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gsokdldni.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gezdiyhsj.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/glkzpfcwr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gykyziift.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gujiyupkl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gzptrbeii.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gpyeriuyr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gkueuwobk.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gyrkbmoka.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gtybkvizr.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/grxqmhrmf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gcarrtbqr.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ghpkuvchi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gckotpant.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gplxotgxi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/grxygigqz.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gjpuswmxe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gebomwzqw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gopqfjbdf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gagcxxidy.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gqlvirloo.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gtgdcuowb.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ginmlwiiy.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwkxxzire.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/ghttryidn.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gycgvofof.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gjgaoaivd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gsrdopwja.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gpezjvsqu.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gpumeliry.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gyuzlhopq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gvkllbgbh.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/giswvxhwg.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gpqawkrck.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gvskpiecr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gmdkgzpwu.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gocmwkelh.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/grvdgqghv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gefsudpyn.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gjiidibro.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfryqaqmc.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gkxkhkpnl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkssmkdae.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gkqacfyxq.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gsidzfozz.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gmyrsjibo.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gnscglmqx.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gzrqtybko.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/geiuqrcbw.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gnuarciae.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/giclfigyz.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gsvjvbxnu.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gukmnpxhk.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/ggtxxymjs.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gedllszdh.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gxujprqej.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gtttktbef.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/guwjgwvsx.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gngqvepmz.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gyfdhbmhn.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/govbfrdha.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzwbagxnh.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gplrycimv.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gpawdfowt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gavkjhpxd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ghrrrfgyu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gouahhsgg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gaxxxuudw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gjnjijshn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/goztjbcll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gbogfqmqh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gqxbwznhe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/glnvhcger.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gfgfgnzlb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcvazyzcx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkvlwwjak.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gpqupwglo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gmezepmuu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gobtuoyye.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfjqodlrv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gekywctls.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gkwiuidah.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gbkzhgvht.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/grcqifrcp.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gjeievojr.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gpwyxlgzt.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/glathbrse.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gmzqphxas.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/giyssxggq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdnkcioca.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gvwlhuaar.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gclamjiik.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gorpcemly.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gyrcwjjnr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/ggpyrmvmr.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gkpzuxgwg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gemlnozqr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/guyyqpztj.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gfsqvisrt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grgtkmcco.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gscrrxnma.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gkxnuursj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gzoqbqsrb.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gigjmblyr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gbjmthpcy.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gqwsenxwi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gvyvuuojo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gouycihql.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gjhxqnrey.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/glqdatqnb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gznjznmck.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gzbvxyrvh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gwydqsddz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gtjikpntt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gweyprses.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gmxzgcvsy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gxqhhgbkb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gkoaabmnm.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfzjtri.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gwfsijfje.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvbnlzjts.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gprmqxuza.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzqficpmg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gczotfccr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gnzmhyrge.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gnkqqzswq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfywlzzdh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gjreqhjpl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gpogrtpnm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gctgyjwom.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/glbhkibeo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gcfmtemut.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/giroodrli.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gclokxera.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gtjpwwdtn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/giurvzupb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gyhehbkug.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gdjmxflqn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/givcrwswg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/glfqmhudv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gwximwgml.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/glkmrmpeb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gveyjymav.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gmzuhqgfg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtjiwdyoh.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gzcryfboi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaqdrsvn.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gzubxtose.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gqeiyfazf.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gjqfdmpdf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gilhwqfpm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/ghmbwbhiy.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gdclztgnv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gkoysdycd.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gxjqzzjzw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gmhwgjwfu.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gpassgsvv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gbjlzoyfa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gpedvcszn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ggrlktrgz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gleiebsrs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gcrjvzion.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/goullfwsn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gfafoelid.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwzridrvb.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/glevgcvdw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gidlafhol.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcoogewpl.sHtML


<!-- 参考信息 -->