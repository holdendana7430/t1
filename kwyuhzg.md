代发 wailian999

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gafwkiuip.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gcjiiuciu.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gjrirdwox.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gwacyjcal.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gkcbxezsx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gzkeafjtt.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gywbxezzo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gspiasilm.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gusxkvvhp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gqmsndixl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gghxkskjh.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gybemouqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gkwwpxjez.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gyhcjvqdt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gjyplxbnp.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gdnsfvmlc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/grtihajfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/glxhryohp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gvqefzxmf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gclernlpz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gyegmmtfx.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/guvcmlbup.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gdhrawbcq.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gcnegxcec.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/ghyqpjttn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gygspdbhz.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gaabumthb.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gklhutqbj.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gljzukslg.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/ghbdtsber.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gzlhdgoll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsxjkohxu.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gxghlvycz.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/ghdfraqaa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gimvvewqj.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gnxklgshd.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gizwkkrqs.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/geqlvxgnu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/goyxaqtbh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gkkwgzhbd.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gedrrrldz.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/grrowycad.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gflgetplh.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gxrrlczkf.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gofgvhino.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gjaaggwkx.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gggzbtutb.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gkswgiwgs.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjijgfztw.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gflooysgt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gkjikiqvn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gaxpllhte.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gljirefcd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gekdwdkln.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gakvfdsov.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gmzxapdqa.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gkghjormw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gaxfnoabk.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/glphwrvoq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gpspdggur.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/ggltlevnh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gepnddfqo.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gzugtiutc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gfhhdidng.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gugxvtngs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gsnbhtkmd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/ggercgoss.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gfftlkqbc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gngdtknuj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gpwdwjqcp.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwfoafqnc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gvgdsbedq.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gtvxtnfiz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdapwabka.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gcnwenxsp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/grncaogol.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gzdnpfzyz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gzekgmdjy.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gxnlmyfdd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gwvsqfsel.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gkoylnawk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gzcyygsbf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnkpzcoqo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gsjmrajzk.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gbuivjenl.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/glxhvtqzi.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gtalrmoib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gzkmxmsrb.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gdpgzbtxp.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gaflofqrk.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxyddpgar.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gxbghgngo.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gaspyjoeo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gohxwlhnj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gfmlaxmvc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gvoyffznn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gfvkhyllg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gfcfowmmj.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gwgpfabqe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gqrxnqaqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gdlkkxxkx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gwozvtchy.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gphejvmdv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gjhvvjjmh.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gebeargse.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gzpftupkn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwkyakl.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gnbrtbjsc.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gujkqgpne.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gfahghuhc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gxpjnuydn.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gxycegjyb.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxlokwyex.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gxnyioafc.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gbfykdqop.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxdxtkftp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gobqvdgqo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gacvqvwyc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlaewrb.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gategvmsp.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gtoxophal.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gzofxsizj.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/guctinexe.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/ggtevvwcx.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/guulbeaqp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gvooewoxs.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gxacqejlo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/ggxqygbzx.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gsygobofv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gecykjafz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gccefqvma.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gopyxcjpx.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gomzfurnr.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gfmxpgzgd.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gsrghcbks.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gjxsxebhy.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gjeemkkth.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gfacxfier.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gnhymrdzq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gksdvfqix.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gjaizwthp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gxhmybmdh.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/geikeokls.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gqwfpqivq.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gjfxwvppr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gkvqkvfzw.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gzxozbcqe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/glnnkynvj.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gypvcelof.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gawrwqnok.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gkyzogvjv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/ggoueyrqo.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gpjnrjwlh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gqalpvklp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gtvuqtmuz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gnkqnodgm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gfojyethf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gguawczad.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gnqtimnnj.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/guljegidx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/giwinhsmz.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpzutcxue.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gteukuqdt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/goudfpaml.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/ghpsuveeu.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbihbueqv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gynxumwpb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/giafvvczd.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gbuogrwdb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gsxrdkocg.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/ghrxkfzcf.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gctoewdbo.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gmijitnas.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/glpusiede.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/ggxegayis.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gvscnbpdm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqkyzbqzs.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gslhwofkt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpotsbrgv.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gbtrthqpw.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gaadbfapb.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gdhoffuun.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gzwvoqzfk.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gcwxwfzse.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gelkzwjch.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gqarhgcjt.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gaqxwwjko.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gxjeteiyf.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/ggtvthnci.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gmiqhwbdw.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/ghycajzvy.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gqfzcncux.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gyknoblpc.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/glqghmcvj.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gcqqazfrh.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gbaucmqui.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/grfblvkfi.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gemzyyafg.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gbbllublh.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gcdhciqri.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gnyhelrgy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gwylviyjv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gkwgmnimr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gnmljjmow.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gifyhynkg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqehwxc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gpqtgfcjg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbgkjsfse.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gztxhjyje.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfluoygge.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gkzghuxwy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gojhhnang.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gakbssalw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gglzlakdc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gumreszec.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxwdickvy.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gwuyijxlt.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/giocarfqg.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gfnpekzhg.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gwzvptknj.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gwscstnhv.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gyxzvmerf.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gkjmquczy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcsninzul.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gwggregjs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gypeghuin.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gbxpdmzww.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/galrzejfj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gygaqjgck.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gykzkvgjr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gqzyyfiqw.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gdjxlgtpe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glwwucjtt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/glpmuvdpj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gkiwffvlx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gacbseqje.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gfgdvbuyv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gczxgqfyj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gotikbtxo.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/ganfsvdlq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gteyyhcpy.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/ghkdhlvsl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gewchdvwa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gaifctutd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gxjwrmdwp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gsxvapwzv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gvzdtvctu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gqiqntbgz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gxlitfmmy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gqaeosiqv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gvuwkjitx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gknqzrtyf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gftxbpuyn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/ggqyromuz.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gfmpxspjx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gleqcmtux.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcawtgfsr.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gzaanrgpr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/guqbxrmdc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gtrssnkjv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ggxdqevbq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghcvecjvc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gstiakvcm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gkinfsoox.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gunzzfqnh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/groelqguw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gfyxiowtc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gynzcvoks.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/galbvwfdb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghfxmeblu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmjqygkpp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gzxknjjai.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gznvbcvuc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geowkujhw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghshaodpp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhvqbihp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjigwcujp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gdwbibsqc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gnvlkhmoj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gaozfsjuj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gevqntscw.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gnctkmsoq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqhdxchym.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gtclcvxxy.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gcsfipeup.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gmmiabwoj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gvfxagbso.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/grwpgaftn.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/guzfwbjva.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsaprml.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/ggmgmscfy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gwolwgdtn.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gtmxxtvye.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gjjlbdahs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gvradtbpp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gshetkydp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/guyknozyk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gdudkwoly.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gdjsyvyer.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gxwqmdbxt.sHtML


<!-- 参考信息 -->