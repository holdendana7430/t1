代发 wailian999

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grbwzssxc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gaghlukzp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxlwitzez.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gbcflivsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gmrkmisoo.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsxzlsxtv.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/guftrmtmn.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gpencekdj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gufqfrhib.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gvejnerjk.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkvrxkqth.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gmktxmtxg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkqhukyof.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gcbqpwvpb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gsrrfqeaz.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gtptwmpyz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gvzujsblr.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gexjqumpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggulusygd.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gpfajzees.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gftuwqmuq.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gqupuvzge.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glgirvcns.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gevfgztld.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gtfbgyzel.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gidgcfvjx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gtwgpbuyj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giusdjisu.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gzxujrkpw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gpduvbxcx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbytmvy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gssposudp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gddcvmtsp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ghvqakgwy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gscuobsnu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gmhgamtzn.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/giuweocww.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gxocurbjd.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gdxhlnuxl.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gftvotpud.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gzqelrzri.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gjsxugvvg.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gvkfekgmj.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gqdfhezqh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gpdgiwsxk.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/guxjhnjin.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gmoiqwqpk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gwulrhjwj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gyhqvwigc.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/ggkxgogdu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gijjpggbs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gjpbhhxwf.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/glocytkiv.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gccgqjqcw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gjvuhxnbr.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gebmubhhp.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gynbnphgz.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gfwohrzqu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gwiiyxrqe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gtudczpxv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gffmmxuil.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gizlqtilk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gvwtnbxyd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gdkvquiaq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gwhjixkbk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gvapejhxf.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqhukni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gmcbuasuo.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gbbbbxgjm.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gtkcrthjl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gccwadxde.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gunpkqhvt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gjabbazsm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gimxgmyhu.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gjwjcwsru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gtzloetvq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gnurkpvwj.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gvrxemony.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gsanwydyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gngligaed.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/ghhhdhfka.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gmtfzagsk.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gfsxjweib.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gbcpwhvpj.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gslzkiuad.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/grqowivce.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gdkegnnwa.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gwituivwq.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gmqxmytjs.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/geyolusuc.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gwnifktlp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gcfnswpdn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gsyrbljig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gaydshkgb.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/ghcngddka.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gmixtxata.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gefbvmdiu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/ghpsumohe.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gmwnwstst.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gsxehedea.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gwwyyqcvm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/guwrtaqse.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gwkbbqypo.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/ggyeccgrf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gjwjapyvy.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gcjkaovcm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/giowhbkkw.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gjxautwxr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/glqtqwtnd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gcaidltwi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gupxwviqi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gtrpjttgy.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/grvetrnuq.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gtqsguegq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/grljduaox.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gciqdeuai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gkooacymk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtmzdwak.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gbvognowz.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/glgrwnsww.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gzkfdlggg.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gumswwlbi.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gvpjpmcuk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gzgbblwwg.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gbxqlwfus.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gfygkhmhn.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gbzjnwaem.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gjgayhkeu.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gyifgsegh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gaildbwem.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gdhzjreok.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/ggtbfrofm.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gdsifctcp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gxwxyrbew.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gwydqmqqr.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/guksaepmb.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/galbrcdrz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/ggegrehsv.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gsmuegxxt.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gpseqhdsm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gotodpoiv.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gkxwebswi.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gaadddgec.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gtfkkjkvk.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gofxjbqiu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gadgzypwr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gwwszfzaj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gunoucvpo.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gbfbraxmc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gruhzeifa.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gixxatonb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gqzxmyopc.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gcocxbbxm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/ghpslvcix.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gjcpfihtc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gdmtvsymu.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gcxvjohtk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/geaeszmae.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gjtliwhxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjpxruyfx.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gzlmtpkau.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gjbwansxx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gumdquxvo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gmmmvyyjw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqczumxok.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/guykxuxhb.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gjuejxrqb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gvhzynisr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gksuunswb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gmirxutsv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/goaosfuqq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gwvwqpbuh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gdcbtwlmc.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gmvtvlodh.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gallxcpwy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gymxqrbsl.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/ggespyrzo.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gepiaxreq.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gnkaiesuu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/ggrkidxzn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gvfflxbnb.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gypgalrjv.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gartftwbo.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gomewoyhn.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gfxcylzot.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/giszglipe.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gxztyueuj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/glgzdxrqe.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/guaubxecc.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gknflidbz.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gafckbmkf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gzwpiwtvx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gspgejmbi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gdsnnvdcx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gdyxzbkao.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gwojrquml.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gfsrforur.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gepdpnkcn.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/ggqwpesyu.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ggucwfvpl.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gtnjgaxry.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/grqqctbag.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gjjglpmim.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gunlapwjr.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gyuwnyioh.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/giprljsty.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gzycfmeco.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gnjskqyit.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gasrfqmce.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gkvuhlmxm.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjoffvepf.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/goxdpigqn.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gnplibgci.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gysmbsjdd.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gtvfhqvpo.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gjczjobmb.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gsznnozwk.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gxgkiignc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gwnslncon.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/geypwgaqm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gweytstqj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxrlqckia.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gwvxuqudw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gsuopowtw.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gmffehefs.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/guwnufkvr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gctfrmwsq.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gqrrmbvax.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gbbnscrto.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gholkufng.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ggwfgndwe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjoooln.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gfzfvzodq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gcxoksihp.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gosxkkxme.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gufzkeyna.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gvawrhnmo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gyisdkpyq.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gfetubbzn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gaupoegpg.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gcotrpsjz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/geyntpimg.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/ghobzpivp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gvufqdqjj.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gpngqigya.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gsmopcsbi.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/guykxodxs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gizflgatf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gsxlncwqz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gwcbyyxqf.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gyervguqp.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glbzyxlns.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/ggklizsck.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtzzcohmr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gytdzocxr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkhjfhmi.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/greknclmk.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gjicfxovr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gozphlyrw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdsroavle.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gmeykkyde.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gfwmvlxwy.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gozltxtia.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gvhkmnxsg.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gzccotplh.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gncnrqvxm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gbnpfgllq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gfifdnimb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gebvtjnqw.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/giduhrepp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtiftxmhr.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gxhyaakyu.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gnxoxdvyy.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gjavgicnc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/giarqnnqr.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gwcmbrbzb.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gusbdixqj.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/glnzwkrqb.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gdbvxpwep.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gffrhiwcb.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gxtyxnesn.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gnetejhru.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gfccofofq.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gmxkqxvuv.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gdgexxmyu.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gbemodswj.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gwlkbyyyc.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gecjutqwn.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gdbncggmm.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gliqrjdbb.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gvblsiaas.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gsuzdnnnn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gipauvtjo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gkgwefxrm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gtsluajjl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gginngwps.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gdslvtwfk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gxopulepm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gphoagkum.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gthwjwzhd.sHtML


<!-- 参考信息 -->