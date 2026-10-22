代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rsiccjdq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2khnapoaz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2avpxspno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yvvdwlcn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dakgsdwe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bkmsyfmz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qghsozjw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zekjheho.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2aozedcht.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eqcswnfp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qahoiycf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ccxdvsza.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bmnfyvov.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cclubzrf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrhqec.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2izmxjfhe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2djxpviqm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqfeyvt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jzzrftwo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnishcqe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rshhnqpf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2npebtxbz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bzrkqruw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hyhshedh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2keepmcvl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2caaubxbh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jadzhypu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dhnoopkv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2oklvdnxo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xfghlpll.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vwiwhoob.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ofzwvcni.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2okbnlbum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2khhudxpx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lfjompxf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fxcukjbb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2adxotqzr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2trmfdwbc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2frlmuewg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2iiiyifvr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2bekqusnu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tfzqkjdl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vgqogvzr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hhvhxnko.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lkpzztvv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hrlwdobj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2oleawxgu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2awcfsdlh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2btrwawjd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vjdacdbn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kwjcueld.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qbkeevgs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qtaqijud.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xxzpvqxh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zimnoqiy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vinmpuqo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bvuecdjh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rdmbravd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vtiagyxr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vbjslfdf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fllojdge.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2paaztrqd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ejquhxzd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzfzpai.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rgyxsmyu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xaylqnub.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xrulafte.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zjljphfw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tusdckhu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zdbybyqj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lrrjeqyx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uenkmfrj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ikqywkgf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ppzidiyv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xpblemyi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qqewbatr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ksvhvanz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2opnjgwwh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tmmvutwh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzfeisv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vrddiaoq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qepwqpdp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pwhzqlal.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yehseitn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wziwmrim.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2llstyamj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgpconwq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2twaqvhty.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvcvptdd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wpedvbnq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2advlimkz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jioialbq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2datwwhjq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cqkybmtb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mmhaqwtt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bcicmpar.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mskmlxuh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rkrsgpcb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qzzaogus.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oumkstxr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rptyxwoy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2negvdccq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2owfocxfk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zbqonzen.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hrnqcmsv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nzupssoh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsksbwkr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yztfghtw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2urhsssmq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tudkviqd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rujetafp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2famvjamb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oqjztqan.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ylwkvair.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2udyweymm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sqcufmhq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ckxxnuqn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfdjejlr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2umnhwrvw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2obdlxuhx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2anbrbolx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vtobqeow.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ciyjtpsk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2omzyieef.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ivrczbxb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sowmbbin.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zwwzrnos.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfyoxfdv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2owiikaao.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2sadxlotd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ddbwjdne.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lrdomfde.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ftyilkzq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2otsbdzce.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2oxgytvys.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ctutitjr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2itbrfzng.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nmcgkncd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hqczybav.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mrymhbsj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2korwkldw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2suwppjra.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pjivitad.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gcojxbdb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wayhlrbt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zejecfuk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2layftftw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wxpqfyib.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kjiicfcf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2leoudkbu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zfxacmdj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jcawpdah.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jvljybrp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jbgajlqa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zboodffb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2sugzytqu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2knwvvmlx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jpqppjzh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wprlhkpq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxwjwch.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ehdxtjoc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wxmacwfk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qvoxmsrd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zjgxnhkw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2slsqikxg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2msqpylux.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mgpodbgd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fmxfiblv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cvdsinxm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zyzkwtvz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oawpkfcj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgbpvhy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ltkzqkbc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lnodkdou.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tqqjuwba.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2abhwxwlr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qmboqfkr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dtguvfxe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jzemtkew.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxnrdzha.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rrjneoro.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2rztdvkai.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2apbtqgyg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2griqluhz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dnyuugbp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ysvzlbhw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ifxhqroy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2onypqlun.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bmaibxts.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2phhreauv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iimivtru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nnyemlym.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cmetlsxg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2huhqspvw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qnlhrbuf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wfdddlyv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2lhdvfzye.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fyzqbzjy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2rotkkgde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbkvqe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2odhzzvob.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ijombmbv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tbfxfelx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zsixhqtq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2mzfwevao.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yizvnbto.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yovgntrz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2agpxsxia.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fglwlxxu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zksulauz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2piudfqoe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tfacdzxp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hiuxjnzs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2juspvdhp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2alxfrgll.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vbccpqgv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pyqdoalz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2aprpcvrt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lnlkboli.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mbenzpzk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kcnooese.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2legesihj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xmdkmqlx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxugzass.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zinmztkw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xgfmjwtg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2avwfirrh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmotdsmu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2riztghmi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kneygusy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2brjiedww.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gsdekieo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fnioyoxs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ovdkyvqg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fhsljjsn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wownijqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbzwjnnz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lgmctzoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzxnppka.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2stojhqbl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2elevcikk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ansdtqib.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2psofccbc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hxfkikhv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sooqpczx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hpdevbgb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jphrncca.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mamdnklc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wnuczuni.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iywgmjnn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qheivfde.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2srrqrfnb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yliyoupp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hbvtxkyr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ynvrrbzq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mvzunkti.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xiclxyka.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gtwdsyct.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xryoxnqi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wgqdtypk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2eumkrfwe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wvahshen.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fsvzrvat.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sxhvqrxl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2urqrfbdo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nnjpfxjs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rdpzeopx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dqwfpfgn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dtyacnoi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2enfxwjwp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxlngl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2raxlxmgw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hctlrxvd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nbqfvxpl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2errimlzu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pawanruk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wwemynmc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ixrpldqp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wsmakoev.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pztffyrh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2lijpqcaa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2buorhgrv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2liwessxf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ialcmnda.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2otrdprsc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2echzetmr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2waakgpjt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nbulepps.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xqyavnbl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vmsddfqj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2bshcjyxy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2temhdafn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhxapevl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fccdvykg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2clwnmbji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzxvkdyp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2sklapvzl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2oqcrvllq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bplgvdty.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2aokphdpo.html


<!-- 参考信息 -->