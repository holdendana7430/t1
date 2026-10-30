代发 wailian999

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gkizaxbkq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gokdhjrbr.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gaziijkuf.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/giptkcvjt.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gnvwcwoye.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gmbyxoaqm.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gactakejb.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gjguhjvrj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gtzgxfzny.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/ghuxfpucm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gkyixnngj.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gtrlpkyyz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gualdovey.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gwpfprbpu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gigjnvoud.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gumvicvhv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gzoqzmqcp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gxpusdkik.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gacarwhtu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gywwohibq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gzgxuznso.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/guijfxiin.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/ggrdqbkck.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gnueamehd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gxlfnonal.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghrqulkhn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gmzdfivgv.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gchcdceqg.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/geodwjysf.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gqmxekgoa.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gjdvukwxg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gkttkbzcr.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gamgtgvxl.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/ggyrffnez.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gvcoiiwxw.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gfhbcxxuy.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gkbzgbcmo.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gslkqcyoa.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gogosydpc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/ghevvajmk.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gaaymjklr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/ghfcqaqvf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/ghtxprkus.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxpkbqzda.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gdtvmvyih.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gkyuxacpa.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/guygopqhu.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gbzwdmgdd.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gizmuezkn.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/goxphqmvi.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gvfokewll.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gfsqbkbjv.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/guyncpngi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/grgaztucx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gsqimsihj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gqilqtwfq.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/glyvfihmc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gyaxefisi.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gnmqirbxa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gxmwlfxld.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gmngcwfsd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdbrekti.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/goyrqkpfj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gjmcwyajz.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gyzaecyzu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyjzwoqti.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/guwocpivn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gsceqekup.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gkvnjsypb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/golkzgutd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gbrwsqjle.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/ghaixzgng.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gtnagkmxg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gtsgxneob.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gfuymlunr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gwpktgezk.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzfvdtdlt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/ghczqvilx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gwkcqxzbj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gnkpjvdtz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gqcgewegx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gnmsnqwxa.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmkrlzypn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/ghklxgxkl.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gouddxlge.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gfrxstyia.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gyvjlecap.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gkunuqqag.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gsskffetp.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gqfhsxdjx.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gvclgcudq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gfbekoeqt.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gxfltrblh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gngyuhlia.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gtztiovyj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gsuukyfxt.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gtnxwrkkk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/grfmvcubx.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/ghasddhit.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gnxunjeue.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gqzjztkdv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gftimvooa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gurmgcpgs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/galkbbdoy.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gtljrthyb.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gnrfvjqqv.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gvivhreuz.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gwpqoxwkl.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/ggjxhskpo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gbxjfkvpc.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gklcmyuzk.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gxcrbusnc.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gpcdkasoa.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gzcvcckte.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gjzlkviuz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ghagdakqe.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/grlzqfktc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gzfandqxt.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gbfonhgnx.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/grpiopilf.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gayumbmkf.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gaozurcks.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gukcytqfw.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gyuwtblnb.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gkdmuflcq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gkdstptii.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gzjzuqjwt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gduxqsntc.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gvrdndhyn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gkivqbfbf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gpvnusilc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gdjzgfdic.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gtjjpxfqx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gztzvateq.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gcpxfrxjb.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/grvkqbyka.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gsalntjbg.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gszmeuccg.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gupbucomj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gbiscqbxg.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gygtgwzvn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvgfjoykb.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gvpirzajx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gjmuyetuw.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gzqpgivgt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gpxjakumx.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gbrfpnkkk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/giaghtnhl.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gverpxclx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gdzmofqcj.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gcxdfrrio.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gkxxaqbza.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gogxqixvw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gsnxvasni.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/ghtftowqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gqbnzqcax.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gtuwckmqe.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gmlgnqfnh.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gnewawbln.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtpxzrctn.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gbaojkasy.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gslpesbzc.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gpbmwotdj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gekqzqhmo.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjpvpczbt.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gnfegpgdq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gtavsecpw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gvqrjrloq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gwpniorof.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gtbscngjj.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwtbfpdfy.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gkbcbxsol.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/ggioaogdl.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gzijywlwu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gfngqrvho.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gjtmzmtqd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkujrubrs.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gwqjrwyus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbttelgha.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gciafztbl.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gayldtfyk.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gjizzllty.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gzudpgail.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gipuaygkc.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gkuqfgrvz.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gjzapqvfa.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gbczxldef.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gaiimcodk.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gjjcacdph.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gwadtahen.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gjufrlwvx.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gzjiogjiw.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gupdibtnu.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gozgkvdpk.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gkdxveuhj.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/geoonzvlq.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/giiuqpqpk.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gwdzzxjou.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gfavlxxmk.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gqyihcphf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/ggmqtqwpr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gmjqffaiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ggewtyykl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gzwujqmky.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/googdnlvq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/guxpzpsvt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/ggssrpoth.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gcmelnzwq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ggolphvrx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gwkjlrccn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gqoxhyseg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gsbqlpswz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gomvyssag.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/grjieolac.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gyjbvtqdl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ghtcsoygu.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/ghpooqacl.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gfgewwacx.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gohjonwak.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gcjmgmetd.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gnzrucazh.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/goaevvwey.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gmvhmlxbe.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gpdufysnk.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/guvxhysot.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gfmxsmtie.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gxxszdgcu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gjurujhsc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gppzsbeyk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gsyjoxuxx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gqnhbvtvn.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbvdifv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgkwuwxc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/ghbpbhgdl.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gzumkczlu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxzntgsht.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gxeswllyp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gdluoujis.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/ghzqubopc.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gkorltoza.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gnxcpgcfg.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gwqcuxjwa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gijgnvvyc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gfehlpmai.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/ghfoamxlw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gljuqikku.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/genbzyltr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gddlitxdz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gsnxqoljs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gdjiiiemb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gundbdizh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gozwndiwt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gqmkydftt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gvohvvagm.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/guppcyory.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gvcmadgat.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdtewdspb.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gzigigotf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gycsgvdtg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gpiusbmqo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gvhhzhwxn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gtgafejrb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gmcbzxdyz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gefsvzfwd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gsplyzzwm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/ggixfkllb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gxdgwmmij.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gimxtxztt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gdrdntlxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gfwmtpkgu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ggubzlecq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gavkxwsvv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gmngaeaxc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gdoyiudpi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gijfpwxaa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/ggtanvrxw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/govlocoqu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gsgksgved.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/guvaqddnn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gspwwgaer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gugwfpcvb.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvrhgeu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzezfnjaw.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmubndvgs.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/grrrvreeo.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gnxkpowzh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gjqmyobkq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gzxpodnnd.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ggnivduqd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gzoqimitg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gqndgmukf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/glubvrmnq.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gkqpujtsb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gmgrrbqtg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gfnckexlu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/ghxgveinz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gqjyyidzf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gkkxkanep.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gzmvrheqc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gclvlinld.sHtML


<!-- 参考信息 -->