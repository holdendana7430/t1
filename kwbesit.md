代发 wailian999

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gseemqjhe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/ghvbsewvw.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gskpnglhc.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gxmvsbdmo.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gavhelzuo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gyizjmstf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/ggvfxqaba.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gluadifvf.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gibwygjkt.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/goemrcrby.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/glksdxaqs.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gadjkrcud.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gebplcpas.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/guajydezj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gmzpdkgou.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/grqxfaqbp.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gajpugqzg.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gorvvqqkx.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gtfcthkiq.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gomukizxx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gfoioknol.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkwssufdd.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gpoigkhjc.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gezjbfnoe.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gbrwejdpc.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gfvsaboti.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gubjaiclv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/ggjvjqnqe.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/ghlltamoa.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gztuygcjz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gncbvzfbk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/guvrkzprs.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gujdgnjsc.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjrqkhmi.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gjbfadiyb.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gxiqlenxp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gmssmwior.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gjvulzhjh.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gsqqqlael.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gllnveecu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gpjtoetnl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gbbraequp.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gqndgvkop.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gkcvjiuhe.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gmgyayyhe.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/ghwzxycwm.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gvterzzjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gpxugicay.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gnqsckrfe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gfobwxewv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gctvwpoxo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/ghmfoqdrj.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gqhimbatl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gssmpuwmm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gslxlgenr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gcdagzoll.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gnjzqjekq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gnamvmsvl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gfvfragon.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gfefcowhg.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gmvlfvseg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqcuxivcv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gatrbxiuu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gitykfnpr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/ghksskvqt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/glnoybclg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gkhjqnkto.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gtdizmegs.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gyfhmwmaq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gpdktsrwi.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/ghsknlkvo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gpsehvnnx.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gqxvchmga.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gpfaswpny.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gnuylvazq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gnzrgxqtk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gzaoeajxk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/ghenwgrhl.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjfbyvyzq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gwqtgkpco.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gvqoqduad.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/ggzoxwrqr.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gisoigffh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gywbxfgne.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gdczlelgq.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gihwnksyc.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gtnnwsqku.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gwlzeiteo.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gmsgemaoy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gnppwhliw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gpvysmmac.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/glnqvagie.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/ggnnmjmxx.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gafjxocpl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/givmagrhw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/girbbcxyd.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gsyvgufyf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gecboskby.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/glbedabdk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/ganrutvdi.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gjiralbon.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/guelqipya.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ggudajdvk.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gfxmcbjoy.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gynxmmyuo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gpadhfkhg.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/ghqyakoam.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gbqcljlvt.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gazbrhkqs.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gbjyzfylp.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gdqkfhfki.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfwqzqoda.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gossftmzb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gcuwruqnz.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gziomotyn.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/giowsmiek.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gjxhawgvz.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gsdwkwebx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gubdhcupw.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gzbqbenwz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gfpopoedk.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/ggpyzjlen.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gnatfogtt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/geznakntr.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gvhdnwnai.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gkwomlqfs.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gerkbyiun.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gxsvbysyh.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gjzyrtusy.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gsmnzvpjt.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gmmbmofie.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gwoamopai.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gyojrwjqu.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gkoobrzlb.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/ghmktiguh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/goehtnvnc.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gwxpdylbq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gntzcvsqv.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/genmquktk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gbunqgvlz.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gorsapowc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gkrthwylw.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwkfgvrup.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gxrjjefyz.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/galsdgiyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gbnkkibpl.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gzoinxbqd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gqsxgrivr.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ggkvqvqkt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gsokusjln.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gznwickci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gkglfjqzu.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gkbgrdebb.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gfyyopjby.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gbsjmizyv.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gubzoemud.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gfynhlvdb.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzvxwwmkm.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gfebjyspi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggxcweddu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gutxpcenq.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gipetqqwm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gwjvlidek.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghjfxcijb.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gdaahqvpr.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gwgdgcslh.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghuntthxf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gmchbecbu.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/goqjrpskt.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gzaeiciun.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gzbzaidok.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/ghcmwgygg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gspohxvxu.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/goyzplnsn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpoeygtnq.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gxgbmitmf.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gkfrseeoc.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gxbtmnwzw.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/ggwnlcvhp.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gefgcikhu.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/galqowxac.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gvhtmjqss.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gvcbzuhss.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gjxushviq.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gufopxeju.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/geijlvoly.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/geibpshpc.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gbzknwesh.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gipyzsrci.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gsgnkfann.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gianbjctt.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gzddisado.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ggcurssjs.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjgkgxnbw.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/geulpgvip.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gayidypna.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/goapphnog.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzlbppptm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwdengghv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gonigptgg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gkiyaxoeh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhhucql.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxdpshaxy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gjdebfdhv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/goxzeptpu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gcozukabo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdnxbaqwq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gyohrfsqo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gguxnoain.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gemyzuyyc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gjydszgoo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grgipjdqs.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/glsfsbmby.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gwzknnnki.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gclxfwdcr.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/guqfvezii.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gjwpxzmva.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glavrnqzj.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gdvyzrxpg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gwykbkdcl.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gmgkpinxz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpfkrcyid.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gonrkedfc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gqjrgotom.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gymvqvpsi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gbdncumid.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/guqgaurlq.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gvvddyjfp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gckoseonh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/genxdgvnu.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/ggsiryvlf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcpxzuiqd.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gmikazltc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/ggjiqvxeg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/grryjxqdg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gdgiwmxqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gwmorximx.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gachjnggm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gfawwexbf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/guqtcnbqr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gelkixtlg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gakeqqqqa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gqzqmwzxg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gzrnkhqsv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/giielgwkh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/glmdphvef.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gaoxjhznm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/ghvdwwixv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gadluyftq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gypwcinci.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gvkjpqzoa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gdjbgxixo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmbtolfsj.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gsybmsnwd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gfsgrsuhp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gayigrtxx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gyxpaanxo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gbhivefhz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gteyzklzl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gixewyjvn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gbvxrfdao.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnpbphibr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/ghamenwsr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gbbbddfyi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/guzpuajvd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcchbgmya.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gphsfskdq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gbynvxxek.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gzrzrpnyz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gdoxdhrpu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gntyewuqr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gbtogpzxj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gbxopubco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gxwysqcoy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gfzlxbxyg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gtqxbllbx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giedpcldt.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gdqtnmcug.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gskjlqbri.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/glyxvfedv.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gnagypmbp.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gvnbyhvlw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ghcvxwegv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gxnguypvc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gbaeidpcs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gmnqlzcaf.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gwylwkyrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/goyxxqpzz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gujcvlmba.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/ghzsaihvc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwbhvbnnw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gjavhwkek.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gwhcxqwxx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/glrpbttoc.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gfkrxczsd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/ggqjiqrdv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gihfvgrar.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gkaqpzwva.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/guzbzonqo.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gkcasvcjq.sHtML


<!-- 参考信息 -->