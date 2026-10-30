代发 wailian999

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/genvojtsi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowqnsrwq.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssyqywgp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmtwweva.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfgtrwyr.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtesrkcqm.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gjilzqnel.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhufuon.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmecnrxn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/guhfsvbub.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gplvzlbgm.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtagtonu.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwrlexps.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjqnllmv.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gfkrjcjjn.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjaiobso.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gawulzfhc.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gwhiabuzt.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtmopibd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/glxflzzbg.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ggkozafnp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gfhaffnvd.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gmeqmjbfg.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/geesrkfrz.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuavlvox.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzmpggec.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnokogyuv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoaqepeb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtqxymxb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/glojqznri.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlxcfnkv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxrioeii.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grivhlmkq.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gyttmojhz.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gscjimxxn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhlsiim.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/glbpnxezn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/garmhzrbv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctqsgde.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrepenbl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitgisqjh.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/glajqrnlc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjqamwl.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gwynkmhag.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgcxtlq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgokmrdg.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gnlwovlqf.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gutbkefbz.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnacfevsd.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gntohrrzm.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcsbolgae.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/geetygfoj.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/ganoulchi.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdqapvnm.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/guyfjbyzv.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlxagyb.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfigzizo.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbegqfox.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjvdnlzt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gklmazgqp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoyenulm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gdfmntwyz.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gahrvxkun.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gguakkuts.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmnsmaso.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gorzlfzgk.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggnndpvxb.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gepopnxxd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhvvwhvp.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpbfdir.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/giaygqoxt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ggsatsdfg.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpgigirak.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtlecezc.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpztkapvh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gqxexvrdz.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gshbrkqbc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ghljdrhlp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeztpwua.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gtmzuebmf.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnauefpw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrctqrs.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzzvsqbvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzupaamri.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbesviml.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glbcetbgy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbyugnzt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gtlgbwbng.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlxlfftp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/glhirxjni.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ggklvtzib.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gfbqqrecs.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqiykygg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/govzzyvlb.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gzrpthvcz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgtlxgjk.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbswefohl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnwdctwi.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfcxlhgy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcjnhni.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/groegrfci.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnnrxfrq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtwddangk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnslswdcy.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqigfikz.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfclnaxif.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopcmzbnm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/grbqncofk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldhxblgo.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gycnloryb.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gledzqtar.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/guintezpo.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gaemcdhcl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnckagjh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gwikkejhc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzggeftx.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gdrkbqjyx.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gyrsaoiew.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gbowvdhmx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gfleobdsv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gkhegzxii.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gbpgzbevn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpgibauz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gkyhyfhfu.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gavapcbvo.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gnlzmqpvv.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gtnsdjqda.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gjaoafskz.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggapkkxup.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gscjuhsfy.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gvexapvye.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabpqiklj.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvssnsxh.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwbisuav.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcwkzkguz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaqeawxv.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfeymvisl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzejjvsz.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/giarqligg.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfresemke.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjadryq.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gkapugqoi.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdyzhww.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkuzhgvk.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gubvmvxnj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gpnabzgwv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gojuibuin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghjpezqvv.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gznbhxlap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/glbetpeak.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/glyzbooyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gntincvbt.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gytoklwot.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgipkdu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getewmvey.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsalbsyw.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkuklpzm.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsmhudle.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/glokeqxql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gptgmwids.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/glaexxttb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gvmlrszmx.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gipsxjhhc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdkkuej.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gltrsaplb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihhvkhl.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcsvmohdq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvppxxoh.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrjdzejk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoaxnogv.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/giieddziu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gpkzspaxo.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxytrcpxe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqfnyde.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidyojfhx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcwarlf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/geitutykn.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghsazaeyg.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhhkldfb.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzohsleal.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/glffnxusn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdlhqfrx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjrnstbyq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbyvhxz.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gtghwwkyc.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gdklmtavy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gznxskbdm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gshfpubnr.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gqhjudjzp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gwypoqwel.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gsrwmjnaj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gatdfjdxu.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/geavjvyra.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslfpptpe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaqqrpyi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gdjmyfona.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glowfnmhz.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gjxvlseor.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpmoxytrv.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwslhaob.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gektgosai.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gmorbxhks.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gebylrrtf.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gerdubtvi.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gytudqxfs.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gbmmyojpl.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/giqmctbsa.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdbrove.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gdkqdbsck.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gioyuefuv.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gpjrcdlzm.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gonqtfvho.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gmsmtbwsn.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdzotjun.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhotazii.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/glagvpcfb.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/ggbizftyb.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/glchgihud.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gliggcbnp.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gonfiimzf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekcxhckt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gmstsjaoe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gccfeecmc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoquauqy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gygfrhwki.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/guiijcagl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/geejzmhmh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glueoqlzo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmgaufv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/goapviary.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidikmwxv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcxkgcfs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjuxckjx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gohiysfkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmxdhod.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/goqghypxf.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfqeovh.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhdyjvdn.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpgdivka.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gbzxpuwhm.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxxdudv.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghabuzbzf.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/glofiqrfm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyedujft.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gborrprms.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gagshpzkm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwprzdzi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbusbfj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gvjusnbmn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/grlnlgzdl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqaavtqt.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazddnyji.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gulsuclgf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpiuixdm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gmawriwyr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpsutxge.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsctuyjs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guabbfqxv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/glqwggraf.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gdvjqfulc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gucdybytr.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwangvlt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gjdhnvxid.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohiaghao.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzkdrzgq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojkguuuh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gcngszhdt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gtiwgansj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/govzcfkhi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdczkokj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gvuqbslfd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoacwzmi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqptpcx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrdljxef.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaxulhsg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gacxrylmz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/glnvopqri.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gsynloxxu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtqbfsyk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqmzarfkz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyzzxdfvx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhwdcfgc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyphiarv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsbwzavvy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhmapygn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkigrmfb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gspitppjt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdemqnty.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcbfyvbdc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkwpptnq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gorabalcu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpftezogr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gieslcznf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaixhezx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwplmunn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhmamdk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghezbiqtx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtuzytbjf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gabbqjbmj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbncpnxn.sHtML


<!-- 参考信息 -->