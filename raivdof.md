代发 wailian999

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gsvdywayh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gtjsvcdmz.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gaubtjzmq.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gfgnundpr.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ghlpciiyv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gdvhawuen.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/grzymxjss.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gzewfoolv.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gkoeenwan.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gizpnwlgv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/ggfhqxojx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/ghlfklwjz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gmieetfas.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/geiuwtsmg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/ggbzdhlpw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gztwplwcp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/glnjvtwma.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/girdttejo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gnoitsfsi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gtuibyhcm.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/geccqvxsk.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/grlgcxyml.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/giswwslxs.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gbkkwmmol.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gtslyjlkg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gqhikbwfb.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gaffotdym.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/ggczpimgz.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gjwtthtpz.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gslbmxkwt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gewenigng.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcwfueavf.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/galmluept.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/grryggfeu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/genxbtucg.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gtmcupvrk.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gcfxmredw.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gofudfpag.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gdzrtydws.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gdjyuvnpi.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gwhcrphmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gejaabxav.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gmkkomqnp.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gmsycxroz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/glvfegnzk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glocuviqr.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gojsnrqry.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvafcbirq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdwnzmveu.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/ggmdjykxs.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gwnvcultn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdytaodub.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/grsgvymsf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnumxxrpn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gnvynczud.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gmaishrgk.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gfxflwdeu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gywdximbi.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gxxybmfll.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gtkaotrnz.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/geyjavler.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/ggnleocxh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/geexatrvw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/grhjkpbzs.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gprbaeycm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gwhfetrse.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gfpvqojlc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gcjjvvimi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gidmvhelb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gbsqkkcym.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gztvfwsll.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gwcvflbob.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gesgqhuco.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gerqpolgl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gnkvyqpnb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gkszhrgeu.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gdckrhexg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gymabszhp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gtglsepjc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gnlfnlxuj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gypdwjlfm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gensiunyd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/guupzxsbc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gfccxsjlm.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gbjizplkr.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/ggqwffpfs.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/ggxwdquwc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gtgfixxie.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gwscphmzt.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/giexptpja.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gwftbvoid.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gorxagukj.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gymhozaih.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gikfskcin.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/glkabrmvd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gwrqnmjsz.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gbkkhvmen.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gbrdchnjh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gehfocbfi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/guzkapfxy.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gtduovchd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/ghslgdtfh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gqxcpbxyt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gbeqmkuhv.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gpcctcbnq.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gxwwdtsac.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gbqcebjfy.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gsrwfannw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gmmhabxzv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/grhcbqbnl.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gwyqjijzi.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gwiegwaag.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gfjtcnsdm.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gylbjuotc.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gclyrplnk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gfryuvuvw.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ggljcwhla.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gbvcmoacn.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gukjoovat.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ghkvjhtwn.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/ggmnggfpi.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gquqsfgqv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gcvqhhdoc.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gpnmrnaen.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gbnnipvsz.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/godapymsd.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/guoqrxvkc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gmlxivcyq.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gwxejjjqc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gangygzsm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gjmhejlcb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvkllge.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gtixzprxg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gobsrqrmr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gdcojaczz.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/grtvhkdeh.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/grtalhjib.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gjyszcgck.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gjeeekxyn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gfrruylbj.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/glrcxkvff.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gbmlswknd.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gvdwxddks.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/grquzropn.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/ghbiludyg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/grxsuwwbk.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gbiwuijte.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gyeayavio.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvmwczzsi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gopajdsiv.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gkqxkkrjc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gwneaxcra.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/grgvobfzk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gxpspjdsx.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gcltdhgcz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/guqzuwnkj.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gdgyvvrhq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/ghedwtdcf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/glagrqrsx.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gsabevzaw.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/glqmecirf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzgfbhejv.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gqzfnzrpx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsudobcbp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gttkwxfgm.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbeurvixp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/grriqjqqm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gimdhdzbm.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gpbtsasrq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gezoppajp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gbqchcpjq.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gnrqxtpeb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gaudkupay.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gmgntavfk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gmayphqsm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gpxviehvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxkvjjjau.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gegluauba.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcgtgchuc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gvomcgkqb.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gsknooqfw.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gcuhnrsub.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gmlegkbdn.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gqqgmwybt.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gvqcyktax.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gqeaxeezd.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ggsbhkehs.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/giblreygc.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gxssjsxow.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gnqyuykdc.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gqameqfxx.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gieguxpre.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/guqjswdsj.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gysqsnoyh.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gjlatcesq.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/grjyijfzz.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gsxaqvimx.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmswksjkq.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gvcujvcru.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gcdwmvgrf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gibzrcczd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gcacwqmsg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/grxqfwllz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gidajaavz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/ganwylwad.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/glblrocsr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gjytmivqw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gunegdtbg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjfhljobe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gckmywfjn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gfmczyfvn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gxytxebch.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gruddgcuj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gbjysawno.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gidglzard.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gwnfzmqeq.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gvwtyehji.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gjgjbyokq.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gfbxtdtyt.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gdlvrcnua.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gaqnlzgfi.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gkxjhrrio.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gblihzpes.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/goyohiiqc.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gcdidcjon.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gychpnefo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ghxjdyphb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gunfsxtua.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gjakolvae.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gwwhelhtb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gtkbdcjnr.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gpiewgeat.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gomrafjad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gpnaliiwv.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/giehhujqb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkcwghkqt.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gxvsmldaz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gqwetjcmh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gmyiytivu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpnekubsm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gmrgvqmxy.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gznuckwcw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gyxrprcwe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/grwkdzuwu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gpgkewiza.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gaowqsntm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gdughbcpt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gkoskpcsv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gdrbvvjlc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gddpbrfpx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gpegotlle.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/glajlbdbr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/guutpfzwn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/ghlllvkvq.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gtklqhjur.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/grrgbinzx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gmthjtuli.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gbsiygjxy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvaouuyha.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gjyjlqvqa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/ghyfxlvsp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gykwoizum.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gxumjwaqk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/grsydxjbr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gzpflwnbz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gxpxheiik.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/glpmddoub.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdlkwmofd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gkhomagcz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gssaqqlkj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gqbgbtthw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gpsmscfmf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/guxbsaukv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gfarowjch.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gawldprlj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gpuuttgsd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gnreeeohn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/givzpovbf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gccncgmmz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyfhgowzd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmerbeyn.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gevaybpue.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giotnyoht.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/geupwmaeq.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gxxyzmyqz.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/ggxytdkxv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gexcgbrcz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/guuosikdk.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/grsjomygg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/ggkxmdosv.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gwrvkfobl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gmiautzdm.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gdmtzzbnp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gbhmxkyyo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/goicrlscg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gczcpnfqx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gmjfihmxa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gchbeyofe.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gxzsuceej.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gfulwklhi.sHtML


<!-- 参考信息 -->