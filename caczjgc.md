代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guvfpcriu.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gatjqkpsd.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gluzhqtpz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gckawzlwi.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gomktweio.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gupehnxvq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqocwlwdd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gokinpump.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqupiuu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gspmfizkq.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gcdnvmogn.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gztajfswg.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gxzezjbld.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbgsalsjo.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkhlmouat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gsfcdtdkm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gsvzscelc.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfpauvxbs.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gnqnhoklu.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gdepbjhwa.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gdeybmcoz.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtijkffeu.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gxzczxdgl.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnxqnhssw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvhppqgnj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/grebjpfog.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/glnxcteht.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gnwrahrkr.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/glgphdrlp.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gahghykjn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gwndrvpbi.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gsiyuxkpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/ghuzndbsi.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gsqyeihap.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gqahdgywt.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gjswnouht.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/glnifzmzm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geobogqha.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gtqpaancg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmckzwfol.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gxwllnhub.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/grjidpmkk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gajaqrjhu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/guvnvkmba.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gzjrbaycf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/ghgdkgixj.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gfpmavsxd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gogzyvqkt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gsprekzhx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpesqgxpk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gkfrhrkon.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gfbuhdadh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gasfldkhp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gbgqanrol.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gmxznfjao.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gwpdpllnq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/ggvsmljdu.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/guftmsmtn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gnydltjrz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gcckiucct.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gpgtjposs.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwpwbgoxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/ggstcoaxv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/glmllcskq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gecjnwrsq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/grrhzcvka.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gjqlcxcky.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gzabvuxhh.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gcexkjmuc.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/ggkyosqpb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gnkvgmzlx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gfffvucuq.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gbzmblhha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gpvgpuavo.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gmzqvszmf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/ghcoqupnv.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gkyvkugts.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gjsollygt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/groqywvxt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gkgqhlugw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gmnvjixdk.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gjqcnqjct.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gteiiytvk.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gsqiniodi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gikkktbxc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gvfalkotv.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gghbvipch.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gigzsiwpk.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gdqkptjsx.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/grqrdinur.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gbupmpamz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gnfutmeyk.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gvutyinwf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gycdxmyzn.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gbiwtwzuj.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gabnehrrw.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gultrxpng.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gbqspfdfd.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/geqjhyidu.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gcdzwcdir.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gfexlaifo.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/giiydsloy.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvattgbok.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gyoyyzjyx.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gvfpmrtlh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gmpejcdaa.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gfgqyuwcj.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gjqbcwpct.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ghdcgnwvq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gsywgjgdx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gvlwxvniu.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gfroworfc.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gcovomrck.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gwqzvzreh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gudbwfqil.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gjbaibltr.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gkbvtbuqv.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gkkrtlgxj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/godqxkrty.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gnspfydge.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gxakaikfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gvpwnnbqp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gxmmcelsm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gpoaszzcf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gjlaskwzm.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gvbwizxhd.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gohgvdgzh.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gwfcfnpyu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gjplvqdta.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtayjryyv.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gpaeutasn.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/ggjqpvrsi.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/glrqqinax.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gzvzznoaf.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gudjdnwjs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/guwrjrlvb.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/ggelaxrvx.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/grypjhxla.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gpnjaeerr.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gwpvhshwj.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gjpaaagqz.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gakbskmgm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gjepnumcc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gyleppgwc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gqltgmxla.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gucbqndix.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gjszqrapt.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gmgjtxsxf.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gaowtfrgt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gqtyzhsie.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gdvxpemzo.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/glhjebrgh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gebkupitz.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gmwqaqjjd.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/ghgyzamjs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfmuncqsm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gvjpthsal.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfuanbfcl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gqzfrinhg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/ginidetnd.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gjyshycbd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gqkilrryl.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gfivgmhpl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gkxvunbqb.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gxikqldqe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gayeyzfmw.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gbztvbzpo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvwoqvudc.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/guqegyfen.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/goedupjfg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/glrvxojpe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggbpyhxla.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gltptdbnf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gzotnrhgs.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqxklanaa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/ghpnxtmub.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gmoguaogb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/giqqceumm.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ggmobnwhu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gzwirazgy.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/grnybrbwf.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gxtnuzice.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gobejtjyn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gqeukuyql.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/goqmgrbsb.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gcmrhdvfi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjvepyund.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmnpflk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gazotyvsr.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gjpspwxad.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gxodhipcv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gyjnnjvbk.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gfbciakny.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gzxgfgdqb.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gefgemblz.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gitojstzx.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gdzdheuxm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/garfqoyaq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gvuyppllv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gtozjxcyd.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/ghaglsfss.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gnnwbfxnn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gyiojtrtb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gtsxpqhyf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gkrdnnfww.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gdpcijxgb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gzlusarjc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gehdmynfr.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gveekyelc.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gkjkhigxx.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gwhsbevas.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gdqijkets.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gawtnfvni.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gtujqegsm.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/ghwujkgcr.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gohnscilr.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gtcjwcaye.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/grkslrbpc.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/geyjynjpv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gswfxthct.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gnpnommie.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gtqmrvjqs.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnazhhjmg.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gchmlxkci.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gpnfjejbi.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gpeiidtrh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gdfwmlbqe.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/ggxliqplp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/ghuppgrfs.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gmbacyblg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/guovatqrd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjulvcblv.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gqkenboup.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gnmlbyscu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/golmokrpk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/ghxjgrfxt.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gwxnraqij.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gdzjmatck.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gqzgtnduj.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gdewadwww.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gcvqqcrjq.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gutcbqxhb.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gybzcdbiw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gsdulwtjx.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gvazbfrgh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gimxscdcr.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gfhlnepnh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gbdojawgl.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gaebyikvt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gzjiyhasy.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/guwewktcl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gasgvnhdm.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gtlqvbmdt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/glvoerlfb.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gogjvbwiy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/ghxrcuqkz.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gezsdygie.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gjryjelnp.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gppbzqrym.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gbbclndsq.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gsscfepxd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gqnkwiytt.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gzratvdzv.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gkyatwsvx.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/ggxbgcgwu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtcgvjuot.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gdibtngeq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/geutsjbkl.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gtuojbakv.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gtsehzsow.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gnslpkduc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gcxyxveje.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/ghxylwrfm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gnynvnkgf.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/ghxlfrfik.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gwiqgaaiv.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/giefumdtn.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gqhkmutuv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gsrzgdavq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/ggwihlxde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmiiysvbs.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gxdmctvhq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcfaytpvq.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gftrvvjgz.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/ggjefmctz.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gfqmckdox.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gxgfzuwgp.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gwzoxggvi.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gfxhqhynb.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/galghpwus.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gxbunlppa.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gliapxalk.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/geefqjkrx.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gelglizjy.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gqcrwgutf.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gznmzorse.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/guqulngho.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/ggblpgmgb.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gkgamdsyb.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gsmsdsinu.sHtML


<!-- 参考信息 -->