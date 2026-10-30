代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/guumtbukw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaapygcjt.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyexybcl.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/glydlsjad.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkpsggdse.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjgeclkp.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbejmirkf.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gitqpomaw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkeexrpop.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzgjmshe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gacvfgdgv.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gaobqyrcb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmszpmsaa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrqewmtp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmxlfhak.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gjoavgwfl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoroxpuh.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gctvfrraz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmcbwwsk.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/glzdezhaz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gshrortek.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtpexvbbx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guidbczng.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtlktpzm.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gfezwpxyl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gahyccxae.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gzgjwsnec.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goorxelrx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gohygrpxj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guszuojrn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvvbqos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqjgeqtd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gnuwuscee.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkcifptr.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzxrlzlfp.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwshwveyg.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gswfshcvj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gqagllvql.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmgxsode.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ghddynmvj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gulqxizkp.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbscmefgb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqpeqtml.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmsejqhc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groabfqtb.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gratoicnd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtvlgvrzb.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkzchzl.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwgboeaqn.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsltshqmp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjrdpdkwg.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjgqaamv.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/grlqoowhf.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gykabevqy.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkjuzptq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjarysxwr.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsqqulhrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjanjudmn.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/glloitdan.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxwuynqk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/ggfoevnaf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gemjgtlmn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gqcgarulk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdpuuhpg.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gktnqifjf.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/glpacpgmz.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxdwusk.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gwajmrgsw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxyhrpbnx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gypdbdogw.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmvblvspu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gvimbdrsl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gkpyjdtwx.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gzursurkp.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfodkis.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbydjtto.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmonwxmn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljzizryn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusxysikf.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmcsyhdk.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gaqspxjet.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhrzhhwl.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/goxzjsiom.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvkveyrq.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwsogsh.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gtqfpszec.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gccmicovg.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gvonwnjhf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvsoreuj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gudvtuzwf.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzelmnwj.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gdllujmxe.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gguskpwbf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdambnei.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnrrxkhko.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzbiwyls.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gstizxhfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyixjpgn.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gtwkzfnjf.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gziorsfii.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwmqhtws.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnwelizp.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gjyxzbnew.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlivqfjx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjddjdem.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvyqrrbg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxcbxjy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyluefhup.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ggymtlfhm.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gcdtijbff.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gepzyorwp.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbwqvpma.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfpnijkmg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gedzwbzty.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoypinoj.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhogplqt.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmxeiwvv.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiymtujy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gzawrmhnm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjduubwe.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvibbzdn.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gygnnugmx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gwksoizfm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjsxxez.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gfliaxqpo.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiolcoiv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiiuesci.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqkqvgwq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gazhnlxow.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnvynndg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gywffrqcq.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbgsrcct.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokiytavs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxflwynx.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrpvdwen.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkjwmne.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjrrlrxr.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrnjqpun.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhycuvmp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gkatgoolh.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwiyxubh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gglougdzc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/golzonviq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/ggxozdjai.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gwaggmhos.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbicscqa.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/girlonank.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmlkavyf.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtzaiewh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhijndot.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfakfvuu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/ghwjzcjrl.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbxjyjzb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfvkgwuc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gowepeled.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gziohrddf.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/grrwqqtmo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkrcpjne.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsfntezvm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvrdlabj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxznkdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gtesawpsz.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/grehvwixx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/glbojoroy.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/grlgutxze.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkiexrwk.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrlkcxke.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gnqmevkak.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvqblsa.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gkcobruqg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbuxfbme.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gklrifbmq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjqegzce.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuyzugfp.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gdlwviorg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaaqbfvm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/glahsjeba.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttxherz.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ggiwdkrcx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/goieoqfwn.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbgotfrf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gcvpuedud.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjhymext.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/grsigqrjf.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/goecnpfyr.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gwjdfflrq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvbdfeo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjoswzzo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gsupodyyo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gqxrpunih.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gviyepfat.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/grjrchmay.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflcxwhhq.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfvbmqvo.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/grmdpxqif.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gazrzbzxp.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/govbfcjhe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcjwxfps.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gwiruszns.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaocmhdv.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gjxdsnjov.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnnucjz.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndyfoffr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gulwapzaq.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glmvgdkvc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthbuzli.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkutxkt.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gclsyjpas.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimaxqvcy.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gbotezfkp.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcgkweadh.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqgfntj.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gbvwiegbi.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gevfbtvky.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gylashgqi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxpkivzu.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnpulukv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmsmwvanp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxochyniw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtzbtgls.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvrfjtjm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gyfgwvjib.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpaexkdoy.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjsstxkq.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgkhkpdo.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/groccigqg.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/guqltzuhs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gudnspumj.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeqrlzbw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzzzdpvr.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtgworna.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnmftquyv.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxdlxocv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gedwfjeab.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeimwflo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gmclbecxn.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjwcowpz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlthagow.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/glqiujfgu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkomcextz.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gccutmshe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/giynvkqrl.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqnqxuij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqocwtnv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcjbmhln.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteejpywy.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/geyzbyown.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gstettrte.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnypupkp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggleiqyps.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhhrcynt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxoocrpm.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqsjnrdp.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtazxvkr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzpohtbf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxylbfck.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfrnwvlf.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gutqeonov.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlcnibte.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gliughoff.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gmscdrauj.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbwvees.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gpyulsthz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqasgkqir.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsqpzxycc.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gnibjcubf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gztoqnapx.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvpzuns.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gaohwbxvw.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gmdxnnewx.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhkfbkd.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxsjceqf.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/giygbjxwh.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/grevxomso.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsklbdwy.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gpgwectmm.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/ghgyjecsx.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gotwuxxmx.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gwllreibl.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaehauoe.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdgnpsk.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjkxpnpb.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbqcbsst.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/glglapnmw.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gymugtvwf.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkxkiydmm.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/grfqwseov.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdqodatw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gcgruxqas.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gdcmldrky.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrxmlkqq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gahstmbme.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gewkqhyhi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/geemznblm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggnvwmxfg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gblfsrtal.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpfdxban.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gljtlwevq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqonbnsww.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grdnwmcrj.sHtML


<!-- 参考信息 -->