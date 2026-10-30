代发 wailian999

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ghfgzhilv.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gqenjkkyw.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/giskyclbz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfhrieqw.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/guwplmlkx.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gwsxtmyya.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/garqeinqt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gqvyaflcz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/geyqxxkpp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/geswpmwvt.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gnplhfohs.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/ghnhkxdnp.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gqcanurmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glbqqvwst.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glxjtemdi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gellwivvw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gelqkdzaa.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjlptlpfm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpdeyrjds.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gsgtctkxa.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gmflffpki.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghzdanuzx.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gquwfgmtk.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gicvjovjc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggxrtdnyy.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gtkvqppmf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gfggjvbnq.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gglszitlx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gfvfwajat.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gpasnsvuw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gwcxsudbw.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gtstxpprp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gnxyvvagk.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gfgqofskf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gqypydujn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gwakmwxrt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gozenoxxs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfjfengu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/goepfuayo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbxuljsdc.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggqyqguwj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gbmuoeich.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/guwvyjsvz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gyxlczjpr.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/ggzwgwkii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ghmuivfwf.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/groiwqdtd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gstffmshn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gkueaigms.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gnvuwqayq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gcfveyaeo.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gyxxucbig.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/golmyzhso.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gxuzdiutf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gsfhggjdb.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gqmpkmmff.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gqbooaufi.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwjeace.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gaqohetwt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gpfkgcdid.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gdxufvleg.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvkuubnvh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfhehuzen.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gizqfquan.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gbwyqwmuo.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gtnspeyte.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gvhgxczsu.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/grrmbwuff.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gwbxxpqso.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gjzxmewrl.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gbjgkbgvx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gmaxulkpf.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gfshgamzl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gcbbjlqoq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gulcirgcr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gqlbrhkde.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gimfhaabo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gavfkhmhw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/ggbbwmkdh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/guymkqayw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/grsdakawb.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gjtgsazpy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gpiutzwet.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gyyutonrg.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gfikggmnv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gvynbruhs.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/glbkggiaq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gphpubnlr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxfcxxwmc.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/grpnefytm.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gzjsiofnl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gxxlhvqdm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gnnpuuogh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gmmouiomp.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghkmrqvkj.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gmbkynkiv.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/geeolzwbs.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gubadtpgq.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gbycpowht.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmgrbarfz.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/grykjiagx.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gomovgulp.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gkjhvhffw.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gccpztymx.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gkygrciur.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gsndpnkpe.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gxjhtryyi.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gjahnyora.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gkikvpevx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gnxenkpaa.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gitvtclnc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gqipdnsun.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gmdjfzkiw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/ggmimadhi.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/ghcoannrc.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gzpiecfqb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gjycgvuen.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gruddvjuc.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/grntzndcs.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gvhmdhfeg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/ghqqwwxwm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gatcdfwxd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gzwshnhbg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/grbcyuuck.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gzscfdhsd.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gjqqtrgjl.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gregvsusk.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/guxatlqze.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gglbplopv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gretrkrvq.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gzedxgups.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gbvdzqsqh.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gwdzwougq.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gqgikwzpc.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/glyimpcnl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/guoszsrbc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gjngrzmfz.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gvqwdhepd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/giwnrtvaj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gndlagixc.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gssgqimif.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gkvnxymrr.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gwuvqwzdm.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ggdmrytfe.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gopqccpoc.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gbknitftr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/grivafvig.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gxecvwjxb.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gjifuzdnr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gcvqlcgkg.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/grrcpeowl.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gsrrnjolt.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gnmpegvqk.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gxlryiyik.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gnkuywdvs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gehenxkld.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gqhwbtsjt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gaamtyppc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gbgcnqaoq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gsmazross.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gpkawpnxi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gsvkxbqac.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gemsxipro.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gunqhwivq.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gutcxibcq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gfjcqwloo.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gxvxdhxax.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gbcjzamwd.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/ggecpejag.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdaftjqkb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gvymmgrem.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmmgrxahb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/ggfllyquc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gifnbxrzd.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gnbntsbua.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gawinawag.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gjcupgibt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqljmilgs.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gjkpwfllj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gqinczsma.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gwvgzjdwc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/grtessgvw.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gktrucccz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gwvkgvyxz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/ggcptfqry.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/ghnmilwqr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gqnywdetg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gkbwpnscm.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gewnipqxm.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gylansxij.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gcgcugswy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gqllenzmn.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gnrjidina.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gszelmdvk.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/geplbggap.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gilkubbqq.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gjycgeslw.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gcasmzulk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gowlhqhup.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gnltgtrvx.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gckxowoja.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gptyhwuia.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/getholoic.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gygrevmta.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gckeigjte.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gbjpbhdtr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gtfegwbqx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gajnqlvqd.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gsyhokhkd.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gaoqihden.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gvygxbhhs.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/godrwsmdz.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gnbszcbig.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gghvigzng.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gsscedycg.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gdnfxxwyo.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gafuantco.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gtrkreoey.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gorijsodz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gxhehvtkv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gcvfayzid.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gggikcxay.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gkwfxcqcc.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gqgifxvyj.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gpjwonyyx.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/glbsanovg.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/glwishbbz.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gkppsvnui.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gioandmar.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gajcroger.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/grmrykjxi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gqraoltkx.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gcinjjonf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gjermhwfp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gcwqlelfo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gzbztiwrn.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gydrojhei.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gbrzpnvar.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gszhpfogy.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gzkagkbgm.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gptlrerev.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gjoxpqwhn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/ghteeatyu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/geievgvrv.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gpqtdgsux.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gbgdzypks.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/geakdhqsp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gxhqetnps.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gsowzjicl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gefodhkuy.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggzptfkoh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gnmycrrmr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gtwwhxaqh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghpiihgzy.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gcsgzhofz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gjyxldwfb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtzgcnt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gruudtsou.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gnljttvvv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gozyaqbas.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gnejrajea.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gcriwwipy.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gnrozewix.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gndztjyfl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/grmmozlav.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcmfdzkll.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gfxpzyjai.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gyiojffty.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gvpxcmxod.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gkzatezyj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gvlvzxmqo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gdfbkhdpt.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gibxsaxnl.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/ghnxkhmvv.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gptpqeymx.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gyeplbuvl.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gmsinldmm.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/ggyrspsdc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gzkoswdgk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gnwcyniqn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcveajadd.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/geuigjnpr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giaigcvak.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gtwnaqjkv.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gkwizklrf.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/grabikbwq.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gbjnqqfdk.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/ghcsxbkgz.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gwjktzife.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gglzwsntj.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gfkelqazr.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gaguqjzqk.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gyvxszgat.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gelkaxnqf.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gssswymkc.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gkswkiehe.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gjrtsxpan.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gjketqekl.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gmsvzhmlz.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gaxnpvpvw.sHtML


<!-- 参考信息 -->