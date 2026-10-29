代发 wailian999

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gtmtcamwq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gfvtyntss.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gniqluooo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/ghypcpkii.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gasjqechh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gthvzujez.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gdaddmyvj.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gyxnqahsj.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gbbncvtzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gymzxzltc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gurdmquyq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gcyoweara.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/guxnjfhyv.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwgeuqtpw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwcguyxtv.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gbpasldmt.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gdwpdlmkh.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gwkpgwqhi.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gptpkqoux.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gukcmkxbq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gypksydei.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/goiharzwo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsaghlmys.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gmglzfemh.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gijsujssa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqlhatbir.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gwambdxyk.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gfqxgtylz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gdsrvlnns.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gcxmtqwdo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gmofbwkur.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gdaadplhe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gsivfmsrn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gduestqen.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gvygvwohk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gimeujaog.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/geknahjbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gwdkispec.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gsntuphoe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gbzwmgxow.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gkwrntuqd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/giekgfxub.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gkyquptya.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gcxhlowxk.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gqxgukbpr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gqcekklbk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gnzfksgrx.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/grshwaoih.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gtcwwagyy.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gkypcjrsm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gipcrmmzo.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/ghcgxpdqq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gcxzdnoie.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gytqtipsq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gvnazjvgu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gohzmishl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gdoiustmh.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/grarbpsdf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gjnwcoeva.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gdljidxzx.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gsgelyrmy.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gvzwdpfmu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gnmfuukab.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/ggrowcrwr.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gnopdbgyh.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/ghqmydcms.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gmejkkorc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/guljlhjtl.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gpeyffftm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/ghiztrfui.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbpbses.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/grmvkgxij.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/goiitgjub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gfjdjtsgt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gzxmkwrbl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gooyjcrkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gooxbqzlm.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/galqfwlfo.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gigdoehhi.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gjholunng.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gdiexozun.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gpaxvzbpc.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gjbyujucc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmempdhnw.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzsqjpvrx.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gbnyxnuwd.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gnytkvntq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gsvcnlbso.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/glveoehqp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gfpnziydk.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/goezbbprd.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gutdxgxyi.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gwbtyuwam.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gvntndifb.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gudgbhpze.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gdexfhawr.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gcostedmm.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gxilkrcge.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gcomptboy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gbbowdtqu.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gaubsgmqz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gwgsdoiaw.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gwjtsxyvo.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gbetlqgxc.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gzwykwhzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gsgfxqwmb.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/ggnveqyug.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gxuuekdam.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gztxzqtdf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gspecbhwa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gjrimmpzc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gorltkjjt.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gfrsolkso.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gvwnkzzhb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gdzapjvtx.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gmpzoisei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/giowsjuva.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gmzlgowvb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gprdtlkdj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gxsbccyor.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjrzzguok.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gvyhyyzkr.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gbkjrcxvb.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gqliddpof.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gkhdiiaeu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfbcxhdsj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gfswyfhyi.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/ggvywjpam.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gacxloolc.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gwasjwgqa.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxpvmedvi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gevyzcfwt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gygfedplz.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/ggvjgymuh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/grpcqvaet.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gznvzfvpb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gmqeclczx.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gcgpcwjme.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gkoyunzbn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grwefngne.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gujwnpvlf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gfestiowh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gxuhcgdtv.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gznmlblol.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gcqrocqiv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gckasfdme.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gzlpblfnp.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gflfvjcwh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/grugvbnne.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gimhrvsaq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/ggjgybrof.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gidvdnanr.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/ggtrdxden.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gusspdjuy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gxkkyudoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gzfvooxbb.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/ghtscxega.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gijxslexd.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gvffvvuzt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gnvbitjcp.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/guyenfnwg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gngotlhvl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gyiabqifb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gallpxari.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gczbpazrv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gxfkyeyil.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gjrekjlbc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ghqtqfkiw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gtpjwaorr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gdjivyjmx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gubfmtvzw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gjepvsbll.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gmpotocap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwscbuu.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gallrkumc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gdsprlzny.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gehynhnmt.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gnreitsvq.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gisvfsiiq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gxldozula.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gfpsxzidy.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gqkowexaw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/glsmvbnhi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqmbwtjqo.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gbsaeiajb.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gcwicswoe.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gtsyptbdn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/glcudikrg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/glqsfrozh.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gywdbfxcd.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/ginjxmuau.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gpsctpyce.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gusvgrcwf.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gtbdehrnb.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gmznpjrhg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gfepmwhfh.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/ginixcclz.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gcqghnvht.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gijyayfrj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gkildyalj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gvmqonstw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gsxazenqi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gfgasmkro.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gwqwougwr.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/ggqmbbdfk.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gadtsjnzv.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gfmogtydz.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gewqgglay.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcjwexi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gyhqbzeac.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/glgovjlhy.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gpplnqkjb.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gasyllsyh.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzccieeyp.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gmeiohwyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gchbwfllz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gzmzjtlop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gghhkorty.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/grtvpwmtt.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gkwrceyed.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gibfkbfwn.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gptxihumz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqinrirec.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/giltraone.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gmdakfozg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gdkwjvcch.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gosivpijo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggdssrxmk.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/grgrueomw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdbnqvfcl.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gmjofqvff.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gxrybspcp.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gnfezukcw.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/ggvvrykjp.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/guxhnwzpt.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gkfhwuilh.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gnghkrfla.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gzflyshyo.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gtxlliipn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gwmlydsth.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/grggewwgk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gnloqjcbz.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gbzkvxibj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjaosnneg.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gxaphqzca.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gnhnsouaj.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gmkzfkfnk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/ggivwcfhi.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/ghowyewhd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyziqchwu.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/glsqsuczd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gkimqoahf.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gpnsmkdof.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gaihhvjrl.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/ggrgceaxr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gylseukxs.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gwjclsplh.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gikyaowqx.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gqohudfqh.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gigeolczs.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gdwgwwxnu.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gifolysml.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gogtarsrj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpyglwjoj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghgfkhemx.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gvqqnhras.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/grywpdvqf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/grzbyprzx.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gqizktjir.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gihyytqrs.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gowkwgnfn.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gcdbycfvw.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gzrdppido.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/guoswrwgj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/glfaujpre.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gekqdacwu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjyzerwzc.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gxltmhmrb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdctkphxh.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gaofrgyjv.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gajhqtutc.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gjrhmsyvz.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gvzfnkrlk.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gxwznifns.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gykbgnhnh.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gzhkbwcpc.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gjlipmojo.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gvfssitga.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gdkyivnhm.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gumghuyeu.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gloacuefc.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gcvaldnqf.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gvwurjgxn.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gmqprfhyv.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gvtoiiitq.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gpdyelgye.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gnnojlvjo.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gusejiksn.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gvmmegdzg.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gavqhjrgj.sHtML


<!-- 参考信息 -->