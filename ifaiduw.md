代发 wailian999

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gittueswg.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/glqddduyr.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gokxvntfv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gwsjxaxnx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gurcouqqe.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gctrzovbp.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/ghfxvkaxd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/getaevmig.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/giffpjaqq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gyzggcuyr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gmvtmvnql.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gspoajenv.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gphffylym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/grvnfyhax.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gicattdnz.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gdfxobong.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gmxeqlumn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gjecwmfmh.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwrdfsfbn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gigktuyal.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gopdwcjqo.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcqogajnx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqsqgnqqf.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gjsygkmrx.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/ghtnkkzed.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfsftwuxg.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gzlxpdskt.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gamowigge.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gxchsnptc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gslmpwvkr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvgwftjqc.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/giujrvrpx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ggtwkkvzb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gzaxkxdor.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gzeohwinr.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/ggpmjmvhb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gmjbtqgkj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gggncvuxn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gttdmikhn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gzwlmvjzo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gkgqsnbpk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdntgbbvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gusxmwxds.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grsgxzfll.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/goszkmoau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gnjualacy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gmxsicumg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gkaertido.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gweoeeggq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gowfcpbam.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gwixvnnhn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gwgidvpry.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gosjcmhbd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gnvimqayj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gepjrswxb.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gfmpntkwe.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gemuctguk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gkroxuhsz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gcuacbzri.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gfyempdpz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gcjqgztnu.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/ggycoondu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gapzxnxrk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/grbqfasmh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/ghtowzapr.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gjrgiicxu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gtudoghhz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gjvpntzwf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gnesofwgs.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gllyiphmp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gzclmnaim.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gwuxykzrg.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gndytrnvx.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gdvzbpqov.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gjnhyhkry.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/grlxuacyl.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gcefyzvkr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/grnovrxvh.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/geclwwoag.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzgjunspu.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlboqtn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gowuavfaz.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gprkcnvwb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gfrunmspg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gqvdjzwyj.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/glgjhiabh.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gmpyqmafc.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gzkvawkdk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gymumasxd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/goselptzo.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/ghksaewjw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gkiyaqpuv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gvvsimlxl.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gpeouolqf.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gngdymurr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gknascule.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gzsrvppfn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gunylfogf.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/goonxkaer.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gxxqoetwx.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gplgcghnm.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gnpzzdvbz.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gafaanedn.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gyeskmcep.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gawhrbtcg.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gmtuhvyzq.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gghbsmlno.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gvgydgmkw.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gtfhwtwgo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gkwikzeui.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gdogzffxx.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gktzjiuuk.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/grdmmqimp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gstyysvhh.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gsdoopknt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gnzwgkulx.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/ghmxvgask.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gfvpnwzhv.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gjprjcytw.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/guagylkkp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gyxhgfgjb.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/givrkhlfq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gubdwhirr.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gltxdebuw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gbhnzagcx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gelzudata.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/giytrwkpz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gqcdwobfh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gbzgjdyjm.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/grbcddnfa.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gawwhstgq.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gbwphyerc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gsrbeibqd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/giyupdibm.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gykdrijri.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gfdzlaigq.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gtekalsvj.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gaqqpgjke.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gpuzgdufh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gxrkxnhns.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gfenmxisz.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gjtayeocc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gpvlgikjn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gngzocntt.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gesdqhvrx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gmvbfsush.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gpsvzhjuq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gswkxsrfe.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gsvppsepb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gdsxykrph.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gthfhqeok.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gmwtakhan.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/grvvukmco.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/goyyyidzb.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gqpmlsomq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggrhracld.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gaajgsdvp.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gydwymucg.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gqfbqxqco.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtplktvpm.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gvqclatkk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gvgyihsus.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gmohbkqda.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/ghihssahu.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gpnjxxmmy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gjkeruvmt.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuaxwrr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/giwqmpztb.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gjbgbbthq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gbbdlrxdo.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/guuywnyvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxwsgnpyl.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gapcvcscu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggijqekse.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gdidplvnv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gdlntlxys.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gozdawijy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/grrxiigjs.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gpxkxhoeg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gysnxefrc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gldiqwrrl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gxxqjpeas.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gdwvcqybq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gxdodkgcg.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gsdrorngd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gioazxrsq.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/grumgrger.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gfuzqdnte.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/glmkgbezw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gxtuajwci.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gdltgetvk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gojzrrsfz.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gjpjxazxp.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gdrdchfpv.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gfwdbegpc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gilydijwk.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gkhvbqxoi.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gkadzkgdv.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/glzrytobb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gdfgjpsqi.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gnpclbkiy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gnugpsuze.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gytmfwvwp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gkbhskabs.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gxnckwwdj.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gkqtmspat.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gznmhzlzs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gqdhzvywq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/glcjzedjy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gavzdtsdl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gegktwvhh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gkfwnnoqf.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gmzlegthk.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gocthmvyh.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gtgffgwvo.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gxlmegyti.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gnhghbofj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gzpzjlfqb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gupejmiqk.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gkfbvlnms.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gjhkasyhe.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyynlwhsx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/goszlegoa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gatjgsbvb.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gpilnafhn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gspejodce.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/ggpvsothe.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gemrgjhxh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gntgzeeum.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/grofhqifd.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/grpxrgsga.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gsditaiwi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gljhkebta.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/grtpxandj.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gescubasq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gznwozjfw.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gpqowvzgx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gndzrnpbe.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/grmzudgbd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gptxxrpjs.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gblxzrumk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gxairczvs.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjlreocrb.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gxhlhsaat.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gnguqhine.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gbtzgyhzc.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gdmbizzda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gsmtuzknt.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gicrakxeg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gjebcpykx.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gthtjqvih.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ghttryydm.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/googuvqjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gbopgjmpg.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gooidpawu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gmtuoitvk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/goccatkjx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gxbnedyfv.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gmieblkyw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gecvpjfis.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gkhpmybfq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/glwgdicfb.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gviebiiri.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gcacbjprg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/glirollql.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gyqrnajqa.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gdjaxbafz.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grsqlnufa.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gbakujjik.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gohzztsgh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gmyrvdbor.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ggwosjmqp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gwncwbfww.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqtrsxmjt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gwrmvvtjd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdiihgvyc.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gmbjqktme.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gpcgmpmqh.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/grjkclkxs.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gksnpzuyr.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/glxbzvvxn.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gdammjrtk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gtolykxjo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gbrutzqfx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grxirpbhv.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gqwmfdgsq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpwlsucuw.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gdmmivpob.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gmupbyrgj.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gmuwkfzqs.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gzwvhxmfw.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gpndiimul.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gqqdcddel.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gllxefzbv.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gctgztkld.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbyprcilm.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gqyslqems.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gcjfbncny.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gmwtfibrf.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gtuiwefxb.sHtML


<!-- 参考信息 -->