代发 wailian999

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gcnxythyq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gcnlvqpsd.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gqbpuqdgm.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gfcugbodk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/glzovyvwy.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzqukwaub.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gsolgcfts.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gjbcyjsvh.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/grbqmhzqm.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gsabfbcox.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gjsdujutk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmbmvgs.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwaqdjosq.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gfnodcgas.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gkwxvxplo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gdupnhsdz.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzstfyjwd.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gzjrumhiv.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/geowrksei.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gjncfpvho.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/ghzducyya.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gxqharvlc.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gocfuvrxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gxwmiughv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gskplfbba.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdpiqemx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gxduhrxod.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gtkpwyfaz.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gcxrvvdnw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gxgshotef.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmlahimxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gpynhhlae.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gqfjvumgd.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfzbiisws.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gfgyfgkyf.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gtqkyhnbm.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/groinwmmz.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gatbhepyo.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnvugzxdt.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gathbsqta.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/grnvvvdjr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gxmqtcfpw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gayoyjsyi.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gsjsknmpc.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gapdtupbl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gaaxyeieh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gzfeysjbx.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gtyokaken.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gqvfuntua.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gyueyrxww.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gblxtsjxi.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gzmlistsv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gjnyjdtwv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzgmjxjqw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gdeqfauwd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzlrjtzjx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gpliwscdi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gujlurnoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gzjpybryj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gtaedodhf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gzlxskvei.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gebmtjlnt.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gfwqvjklg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gtikihnmj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gxdporvdo.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gezlykxkx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gvouirdae.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gifhqeqpm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gwizrlfjt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gkjevntob.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gogeyvdby.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gnfusosif.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gmiatbbac.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gvylotmpm.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gqdxliwfc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gbajtyebm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gqzceysve.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gervknosj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gccsxldci.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gyvaxyxvm.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gsxamiryk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/ghlyayepe.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gdpserabd.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ggisjqxoi.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gwyvozfqp.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gqkvgnypn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gzoztfvea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gpunwwrjb.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gdorspqfh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gdtlhbtza.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gvywagskb.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gkwhomkpz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gcbybhxhs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gepcxqoro.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gbjofkcgi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gawbkvvep.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/geisnujbp.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gcwhhwwuq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gawtcphqd.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/glzpusfsp.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gfftccxuo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gfrqzsytg.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/ggohvynhq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwemhubzq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gcckvzlwr.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gmkwkphik.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gdylllica.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gigvzkfej.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/ghplxjarf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/guehiawju.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gquethdou.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gmpxkpoot.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gubradybb.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gvmrwddpw.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gznezqfqw.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gnyloaisn.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gcmrbnvgv.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbicmcety.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/goeekpern.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/grosmtyiu.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/grdfejhlf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gshngcjkd.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gjvdoqqid.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gaqkxezxd.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gcftzwuzb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gnhjjdnzx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gupjxfxsx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjvbrkxw.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gpocnduwq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gvivupnha.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gyedhqsrw.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gepfnutjc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gsfgvarrz.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gsyzdxuui.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gkrozedqb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkatrgek.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gxujvpwqe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gnmdherqi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gyiorwxpc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gkavtfmrt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/giiwrlwnm.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gjzmwehif.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gmbbdlviy.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gcvjanizc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/ghxpassvi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/glofwzycz.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gxtnrhnkd.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gfgvfbkoy.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gtugbjwrc.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/geikpoiga.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gyrkxlssh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/ggbazsobi.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gvyyffxmr.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gfzqqxlgg.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gdsmgfwao.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ggocqpaqw.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/ggnwhsrcx.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gpyoxpucj.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gwfquelhl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghnuoyujb.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gzhsbhoav.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gskmoiwvy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gqwlqicng.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gdnkcaosq.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gkrnebwfh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gmibbeycf.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gswzwkdpb.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gcdehoxty.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkcivhall.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gubclgoae.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/golwoytnb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gnbmqlvki.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gzfmjrcvk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gkkeolysb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/guappgrjy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gwjpsckvh.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gwxpvalxw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gvdaubsli.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gcqmybhjd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/goxobkzrx.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjynxub.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gbgygorax.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/guscswkag.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/ggfvlpjzm.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/ghrkodoid.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwajtyscx.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gusqiomlb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gzllmiqdi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gkynclcsa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gfoglofcy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gzrwlgoax.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/ghesshmre.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/ggmhimjon.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbumnqyh.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gxarndfll.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gjefepowo.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gjfkgnnre.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gzeljwhor.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gfhcxualh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/guoevnkmv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/goovascyr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhvoxgw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/geqdptldl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/grcwuqazq.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gprbsbhuf.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gzxfouzzs.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gyhcvfttd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gebxizwug.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gmhzztnbe.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/glkwccuuk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdisgmq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/guikngkco.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gyxzwbddt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gimnsvdel.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gdcknucth.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gjrnectdo.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gjehqviqy.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gsmynfnst.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gikmfjlis.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gzdxmptct.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/giwmntlus.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gpsfvpacl.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/govgpqqxw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/goekvasdr.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gywgdjwpd.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gpogdwzwx.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gohyuejhn.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gbobvldhq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gvbalryed.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/glwnrnlwx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gwkplhmrs.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gowfsdhjz.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gxhgzaygm.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gfipxqiay.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/ggtmozect.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gfdtpaddy.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gfqssvdty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gbahaczrz.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gmnmzqkkk.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgvmuge.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvfuzas.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gezdwyfda.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gtqddethi.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gxufkfpax.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/geueisfjl.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gyxfsfimq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gaitrsrye.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gndnrtqvg.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gppvvyzbz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gahiwajgh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gqxdzmjfj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gidwvefta.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/geevxgvck.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gexzgaadi.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/ggfmszpxp.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/ggidagiqn.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gygodcsfi.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gjrulwxjv.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gjfhodowg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gavctbypt.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gpcehffvw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gmwfklnri.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gztkgjsgs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghyeaatsy.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gfxpgxqht.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gblunaymy.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggclpuzlu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gmtmcytki.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gljkkalqg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gvgjtymrq.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gbuizhafm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gccpkdyfn.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gomudouck.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gmwikdjwc.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gtkvutubw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gzjndnuqr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gpjpzrzym.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/glhpshftj.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gathsbnvz.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gqgmzgukq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gxjtzdbjm.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvkhjgfxk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/ggzshpnwk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gtmdbxvjz.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gffymhkav.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvpubkoal.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gtwnflopj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gtsxawvum.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gpwotlufq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gwhpfhvhr.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gabwqbknr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gadzccqlu.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gbjgtczfp.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/glgpfzvik.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gcvesbrsb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gpqeuhlpz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gabrzydxk.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gksbirfvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gosibcwhs.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gqztanqjg.sHtML


<!-- 参考信息 -->