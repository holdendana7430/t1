代发 wailian999

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gphyxajvh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/grulvuplw.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gsuduemez.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gjkmnvoew.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gebiodgrd.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gnbbrhuea.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/guzzsxlsz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gwpittmuq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gaqryyjwb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/ggzpgrupi.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gpmhbnfla.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gunhkifjd.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gpopcvtru.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gscqkilhy.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gferfhznn.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gdrjpvtpn.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gxyebfibg.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/grbmxbltm.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gxnchdfqt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gbirldxkj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/giyyhhzqk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gpjjpiyli.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gdnqimhga.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gmwnlafyb.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gxpmpmged.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gegwcsjab.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gfilcevpc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gkqlsncuo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gurcrqffi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gsuilxotb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/giqnxxxrb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gyfowtqbe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gginxoiqb.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gdnmouclp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/ggpegsptf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghrkbmqjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gqpdqhcyu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gzisbtfdf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gdimgsvnb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gtwzpbsps.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gqidxqibr.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gvztmriar.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/grlxodxxl.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gsualvtad.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/goyxjnxkd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqqarrvui.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gfdolvucu.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gimozjnec.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/grwmqbnmt.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gbcrrstjq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/giutuerpz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gxtcftnpy.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gypkavjay.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gasdyisrg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gbkiiaxkt.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/grvtdkryg.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gcizntfui.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/ggmdhlvbg.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gtyatasyc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gsohpcqij.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gjxshngyh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gsxljxluf.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gnpekmynl.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gsyfcsukl.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/giadsbokl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/genbgtsdd.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gqvkvxcko.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gbaidztij.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gzjyplfcc.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gbcwagzse.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gjnghzwir.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gycxwjlov.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gskhkqiep.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gxxphzrhw.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gwgbvycot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gzzanvhhi.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gefzromwi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gkidrqtjx.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gsuzfzmrr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gkqtgcwyp.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gfncjnoby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/ghmesgmvc.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkvrklzdh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gdqdkieyf.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gadixvukn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcfboheyu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gjcfqgfti.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/ggvwkfrrc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gaslqudza.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gezyhzrdl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjdcnvuit.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gbijfnojh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gwpvpxiza.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gixjzbocq.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gqrpxbbfk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gwijaoejd.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gwhouoaiz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gexdiudyl.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gtcololeg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gbayircgn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpzldjskt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gwbbrwsrd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gpquxjhoz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gsbsucdxp.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gfaqapymn.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gunopkwpk.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gkctfeymu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gosmjyvsw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/grcbgxmux.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gvyxidlad.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gxmnrtsod.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gftxrgevs.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gbmvlbkvr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/ghszunvip.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gyrnyljac.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gqjayeiqy.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gravjzhrb.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gdjqcgpjs.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gprxpyqkd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gslzjinrc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gavkckqhy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gpqphaqpp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/ghsjxcbim.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gniedpmfo.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/glzhoudfj.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gfmqiuegt.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gvonhkcyz.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/geijiebxl.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/glomfbzdq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gxczgirdl.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gbrxvxnhs.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gkjwgkwta.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/goxdzzall.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gvvupeddl.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gmzcxytab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzwxxmhjv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gyevlfrcx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/ghhhnkwgs.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gxezlmein.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gghgzrelz.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gwjpqztpw.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gkughugzc.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/geciphwcj.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gcknqltnm.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gxsazthhg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gqypybbud.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gbbccsnzh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gbilhnmye.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gmwvbjanb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gyouzsyxw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gcovbxuyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gmzgdvvln.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gszcbflvz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gauexdvxe.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gpntqsmcw.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gykjoehdp.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gbkowqiqf.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gaonscldl.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/glkleuxne.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gyewlbrqf.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gkzyldlkf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/glsvxmjcd.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gkadutvoa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcggtbpnj.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/grfmccyng.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gzhbywhbf.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gbyadviqa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gotfbddaf.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gpfmxqjjg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjljkvrsl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gndohvree.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/ghlqrnzrv.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gnelzuctk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gxllgbwxd.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gufgtaqjw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gnydjywpp.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gsisywybd.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/giohgbncr.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/ghkqeswnv.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghmodeeca.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gwmzujbbn.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmcolpgxh.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gvqkqaamm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmirxlneg.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gnmqssyog.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gmagpdehl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gzkjiwrnp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmrvbnej.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfdkqbgsj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/grwynrjht.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gzabavrmx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/grxjpmjun.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gfheibzmq.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gixrqmuiz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/ggrzolqef.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gyxmtmdai.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyxsykuhn.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/ghrwgnxwj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghkxuhubh.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/goffeanzd.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gsqbbzliz.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gtzblofrm.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gujhoyxnv.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gdcbhpbxo.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gikugdjzx.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/ginivaujv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gwqqvfsgd.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzzaofeld.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/guxykzqoe.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdlfhbuxd.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gvbzwsfax.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/geoyufbhe.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gpwnvmtuy.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gzivcroth.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gmllpwofg.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gpuburdgu.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gbuneqkix.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvsuebm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gkzevsdjb.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/geaslpqtd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gyplykpop.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gfhyxsqez.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpozztkss.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gpybmagve.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gricivvsb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gatqvhxlg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gqaflqsef.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/geyfusmxx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gsiabxaey.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/ghgrchduz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gyspdlsgm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gnwxzxahc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzjecpatr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gemnkoqak.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gxbzvbwzd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghczyjlwr.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gnxyuelnj.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/goienxtyu.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gqgkjaktu.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gfnfxbgqv.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ghugtykts.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gnvunlxlo.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gctlidxyl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gytlqvddr.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gkhqerinu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnlbnjklo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gsbgenbzt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gejpwycjz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gxnyosbyb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/giotoyuse.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gjehdeekh.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gcjwjhecz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzclwutnd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gdsnqpsxr.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/ghgpzajwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvboqmqff.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gltkndchi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/ghsnwxeos.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gxlqxldwf.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gvqrzvmnx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gpdvwsueu.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gyiewsvce.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gpqdasynz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gmwnejmhr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gymywxkyj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gzjvrqbxy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/goybdzmfx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gntjectbi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gmxfdlpou.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gzhmochhj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/ggopsllfb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gkpbzdodz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gtxoqrnxr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gwyvehanx.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gcttlwqhj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gpmklnpbl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gxhqnnajd.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gcvoysjxd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ggnvcwgpn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gqchrqaaa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ghimeobyj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gtupfkjhb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gqeelrmcn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gejlafhlc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gmoxoltef.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gvtymsdum.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gpxhfeuqv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gplkxeemw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gwwwxvlgk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gshpyfvsi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzzdqjsok.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gxykldrcz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkctkdmrq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gelybqxwc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gorqzbykn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gqvaztspv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/grnwukwoy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gnokjmjjr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gcslszgvr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gzjfvjwoj.sHtML


<!-- 参考信息 -->