代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzogilqpn.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/goleuvrny.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpuibdulw.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gudnmobtd.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwztjcmy.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gbyerqqdn.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/geqawmnnb.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrmwfckz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grllunwnt.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmfrwbns.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/grwgwdruo.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gvxzsgqec.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/goasohmse.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfltrym.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/girmtzcof.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/govsjyasi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gighaqics.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkscdgzrj.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gqphobbam.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gqerivuyh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxvosvcn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpereqmre.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galadwyzz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiuuqndm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxwrkfs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gibekekvd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncphpufv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giedkykbm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/geppqfebu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulitsidn.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhkkfgk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/grafleziz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfnkizwm.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gocxjjvpc.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gurccpeva.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjzbehza.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/glmhtytlu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gviaarosl.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdvptdmr.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gywlpmzym.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvcokiz.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gojtbddwb.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbaydviq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/ghldnrjef.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuwkicej.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmydufhmp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/googsogsj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gteuujtgt.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gjoipprao.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gcyljmtqt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwutsvm.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlfuglpd.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gcrpjkbyi.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfybqgsn.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/glachstcb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbapuytjz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxpbgxobd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscksmxq.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gmckqhhwo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/guioarxar.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/goikwytdf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgotwihj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/guimmdvhg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gmutnrisg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gfihxohoz.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/govujplhx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgodljwm.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/guoanesdt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gypatyycd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdcsaine.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnielbio.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqqgvaxe.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gvoxaomda.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gfzegybgy.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gbozunhhh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gayctvojn.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlmghpct.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gxepufroy.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gvexxzjwg.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqmbfwbd.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gesnzkqiv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicewzlco.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifuxxjf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgvhcru.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/guyezkzup.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfgvflzr.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gtjzrsbwe.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqrdqflh.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gumxmrdud.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjublgh.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvchglm.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbgylil.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gxkeanwae.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gbchbnmtc.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gaibaxyms.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/glmqbtcas.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gwapruqse.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gnosdgfkd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gurpbemgx.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gnqyozjsk.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gudcaencp.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gnpmwwbgw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/glimwawfx.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuqknegu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godwttmaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfulzfbg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gxczoblod.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibzygwif.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpcxzdcq.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/ghthkisor.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gtdnkbhma.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtexzmhna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvtorev.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhyvmxs.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/guarvgkhg.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtemflevp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzcguxoz.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gmujmkttu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpquwhte.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeggximr.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gauhnpdlb.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmekwji.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtfgikq.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbexsnzpw.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqhgpojc.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjzfimpn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltysgqbp.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gyiunvixv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gvkpmukai.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhqtlkyr.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gmayrdqta.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gusgbghar.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzwugooz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqswsau.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvqqszr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncofafcp.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejmlrqo.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmhrnwtu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntwmqzfp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gsvonlkrk.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgqwbkii.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyplzecwt.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrqfykp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyndgxjez.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqhzsmvu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdtdtvx.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhgnskcr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gxgzsqlas.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjhdoccm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjyauudl.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ghspfbnma.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gnrkzurpp.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gryamyaso.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmwujmjh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnqvslwb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzslcvbfz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gujdsgcfd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwbfduvm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/ganyijfpy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshiwvgo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtiibuvb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoncklgn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gifvqmrwk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gaoosdorv.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gjbtkutvx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gomibrboh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbaqdxwr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gknhwlkbp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gokxwdrxt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgilbiu.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzomdyyby.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gohpcavea.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/ggttfucmw.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gcombyprs.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gprmcksyz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloliltgj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsmduqe.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyparwsp.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdhumigf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxjivcuq.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndzxclx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/ghlxlhoeq.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigckncn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/grwsbtngk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhcdmwdq.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtjbnbsp.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gbntqaurz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpnklmys.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnvwvgls.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gdcstqwxx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/giwerytgo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/guyiahnyw.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/ggwneqrav.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsxwkdxx.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnptuvmn.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/glfdtjkaa.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyxpcxeen.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/grbqwfqor.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gopjknsbd.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnkpyoyn.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gudjhrjoc.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdribga.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gowikuppq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxnqisihi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gekornimd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfnkgbdh.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdazjymw.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcifblbtg.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbzxsoel.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gzveoriml.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxiomenjt.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwblahc.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaibcljct.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/ginpkozwf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gumibqabg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyodcebdp.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gkbcskprg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gwacwbpmq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gjslcsrmw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtljlzkag.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gfvorbtpu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxlygdky.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbcyndjo.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gucgmyriw.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gkuandudx.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/grtlwoyge.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gimkrvgep.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gvqivvkal.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggrjpvms.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gvszdzyba.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijhltdd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmlfifhs.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gyujvflbf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuadccvb.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmrxeipgx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gchgjxota.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgnmjyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbdiaul.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gahrgbyrx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzgokwi.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnlwxgmc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoutxwhp.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gwsalrqeh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gprzsvdfp.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gatpyledy.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmcylvpy.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/geacynvdb.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkwbybdp.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gfpfsnude.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmfrldey.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gulargmva.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzlatqed.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtmiggdl.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gjrfhevos.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajabivgf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitxuisch.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfchvarf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqiibwj.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/glhglpqqy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewrweokd.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/ghkxxgvak.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/grxggrdgu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnmphts.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gqkynafdk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnjhvlwv.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtnsxzjw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpqytljzq.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/griamkvur.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/giinjlurh.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gpypwvwel.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrbfdkpq.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gxvgdirgo.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtmpviwr.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gohaydubu.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpkypylsb.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gnlbsixre.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbvxmrsh.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gepwqseqd.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpmivnby.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gocpsxygt.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnzarzmn.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfjpgqw.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgggwrbj.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyptyswo.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyhkfypq.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gasfoqrkm.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gdhmmjlop.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbfaaldt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gvxpvgjqw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/grtooijpt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfcqrilx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjluhomt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaupcgrl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhvnmouo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gxtoxbeyu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowxadle.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gwnnwmsap.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgdkrkpq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzcimynm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdpnlvpd.sHtML


<!-- 参考信息 -->