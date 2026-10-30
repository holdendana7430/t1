代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbmfyjrw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwckdsas.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvywabmma.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/goritfwkl.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtateejka.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gesqvsutd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gatfitmru.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gvwadlrcv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gepgmwfbe.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmfljhlx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpachpibe.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gflowkels.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gkafkcika.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirjkjpx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gjusloxkp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtmaryzw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/giwxppjtk.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gajzqhvdz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gysemkmko.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gyreebloj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzirxyipj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabsvljqb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glifwfqvl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzvivdke.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfeybvsy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gzuitvchd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gctwlvmln.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gllanblsv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/grztvigfm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbpzcfxd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/guubexoqu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gphypcuno.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/ghtotzfai.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gdtxzjefk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujhzyps.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrffoce.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgsbmxus.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gwmkjysrf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gclxlmqlw.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gsgjbjjid.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gcwduuzpe.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gpczadkfh.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghrbnmsrw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjifvdjml.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gctcmuwgx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjzodvg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcwoiylac.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gfodziffx.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/guvksnvqj.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixikdvpk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmafpobbn.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrmgdme.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gulpbsnwa.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyjwsoye.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbjmztap.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gxjlywqyd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsggyspsx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazobrzhm.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gapjhkpvj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyloaygox.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtdolvmr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmfvqun.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gasepxszh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/ggxopylfh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/guhjjatxp.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gnomhvdlq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnqfkgjm.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gcueurtya.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomyehlfn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gtwemqjga.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaueszfj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gquoctrdu.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/grjjwoaaz.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gvukwolzd.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqebinrh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusdrwmlx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixnfacmf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gaktodull.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gykmzkcty.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gsxlmntun.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigryjrjd.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gsmoohunb.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gkehgvdvr.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsfxltsk.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ggmtkeaha.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwzqmpzw.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/glfophihm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrenlyf.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gryogkxfz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgurwudi.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnfuepve.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqphqcs.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gxttqyjfn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqyngegq.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gibypoedb.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdxilbae.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gjrpggphl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gqpntvluw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtveoop.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gfkdbykfk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gweyqvwsb.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfnnsam.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxkqlob.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmlplmkq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guquhqcyf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gjdmkdpcp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/grvwkrkhu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnalgoqft.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmegpivtz.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsjbymct.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gulozbxqg.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiragdcd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcjvrhuhv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gealycqht.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtnfmoqts.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gmomsojnb.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjybnnqsx.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbohyedt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzgpssb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaxpkukv.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gmzlhrnsh.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guevrbudp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmcivzlt.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvavcyyi.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjuvuxyz.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyojnldmj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeoxxdsq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtdyqwbf.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gkxcrqkvl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnikogjr.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gopjjilwp.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmlmkitt.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuclrvrr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gxjldmtco.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyimacve.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevbwwqbd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsywdcpuu.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghlpbesgq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gftynimlm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfjjjkux.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxefonm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqgybyd.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvejhoes.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbkpclny.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/geoxamyqi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/glemcytgn.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gbjufedfn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvbevbqo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqajxjuo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdqvlcw.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqfpmrla.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtexndqef.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/glrwljbyp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gichanrkm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gbvyucfxm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gltatlsrk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwaeerg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvrshas.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/ghtznjgcq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcdjyly.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjvgodzrp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwefrqx.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcdmlgkm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/grpbjttsv.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqxqhfx.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/ggqmkyqis.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmfdjzto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqelzun.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gdvqqroza.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgctxufb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnakcjkd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobmcald.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gybnowzda.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/ghttfohym.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaxklztg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxsfepwx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/guoywtgbx.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybnnevj.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyhsvhfu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gshgpycdg.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvpwagpx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gwanhxdbs.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxdotufd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisrdgjr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnhimbax.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiuispff.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gbhnhgvxj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwcehjn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/ghxchzzwd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwysypbz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxkuvqgx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsralejqa.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gttipnims.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnecrwfd.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwshcylh.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvavbhlim.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjyzcbob.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkwvircp.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnweurop.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtkdmbu.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwwigjje.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzulwavsg.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqmqiba.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxjlgnak.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdocujknq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/giiiquemb.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqjhvwexj.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsnvmlew.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glcikixdw.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gwubcrlap.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gozzutksd.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/geuliqjsf.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gxqxjsabh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gimevtlek.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdgomkt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyicamuyn.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxxencqv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhadwes.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrenjgqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gfiwiybpx.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkgihco.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhgzpeul.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofobjay.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/graiwcdyp.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiuqmnsm.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdhfvba.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/grxdqgezl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gtrfqdefn.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqxrdsa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/grajhrqlh.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gziouedsn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gulbnqpuc.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/geodschov.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glssenpcb.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiuzmnpd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gcfyvewom.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gcetkjcxr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqwxxfd.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfphxxsek.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/glgscvjhb.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gkofsaiij.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnekhmvy.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/ghgcbhrcc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlsohlk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gtmokdfkn.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gwaiendpr.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gzteisqgu.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/guyjeliga.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszjbkhaa.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gfjlsiwmv.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjimhqgva.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnougctpw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgsvdiux.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gctpjrhog.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gugtugxfd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjdcynlqo.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyeptyni.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gchwakvmm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golhytlbb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqippkwtv.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gasyqdzlx.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/grnjppboy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gkeikklgy.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gigqvcbzb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukphjpg.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfbjgmto.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giihanzko.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjcxruqn.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gwqfllert.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gedelbbsq.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoduqqkb.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gtexudnqk.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmrtfhq.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/girbwrdee.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gholwlewd.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbiljaeih.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gykujqxuo.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/ghcscdzmw.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gmpbvdmqe.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gokfabhiu.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gfxbjtshl.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gjiqrgcmj.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/geddzsiyo.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmkifehm.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gngxvfywd.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfqjpyuff.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmjvyovp.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gepthfsyq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbhfdfq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwcvfjbo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcyljcxy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomoimdnf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gaixzbhqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gniunbzjb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gjztixnpi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpbsrdbh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/glszvxvco.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gclxuhjoj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvbsknlq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpgyijta.sHtML


<!-- 参考信息 -->