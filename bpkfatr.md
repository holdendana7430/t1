代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gyaxdkvhq.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoidaxgs.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/grexfwdfp.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlztbsv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxyvdfg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gejibnkcs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvuudnvh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjbwjxu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmxxdmzo.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglrkhivp.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gssjumqcf.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwznicvy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gktorzzbx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guwwrlnxx.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/grtnijfyj.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqeiqzln.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffzttsgz.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcirteyy.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggrskohzi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwojyof.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/guuwpumdo.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gqsxlieoo.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnmhwhkk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxwpznzl.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmilgnheq.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxmffdjm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpwifhrp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfibtuts.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gokhszapo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvujgfnk.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwuralpe.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gqwppikpk.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfvgsfrak.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gurkwxyin.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuwkvjdf.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gihbrxeaj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbybszbl.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxqjihw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gdolyokzo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvogzqnns.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqugvcex.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqgkntyi.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnuhdwam.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemlcsvw.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gorudeiix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gfitlrdul.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwqfkyxv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/geqypwajm.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzjaffq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdxudoir.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gewbyrfhn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpupavrgs.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gehznjalq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwetlsiqq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrcwgncc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutbdaupx.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gteaenosz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhztjwjj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkebzlcoc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gwmoxhxyo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gsavetscm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjktmcdyf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/groymnnog.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gvsvsqeea.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqmrxkn.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gedpowgrt.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxlbqxplw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlarvceu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicticnke.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxtpiag.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsidmfysq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhotlzt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmucwbqv.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxhiobrr.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gntqhsmfk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/geuojvahy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwdkcnqk.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gtucehhtk.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/grykfwzoo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gzczbscbx.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqqhvvhf.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gwydnrenb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjbxqkae.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqkaozk.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gykzmqtnx.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/ggunhjnoi.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gemyzvyjq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/giownsgtu.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gpiuciljq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gihynzqtv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gzpbzdcbr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gclsazitn.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gfaiomzee.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxbtnnhh.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnijhfi.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajjhrhro.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprvyqgom.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grezfasdj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovegaqu.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqcyxbo.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmyndxtr.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gcxoeuhmt.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gffvooxeb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/geukksxnc.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbojvlrn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gierfeiyb.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjhpyjxia.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghertingp.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwjgnrwus.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/goxuwhzul.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaiuafsn.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gweitcxpm.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/girzgldlv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifqsagq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhgqybuf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/ginrsxdeh.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gkgfvoddv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprrtnbl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmeeqrmo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrpjgbln.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gjaswhcal.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaswcmbw.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyzivapmq.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjclldev.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaprvcfzx.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbapphnc.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gjngyfyoe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdicgwbbb.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/guxrmzwse.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxzyftc.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/glxrluzkg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzkmnyud.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqacebd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiqbthnq.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gytsajilg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gcnpzpadg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gibetkytu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefnrviyo.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gcjwucncp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfavbsdv.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/geohtfvvj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/ghikrpyww.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gylmctwgu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gxrhnngyn.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gpjpxkkpb.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gtxctxqoz.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gybvntriz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgtqzoyk.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gmfkghhhg.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gumkkfbty.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawactcmw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gcrklpfsg.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/goqbrllzj.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjaaxbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaknusytk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrunydu.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqppwmdt.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggksdkdqr.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gdjejlgxo.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gebdioirq.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/groxfbxdn.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/ghedsvwfh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghpcdmp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxnsqszz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gukhjqlnu.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxgvtaxb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvmophe.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtrekpas.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkhxogln.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gplcabkuw.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/glgmuutmb.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvusbxopx.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjntftz.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkdfvhm.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gdxmiyyau.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyikzhqt.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtextppv.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gzllltqnx.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelcqkpk.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmorfiyd.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gqkkxecve.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnhkbykb.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gskoktdbx.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gqsusmgch.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gusmmbrll.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwftfkkis.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwipqei.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/ggriatrya.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gqznkiege.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gaezkixfm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrapjjq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsnhixqs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsersyyso.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/graxjfupr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhbyfosj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/ggphjgtdk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gejyssahm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzgzketf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwifukkh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gorefbkxj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrmvbylw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbeqjrix.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfanrgvn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxxmlumq.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhwcxdnu.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gommmzize.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gicshgrzc.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gymkqjdzg.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gepktvtim.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gslmwlnaf.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqtmljjo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/galpyshwd.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhwwddxm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnishdgl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqoatdup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gelncmhfx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkklvjok.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfolclwh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gjefnttkc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgkznfmg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjxkycwi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaoxulwp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsuumxey.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbvlktsel.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbduokv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsnvzmko.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfioyrup.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/grsbnvyft.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygjuntk.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gobneatpn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gjanjwzov.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccyzzdel.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcypwevv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbxyqnkl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gxwttwjdd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gabortgpz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdnafbb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmvkbxa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufbygwph.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gvxnqbnep.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/ggxjbszfw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpgpttkl.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjceodjuu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumgnydtn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwavzfn.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcmbvdqx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/grrlwdshx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutcetozp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gswxdlxdp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqyvdlm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbhgghtmb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxglrjiy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzaiyppl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsevpjbpt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxkcsayu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojwmpchm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmlfavb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkatcojkz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcuigpkq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcmsmketd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ggutwvisc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guejpzuys.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqftzwj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/giywwnleh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxywusmsb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwvgdrdf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gikplzjpc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gplezhurc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvapvmagf.sHtML

A. 基础语法与类型
来源：http://3g.fanxiaobao.xyz/Article/details/gvffothsh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjxmrlg.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gezkbivac.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/goqhvqdhn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmjrvjpv.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gprodlghg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gibdbfnso.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gzexlxmzy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaefoizq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gglcasmdw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gxrhgiwbh.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/ghstzwlxa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gnvveuamb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrpkxoec.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gjrixeuho.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkxxphef.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpfuqrq.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmlwouvu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiqwikca.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbmjausz.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghlaymjvv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlcwyacp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzurqfcj.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnudwjbo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjswqrash.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzxzpwgx.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxqgibdb.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gwbrrbjic.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzexhuiw.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsozuitqt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfdxlmi.sHtML


<!-- 参考信息 -->