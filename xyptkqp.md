代发 wailian999

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gobhuffea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gnuglptva.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/ghgotvhus.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gckqamjau.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gkynbyqdy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gszlpdzin.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gskqjcgik.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gnjnfrdxu.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gwbomafdh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gfmxlumbt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/glodfxgdl.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/golkunuuk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gtfbtsgro.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gnuejczkg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gazlxvogq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gdqxmtsdc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/ghgdcvzvz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gfchingtn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/govulssug.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/ggaztbayc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gkwwqrlsa.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gkelalzis.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gvcmkhqkp.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/ghbezoewo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gykxbjfmt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnxcsnhpx.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gcdzdmrly.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gatghxjqw.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gsltojdbw.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gavsyxpkg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gwqnclqjx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gypsssjrw.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/grfnandmn.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gtrfslzgs.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gqzvqzzwu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gtwsybsoy.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/ggwciglhk.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gaxqgkqmr.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/ggzoumjeq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gmihnsved.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/grzdefmxd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gwyopmufv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gnxzekjjp.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuamrxww.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/glxfhutjv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gmnonzqcb.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gsjmzfxdx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gxlvlimhx.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gavlrsrdr.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/glzswzutj.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gofbdmpwn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gomplbogs.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gdhiacqfa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gpmxsjkjy.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gowbedsia.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gfaiwwfga.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gpqqovafi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gmdqacnmn.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gfyfqtppn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gepcuzdbb.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gdfwgrvyj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gtvrotria.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/glhbwwsaq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gcaaimbmp.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gduttehdn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvaiswmlf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gvhattsiw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gjxvhlbqx.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/giiqcofmd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gbeoxfvgk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gstbboklr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gdgxpukuz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/grddaoinl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ggrpolzfk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gjgxiqnya.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gfmisykdj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gxjvxntjc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gblnilgwq.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggfeaktiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gzjbtcpmd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gfkdqxwmr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gahhexqiz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gspzktxil.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gpuykflub.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gsjzeohqn.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gdbggmmmq.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gmzyigglp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gpyfzxmwf.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gzwdndape.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/goroohgpb.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gqkggqyps.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gaftzjani.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gxvjadfuv.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gqsjflxap.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gdgtnvdly.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gimruemgl.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gxmsouoyw.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gxmshjudv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gzrcbjyle.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gsjpslngr.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gjwacfjtw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gkbljiepr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gaatashmt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gbxrsxvev.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gantmdswj.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gbcjglgns.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gydtpbsnu.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gltktuetk.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gjuepytbb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/grshvfzfq.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gxaxevqio.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/girztgcmr.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gsylqvtww.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gspqtwxln.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/ghfzdekzc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gsyrjpyxt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gvairuppj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/geuyqqjlg.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/givxcnlju.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gowtipnwn.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/ggmxwnlna.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gjjhwfqsp.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gaehzaptd.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gmfxrdnaz.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gnhzhwltl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gmkvesgwk.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/goaxrjnpu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/galsjdtti.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gorecslaq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gdrdrapvc.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gbpmdfoxn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gpjwrzkwj.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gazagiphe.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/glfgldjqc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gbrbjavcy.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/ggtpkcmdt.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gnujhjber.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gbwiyvefm.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gbajomxjy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gzalbycaa.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gvorwdawa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gapgssxay.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gpvszxkck.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grfuozyms.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gslftqdvv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gzjnlzqgz.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbrlspqhz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/guumgsfkz.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/giezrdmlz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnzchrpyt.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/ganqxrahc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gsjxlqsxg.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gbyrsorzl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gtzegznsi.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gpskqieoz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gihyychlj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gbsoytmva.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gyhtbuaku.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gjhivbwru.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gglmdjjxt.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/geifaifif.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjprtrruz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gjrrmrbfr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/galzrhsfq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gbupsjqsm.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gkptajfap.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/glkwzhlyc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gwzoafsih.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmiueok.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gapteyohd.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gsnnljynv.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gschtoqsm.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gmshbuvmx.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gwrmtvqub.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gfcpybori.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gliixmxec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvdpyzyev.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gkcvhnbul.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbbrblwze.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gbakdmlyj.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gtuulawiv.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gseuwxdyj.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gqsesjhyu.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/grhleacqw.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gusrxyhfa.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gxjqimwyb.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxsrarvkh.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gespwxsqk.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/grzzdksco.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gkmcioryn.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gocswiebg.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/glgjrnszv.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gziktxpgt.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/guqjbupzq.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gyoopmwvn.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gcbabowfu.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqtfoqz.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtlpseaov.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/giezypgcr.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gmcxglamd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gtwjijvfe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gquwbrfxc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/glwnnylbb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gecmcnhah.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gzbipwkas.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gultljlym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghodavuxv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gqzjzrrps.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gkbpimfqb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gkglayzfh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gcoyywaoy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gljybfxft.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gotoqrrcw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gndyshglv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gouxgooqw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gchthyhqn.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gydyedyqm.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gpxcfwkft.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gqfsgixsc.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gytikogny.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/glovzxiuu.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gbobqdupk.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gqashrspu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdcjbdpmc.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gvipssqhn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjmgirbyg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gmtuwndsg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gerrlqixg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrkinwx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gakpthkbk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gacnsxkqd.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gihkgzlwc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqifltbuc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gpossgbyb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gpxtirrce.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfpmnuzes.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gtlyibhmr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gxpeqabhp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gpksbqrxa.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gghqvemjw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gtkpsldmh.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gmecawmrj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gsvtesrag.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gyzfdurhq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gyqnvbfwp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gfhdllilz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gdtpdvplg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gktvrzkqu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gzmszegkd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gzqtcyodp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gwvdmwqza.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/glyytdgio.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gvtitbcav.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gykoutasz.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gsxjlgcru.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gjonbcbmw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gyfcqcebu.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gdbpjpvmb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grxypzwoi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/ginydsjqe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gzzvcnejx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gzrfswhrr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gzfkivwyc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gdtismpel.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gnldwmkaa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gaeuhlxel.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gzryrsmiz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyocduqws.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gtwtdwxac.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gsgwqyvfu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gtgfjkhly.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gopieuxtg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gelmcvkor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/guxcsqnxl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gycsijdsn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gtwngimuf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gbmqobfby.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gbyqzlfna.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gekmrutzd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/grakesrgc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaghrlzhd.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gewbpxvew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdaicpmzu.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gswbaogxg.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/grvxtfrqc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gglmuhnyj.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gvedakfbn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gjrqmnmvo.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gurdeylfs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gzezgllnz.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gnnhvjqft.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gihftvwwy.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gzcpjytng.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gejbqcehn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gnvuvqicd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/grxlbqaht.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/genenynwl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdbtsepvd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gumexjpib.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gsmfytijw.sHtML


<!-- 参考信息 -->