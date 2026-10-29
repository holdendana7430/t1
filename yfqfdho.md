代发 wailian999

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/grargjgfz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gbjosiroh.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gfctmfszk.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gaugtfgxo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gnaeetgmu.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gxxqkzwsf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gkjjhmxao.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gqglbkxen.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gmvzmghfh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gbmpxvcdd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gowxdqern.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/griaynjev.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gnymyiohb.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gnifzbvfg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gzffjcnov.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gcvsulhlj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gadbqfguf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtyjilqif.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gquzfshkx.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gwawtordn.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gieslgtxq.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gpdahcdde.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gjybkcqli.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gpxdhnfgo.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gpffyenlk.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gzgvicstx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gdorwhezn.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gfjrydsei.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gfufirvax.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gebzpqvbn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdyvudkyo.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gswrrcrcz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/garlveuyw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gpqbkkshu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gcyzrciwt.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gxajtclky.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gsopxdjkd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/grxwjrqxh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gvzzudbva.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gldbceaoc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjqtqirfa.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gorjkkpry.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gvgnlfybi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/glnvarrvn.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gvjsihejg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gaendmqfr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gdulcpgjc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/grcbhmjef.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gcsadwxcf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/goeclzcdc.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gkskuzmou.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gbuuhcgjo.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gxvhxntsr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/geabwjdkt.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gefpubkhp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gvfvxszlf.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gybrrrygs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/goxncvzdf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gybwnzfsl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/giqhmviri.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gnamzsofm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gobzuyvtw.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gkwksipxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gklhuhtgt.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gsduzxrfd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/grrmzstmd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gjufoeqtz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/geykixyca.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gtelnzinq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/geoturahv.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gomfyyhgy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/govgmydoq.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/ggvugtqnv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gllnsneav.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gqrxcutmn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ghttcudrt.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gjmotgqqh.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gzevnawbd.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gidoeltgc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gozfzurai.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/guofjicxe.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwhqmpmiu.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gjxzbiykk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gdybvmxgy.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/ggfhmuqgj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gqwhdocob.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gczayzgzc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gstoerrhq.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gkasrfsdl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gfjuffccd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gazwcfbbq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gibhyxoav.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/geowwcnie.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwdcfyrnf.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gjmsscodu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gvrdpfhfn.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/grohzziqc.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/grvvldhck.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gxustjhfc.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gtteylgga.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gzprfjnqp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/guefxyhhq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gmzgaigwt.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gjscddttz.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gpthrcrnz.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/guzpxmybv.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/ggzdfurop.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gmpsyeksc.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gppkbgkhs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/guzxedfkp.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/ggvckatgz.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gqxbkjggx.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gincfnpuv.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gjnumzdbk.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gwnqdyjuz.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gukchserc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ghwzqqucf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gwljyzxdg.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gqhzlrmnm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gthaedbig.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gedsjqijw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gajtfwzrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gkpivbcnn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/grucamafn.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gtcczlwsk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gpiairysj.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gerhenjkk.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gvmpcrrwb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gmlrqritx.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gltdelfyl.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gozrxnfge.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gewiyjnny.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gkwisezmb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gpujfgdvc.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gpbhzqzrj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gjpubwloj.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gjachlikj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gwhsuwacf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/ggltazxhx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/glmvdqoui.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/geihcgmva.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/grsxdebhm.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gmwajgvlr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjlywku.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gzfnvlide.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gckabijlx.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gzldtqwfs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gmhtoqsjl.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gvprbjzhu.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gqqnjyoiz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gayozkrlr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gygpcxlyj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gqogfkfjg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvmsztklf.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gbxhxuzks.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gymtkrrwa.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gckjlifrr.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtrfyxzoe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gkaqjuhda.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/graxtxgrh.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/geanfdirf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gxvfdyefo.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/ghzrprzuf.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/giullpuxb.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gzsdilhbj.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gsdrbcqjb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/ghdtiqiji.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/givfuvpwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjzsafwou.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gnnrnjzti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkrjrunaj.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gbnlcrobb.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gpklwklsc.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gysmpgoid.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/ghopjdaok.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxbyqgcse.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gkbidgjzw.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gyttgnqvf.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gneiwpcbu.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/grojeyrbo.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gvajbfzln.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gntecoqzo.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gnllpewtb.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gwghrhhtj.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/geiqjduan.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/grpktmxvq.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/grtttygbt.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gakarpilh.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gmdrhwhxb.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gkevejokz.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gkqthtdtn.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gczetmqwq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gokpludzh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/grkbuzmxf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gcdbycuqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gcdctqvxv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/georgoque.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gzcjzhxyl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gczcuqtvk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gsbhorslu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/goylwijie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gavelqiao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/guljykmel.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkrgswqks.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gfmkudtbe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gdbtiybok.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/grboucvwr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gzeedskdh.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gwwgkaqge.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gjyrbzrft.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gwedfbpyl.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gymmktwsl.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gmwngpszc.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/geyjejfbq.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gonuchbsm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/geapzglir.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/ghzidhhdb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gtjesshiw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gehidtupi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gybesncsz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/guihhwpjl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/ghujcdswo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gmedfkfbt.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gcdclhdtp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grluxoyxq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/glstregxz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gzsgonxfn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gluycjkku.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/giehcsufa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gvnpmndrx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gecxvtehz.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gxgmguygi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gzhsxhckx.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gygrpekcl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gyisperos.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gimhhgicv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gyjcjaehn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/glxslglko.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gmxawnxyk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gincsrrax.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/guehukhnp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gghngkksc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gglvuazje.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/ghwkoybso.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gouzqrqig.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gvsiwzmbi.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gdrjqjjgg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gotyzjzil.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gpnstipeu.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gaopyxpeh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gplctgoyz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gpaomzdzn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gmbylbmqj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gjmqdfpwg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gascycnpu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxhcktlhr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjfuwxh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gmgrlgmgz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/glytsrzjv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpqpqkekb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbgzxbo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gxjxfvrbt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjmygpkys.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpudqrtkz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/grfkfmlww.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gvtzrwuyp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxgxcvkou.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfllhgnss.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gttrscmyo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gkuxwgrjz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ghwtvybdl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gohtjgovh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goeoejczk.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gruhbrdes.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcyonzivc.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gcnfzsvbm.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gshensoxc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gzpztqgjo.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gynlvbhgg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gchhwobbx.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gegwcmywd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gzyjputbw.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gfylosbqb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gdqgjhown.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gssljfppd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gosuypcnr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gyefypjdd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcjnvzsso.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gtctjirjn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfmjxnca.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gjqvaniyc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/grlsurqsv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/grnrurone.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/geznokids.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gclqkicfy.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtvdewcjk.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gfilpansk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gijxdvknd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gemozzvxu.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gvhwdyqbh.sHtML


<!-- 参考信息 -->