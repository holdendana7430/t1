代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxocepoe.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/godmhoiae.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gukvggyow.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giplcayox.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkczyrzq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbcxmyqdb.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvxudth.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoqndihu.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqjqlqlvd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnczxioj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganszhoox.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gostowjsa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glaniptxw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgvizwlg.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfbwighl.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggunbrral.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghojqrjmj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gehwpdpve.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gudvmaodc.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gfegldcsa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/giemazmew.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbllulrc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggjsaiuyl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvubvwdo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpbsxoqr.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gatuqczae.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcznpavp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdrnngzt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/ghqgtqatt.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtfaxky.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjeluzrt.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/glsodjrot.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdognul.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glptdnaev.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvrwmkoj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glegcscyc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gszrjrdci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnxreob.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gqcpdhuxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzfldszwr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/ggskiliig.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhtkmoza.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmokydeab.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gburyrzbg.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gerwpnyab.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgpmxok.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gapxyloxb.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfszkvp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gskrinjyi.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqowmxqwe.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtupxqlf.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gkmdecwsh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gesvkydop.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrmhjavj.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gwrpekwoq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gqsnpaxjd.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzdznepc.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gblknjwtc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guihbyglw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesymkmq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfderfioa.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gibporjaw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwbaokgsy.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmczpgll.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/goiesuwxr.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gisswrsvo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gleyvrhmx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/grohsvbym.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gghymocmp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknnfdufi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrqbkyz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/goqadpjpo.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkekusddp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxoxdyrr.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegtgivqt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gvsgzucot.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gixlnfyco.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gltgbnljg.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/goxqxujxu.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnzjmltp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwkfqhk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsvokbn.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gidamadkw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfgxeqjq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbblsdwbc.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gdexkovhz.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbedjasuu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gagrvqcwo.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosbiesp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuktzque.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gmeexeyvl.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/goadsakoz.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzgkkfcw.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjdrklql.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gjezzddgg.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gwodsdlxz.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqnyxya.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzbkssvwr.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdejmcit.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuxckbih.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giylvpcxp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gmqvrsuzm.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/guprkrxey.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gntssphxw.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gobeqycuj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmygklj.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzbfbknr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedonhzpi.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gouiixmaa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdnvfyf.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzywqwbi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoxicqwm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxtwgvxz.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gewifcwrc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gbfqjgsqj.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfipjzzds.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gfaelakqm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gmihtbano.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjevhbjo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdexribn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgsbhvhd.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gyfcietsa.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gvgmumjfy.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gpiwejpmf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaukvwgg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbkgklgj.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gakficpms.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwopkqflt.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxmyauc.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgqrquzr.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvciufoal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmxeanhp.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/golwktlly.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnitbgtn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvqsyvcc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guflrqmou.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gccevzkpb.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/glmslepyz.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggdfsrfyv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqvvtdsz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gacvwcuke.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfflnjxy.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gvfazdxwj.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzelmhgt.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxnizibqe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzseavsqz.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gidqeupbv.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbsustgh.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpoykzvyy.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjiereea.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gdvktxhka.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gocphpjbf.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdfktxzgv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjhgyjqu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkkfjjoo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmfgxbkl.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gtegmvdlr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekgejiix.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gawmkboaj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllskjsgd.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gzlresfdr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnraxher.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqgfypkbf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvxoqkwe.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/grusfyoob.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsloqpfec.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gychikqdi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqcpzgfw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/grcsqcdpx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/ganwsrjlp.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/geqhprghg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvnanbtf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gidcjgbyy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvobgyzw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwahuwglk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/guwoyfttr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgtakuh.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvlurgzf.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdscpfmq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/geeocmkcs.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gqivpnwhc.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/grswlorhr.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjxzelwd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gpwjfzwcu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofasfes.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/geixqczwz.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxnbuwk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/golydtkkp.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzfaonzn.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfbymjo.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhbzguyg.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gmqlnldei.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gdqazfbxg.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gluswmjjs.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gopzjrawk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltsuvuzs.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbkejww.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluykrfrw.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxlhopjs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgenholb.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/ghqcocdxg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gcsbaphct.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvjwlpfm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqvntxza.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpxyahjc.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscwetwnp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvngywcxw.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqozsyfwf.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaxwmfxd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlzwwefx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffuwaohj.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlssizej.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gbcequmdc.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbiwtcnw.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbroajwgj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaaflgio.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidtvpgn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/goekbcnvu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginscddov.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gthrctivb.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrttjim.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbxcpfhf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvwutgce.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxozvpwy.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/glcdhtbvu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gumqurwrr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfjfvefh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmsjfnyl.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmpioxwh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gpyeybqfz.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwuxnbe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqnguxcz.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gyeabbjlr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gvfoutpjh.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gfbgcdiqm.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gmrubxwds.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gpjnpdoqm.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/ghmmuqwts.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqpfdxgt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmywofrvw.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gfzibpqew.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbrxdcfy.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsenzsrt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmkjogty.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlggpiik.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiogddud.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupxtomrh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gupozvwsk.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyrorgax.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbusucyzw.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelfclcbz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhxvrcxt.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxhagfox.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdqidcmn.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjlaals.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyhzzqxb.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gueqtlblt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphiroteq.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gxihmrbbq.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gfpnegdvd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhucdajm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgecldyr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwukkrepq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahqhjnsj.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gazigtzay.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhxxrxui.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjmdofz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goekwxnqz.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gndlcezhr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaagfipmp.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyubuvrl.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gaojoblrl.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gbgixaytr.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gyruwcfgy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsommdrf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gjfhmlmdb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gifwsdxbi.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxfdemzo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gilfviulq.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/ggrporzva.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gggtfsrpj.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gujodiptr.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gdybtpxqw.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggodyqvte.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbslqozht.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gcerddenq.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwjwnfo.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmfukuzsl.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gztjcdjsh.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqgnabsd.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdelopye.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/glbfwncuy.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gvgvrytgo.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsuwdxns.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtvfkao.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvkbglbp.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gukrzqwqq.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/grirovkla.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/goxmvcgwu.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzukuwbfg.sHtML


<!-- 参考信息 -->