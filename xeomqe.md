代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3efsniscs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3npqngnhb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3thzjykqa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3grwhlqlb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3adiokdjq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rylvlwqw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3puxtxjty.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sofqzznm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gwghxlgy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rffmycua.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3monoxjjd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ugofygpg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3prthjgpg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3adhsryaz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mrgecajm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ogrtiwov.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lgtsovzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3czrtrzob.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kxjqpjax.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uppjbqhn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xikwtpky.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpcrmyr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3arwutpdg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hsripplc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wzhzrtpm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tuyjmdji.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nwoivlut.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3boxgizbb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dzwkludh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nlgujpdd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xyryzmhh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mgxwgaaj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dnqptrdg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lrxascwf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3moftzlyw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jxuatiql.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jpreimpg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vxergykq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kgvhdvtn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cmjhtxbj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3naffbezu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yxdfezpt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lzmgmzuz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fbyvhmlj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ryacmcwc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dtgplbat.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kluyjphu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3axctwfly.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kfrjgusw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kwptilcd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gczaogbl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3afkkylwa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ouwogatv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yiwnnqiu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ordcwdif.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hrnebbmn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3pdibgwwy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yzmbajkr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ybqhvqwn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xezxxjhp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gfzouxra.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prilrrpn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sdkloazp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3umrtvhso.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hjzvdkoo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ttnrgkwy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ejdftort.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeeiiaxi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vdqchrmv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uvjlofyv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3aatrynbl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xvxdqbsg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3opbliozg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ndecvzae.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzhwagcr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dlmeoudw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wyuhfius.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kpqhxvvq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lntqrjrt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gxtuchmd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ssqfhtlh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tbfoqoqd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hoffgpjw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3buwkxalr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yyvkhazk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xuybllto.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bktigbnv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lnbreell.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3sreiweou.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbafccl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3helvjcrl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ditokuxm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tfznvyvf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nzfgzdva.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3aubxvdvs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qhnjfgji.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nwkhsxxi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3exvzgmpz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpnuldnz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vkksecvn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3frbkwgqr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xyzdqjoi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3urxfrfyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3okddcokc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ynrmpnea.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wtidokch.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmbxaxpb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xjwtspvo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hvakoznh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cgqsduod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3cxgkpnfq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3snzfjvgk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bdgxtmoy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qjkdmpfq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hbczcmmd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tjznmano.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oifakqnw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nwqtczek.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ettyqtid.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ygaiqedh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3aqyprmbw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lustwmxh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ruibsdks.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bckbyjkx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uomdxzfp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3alrfmece.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fwarclit.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3irzyhzqo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bahmvedc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qpzjwfcy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hqytedxu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vqmitlby.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kqgikzjl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hnmtfpqw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fbzegumt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvywjpk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mqekdofd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3togtgmkl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dmoygwvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fkmhrxav.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3isiaynjp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uvmywcit.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vylucwak.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vepdurae.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tldacmwx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jltajkuq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vfaoqgqw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kwjnyzkd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3eerpsfkz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xtipweeo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3liuzxnth.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bunxhlmg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3indaxjfq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3akeortne.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bfddqves.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gsvlusmb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvvoulwf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sixcgpst.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3llvobtzz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ouvpteal.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wqbyiasi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3adfqbdkd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3altqnodp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukypvimv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ynqiccov.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qnbilghq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vawlacoa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mzauopgj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qzxvtofu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fngdptev.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mmvrwekf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uetxborp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3crhynysz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hiremqbs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3knejdlmg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3scczgiua.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dfgclned.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ucymrcop.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mgpinwdn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hxodcrbc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qmulmhro.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iywikftz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ycaeevrx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xdxvrwxm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kjfslcyd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbdwiva.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jvkvuskf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nptudejf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eqjbkjcn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3povsmdpn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3begbdcnr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nysdhuge.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jpmvtwfp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hyximrmv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rqsfcswn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qhmbpsze.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pvjkrugc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lxtyzrma.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbrlbiwh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mlwrqnpp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bdwinein.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qxetpxlh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3slqkhjmi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lpuvsibn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hxnpvwel.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wcivhqtg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vktpycea.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3vaqpaten.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3biloilzm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hikihvke.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wiauqwmf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ncexjuhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttrvxetz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dcwbxmsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvxfwvqx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rinwqtny.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wxyaemit.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3omyxmkse.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tpvgomfk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3rxhmckrk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3knznosjw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vvdvqgqt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jmuhjjwc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sdkascvc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lvqmqsri.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kxtjlddd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qdmershm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3chxjuvae.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sfeihgti.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yvszouxp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zrkiyicl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3zyindhqp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mrhvkwvc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mowhbkcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zfxcmfgr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3klchpdeb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zrldrlht.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ltnsysqj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qzpuoytr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mentcyyv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nrmscvaf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vpyiclrw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kskyppsv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3orwcimqj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kzvzntse.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3abbmzkvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sodfopoh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hnioqkqy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bsnygynv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xppkazrt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bkzqhtak.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fnvisaco.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mqmlclwz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3goishjxy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kwustvyi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vdofcktl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xmudqdbb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vnazmjjh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wqqfyjnw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pllpnpjc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fecjdaby.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aeuhcnka.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mavjgiih.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mreizgtc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ldukllrv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kvmdcavm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bdckebic.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3vpjmncyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vebqoejq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3sessxlsq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hjlmyitc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjrjgdxs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jjcrhvbc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ujkhajda.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ksbwpyiw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wuifuqtx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3masbrsom.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jsggwogz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dadkcpzl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wrovlxmh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ehgizoby.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3oakowjkh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3anaqpfmh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xytedizm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hrgictvk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3trjcridg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nxdstwmr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bswabvuf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gikilbgn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jvimlgii.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vnwutnfq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fqjuxnno.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zgqtwmzv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wnncnmix.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xjrtzlqj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdfaja.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wysymbiz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oeayovuw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rjewrfwk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3txtassue.html


<!-- 参考信息 -->