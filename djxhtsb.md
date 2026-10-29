代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gzvairuqw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbtabpj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/greotqafm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gilvphqjf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/ggmqnhrus.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gqltzkzwx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gyumubqbt.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/goacfywhj.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/ggorgwjfh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/ggukntaqt.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gkdsewzwv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdyhahqnn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gturjhtbq.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gvhfwacbu.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gocobtpvn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gxfldrcsp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gzaetwxbx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gzjteaaqr.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gidtszkkz.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gqrzuzygr.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gtlsbiykl.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gsinuzidj.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gsbnqczlg.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/geawqaqvb.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/geonarwwa.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gegmdrwmz.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gsrzqokqp.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gstivuxeq.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gbpzvszvp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gknzawqfs.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/guhredtes.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gtgucqyfu.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gzqgoopqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gmsmghykg.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gqlaclham.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gwkjffgpj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gvfqgdzws.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/ggbpegdxk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gqlwucelq.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gmcgfrhzb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gtaseonqr.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gnrimynio.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gwwigikqh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gsvkgekdo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gnappxjed.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gauhbxfef.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/glxtlwjwb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gloaqzops.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gfjqkvwqx.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gjthtjfmh.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/godmfylvr.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gcslkdcnk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gjxxsnwgh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsfyymyun.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gqpiyhznc.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/grdaugltt.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/goelzwmcj.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gvqyrxxms.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gwoutpwnr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/grutxjopk.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gmupuztat.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gatloujyi.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gbnvuddte.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gyudahreg.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gsfrxndpx.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gxhjzqsyx.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gydckwwze.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gafewvvlh.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gqgjxqodo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gmjpfdqgk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gfsndokgf.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gpzevisjk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/ghmvhpxwz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gzcyylyfx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gbtguhvak.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gidawoyru.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpacudhxt.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gatkpizww.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gdtbepzny.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gpmecsljj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gdhqjvajy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gzxaosabu.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gewqahrmc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gpoyblafo.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gfuwfmmim.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gqcmxsdvk.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gpuznudlg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gsshfopbe.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gooxjugtp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gqsejuwgz.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gswgspvmu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/goifymaje.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gorxsdgbv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkcgxktvc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gdxkefglf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gvjponysn.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gnpounvbh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/geajefawn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbpntrdth.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gbmuukfrx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gtnmwrhee.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gzheeyjlh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/grsxgfdvv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gjzzkydey.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gqefiuzrw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gusmhjtjg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/ghqbynswt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gkjecpdhi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gxcdpktqh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gnooiqtyt.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gqsqvdwmi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gqhcghehi.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gczwqpect.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/ghwznggyk.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/ghqjasbcn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gwaaiqixd.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/goctyvsxj.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gwxklhzko.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gsylkpmbx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gtugtkjys.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gxavzobon.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gecrztyqt.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gxvsdsucy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gokwbepzq.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gminjnyzb.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gqiyimgpc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gmzacesap.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gldphsiei.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gfnjysron.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkvpojdqh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxaycfc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gbajdcvsx.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gquiwfpvf.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/ghsjnzeqv.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gmhvmzbwf.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gsthacgib.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gigefqbqj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gfonkayqh.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gegqswzcu.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/grdvcewow.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gkeesyhvo.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gycybvvyz.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gpiwrfext.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdadzasea.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdnrimkaz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gdzznuelb.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gndnjkxvm.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gxgsyuxgr.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gzsvyufee.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gahnzzxjj.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/glsqimcpj.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gfchrytjz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/glzajjicz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gzjncxvyj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gamuuyyub.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghpfiyrvv.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/glvmsrdmv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbbrfiaek.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/giqsrzlgc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gftaxlxlc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gtowbcdpl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gphaotzqa.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gmwsivsze.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/ghdpyzoct.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gwyxeraxq.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gmoksqyxn.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gntmnbeel.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gmwzzvngs.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/ggngbmtnc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gxwkowdia.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gbwxnaqnu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gtvgflnpy.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gawiyifqd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gpccfqnsd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxsajjegp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gxktfaksz.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gayceqywe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gshcetxeh.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gfgwzqwuw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gcdajtqbv.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gffldpfnp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcmjwapan.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gibywodgm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gjuulycvq.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/ghomhljhv.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/guapfkdcl.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/guszgggwi.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gftabnula.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/ggrjtrtaj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxclduyfe.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gjhqjihht.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdtbqdysq.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gswjxceji.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gbpotmoxi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gscibcvxo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/glcgkcwmj.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gxdfpyspr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gtuifjwin.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gcatmawao.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gskombizj.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/giyvjsvkd.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/ghpdcmqot.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gzybtidzi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gzxokxhaa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjhwlodnr.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/ghbhpnlbc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydgdbmfc.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gnpaihzqb.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ghtzkjipo.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/grljpupve.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gjvjdmdss.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gzlqezuyw.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/godauyzdh.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gocyppgcb.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gzxdvvqgh.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gtmocsmql.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/glyzivyss.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gpeapitln.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gaqvvlugt.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gscerxhtq.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gmnvmazmk.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gjewrbqdt.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/grebtqxqh.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gxevveaqy.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gcrnvniwl.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfeymqnxf.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gejryuqad.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ghfhxkaff.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gteamfpmo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gfzhrfnee.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ggzhtcpzj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gooqstlss.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/guxtimjfb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gqoviqctz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbobuzucf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gwdbyxlnb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gphqaynao.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gcgohdozj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gzilbagxq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/guprlddrc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gfffxykzd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gvreqpkfj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/goiajinpn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvoohzlrk.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/goyqojmuw.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gyakgbcbx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gnupuvyxi.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gbpjxskqt.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gdwvmaxft.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/githeamrq.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/grtshkegw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/grqtuhmvs.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/ghtujesin.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghvxtzxot.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gdpbzbxxf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/glkjrtiuq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gbnacnbzu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gznqfxemk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gizbotfdc.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gqsunkpvm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmvaxebwe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gqxljuvql.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gzsosupsd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gigipipnl.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gbuzaivnl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/grfddebke.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gneemkmzp.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gqanexjrl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/ghnxyecdx.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gkfstmifd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gxeygajad.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gsgnetixf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gqheivqdd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gszmxlaom.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gbzdsuxej.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gigyczltb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gcfjfokgp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/ggtdwifoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gxhwoplfq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gbyhvsngx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gxljlrmhr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gkpqviojr.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gyulcnsuj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gmnuvilym.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdqjmikjx.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gubotrfkt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gfuhvvlmk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gijqygjcj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/glejjeauc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gwbbfbfpn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gcpexfoul.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwdagxoaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gpcjydfoy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gcralorag.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggbbzpwap.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gakbgyonp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gfvtowddz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gkrprbdbi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/goctumnea.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gryconmwh.sHtML


<!-- 参考信息 -->