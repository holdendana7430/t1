代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghuexuzjs.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxyoopyb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcyvzdmq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gljprjoyl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcevobzi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvulpenf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gqplabzkg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptindoe.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndbmftb.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamvhtozs.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpweznpay.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gtknywfyp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gizhclthd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoczoitm.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gslmreibd.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/ghfloqqhd.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gollcdduh.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbyoascc.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdcwlvwkd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guswjipyd.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/geibntisl.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/govcselzf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtuuuitb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzmutbkc.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfsqkqcr.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjaovotf.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdveffqf.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gvmndjnki.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gioddddkz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaavkmrg.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gvilecpgq.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gdvtpltwy.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhacyfnf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxubivjg.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiwaxtll.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsveyzxj.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/giucwypvk.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpokxatx.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gsrtarfra.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmgftrht.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsidleit.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvxhprni.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gutnbqzye.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlytlwdp.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbblzosk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgpramlg.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gggbhuqpe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gimhktvhd.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gcftdwuqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbfdsstb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gugtwnqnh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyogjvtrm.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gsfctevth.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnanbyf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubosdjsy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtobikxxz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqesvnw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gmyzzkitt.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvwfzwbx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gbgnusonj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/geneckiat.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/guzefaywy.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwffxbro.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwulrxlk.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuouawsw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gnkdnburo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkyzqla.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gusqpmlck.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gcljjknyv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrouxia.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrdoyxvg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvhiqlud.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gxmxynbwk.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gseirsper.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gsojcjgpr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/glyyqeuhj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgeuiza.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gildwoirj.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxsibud.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyekicd.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtkrwnaw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahfysldc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gspskmfvn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gljqsngnq.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gjizjatnp.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/govmffxpi.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/grgcrxrfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgrmoshv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gianiodjz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/giuxdnjes.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxyocst.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdtlwotw.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gximzurdw.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/getklqjma.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gnxbhkxnq.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkiqtsnw.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyztghdpv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpflxqfst.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/guaihyvmp.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqalmtc.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gmmwfuwoa.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gzdwbsvyz.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggapouyxd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxwwgtpi.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/guugqwwec.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gczhiasfm.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gggdvzhtd.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpewwial.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbndbxznb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlmdguq.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiypaaan.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gikdxtaup.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gudtfckqg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjoldkzy.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gebkrjtrp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/giwynsyrn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxmkjwyo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahgkywmy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvtqnnymf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcvekomp.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gwxaztnis.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzdxitfo.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gexdjtkqd.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gffogzseu.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gyxlnscws.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gilbpdkef.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gthkohyzf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gterkyhuw.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxykrea.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtztpwwce.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/guceovjgy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvcdsblsp.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gtulhisjq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnojsnmwa.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwhzbyyo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gmojvvrwy.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpfnivys.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifmkduo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/getssdjyj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrlloxoq.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gazebvpqr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhlxynnt.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/guwnlpvpm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsyclbpd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/girlojdfi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gleussyyj.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvggdmgbj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqnxjpcl.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gjckpachd.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gizttvyem.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gexqzvbfo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gxxdepfei.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gneyhxrrb.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gdgjhlxjo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/giuumwosz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtnmyqeev.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsvtnvni.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gyppipjfu.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gsneojhtp.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokdqgmwp.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gbzvizxuf.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulumrdbw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycqurvnv.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgvgbddb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjjgdoihx.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbkgsgfc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkbyakmzz.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gaemxryhf.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gousdtkse.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gftapxvib.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvfxqsef.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwlrxcasf.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrsfkzyf.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gcuprsijl.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmelmstzm.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqacalxa.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/glcrbsjmg.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gwwgqhkxb.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gcwrevdnb.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbgwkppb.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gidsciucv.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlxdlkwg.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gmmfmftkp.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjbqkfer.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvxqmzaaq.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gxobqcirx.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqdrkqoz.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gvihiokuj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/grgyawabj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoutnqxy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gkubevcdm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtygkep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galfrcgdj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gjntxtmyr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmqcmjlw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gueasgott.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gjliqgogz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gwfmgdgxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzbuioy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gikqfsjxq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyqbkqgj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqvklmue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhzqjudc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltrykvn.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/guqsbamrw.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gmheqzzlx.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gobddyokp.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvjbqxu.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gnsyhxilq.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gtgfignbk.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gxqirwpcv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gfihnizea.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gxugpgkmq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ggktwqlqq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhphsnhw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/ghqcrssml.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjeesfd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfftmyqkf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgdpacs.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtjmhzl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpezdxjec.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gakajdxul.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gjmokpajw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcojozhes.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvqnslwh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwxihcls.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpstaeevh.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gonqfvoli.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgfdhix.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gyakzocsl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpgawjwo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwosbxxb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeldrvuf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gvqkxndol.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gnryqeypg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdmifeet.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmozfqnl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/guwxtjkti.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gojwleuab.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gmckuvkqd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gftslfocp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gbebfzhpe.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/grlyjwzne.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkiztgao.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnpnvupg.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gfrpmoloi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gukibgtnc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gpbmnfiyr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsihcylor.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmyttfju.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsseemawp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawnyzaee.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpclbjthl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/glnwmrrkp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmgwhrb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnryukj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/guwtflmcd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbrrcdhfg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljwsxsm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtetlmwd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqmiqqqy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxoxsmcpq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glmiavsdh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gynqllzej.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlnobljw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqqsyqo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gwymeklzz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuaanegf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyfkvnqal.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjuoahbb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvidbapqj.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxohadx.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gqutknbgl.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gyoutrabf.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gshydqdtv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbfsqqzh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gadygwlvg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhloqbws.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkxkdznn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gurowakis.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gadoxrujg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/ggrsyfauy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjzwhsw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpgkwntk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/glwplhqyq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqccqjjrh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gzmlwgitd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzpufod.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/griajxjqg.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbrafuysc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/geugrruat.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gproijlnr.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxsrfdpvd.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqjecsv.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsrscmeil.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gxekioibt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gairxprrt.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpipwycrl.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gyalbobjj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glxtypisb.sHtML


<!-- 参考信息 -->