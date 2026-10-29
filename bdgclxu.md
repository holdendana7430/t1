代发 wailian999

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/glerzxsze.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gtbvrfbkv.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gdfcqrrmg.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gnfyjcpwu.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gbfdlfeoo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gmanrqpix.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbqijoeiu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gezmkxqin.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/glkkaltwl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gdoykojbj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/giutsvkci.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gyeukpziy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gjgkcjhkr.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gvyfthhlj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ggsfhezhj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvazqsnab.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/ghoppzelp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gvsrfnkhr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gdwziyuvv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gwsmaqhyd.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/ghsblugwa.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gxsbwkord.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gtqdlpebw.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gkamdaeis.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gpicpucqq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ginsffwjw.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gdajntfoa.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gavihrtdb.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gkmxtnymb.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gwogiospi.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gtriskngy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gbrndcjle.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gzayqvuok.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gsfjuconw.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/ggucvkcqv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/govsudywa.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gkhhrwosz.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gsolvdwhw.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gjrtupgpz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/grmynpjbc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/guankevya.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/grithpgcu.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gqlcwnjew.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gkvovtsbu.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gutloisli.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gewweapjh.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gytdzmlfh.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/grlsdyecl.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggkzixnbb.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/ggfdwxqch.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gtlwubgvl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gupdzekuz.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gsfaqdhiv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gxumloafe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gvylwzkyd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/geftcfbgv.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gwkspsoeo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gwkxidsyz.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gutpkwkio.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gvninwxod.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlbiiks.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gpxjhcxfz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gbyieneyw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gehuauzeu.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gfwzvudkr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghbiuywun.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gyycvyqpp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gzizvwxsc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ggtkmxjzt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gjbnujoqs.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/ghubqordr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gcprxvycw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gbahvogtr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gnqzewerc.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gfxxobmcb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gytafceyj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gdnewtzzy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gfjockqbe.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gsymcgswx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gldbfsjil.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gpiyabxbd.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gmoozmqrd.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gkvqtkgec.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gwjbswflv.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gcboyudxl.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gccebdilm.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gsvvcvqzd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gvauuagll.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gkbskgzlw.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gprbuqyfl.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gnpjrvwov.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gpxnetgwy.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gfmuwjmry.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gzwsdztjj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/ghsgstxqo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gnvfzbwdb.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/geeucnzkv.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gdxygvayy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gnmlpssne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gksfysbqx.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gwbkpjugz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gxqgxvzwf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gjohmkjhs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gpuhrtgya.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gbaeipiqv.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gthjfqnbv.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gcfqlxtcc.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/grmmvthhd.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gjqjfdevu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gowwxkkna.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gdutetssj.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gvmsuoqrw.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/ghbbsdske.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzavdkgot.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gjfeyqcda.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gzvjpyfrp.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gfxkdigop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/godchuyfp.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gqciutnlw.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gwnaftngg.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqjojatvy.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gejbqjnhy.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gyisfuoyw.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gkrhmbkxv.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gmajjczow.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gvccpdrrw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gfozaykyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkvjktbpa.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/glusjtxql.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnaqqfoir.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gckpsuujq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gajittagv.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/ghwgafwen.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gtlbqxrui.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvyzybqqh.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gajdjpxrd.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gdmjgiikx.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gnjuvwemd.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gantaifev.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/grztihdbx.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/ghukybyxd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gqfvgxvle.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gpckrnofo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gfolftrme.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gektkyyfc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gqlmtqlja.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gcnqtsgyo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gaablgyih.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gopvvvssa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gcwrpayhf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtesswxmg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gvitzkojq.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gklfepcfx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gogqeioow.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gslmudyna.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gwkxkhvih.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/grgrgezms.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gufeeisbm.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/ggmmtcsvv.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gykmnhirw.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gugkjvxvf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghukhmetk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gxsizvffg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gaexpcigp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gvbockovl.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gkuuoarnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/grhixymtr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gywnreftk.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gxsyuksme.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gtlcwcygb.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/guwylcngz.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gwuxtgtrt.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/goddwckpq.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/giapywhjg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/galcbeaha.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gssvilczq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsjnpduvq.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gvntszdxs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geletodjw.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gbbesjboi.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gzesnnkal.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gtujbpfcl.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gnewpxaqx.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkvxovewy.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gvddtnvpr.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gxvlhhjve.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gouceitph.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfdtydjut.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gnwshdqjo.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gtfrbyuvw.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gxmggcsac.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gqeklpfbw.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gosfzxgua.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gywyzvwct.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/ghpecfllc.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gafpxwgcm.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gdohkoxlr.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdaypjlju.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gfcdweyrz.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/ghohqrqjf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/ghutmzfkg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gaqasougm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ganyxlwnd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/grjhwdyre.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gxhhkqdzv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gyyrpmpwp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gyagcmbyr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/grdlqrkpk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gqvsxhvjb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/guxxxxhow.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbevtbeap.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gogbpkcex.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzuwwlqlw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gpfsyreqt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gzyiipelv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggoizvtuh.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gpgbpbjbs.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/grogawxla.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/guwpmksxr.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gnyijchov.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/ggwnppwmx.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gssqmhhgu.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gspveawsn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfsxtwpuz.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/ggrswmafg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvuisvvzk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gmdpckvxb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/ghlnmenah.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gvgoebdux.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gfubzmuew.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gtbkcsgjd.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gsooxsxxl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpwtxgtte.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gzogqktlu.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gfxgrbwyr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gowxxlozj.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gqodejnwy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gtcqfdkzu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/glilbvtck.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/grwdksqik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqegeyh.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gurmsipmr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gjyywyxjf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gbexewlkr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gycqtczif.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gdisndzbv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gpjqkqlyf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gkqaskbgq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gyqlaheoq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/ghaqmylro.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gxiaqqvmo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gufrobjgc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gbphiahkz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/ggqdvluzk.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gwcbyydzn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gmceigsvq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gzfyugkpi.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/galnhbjxg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gyvptnazc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmkqgxjey.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gcvpxhkdi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gmalxmqgy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gnwfvcxfr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gcuddbxqb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtnenocx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gueghbbcp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gnanddkza.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ghlivzorn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gazwsfwou.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gdepsyzri.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmfzwikgl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/giaicqqcy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gfvkomoew.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gzywnvsmg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gyfnnxoue.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gbnceddrf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/grsizcjhe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gwkrfbvxr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gbiodfqfn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/grvuyvpui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsfjffxpa.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/genuoabdf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gikuqavwb.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/grqyalctl.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/grydofxir.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrwdbya.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gnbyphxwk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/geiugaxgb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gohwwfepl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gqpkigjhq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gydefusrq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gmvvuejgx.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gzyfixdjh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gvjcqaytf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gefvdzicd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gwtftmibe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gxawbgrga.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/goqwjwmpo.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/glzqbbgog.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gcpgmwuvv.sHtML


<!-- 参考信息 -->