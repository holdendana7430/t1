代发 wailian999

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gfccyppfd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gucxzuhfh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gfbwkrvcn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gfaqmjgxx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gggfavruv.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/ghvyfkfsm.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gkzfxeyoy.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gzyhydpqp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gkyfdcwlm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/grgptdcyj.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gwkfoklok.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gibifpprn.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gdkwxznuo.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/guwaxxnpc.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gqawcveqc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gxrniwtsf.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gyecfvaov.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gnixbsyaz.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gnucejkdq.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gpqxqyvqu.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gmwyhyduj.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/guvivemff.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gczoumawp.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gbdvkeosm.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gypufwplw.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gjcwthxws.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/glenvpsca.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gtvgthwvq.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gmcjgfbrx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gsiqnqage.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gnwdlhfdp.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gpauxosis.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gajkiispo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gwoxpsgta.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gvswlcqng.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gtorpqqjh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gdyqnqjjb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gkjxdfzaf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gyufttkrr.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gmxzasyun.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gonywlbxo.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gwstdmpgi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gkbgvnkbk.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gddedjzdv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/glhrziyly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkusmvu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gztncolww.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gacqggewl.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gayuwpjea.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gyptncxnf.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gibqecdxo.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpulqwhg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gpredgtwd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gaxrhrdqi.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ghxkdmvpq.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gjveidaww.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/guhohkfqp.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gcsxcdocj.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/glfovykha.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gofeqohbl.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gpfejusme.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/ghrusrfje.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gtwymsiop.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/ghsrzluop.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gapceemgl.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gfauzmgpe.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/ghdfhxaby.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gdosojheo.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gzmuelvwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/guyhijisp.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gyoernxwj.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gircghwmm.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gwzonphva.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gynrnqakh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/geordrizk.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gqhwfcgqe.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzmllnuhh.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/ghjxjqimm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gssgofvgf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gkoetxfdt.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gsuzsazht.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/glbztvcmg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gmwpllevb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gncebtxbp.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gnwoidpmi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gisyrjkkd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/ggukfnxsb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/grvoczyfc.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gmqgnerpi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gvuvirkqx.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/ggtxcksmb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gdywhvjuc.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/geylwxsmb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghlongwjc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gsfhkucus.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gwwdfuxxr.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gbauxyqzc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gntwgvgjg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/grucnnpcf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gksbqciqk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/glmfnuxoq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gcdnhpxgh.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/glqkfehjm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gynqbjkjn.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gmubwomyn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/glehwftap.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gvdnhrgib.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gfkzkknzy.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gmbczpwbp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gxscwfwoa.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gfhfbskxa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gxgbmpduv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/grufldkpg.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gyzdqobmv.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gdanxhyvl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gikksobhk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gynmvujvg.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gcwpkgqwf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gkibxrypl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gcqnayajx.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gnykcvtjz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gncxnwbzh.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gvloesvxa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gbedkgupf.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gvxpbcsvi.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gkcosbksd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gwzhfhxnz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gnniyzeba.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gvkyufiah.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gxdzurkac.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gmcsmqmid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gqxcgujka.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gqymfplll.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/goatmdtcz.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gxowhnhvs.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gwapovoor.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gspdlrgdp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gztmjsdtp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gmvxylfbz.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gmalrswbl.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gefrfcval.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gbhojjqjj.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gaabzuhki.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gqotsdryb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gwxuikrjy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gpdsnjghq.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/ginaokzen.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbzbgruja.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/glaylfzmi.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gwwcvpppf.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gxjwotopb.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/glveuyksy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/goeivyhad.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gunizfgse.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gboffdkcj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggzdxswzs.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gwsrfanmo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gethzeuns.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gacjmwghd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gofzlsyja.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gyrxbwsnw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gczpuhqjh.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gfnibvemp.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/guwueqeho.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gttlqrmoq.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gbhmxbsaz.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gyaorotgy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gtvheauez.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gcrldmvyr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/ggerpzyjp.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gytzwlksf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gbimghznk.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gfaimjlmy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gjhvipaxp.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gigfsgtts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gbtxidzzm.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gepjsogrx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjhjrbxem.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gibptfhvv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gyornikrc.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gylgfxeto.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gntasybdj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gpjzvclqv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gfeesddtp.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/goqoagpsm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gptvibydb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gwkhtczxm.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gdjulrsgy.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gfcyceowh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggzsqzmtn.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gudqfkody.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gnrgdjojd.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghuisbans.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvfogagni.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/ggggesnxw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gfjfezqbt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gweoezrtr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gtsypaqmw.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gzjejgqzn.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gjdfaqbgh.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gjcpqnmii.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gtlsddgax.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gdzyhlggf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gbwwrmenl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyyflordb.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gcxxozvnx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grfvkbuky.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gpajiuvtj.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gyrhtvozi.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gxocxdrcy.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/glbpmdtwe.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gefsypswi.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gxcduftbh.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gvuqyflen.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gjvtlmdag.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gnadfjiwo.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gaxbpmhkq.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/giikuhldk.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gmygzpoao.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/guixtaspr.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ggsckvkai.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gexpzvqbz.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/ghlyezspp.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/ghvrcycmx.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gltehuqfe.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/goastddpb.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gmzcqnomp.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gkvfhpwki.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gwhrwqsgc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/grkdfxygg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gtcrvszvf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gotmvqdqg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gejpxprxt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gcudhkvem.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gxqrnzdtf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gjangujwf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gvdbrnees.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gqphunfoz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gyoryzmtj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdywcykux.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/guwlufemy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gvziqstrh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gievmbdxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/guirajemi.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gibhwaxki.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gecxljvzg.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gwioucnng.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gkurpfjbd.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gwcgoxsfn.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gpwzqnzqu.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/ghdqadinw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxszscmts.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/grcatzwmo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvealumjy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gsixkysae.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/govoayxge.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gevgkxywd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gvwwtouhv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gwbykmpxz.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gczwbyxfw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giszpsiww.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/guplfeqlv.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gfuouaigi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gelzxtsbe.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gujxyfvaa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gyhlyvnkr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/ghlyamdiw.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gciwznvgb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gfiiqvcjn.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gvwaprfoa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gpiebqdwi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/goeknaqal.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gsmxwydrz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gycxfrjlq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gakonpzng.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gdqiryaaa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gwevincvn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gzqsyhdgy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gtklwhzmp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/ghugohbju.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/guhxemvyu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gpgfjbjyc.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gvlrjbksi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gmfepygdz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gznchxokq.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/ghkgedcdn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gucaykwyq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gqfcgnoci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gbujlmrfx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gygfdetxt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdczucshv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gvgfuklqn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/glmppqqtj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gsniebcqk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/geznpciql.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gqlkwvewy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gyhcmlxnh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyatwtccn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjdipewxq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gznuwcaej.sHtML


<!-- 参考信息 -->