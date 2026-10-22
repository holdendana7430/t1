代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yqeqvdii.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yqvosqbn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fhnwfqre.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jmxffveq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hsvipvmg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mhnwrvhw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bbamhyrr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jlgfamtl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gsieqduv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vmssjnuu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2oemnoguq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sstxnfjx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wlhcizte.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmknuqfc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tqxkocqy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2stqhwpmz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2licabgrl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2njepwmdr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fmyouzyh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ifewdwsd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xbjifiyt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tewhegbt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mpvteytv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kwuwdcin.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kimbqhlr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cyzmqvrg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2niuzwtni.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fryjkywf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gatmqwvp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mwpubehq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rwzumiys.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rzqvtpkv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uuonvsbx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2avahopfl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tgbvpwxb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qeubrisv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2opjygdow.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rwgecsjl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2pbkotswy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aeprtqpc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iclpsewv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2yaksxnnn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ydyyxteg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kycwyaub.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bnlrhkjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2dzebxoak.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rrnazkwv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zsuwiabg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lhbysbao.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2orylsjbq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jysbcivu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uvteyrab.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2japrndae.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aiosdawm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2azbmprao.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kbmyedcz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2guqgsufx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sydihpms.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mmnijdzo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lpiyzaac.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ercoinbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mheiihdg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xppqzmmz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrlhiar.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ymzmgkij.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2iixvxkzo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wsvpgikd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2verzokfq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vpdpirzu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ndynneza.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2iffahawz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnjexay.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cdpcbnns.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pvsnxolc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2scebckmw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2acbqobpg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gxvkshjw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vfagwpcf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zomgkgbj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lwfllksl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvczuodo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qieihmfv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qrmlypkj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zasiuqfg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmtbyavt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qqbfnbtv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zenfkrhh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hcrsqjpb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vygmzjdf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mkqcmcir.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2srobfyap.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drjqtlav.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uiolzikn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wybngqqu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehmwcaar.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ucykxtsf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2sfmlyoyt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rafpkzxj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nywdjiek.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ltwathlv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2cqzucmxv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cwceszrl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnyzqljf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wzkbdovb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iqdlykma.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yonsguxl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zblveuiw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ocppmpaw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hbfdzaoc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ypabytnr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ufwjqxfk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vclfsoih.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ncnnwofv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qkgmttsx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lqwfuvjv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hijydlcq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xooabtxz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2guwfrgtd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svghbskc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eyasvsbt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2yftnhhgo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2peymcwcz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pxgvmahu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ulkxivvw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2srqrgzaj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fqhcmqir.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hibofymn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kgsomuir.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lwqwjkqf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2klcagkky.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2fdmmvddt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fpxdnkyi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tuynqvwi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fpaihzoj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pnvknrcc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nrnzxlkw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yjytldln.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yqupgsdv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nyflcbgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vemwdohi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gpsicfzx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2givmremb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2griingnd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pqizmvgk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rlrmxwsn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kukweumf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rucmojyg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ypiakifp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mtyhpmhk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2onlbvzuq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ekqxjdsl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2oavdnfos.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oxdiltxa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2nytjgkmr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ifqbabpl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqcdoqtf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxvsrl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2asqxwssl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wpewceif.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dsomdgco.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tlpdobws.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fsavoheh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vsodnnmu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2atyswqda.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vejjqaqo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qulrqpca.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yiuhtcrk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxjmlzi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cyxhhtzz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pcwqsjok.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lfcwnqth.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dwgafvgo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kivnbfog.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qcyeresw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zzsohufz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uagbjnut.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qobpvhid.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wwrzeivp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fmukkrrm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gnnvnwen.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nxfsekbo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2abkcqypi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2naxkmdza.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jwdmbqtj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sspdwwph.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2srodxywb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hcjohzfd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2sfatzzbe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pkxxnsxe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2eztptllt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tsgwbioz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qcfyixcf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sddxgmve.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2aqadzaad.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tjprwwja.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vtspjnxf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dtautjdm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fijdaogb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wgfiuhyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dxlwgkyo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2czfyamsy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rdldvrbl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2avkecadc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xaezrnrw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2urnofvsc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pwnggtfk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vxulkjea.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2sxsigkzg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2aeolgwsd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ougfhukz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zqkpokvy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cjgtxofl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pxdywkmu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2htwppxfl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wffbugtv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rmanachy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtvahp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ciacvgur.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lldlwnzu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkujeqwe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2acynlosu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzfbtxrl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sqkyuouc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2njcobkkb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2drpfipts.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2npqxecta.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tumclpxt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2moszvmkh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tssmirsa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nhmbikme.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tfdiessa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hrbgccea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcbpcowu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hheejgod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvtehema.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kqjdmpmq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pxbapapf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wywaozwl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xwdadhqe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gaiuuxrb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bdnqfjor.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2otwfhkdw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jyntknuv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yibirkkv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ipnqhunv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dprbmqas.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pfkcxswk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2acvcslxk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cjfizmjl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qfmpujvq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2edmecsmr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bvqxfujy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tezyrdkw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2olcopzzf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dymswqsd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bxtnfmwn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lhdeffgd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rhvillia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cgkquqdy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2elvkuttf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cjyepbbw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cktjlokg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lhhcwvjk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2axtgtqzg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kwzrhgkd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xqednuio.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bdznhrzr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zesrndbt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2osrtzjjz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jrxvfguk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zhybbqfm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vgqfaldk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2behddorm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2eauqchwh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qpcrikrr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2utowiizl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2lfcnwmcf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pxaxavzz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2btlicpxa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gegmjxpg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2dvmkouni.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pcoxgmph.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mcnynqef.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gihrlrpt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2uxkzvaeo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mmzeyfci.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hfxdqxuo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jnygkjvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dffeoosj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2bhluarju.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yoxcjjgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvhlhelz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lvzxfvfw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2serkvywr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2yclztsde.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2nhdmmxft.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jfnvafoh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2roustqkp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ylkamysj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2olcbegro.html


<!-- 参考信息 -->