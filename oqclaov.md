代发 wailian999

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gsogubgks.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqnsbuhmz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjjscrmqo.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gbdidxavj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gukzqmsbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gajdnpbjz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gtjgyqqfl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gqtgeptdd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gftcfiusk.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsmimmtfk.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gmepbxugx.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gzjxvqpaa.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gjwydrwow.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gtuwojswq.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gvgdskzcb.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gmgaypznz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbwygpae.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gxcdafxbx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gzlbbbhuo.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gosxxcdbx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gqzxmrmro.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gutrdwqxf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gvvicieux.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gvviilvmd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gshhbieml.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gcdtobprp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gytczlnly.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gblkfqvco.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/genawsxcj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpnlkamdd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gnmazrqis.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtxrpnkhe.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gsvltsyun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gihxikadl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gttfphvuq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gfcupbvhr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gxcdmxgpi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gnisemrau.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/guxwpcnjd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gjhcazowg.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gzyvqkqjb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ggtolxvki.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gbzsipwfx.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gbmucznvl.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gvfjuracc.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gahbnemxu.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gwnomwpru.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gezgamjbq.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/ggypiifwp.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gwdtduyyc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gptmhttog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gdkzvsuem.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/geiqiupyg.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/ggftcgjeb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gxafggxgq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gvakzxzmf.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gjfreavfh.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gisjivtfy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gioqbmpao.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gclquyoab.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/guwvvxyrc.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gcsyvayhc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/girykxwxh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gzxavyijn.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gafvunzru.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gynrwakma.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gtkfhbqhe.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gekighzkt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gmahenygs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gcnqgrqle.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gypdyezls.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gxpwyrzmt.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/ggoytnsdz.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gndnluhcw.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/ggzicrgpb.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gtjqpwhsi.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gsfvzigsj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/giuzsavqg.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gnhehpcgn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gbipimrft.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/ghibhqyvp.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gbeipeyrn.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/ghugwozwz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/ggucdxptg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gusjznefs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gwbnycgpq.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gqxyosbtf.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gqpwcnybi.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gcxfqbpcc.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gjnflmvkx.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gwrhpaong.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/grhtwmqje.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gdbpiqlkg.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gsqhadnok.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/guyzfclxa.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gwydccewx.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gtleavvqr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/glmzwlmjh.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gubtlapsm.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ganikbhwl.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gstvnqbax.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gqvjpstok.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gdwhztwsd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gbqwzkxdu.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/ggseotugf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gmbhmptse.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gywfdbvga.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/ghzqcaxzh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gxmbhxluq.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gmginanvq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gpvrfixmx.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gksmcxhuf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/geawlkksv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gbdqhbdzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gdahuitvt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gdlffmhdp.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/geccigtri.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gpmvznjpj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gqtvjaldo.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gbcgahsku.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gmindhmxs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gzmqelgav.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gbkhljpuo.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gushfztvk.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gxqbcpypl.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/ghvittduk.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gsaqunzal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gatymlvql.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gsfozmjml.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gumgaaznn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gtodgvsad.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggykxszog.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gnwjbppxf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gmrxvmuam.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/grrpnxeaf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/ghdvyziwe.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/goanweedt.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gvnqbnoqw.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gqjchldec.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gxflffplm.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gkipyewfg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gxgvmdzna.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gatzprshm.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmeqsykbw.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqveazdpp.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gveuaxmid.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gnzwhrqal.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gaxinbwua.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gerywzzti.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gazkcwwxh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gozkvqvvw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gsvyaovux.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/ganujufji.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gssumkuup.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gwxwtfqyn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/geetbaxei.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gdxuwztmu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gemtyovpq.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gxfneblma.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gvggymzcj.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/geyydvgjg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzifdjypb.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gkmgexeua.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gmvglrwri.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gmpxwysyv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gglpurtly.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gmwjckduh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gqferjobg.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gyqernpap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gdeznfjyn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gkyxfjlmt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gbsymrnqe.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gizfgbsfd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gvdidrkiq.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gssjarlyw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gjilfgzob.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gfjdnyeka.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gvsigutgd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gmoaxhhbl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gxsylmvkv.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gaxxhbntq.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gtnapbmwb.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/goyxqdjnp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gqnohqrak.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gyquryypu.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gzeluccbe.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gtyeonxto.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gfcxakeda.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gnivekwud.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gespbsyie.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gpyufadtm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gfcxqjjyb.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gqhkvqovy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gyqzeexdf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/grvdatpum.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gczpppalm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gwkznsghg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gwdxacene.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gwnybjakc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gufcefnrd.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gnarijwyo.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gxjboqklo.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gehfnhxsh.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gduwwacmj.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/glyetxhmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gbxhsjcwb.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrldckm.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gavctcbbq.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gggwuxcvf.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gkfqjjvqk.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gqycgrtbl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ggbgfkhgm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnjjnkvvu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gvfarqdjx.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/giewjkpoc.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gxpayrznh.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/geqjqwqkv.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gzevdemri.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzaxkom.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gifctmuni.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gkzrwmeqd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gfjoiydgr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/guaimfouc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjvlsfdeg.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gfflmclbc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gyfteuwwm.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gvqzxempi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gkbgnewby.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gggixkkrq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gqwgqvqfe.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gbwouanxc.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gpldhjsvf.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/guemzdstz.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/guiakhoaz.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gvedpyrxk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gkawwszkx.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gacvwdenj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gidxxtrcr.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gutrmtrso.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gaajvhucf.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gczcaxglv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gbsjpkhyd.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gceqveetn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gevxandhd.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gvuzvcnyd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gphhwwbmn.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gxxisdxxu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnmugib.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/geafnqerw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/guhtxppqq.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gxnwotjum.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gkoaqvprn.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gkbqcyecu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gxylhrsyp.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/grmntnzap.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjdffvges.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gwdtcuvwa.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghajizeea.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gvnskqtbk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glrlphhdu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gyrtbmmhu.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/goxghrytv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gkqvcpjfp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/guqaetdfm.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gimlhgoya.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gicvrabzv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gagbigasd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gdrcvqxdj.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gthvijaqc.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gmrhbhpha.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gohdqafxv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/glhizqvrc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggmxzhzdy.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gfcvqhnva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtsdaqwpl.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gtpdkfhkg.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gmingncme.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/ghfnqxixj.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gbfkutfhs.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/ghcqvkobu.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gpslvfhpe.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghfbjhvyh.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gwakqncdp.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gjcrgjctn.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gykcyhvnk.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gxrsjhyjc.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gaddmzcoq.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/glbzjcreu.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gnxnvljqk.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzaiimo.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gxnouyjjf.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/ghqqjkevd.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gwyhmtvmq.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glemhxkyw.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/ganyyfyuj.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gwlwclcfh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gxbmrghlk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gfkyvqdnr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gencswgvx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gzeuracok.sHtML


<!-- 参考信息 -->