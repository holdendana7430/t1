代发 wailian999

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gmekwaatj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/ggwfyyqdg.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpcgzvw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gnombtvts.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gwmnphqlf.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gpcbrjsep.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gueiyunpy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gutbqiytx.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gxaqiwbqr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gzmcjsmni.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/grkyndpls.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gxgtyezxm.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gaqxglxmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/grhyepndd.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gxafxwflc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gsvfxwtbv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/ggyefzcod.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gzlwxtohv.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gwbfqbgtw.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/grrogkhfi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gmrehncwc.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gkgtrhxnf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/ghxeegrgd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwfutxwqf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gwmertwot.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gshzihvfe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gfmvazzwt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gmmwjprjf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gcbdaekvo.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gggfoiigz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gmedttzrb.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gotcblgxr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gnzebsgyv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ghhojasak.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/giqkmocaf.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gxonehezm.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gwbiihjpj.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gqqonxnnk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtzjuvukd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/giyqqpkdo.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gzjmrkndj.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gqfmftsax.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gfhzjsrdg.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/ggeerchfh.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gynhsjqkf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/goctwivcj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gkmuorzja.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gptjsscpe.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gnamtljxs.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gvsvfnpmy.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gykjknwll.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gmcylapzh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gaptiaflh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gyezcfmfe.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gxnhlkvlr.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gqjogbjft.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnoxkhqlu.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gofbsnqwp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gecrcaxzp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gqwadevix.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gjurkxqiv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gwsekzyjr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/glfdztgwi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gkfpzwnul.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gcodfuqqd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/guimatxhy.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gvhkkuaiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gjgjhpwvf.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gmualaccb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gphprycsm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gmfqilowp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gctgspxvj.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gjcpjrfaf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gaxblfnjo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gczmvccct.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gasgqeekj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gyhonthrg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gycctytrj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/ghdjyjzpf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/goqgbjszh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/groqtrsjy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gsdaozcvh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/grntqbhrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gkahxinwo.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gbekfqfse.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gqzrfyzvw.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/ghmeatikr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gvgoaqcxh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gdifmrvrq.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/glhfvcbwa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/goribuzhm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gsvuaxymm.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/ggmwgqopa.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/ggmnlqgjy.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gwhidjbwg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gcsccdmfc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gpxclwpuv.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gjybdwnre.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gttxayhnl.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gqdlndmxx.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gndoirbux.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gydtluhsx.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gstualqdh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gpfbsukle.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gljcdfmdz.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gumxnfauj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gfhylygxv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gxzeojsac.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/grfmhouvl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ggqntqxkh.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gsvurqsbl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/ghkisyylm.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gpxmzolwo.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gkflaalzj.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gxevzyktt.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gugvugyds.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gsckevnha.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gkjhdagii.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gxnfphtoh.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/grhpueliw.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gcombotzj.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gpnresrke.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gcrterlvt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ggmprgxdq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gwzwruyhv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gpajdrlvm.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gkrhsuzso.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gwzusxxen.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gjpkgowzm.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gdukfpyeg.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gikfwizch.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gdwdbjufo.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gasnawzpd.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gwzetflhu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/giuozfowt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grtxdggdz.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gfqfjigcb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gxxtvlitq.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/ghdlnfyzy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/glfqtfuaq.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/ggyrasgiq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gymdweppv.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/giwodhamk.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gzvyehkre.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gvrxlggjc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gkeiszbqt.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gpvciocsn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gnguoxjan.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/getniybmv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/glczaacnl.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/grbkoyckn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ghgtfonbz.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gfezyzsjf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gvdcqyajb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gwbfpnrlz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gugbejpjx.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gikuvevwm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gxkkkaqxr.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gghgtaats.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/ghdxiwtlg.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gmwjjmsjp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gsrrkbyit.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gmeaiwguk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gipyiwavf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gutbubotu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/grrwkglvo.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gictelmxj.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcnfvbqhz.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/guhhkzvwa.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqtjvcaxk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gcekmzqmn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gqcoqmboo.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gjrevypvs.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ghaxdkqll.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/ghvzrijgp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/ggocdjtmj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gipjuqokn.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gqqoycskv.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gjgrrdfhn.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gwhwyluvq.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gogkqbopb.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gfxyvwzej.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/geheiqfmu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/goispeqnb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcjmdnuqr.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gvewpvrcx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdjomvkcp.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gavhtivdd.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gddchvxmi.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/germvjcgj.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gunjxqvpd.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gsimfvuin.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gibqcwgvy.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gieknxolu.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gjnhztjuc.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gtcbkeqvm.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gehwxritq.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gbutlwngj.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gbaaziafy.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gczjsmjdy.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gekgtyabp.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gkdfkqrto.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gstqiqolq.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gpreazwzm.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gkowflxmi.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gocpdwrfw.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gzmngqfmu.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gjprfloxq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/guxqeyddq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghijhjadl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gdiyowoho.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gyjihouwm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gfwkrbcgo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/ghwtxokwa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gnsyntotv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ggulwbazh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gyqbbparl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gmqcpmayq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/grflgxpdq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gaasfyjnv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnmboeoqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gdgsepxhk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gojhiqtov.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ggpgzjphi.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gpoldccll.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gubbigcdg.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/giojkijvz.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gkegurlbd.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gxohrplcp.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxkcumgnj.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gxnqwfyov.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gichzwkij.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/guuxofsmq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gufhpqksa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/goxfqbdyp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gnojjjmbr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gmrzyzdwe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gsdaxdplz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gfdwkfkio.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gknryrklz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/govkicmut.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gvypezqst.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gltgaryju.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqjqprrm.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gnpamjzhd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gtkpdkbbg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gtrbcbikg.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpdukbf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gwxcjekkz.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gmxmngngg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gpfqdndph.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gglpbhiqx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gldzzblzu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gugjyxlqt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gmxrvqgbz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gcnnxuyfu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/ggbmigakj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gifkgauio.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gdaozznix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gwavsxuok.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gobsloodu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/guihvxpus.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gnwxasrga.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gbexgswna.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzaekduag.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/ghfrdpong.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvpvynaes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gvjvgctgm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/goaobduex.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gcfrlqdgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gkorqaseq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gdcmemdvf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjerguhxc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gkgpgpzxz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gwipqrllq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/grwqokpbn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/guftkzuph.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghvcdyjnm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/grjcnzciv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxwhbkvwu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/ginzmcstj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gqjwussgl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glplekaec.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gkppmkutu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gdywqocdu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gthdnzyqp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gbvoppprm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gtgqndlii.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsajeovbo.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gkhlmjura.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxwgfauxg.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gvxkidrav.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdzngqved.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gskhzelrr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/guucdfdvf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gtfrnmyoe.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gjhkedafn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gxvlymhuz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gjzrmaypv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gnpsaodnq.sHtML


<!-- 参考信息 -->