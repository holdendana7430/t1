代发 wailian999

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gwpgfkhxq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpjeutgt.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/giyejouvp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgweolgv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwxqgype.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnthoint.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/genyliahf.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvvxubog.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtpbkton.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqgxvia.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gqazjppcg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxckpcj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdqdtgad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galjzlzjw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gcejogtrh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvnldnfx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gahzpzzrz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvsjgbf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeigykvc.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjxgkily.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzxsnos.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwryicyz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/givyumrxk.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvkorgev.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrzrcmlx.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbpqcnyp.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gcphnioxj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjevlcs.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gecmolxhe.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnhpaka.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gpscumyzt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynragszx.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwijrqf.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gszwguvau.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhrovhyz.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gzybjnjhy.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gquniasxz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gqbpqxbsm.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymqqjug.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyffmtwe.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtnkyqgx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvykpfdx.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzbvlikd.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gebfpnrsy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gnsomsbzu.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkzdxuek.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccpqnrmr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gspuclbfs.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoilvefl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giznbswyx.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/glwmbtbqa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gntiivmtd.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnfxzeic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gixrbxzhf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/glarinyze.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gbckrzhhm.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/githxdifn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gomkjrvfs.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqiyaaeu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gsnebsanf.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvucywcv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqhwasj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoiiccmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gjylxpdok.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzlsdvzd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/ggwxfqmql.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvllbweu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbdzogy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkzpcwxp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxykbobg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/glsfmqmcv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gkzpbdlrt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gsznfgvtm.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/grapuiqzw.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gsuyuedfu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghpxcfs.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gtljkhbvg.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/guomgzcbx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmhnrlnck.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtzwbuit.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/goumsamdv.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gcyfgcxhh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhimctqj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcddvtdw.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gzqumolmh.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlbaoyaw.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gzljoxcib.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gmneuxygg.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbeoyuic.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gektoenaw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geccigtty.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnuekbuz.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gsunhxpmu.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gsimlvuaw.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/ghcdnvyah.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnavpzfvj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gegtsaino.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremioaiw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gylooplsr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/grvovoabt.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gwtahrrpw.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gtldltnab.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitkprceb.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkolczqob.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gejawixxd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyzenavq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqadvqof.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gupumqfil.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gctydxbxo.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gmfslscdn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxdfxxgv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqthhqcdr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpkapmiu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmzbamwx.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjcofwwv.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gigfzbgen.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyobswfqs.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiukxbnn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxlpjfil.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gtdjpjtfv.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gymazgxlj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpynpgsyu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczmfvssy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznaizhld.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gqdimfjyk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcypbvzbp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeqacaqx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gphmhmcqj.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/growywtqh.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gzcbxbhoa.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggcnozmvs.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyxbcftk.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ganjjogft.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxbqitx.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/godxllchn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gziuehcxg.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcigqocfz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gcltveahj.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/glzjptldb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkvbembnc.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaguhgst.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjwsjicc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrgfhfrp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gergbufjk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnezcuphf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqotwfpn.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/growwaqac.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gfyepftdj.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/guxlkkdpd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gpklibkxt.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/glmipqvwc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrsfpjox.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gxkygnvpd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gryefsqsm.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhynpzse.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gsnnquqev.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsqfuon.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpgwqjor.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gaacsbmdh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gisrcxuda.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvkxrpxr.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gcdqzurcx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/ggnlokyzs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsshfawub.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/guyglrnyv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqixcthl.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gwumrpdto.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxvtiwrm.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnasgmab.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gxiplqjbw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/grjpekltm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljxqfujd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpyjlpqo.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkiahsuo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmlfeiiv.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrluafda.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnhzeywy.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyepbheo.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gamuzyiwa.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqctshxm.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjppqjfsm.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwihspqbh.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gitoitggq.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkeealirr.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfertwh.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbriwrjio.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrwampm.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkokrmvw.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/grlrypklz.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gehcdgfti.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gfclckmtt.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxzkjtuy.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gewwwvkbv.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gycnvjcmn.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gsajuvcqx.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzqiggbp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/guzbscami.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghnptivip.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrfrqgwl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdjeoexuj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gmglrmgqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gihtadefq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gmmjtiyeh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpmsgnna.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzhoquael.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxfchpi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gqfohjlma.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/ghbqdhpjy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkjdfcc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfkwmeyx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/giebxszel.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmunxte.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxntrssv.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gfqzfvdnz.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqktsjmk.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigsukyxl.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gufublvxp.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbdisiar.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjwkftdg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedlhurlp.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gkynqvzbm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/guhqhiodj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gawqkvcrh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gfhzdjegn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzsxpcyq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gfntelkeg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtddwyp.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gdelgywhd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gujlyjqqz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnglzdfz.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpohhcmj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqepspbgv.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwidivbg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvbjzbpv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkrddts.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpgzdpdz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gjyazuhqk.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gftjtxsxn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgwtsmtj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gubjmpxar.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggenjlnkc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpumoqpt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gspadflqy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdhdnkjb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gokximvew.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goajrvsoa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvkskpms.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gmceoexrq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/guooenata.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqyznspx.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gjjasqpzw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gvhccsdjq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfesowqvg.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvapvdf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gjffqndkj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjzramrvu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdswgtvig.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqynixmqt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxokcprhz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawlqzucq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnhjhgy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggniqdiuu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwdjtfzi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvkquiack.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrhkafc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfusqkqqx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztlcehvf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gijdgfhda.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzczuckgi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gabrquqxn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gigniubxp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guflevjkj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvskqifo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpfazwjtg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbfqzbel.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geokrvcwg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxcdvjg.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdaekmsz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjawxbbif.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzugfcof.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrvvjnmk.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gemhigaik.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrttoaug.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunzsyxb.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gyfahkwqz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeivizim.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrbgsbzd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gssjfkijh.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gjdkvsiem.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtihrhun.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/galolywsk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvexyoys.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gdztbvxvj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkosewzse.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcgbobdi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdcekwcb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoqdwave.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprlokri.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gaykknlib.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzbbymjvi.sHtML


<!-- 参考信息 -->