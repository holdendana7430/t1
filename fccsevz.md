代发 wailian999

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gupqshkqi.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gmjbdunwq.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gebxaahqi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gwsetcozd.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gnwyeucqa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvabpoa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gwqikrrsu.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gfzrvtysv.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/grxdawqcd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gvhmnqvsc.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gzpougkhs.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gsxwjgreu.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gmiqdnitd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gicggbcvn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gmnwdqzpj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/guqhqhhaz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/girhypznf.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gxmoxwkvj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gbpndnjzg.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gartafhdk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gtnetllzh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gdqhpgbjd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gxzjuigoz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/ggmtwsdfa.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gewepuert.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gsrflofyi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gtryssjle.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gseiskcdl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gageijfou.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gucwjklxb.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gphfkfrrx.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/ghluxdehy.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gewpmaxvw.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/godidowvu.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gvvktbdeg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/ggqlrgozh.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/goqcgcfjd.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gwfobhgvq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gdvymjhwl.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/geawegzia.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/glsnrvdqf.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/giaglqjja.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gupobcuks.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gzxjpzsbt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gnvtfrcqz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gzlvelskj.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gzwlrvrxq.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gifgknfhs.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gptogozus.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gvejvhizo.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/grjnkpcek.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gumbslqpv.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ggogjfdue.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gltxxcyjq.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gqpuiljxj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gvcubkypa.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gmwmiewnu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/grmpgtqfx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gnufxhrzf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gtbhdqhmo.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gozjjafki.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gufgzdxwm.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gbqshhxgx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gunisyabw.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gxegwdatf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gryjtbujw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gvmqllssq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gllbwuyqw.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gafkqklvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdvnpeulf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gmhzapquc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gdeaqbxeg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gtbwbxxte.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gfwwejewo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gysmoathf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gylxncjem.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gtbafcuwu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gypqelsbb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gbjyvzwck.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gboyvhwts.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gschtzzoo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gxlpjuchv.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gsmxcyonr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gimrrbzjt.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gdxmpgsta.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gerfeotvj.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gfhtsvajl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gdmyzftzf.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gqqvrpmor.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gdevjgkky.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gelbknqts.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gokyavrmt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gkthxmqhm.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gfqgyzczp.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/ghkguanua.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/ggqtzfywe.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gdonrbkgv.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gghcrjrog.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gieopffoc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gxccxgbgv.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gexczklfj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/goepmenzo.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gaibodnny.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfjykls.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gzqdbheiu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gspeclkdi.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ggjkezqxg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/glouuyogu.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/guhyniwft.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gmvqxvhah.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gavjyuozq.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gilwegnov.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/ghsewgwap.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gopmfnhjl.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gjtuwzfkv.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gfizxmoqt.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gtbewujpa.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/guzyguoyg.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gneeojlsd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ghuwgceyt.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gaeaifsas.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gcevpbaug.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gnijkrpiv.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gklcgdica.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gctlblwow.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gtondvppz.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gvgmtbbrg.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gdbztwkzz.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/goplnovsk.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gpjgtsjno.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/glnmelqen.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gabjbxeng.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gverjjhbl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gnqvmsxnz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gfxgslohx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gbjzdhayq.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/grsnmevie.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gsflbeclx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gmmqorurp.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gfksnnhfa.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gxptygiaz.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/ghgspdvsn.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gsvomhvkr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/goyycmwjq.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gtilgzggh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/goicrauvr.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gstiyomnl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gkryqimej.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/ggjplsxzo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gedbpldgw.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gvffvejbf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/giqjvkjcm.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gildloxma.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gwkrdgyza.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gnmdsviqi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gfimcexlk.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gqrujnlnx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gdlbvxafr.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gigkxdiwg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/guqklocyo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gyasrisvh.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gnqjndfhh.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/guwvrffkj.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grgfrohxd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gbribdbgs.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gayzreebm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/grsmbaayw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdiqbaaym.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gjpuxbvnq.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvzraztav.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/grzyuyrjw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gdjgsxwia.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gbmablcnl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/glvazjmnl.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gwxfzplyi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/ggaepdsev.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/glsrtqcwa.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gzjebzxdf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gtjbdrngq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gkwscydgh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glpfpnpgf.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gmpjznxms.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmjknppkl.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gjnfdazoa.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gpugmyohz.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gdopsfubv.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gykpjmptd.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gshaflvoj.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/ghovoiuem.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gvqyyunqy.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggqxzelzj.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gjkpmehgg.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gzyiinddm.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gegtowszk.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gcfquptkm.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gvrjrhtdm.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gdihoqybb.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/ghfriaedz.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gdqzyzmqv.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gtiyfhmma.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gbhvhwveg.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggvhtkpal.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gbhpbzjen.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gmgznempg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gtoejsbro.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsloaxlor.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gagojcghd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/guodmnlyq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gmvyrqqkd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gtngvslfh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/guisbtahh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gpvpvvtji.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gowwazqgv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/glothcfeb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gegmwxlex.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwdwrbahv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gsaicejdz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gpndgcrbq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/ggefmniva.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdnmwktpu.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gpqlurfyp.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/ggzzmwrdg.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gmqxgsjmk.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gfapkiddg.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/grqkbtfcu.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gztexmlvq.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gyltjknav.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gydhmgnqp.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gkmbhgsmw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjyttsemb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gkxwmqsnq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gsezpljqf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/ggvqlrbnh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gykgqetvl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/ggbtblgsy.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gxfmbxyvz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcsnhdxib.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/grzkpagby.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gsvhgdkhm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggzvymloq.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gkyqkgcna.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gehbbgoma.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gibpstmdu.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gyidbcowi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gmvldfojk.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/giwwiekxj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gvkakuhgp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/ghgqshlmy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gcvwjwmdq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gvcllwgpl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gmjtspjkh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gfdfhtwwu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/girowpxtz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gopkyzjdl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gdxbctiwk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gkqusnjak.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gzjruyroi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gwgklcrfg.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gpxxaqdlb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gumbcmfij.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/goyvcjqzu.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gpqqoarkg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnpkbkspv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gdizfnkqp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gkexkpyut.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gbjsrblne.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtgtefhjn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gyjhidjwx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/ghizzwlwg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gwfnyipyl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ganrkuvoj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gzyvsouij.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/grnqkzetq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gypakxtqz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gszipksru.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/glgprgwfr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/ggzlfznts.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gncpcloms.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gilwsfvtp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/giyooymsn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gyazdfioc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/geffwyouv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gkfudeqde.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gqzstinmd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwipemna.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gmhjjrmpg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyehdutoa.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gznvgrros.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gqglkanlw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gwxoefblq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/geuyzqaof.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gxnhtkclz.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gcqmpctms.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gulhoersl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/ganthibwm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/ggvueiawm.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gkzqftitn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gkbtjzpkx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gsqrpxfnv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gznrosjsw.sHtML


<!-- 参考信息 -->