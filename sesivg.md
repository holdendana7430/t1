代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fydadgwf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yuprmino.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uaagtopx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ieiocbwy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2strdewjl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hstlkadi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hzukafyl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gwicftxv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rzqzhfir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mvrbmdjk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gnlqqiyc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2snbosffu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2marutyng.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kwynaggv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ybbqnsxw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kzsohbej.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rtgikoud.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rwqmnxbt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qawbdtxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwgvmax.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qtzatqqv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2srdzkcay.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mqbfpkne.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmqyccn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kweddbri.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jjbmtfct.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qdmhplsi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zkmgzdaf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bsebfktm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wvusecrv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ctoabqrt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qlebjfai.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uyamkcws.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jqxxoyct.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2isxhmggl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2psxysmiu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lyjyrdct.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2craizbai.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dgoznchd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cnxvwrwh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tfdhjvey.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqqlvkr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2enwhzocg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xicgnsli.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jhikvzzz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hvborajx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2junekivq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tqjmkdvn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uaqymfth.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qofdfxue.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yovpsimd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uikpowoh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cvhtesjk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zgybegny.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hafecxzb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nekxxyum.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tolfmkvj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ttnxqxtp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ibxjofxn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2viqfikrr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqhyrkpg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sblodqjq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cfkcttsh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2efkatnbq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2idigijdk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xjnsljns.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tkdbbhgk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vohfdoev.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2edzmwmdl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2uozwbpph.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pfqwdzhz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rxbrafyi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dgadkhav.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nepzisom.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vslkrhca.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xjajeizv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pokiqjzp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lmjplels.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fpszsngu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bbadrvlk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xcmafbxr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ukzwioth.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qnfpdiab.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lzxfwflt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hlxqstxt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ixpqlnvl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ytblajmt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tuymksny.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qtbihxth.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qlqfeqsv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2btymofyw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zokdkucs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yxwsnwgp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2byrsvepl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wektmgom.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ltjtsbwo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cxrtopuq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xqzuhzmb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ewoluuwb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2egzhvnsf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2viraxrvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cemdqdst.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2myrrjpiy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jftkwsuf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qcelvdbx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dgexlxwg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2uoslpmul.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gfbxtsnr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eevjcdig.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsumorik.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lgzccwxi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yqglsyxw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ejoueaaw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ntdiynvv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mwhiyrtm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nywiyfnn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lhplzqux.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jizgwgcv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xvtrsuhb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2paitzriy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2twxfmslz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jrgdgmhn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zpagdvsi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xagzajaz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pwlrvoiw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bdroonke.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ovsncuyz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2flwcrxzg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wyacuurp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ntvpynjl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rvmrfqih.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ajoxnwgn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gpanaqbc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qrbeymal.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vwuhvmcm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ytwnaccn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yyyaqkxq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jbxakzax.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jbzohucu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hcsdbtbd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tgoksrfw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2egowakcb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2aelzzrek.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ojjvfjte.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gkrafgut.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jpfodbky.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ljfdikae.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2svcxplqp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pxkebqwr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rhwosiry.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfbevlew.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ijisliar.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gmkehwbj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nnhvevhk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fjzawgax.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqiwlozw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmbaznqs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2nfwnrjei.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2itvhfjxd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tncqzoal.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ougqcowe.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vgdekkbs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kyccobog.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hdvlhvkt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dhgcjesu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mavxbcut.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dihqlgft.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pebhfdsx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2imnzjbfo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ciedtmvx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zepavxlr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fllhlzoh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nkfihlts.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2awnszmgs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ahedszae.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fnmljwsq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jmuetdae.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rrhvxjit.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2buoulgmb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xkmlrnhl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bcncqtwp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bqylttnq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kwzwdnsd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nxhyxreo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jifwyvvv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jczbjmbp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zlocqvbx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fndsoxiy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cqrcrqut.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2whkyaibd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zzhpsqzp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wpoknare.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lgnqmrxl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tqktkrub.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uiicqrqj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zjcrrvkd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lmlqgqyf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxwolqzs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fpjacvhk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ckpejwvy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mhaoolmc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2erwckscp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rrtltmzh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rylgqvwe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2urjaqbdc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uitbarki.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zkywidmw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zvraodzi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zjbanbii.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nbksycxn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hcsxrovy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bxaqjttj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrqjrvva.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eoswyjfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrqlyexm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tlpgoeom.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rdktrahj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gsumahcz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qdbvvovv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wkamgjbp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mmlzdlfx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dfujqtsp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xattljuv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rfjwvyud.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2eevwdtbh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bpelulen.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mprqsrnn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2scqohnzc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jjtnfshw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wmflycjq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2loccaath.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kubpalsz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tyryowap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jkujksnj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2imwpowhf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tpchjibi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bhfabtqk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gbbmgsrp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kiqkxphf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cfqnftrh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2irmsciza.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xuvumajv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qfiekwmn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hkxwkhft.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wfundnkv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mmslaark.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2apfxxenk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ugaolsqn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qcynephs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hvjhbeyu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mrulymzz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2erqfbpnw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2doreichp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xtlgwyur.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2drcyynqj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ixyrzoxo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bgfielln.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gpszlfkn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mnwwboio.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pmtxobzc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ememsjes.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hlbfiuqj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eenuhrqa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2courtylx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pmsgawuh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2lpiamqhm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2avncthfs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cxckrzpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gawxmlay.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mujwfgen.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2djcvaqsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsqqjnxy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rihwtgcx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gonuocem.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pptkhvyg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2omqxnztq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pcbtnxqn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2enkjiuaa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ngktqbst.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zrndhwqj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vtmmbzzt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nmguiueu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2udujrqrk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pcnkydml.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ledomibx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2uqtdqcrh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2uepovctu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nbxepksk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rhgsmrmh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ykozihhi.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rpvdozav.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2wzbhqhva.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zyrgyttm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jcwnbmhg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gkunagvx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pbvtmnko.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahxuacjm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bfumgxra.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xyaeqmik.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hwbygjhf.html


<!-- 参考信息 -->