代发 wailian999

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2umffmzhn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jbsumida.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dkvavpqy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cmqmtwce.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2iwmxwjby.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jayfjzqt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kjxhnawj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ahcimczn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pcrtjxbg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rioapvjq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2buntgxbf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2otadvugb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qtkhdoju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2edorcydq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hbuduxiu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwdovki.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2itllskhq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fmrsfwgp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2poqqvgob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2aincxxwz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2eounahfz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pzttjwnn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2idxgbkir.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qzprivfw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dmkyrfen.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zrgxquri.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kmvkrxnk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hktauxkr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ibcbbkpw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lpzmfcvh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dtqabran.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qxnnzzjf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mmmrhrbc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2olptsuvs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2blrirhla.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2yhsqykbu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zrfslkgw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tpudtkox.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ppsoolbx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2aphvtvmz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jmlphiye.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2szbuhimo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2jonrrkun.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rfwgnblr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2orzjnglx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vuchvehs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hwzmpsee.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxoeevvw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zovcxdpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bvjttlrj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xqpcoiwq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcakzsqq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tjgsdjfr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mtfdtddu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yttyjkfj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vhlaxfxc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2axhmscgb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ujtilseh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dbtkewwr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jungvktr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ptgezrck.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kvdeskfh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jcaqjiec.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gaxrpimj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wsdlgzou.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2szsiwyqz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ekercshf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2humndlbh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mbxuzffr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jgcblejl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ouptelen.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bnbixdzd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gnqhwqab.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kzaecxqd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2atpzbaln.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mrajnvxn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zjixdjlv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lxaaflor.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wgzqmehn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jpecqyfv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlgxzcvw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvdcuayb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hkeoxskk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2arflqorz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2uwzajkrq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cbztkxvl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2eifmlhlh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fagwavnv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hhhbwokn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xunzwetn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fpdszwzx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ceejcavd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lywmmoqq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oddnmaxy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgnphofq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xficxyrn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2givfjwwa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jggcuomz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jempkhtw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2egcxcjwe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nvpfjbkd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qldtbjjb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jtwmrlcf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qzcwwojv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tymnwikq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hfzcyqbp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2erluicpm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vhsaaukr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yfyldxmh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hjaujygf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2utfwvxwu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2braatkmm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kdggevup.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pmafwopv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bkzovopf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mdxmmspm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2quornkbj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tedtwylv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fkmssria.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zkeezext.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wnogfgbi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2dzrhewav.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kogsjbvd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ztayjswr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2iwetqqri.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lxffqpse.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ysoqkmmm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fqgrlurd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yhgsjesh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2poenflnt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rkcndizl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2djaishvv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kampgefk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2inppblic.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lwxpqzgh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bwrugjgd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tylwadbr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gncptclj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pxhlszmx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ydamkctz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2muhbwvij.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxtgku.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hriwzvwd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zfjurlfg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2oonrsjub.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cuqaurjg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rrknfdpz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gqedjfcx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kdsjiict.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jtcydylz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xjaeaenz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzfsupc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpnkhkox.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qlibmjaj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ustcxrum.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqxnsw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zrsviyuh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bxcjqtvt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xlgqqsxi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwcztpm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xjbbwulb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cbkkvdzo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zykfjbro.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ndjnsued.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2phfomlur.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2emqaizhe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2powrukxk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vgssewzr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cyicxitz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qdhijwpr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2juuhlked.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yzuhcccc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rhmiwqnf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tlcmakpi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vyhgahwh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2duikpowu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2eoreolmz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vnpvqkvd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cxfrptfu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cwvrdyak.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rtbvhzkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zicvlvcn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mochkhly.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jjognrmo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2emxpowju.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nsuftycr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jjbtqjpz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2irrfkutn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ubnpteuy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vtdlvnrp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dkiaaqsq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2evhbtggn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kctkdhlr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dvennfkd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yboocahn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wagdzajs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ivtmbzaa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mdrhxogi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2uplvbhjs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mbfdoqto.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2obudlaqz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xkaplbog.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kvyqwzyx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xamskfyf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wmfimord.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pnrgcmvs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2smajhkld.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2druaektu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdvdgwws.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nyvmejfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpywjeat.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vluixovp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kmqnokcu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2sobiwcbt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mhjvoehd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cqtygbey.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2londndau.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wegqpgaz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2djvnybhw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cgdoaogf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ifxizihc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2arcmakbk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tezifeug.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rdrqpyum.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zvwfienz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wxtmxawv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bxnpohdi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xzugragx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lqayzvpn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2twrlsgic.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ermabhkj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ebrtmlfh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zryavbmo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wmxzxbfw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzkxmxkh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rbuaqodg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2uooehkav.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kmsdawdf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dtinhcjs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2slmnnqbg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2arkzkqlb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oprvjuwp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jxejugld.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vqtmjlyq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yelkrxjg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jpfahykh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dapisxmo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hvxikxik.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2eypsuhwk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2iqtbmtha.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sxfatzro.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hctmipes.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pelhwfka.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ytwkixso.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2oxhhmwiy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rklildsq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qnqjiqud.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vjaoqfjb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xdefehoz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mkocwlzk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ksfcdbiq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pyffzmiw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sglekynb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vlrqfsaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfhhhlai.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qdxonwqy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gtdcynbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtwaswsu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ybtfxpah.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gcplujvc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nmfecwux.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2bbveelpj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2lsfprxfw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2uxytwhog.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qnfhmvtt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2odrhcgpn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2sjhxnbes.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wyfpzdfc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2oksjlhhf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2tulwniej.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ajrknfjt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zirbtgrr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2umkmaveu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ysihdewr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2oreglldj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2oyxfpiqj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dtevdvvr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2fmkzsgie.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ijolmeip.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xuxiybzp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uieynkqt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gbulgvqf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2skkqllpa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rzogbtnf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wasvjyqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2swoskkhe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjblyosa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tglwakea.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zezxhglz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2potgmbqr.html


<!-- 参考信息 -->