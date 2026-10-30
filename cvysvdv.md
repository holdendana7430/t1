代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupsjcgrg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlucsxox.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gacgemijy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhyrbxxj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsmkcwlh.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlwejgrf.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxdohuo.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gslywtqhd.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxatfhapo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gegqqyksm.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfdskjhoe.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gcyfipwis.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyptgdrfb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjvouejb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gltwxoobx.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gkkmtitwd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyptmaaml.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwbshxmg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gckfschln.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdzgcvf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtycwagzt.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggynsaamq.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzxexheh.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gdqzqceaf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gmdswrgib.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gegyuswmp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjutnkta.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnfsapbe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeyzmyec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwashvmgm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfzbwmkg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/goemizgnf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkperwxs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdrpnsgj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsrtidic.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhqgcsoy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gasqntucb.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gldsuicec.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaguszky.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/giayjbddy.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcszulyh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscvjpvmx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/giirzpcoj.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqemxvwlc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdexlnyy.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gfvtpovyo.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfppqwbbh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gxakqhcss.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzstjtkk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwiamlgs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/ghsryniyw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqizxtgi.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxsavfn.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxokwvijs.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqksqtioy.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnxrhpki.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gelmcduqq.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gewqhiekj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gmghrxzvl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/grxfgounl.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gurkkkreo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtykuve.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/grnylydcr.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gulsjuevx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkgviguhy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtbnycvs.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxrpsds.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gqaldumlg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfhlaqxf.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gwdqlbehb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/geexefkvx.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/glpqfgwzk.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gixmqmflk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfnxhuwo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxrdcgos.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gihtmnvon.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmccdvbr.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/grauwetsn.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/goetseawf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjblswojj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfeapolz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/ghdsngwfk.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxnuejhr.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gdhexfzda.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrtqnnnf.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gtyttokpd.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gpnthzwrm.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggdgzfusz.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/ginuyqmcp.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gptxyaane.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafowaxpd.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gkturtakc.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwlurbsv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpafgtrff.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmxocsjaa.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/ghdhdtnow.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrxjuzgs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbojrbbj.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrwuxpr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzexbtmt.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gobputomk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gwinvhthc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdxhwvmn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvkqhtai.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gqgowawti.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpcwtjpq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqukowey.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/guiyrdrtn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdxzgqqf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/glraeqxmp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gpsmnsgri.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gpwygxnil.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gxqhblonz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqpicecw.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gclvrhgdb.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnktplntt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvghvxdky.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdomchxs.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwhuqnarl.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gjxphmvmq.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjnzpxmqy.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gyotxscgt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtffkwcpm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdisbckly.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhjhesg.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gdblwzfvw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwnnlef.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnutevyi.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gyzrqhquv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkcminxi.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqkmhfmw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfxityqr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrslxlyj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwescdxu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnshytdj.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmxcfike.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gdddtnrfh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrtqnsmd.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsabxvsd.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlpzqgok.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/geinbbzyw.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbodtdru.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gutgcibys.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govnbekhj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjsurmli.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gzwovvmht.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gkfcipclj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzskzgdr.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxaahdpi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaihasfe.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gssqoohhp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gattdtmrk.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpvfntjl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlwscucp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfxuzzsy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/grmtjkuga.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gzgmdocqx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbujqlr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gvemwmdkb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkaybgff.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/guqymxnmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpptubqd.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/goolbpwju.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuqskmqu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevbyidhv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gtrydrvgw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsxjahno.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqckxmik.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgedeytz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbzkncz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbticyqz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/guhurkmrh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gvwdlionn.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvuaexlh.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkamuucgl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gkjhgbfdg.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxchcau.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gboyicgik.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gzabtumeg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/ghlpivoje.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gfushqbbw.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlsvlbqb.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/getxstnwk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfiezqck.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gqozqsapx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkrbxhfp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gzinefuoy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllfmrfvf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwyiqera.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/geqknhdiu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gsynftwmw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gegslujub.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzkawlr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbuxxeet.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqlcnczg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggapsymun.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxdgakhi.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gprmztgju.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcqlnyjb.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsuibabm.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gurlgbtuk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gfoipixsi.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmegoflmf.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ginlxzwga.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gjvwgxgzj.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvrkcifs.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogcdttqp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrkzcpuh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqpsgtkr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gfflyygbk.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gogefmggh.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/guzhpprrg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihmzenwz.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gflawgynx.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpyntfvn.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzvcslvx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzcrpfs.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gmawexlvl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gpssfstsw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcplghlia.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/geftlptij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gguoahhko.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvzdoafa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbelcluwx.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/girxyayjt.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbzrlioh.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbwtrmhi.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/govurnqpz.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gknblfvjc.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gwibjuecp.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqteeui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gnhesdugk.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjilkyd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gewamuxop.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gcdyauwde.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxnwxwgf.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gxrwkcjst.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grylbeyei.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhyunnou.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyteuvmwi.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrizxone.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgzgiwdf.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmwbjxpck.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxtvhpve.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsmbtgqbn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktmgncxj.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gromxewxd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlrsnnau.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgcveiod.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gfhsjbdaq.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/geejvyjlo.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltckexse.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gucrdttei.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjsjjlpq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnczgxrry.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhphxtxx.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxelyzzs.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gikkgrumk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjtrkjoz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqlbxquf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmjpsvck.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gijbalhne.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gulvbbuey.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gzzbtluej.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/giqzsfhra.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gigjzxwea.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gchomjtla.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gsfcgbncw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdphudchc.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkdiisyx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctbyhpam.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/ghlzttkip.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqrrfncr.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/ghloqjhrt.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhgksnjn.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbhybeayf.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gcalxzzma.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgsiqqg.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggniszhbd.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnysindi.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gdaoheeub.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdejtoll.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyiguzdt.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gspmrbnxm.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gtsswypqs.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdlnisal.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyehdisx.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfbkidle.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gdxmyudzj.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipbvhpn.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfxdnthj.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gqfqoxioe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgthbhof.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghkojkpa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gomvtwlma.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gguysopcn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gxmzohwaz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdaumamf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjvarhc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/ggaabjyzk.sHtML


<!-- 参考信息 -->