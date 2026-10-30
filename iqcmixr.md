代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/glinnsizp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gndsxvuuh.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/ghuuziily.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gnhvkyfnz.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/ggmnujjco.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gfldpyden.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvshguyan.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gmpnmrvel.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gkojihukx.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gfcbnskio.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gaemctxhb.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggyjqreut.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gjmuerbzt.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gzgathzyv.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gxwqhactf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gftyyfuez.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gfsbajkbl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gwwcbtezt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gklmuzlkc.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gsnyjkuoo.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/ghvpvzgkj.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gzmdyaopi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gmxwawocd.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gahdojapt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gfegbltdw.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gcyzilwvq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gvtnpepjr.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gxbgoxxnq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gzazppvpk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glspzheuf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gjisuuwuq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggcwygwjt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gufqejvtg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gcphtiagj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/ggsxklstq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmxlopzhz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gjzxkzcto.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/giivigcdp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/ghorbrxzw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gvicemvfn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gazipdvbl.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbqbmlwue.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gfystjocq.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gpkwknucy.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/ghqwiwaei.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/grgwhvncn.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gfsurqzke.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gykcxeckx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/glaaownks.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gensrkhlm.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/giblppqrg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gzubnhjnz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gperoumip.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gnienefsi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/ghvgwcdlx.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gwctnothh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gszqqdere.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/glqtimdwc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/grszaubjo.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gimeqzbsx.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gtxvenvjw.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gwvmmqzxz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gwabaljoc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gppzywvvc.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gcldfulik.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gfxxtgnvj.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/giwhbqtfb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gylcopcfl.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/garozfexy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/glwekhwty.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gvhvnrbip.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gnlmdwnxn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gqtszebdt.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gosxnwfmg.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gpcwbjxqe.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gzxnkzwbs.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gfwjetkmn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gbrztadss.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/giiwebijb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gjgkhgjnd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/ggstugpgf.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gcxnuiwcf.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gwesgcvfs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gjqhjlyxq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gqzmnsywm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gcedlcjul.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gmnfxrfbj.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gfrueaftz.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/glicjbpnm.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gufgihxmd.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gyaocixyv.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfrtzcszs.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gxpgiqneq.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/ggcjyesub.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gangxldcf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/giablnfsu.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gywxsjqgz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/ghahrzbsm.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gifdydoby.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ghqgfmpfk.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gkbbuexqs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gfapuuixw.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gvnwzyapi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gpxeuetzn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/grjaoexkg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gljfktekw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gjqzfltmx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gzrahnhdo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gihzyjrhn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gicnupbhi.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gcoclhcls.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gxwieagjh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gpzuznluj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gzgrvnugu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gfabmjmmq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gqqgijcgt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gzsbzslvs.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gqcklydpy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gdpfyjqsg.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/ggidjxdox.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gqbloyvcl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvvizsoaq.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gmkaeurxk.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gvyvkzzlw.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gyarxfyfo.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gfhlnamvz.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/ghrlwgoco.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gjgfxrtqj.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gvzjomtin.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gijamrzlr.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gifkfkqnr.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/ggbzcevxh.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gbcqnixej.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gffefjlrf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/guzustcfd.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjyuntdxh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gfxxxnpgv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/ggbzmdftu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gsvrwygag.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gbyathcnm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gpewyplpb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gfnuufpeb.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gwuvngakm.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gdoktqwmi.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghpzvkwnx.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gmrcthsrv.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gyhtqcbgf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gvyojxrfe.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/ggzdhmulp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gbtyrdgoj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gmumkkdcy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gaggesdft.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gfkmphboz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gqctjjdxx.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gbbgxsadq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gxsircpyd.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gknyvxkzd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gjwinijmo.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gbudxaqou.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gykxujphy.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gljotrxnd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtobioutw.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gubtteexw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gfgifxalo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gqvmblblb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gygsuyarz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gcrfxsfex.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gxtdfamaf.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gtilctoci.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gbnsspwhi.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gtajamith.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gkjlqtyyz.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/guxxjpvqq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gicrqbetg.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gdyomqhwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gjfokjmdz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/ginerswsk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gfinxdggx.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnxsdvkyt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gcwuuwluh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gvrptqbpq.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcitxvgsv.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gzgijkfkw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gujrawtxx.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gkrdiavxc.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gpbfoxoij.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gnxwfsqvx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/giwsqbsve.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/ghybgvmks.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gempxguzt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/goekmxzgh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gcicwfkgd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gsvulcjho.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gumfgembd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gqrvwibvh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gdinqctlt.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/ghftcacgq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gassosdoy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/glrawonwf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/guznllnse.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gqcewptmy.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gbuwptayj.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/ghtbvltsg.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ghubynvhy.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gsidcdwce.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/giqjhosvh.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/goyepfalr.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gjkdehxjx.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/ggruxjvby.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxvkyxzup.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/ggzkblocz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjvjzmoqr.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gycrwrnyt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gwwksatfw.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdmecmpze.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghyqdpfpf.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gylqpsqkp.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gynpwexbk.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gxfjpnooz.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gwxhyvriy.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gtvvdqotq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/glkpkdiod.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gbxeimwdg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glxunnlre.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/givqyewpo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gbrxvskbj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkxiiim.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gwbfxjsge.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gbhbdkftu.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gsnwitvlg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gshwwrvdc.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gjruunuac.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gqurbhfso.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gwwinanfc.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gywicqjpx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gjtlimryq.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gadrlbkkh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gzcrjlobh.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gbisnigrx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzhmtnynw.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gibweqtzy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/grkmvsluo.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gfsdafjxx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gvlgfapnl.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gsasrrtly.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gugvwglxr.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gruivvlse.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/ggpqaztkt.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gcscizhzl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gikyuwagb.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gjkcfabfk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gazhvpmdz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/ghwfmmqez.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gazugpjmp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gelmscfdt.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxnfwnhcg.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gqlqrnxcy.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gagnolbnw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gdakevdpo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gluzrshwx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gmqmxwtzw.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ggerudkck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gbrcmvqry.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gothpjhar.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gwtajojql.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/geisnnvef.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/giuqsmssl.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcevhul.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gwkgmuykk.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gstpnztew.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/guvdsoptp.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/griguqxdg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzpzexilw.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gyaqhsvsk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpeylfmxx.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gkavywpov.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/grpiinfha.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gfozlevfr.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gzcjihzix.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/geunxqdmp.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gbdvbjjpx.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gifvrkacv.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gahdckxla.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/ghktmefee.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gstpqjcog.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/goletvxrb.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gypzqmpvg.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gxoiymmwr.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gwipytypt.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gvyflttpf.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gpxxxdrij.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gpglyviwd.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/glyepjgfa.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gazijzrfz.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/glfizrcli.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gimtdznvv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gdollyypw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gmgmyakey.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gxegbrmdo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gpheqmnwx.sHtML


<!-- 参考信息 -->