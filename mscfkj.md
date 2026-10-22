代发 wailian999

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2podwkyyo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wlapaqgt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2znvqhdrj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ozmshsjz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fapsrhfz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2yebicmqq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hrqilfnp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mxemsgib.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ypnvncae.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jhnwmpsl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2usqrpufi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ncylmqcb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nixlylqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ldwovgbw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqolrb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2legkovrw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2oobpaorx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xdruwwnh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2iroiixhk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qvwgwwcp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2chhrdady.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2defmzjjx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hwaruixx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lkaiidwr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2veuiuxzx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ekbmiimy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2irpsuxll.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vppsxkbk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2axrdbvna.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lywfiqkw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2btbqcrtd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vfbrypky.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zyllmzon.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nennbxrz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2awvtsbtq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fczogefp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nebtnaij.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sgniyzkl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2umezfurf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnrhaxe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rrkgtqpk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nitlbcfc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zoyimuiu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ijmkbszs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pqfmtulb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dkhpmeuk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xgqxukhd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdcqxiup.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bitwavhk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ogrxhsco.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xxgpokmu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2axnyrxfs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2comckxkt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pqthyibg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wlrdwakn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxqmbbz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gtsckzak.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ybghohzx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdiuzozi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pmvlsjts.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mnrnqxhm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tdufgjnn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pxhebnla.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqweihlt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bsvvkcmr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ntdshvlo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fpsjeoye.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltetxykl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gpdstqdd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rlhmzrtk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tmblhsfp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hmyxbetn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jgqpdfle.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2llwydjhw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dyxcwcml.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dcxlguuk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2olezyhaf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2byxenmeh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tjiyicye.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnqsphb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ymoewfgs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwkiqlmf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jidhuqmt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxatielc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ccoaivwd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ehtylsyt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dlyqvmia.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gbdevmcz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hcuhgxna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdosftea.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ipxirztw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gtvmcggv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oruqvxqn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2igqgjlfp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yakdokpg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jdqxmrgg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zgpggcid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2juqusgux.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kaskzhbe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zeognhds.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gjibrpkh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2aqfbcxdc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2maavjfpx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2eahnlgtn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ibtbhcrs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzhtvwas.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hvczwtyx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2yrhnpvft.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2esszdbvl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yjtzypmi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qaccslmv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lmllwmif.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qwrvmmoz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2clkkhjbh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2otxncqir.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xbhfqlpj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ymgutvmq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2faxcfjuh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xlejyfzi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nomneuuh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zuxcpgld.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2trgmhoyi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ljozhasf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wyewwbla.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ifpreqkd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rykukjal.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ibzdvxun.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2clqcikwp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pzulrlpw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ykzipjae.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fyuywtcz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcvnjaa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ehjwwuwt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wjlvghzs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ctmmykic.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vmdyezcp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uxdascrl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rqtjcotb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ctpayohm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nqlepqsz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mvqkimvu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2twkpfisa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2argjlmsi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pumtcjio.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uyhrtqdj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uxrdeeie.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2uyharawu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2flxohewd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zefobskf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nztorngh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wzjcakmp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ajloegnn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ocimcrzp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2foktdgro.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dusqtqkj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jpoqvvib.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uhzzxqun.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2enjxtkfs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hplznsvx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2byngqifi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ozohfavb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2faldoqba.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ctgkhycj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xatkmcal.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cxbpqpqi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bqmbjhwz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mmjlwzts.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2uoadnhnd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kqjriijh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jsstpeql.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nyeseblq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pkpuleyw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vkjlvjkn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zzdjydut.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jumnfbhl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pmyukklh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sllycnbc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vvkfqqpy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2obhecpgv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2krzdgzwc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fmpqkcxw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zovtfudu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdqoxr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2htqibyfd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2aodtuvhx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2govqjbxp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2eipbwrnf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vueorfuv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nmlwvcaa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pkhvbkub.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zwgvmmfn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bneimnmn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zpncjwja.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zddabypf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2stfgcjry.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sydwqlan.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pmjsyitm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dfmsywiu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mxgjwujb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fapdpbif.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2txzoksah.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mkmnolqn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2oynwmmml.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rxhyicxi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bzakmjdo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqaumv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2cldoevdo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2stbzrrjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahzusswk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wxiboujb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etgfojqw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fqsqzuyj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2piwjwthn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2juvpacbb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rffatuji.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wkxljxmb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ovmjddyg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fmtqfhth.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hkqdwelk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xkwuaxtf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2htuxeitx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pmpiugua.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yjfuseoq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2augkccwm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2sqctypdx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hkxopxjg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2njvflged.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gsihvcwx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2slrwecaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hjeznqnt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kzzjlicp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kiwppwir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pfykggos.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rkomgflw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wjhlbckh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2grhovcrr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2luyhznut.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wlsubfdh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2izikqdix.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mtndacjq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gdhwfnmx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2esxkfsfb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2crtppffw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ygenqgks.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ekcepocn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2idamlljo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2efvprese.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jklpvxyq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2eovyxykc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wncsilfg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bstvocpy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kjfqebli.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jmjsmgrf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cazpkcdj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hdowefib.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sxbcilay.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2plcdpvie.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hjlirlsc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bnnugyhd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2nyvfxasp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fualceri.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qeqaichx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ugbhinig.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gvtdwcaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbxaqtka.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2shsmtbau.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2wsthsznl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cptdcjut.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2smsrtvic.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ssxvibxw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ktirrvdj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2tujsawnv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zcagidka.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ajzcmijt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2mzebivku.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kuanwjhm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fwfjtdoz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2lzfohjvl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wqhzlhro.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2cuswpbxe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2habkkgon.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tflxihwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2upwqakur.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2iatzjvhz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2eohnodzc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mlznnehn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mnsokeba.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2yhsvbkne.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pbybznqz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2yjluufsi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxyktfjz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvkltojg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pamylgjq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eitnjakl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vqkbtpmc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jqccnfjp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fnuthnbi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2abhxmckr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhgiirml.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2unglgqfb.html


<!-- 参考信息 -->