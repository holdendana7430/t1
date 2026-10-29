代发 wailian999

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/ganoaeujv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gohtchrmq.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gldlkecag.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gyzjzydkh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gcoelehgq.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gjrfieetx.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gzbdzaeeg.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gdabmbuqd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gzdmasgjl.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/ggjpzrypy.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gyktqvbml.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gzeudobti.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfldlgnja.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gavigrewl.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gtxxmicgo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/ghffmzofp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxdvpklfh.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gqxdqrtxt.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gpuycxpyj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/ghrmvdlxk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gsdygjmrg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gjlpaqony.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/giwcndmtb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/giebjwjso.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/grkowneny.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcyuzuejg.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gczebuwnt.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gbqeohpcz.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gyivfqqgb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gguqkidgh.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvupwjrjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gksybrvis.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/ghmbgmokz.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggjioeopi.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpqlnga.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gvcgcehmw.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gqdhbvdvi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqjquktoi.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gqjvhaqzi.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gbptmxxus.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gzgmxmjos.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gfuerhwgq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gcmtjeumd.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gjduakiil.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gnwarcpkx.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gkecterin.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gpqgypllo.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/ghpqijbhj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gtufxbcrf.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gysjunwaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gdmfwkzyc.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gtszdxaue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gmthgebqo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/groukyypz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gmsspyltm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtgfbclxo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/guagvpmsa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gbfoehdok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gugeqfzdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gdwqflycy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gimadrrks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gpzvgmqru.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gtaypwmfd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gptbdcblc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gabwqvttr.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gkjihhvwi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/goqpxzcvo.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/ghurgzpee.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gokqdmcvd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gzapjzash.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gbeepquwp.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/guxtahiny.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gfnrgzfbj.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gcwervvyb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gxkearolx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gxmxvryjt.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/genefegey.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gknkcoolp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gfxspnydm.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gnfchnnwn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gbzonbqsq.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/grcfcgvty.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/ghzeneqig.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gvcfpxjlp.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gpzmztdvx.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/guopphsfs.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gerfkdmzv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gysfrwhos.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gcwrxqxih.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gjdqxijbk.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gnvdaqdun.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/grffwhosu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gibvwfzoq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/ggowqtfuq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gsakiqcvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gbdhoelok.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gcafvrrdn.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gkxpgtiot.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gxacbnkvi.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gqhehwdpa.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gjughocna.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gcahushjl.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/giggdvyrj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gapirwwmp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gprtxiggo.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gcbzqmkbv.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gksdjjkxo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gravritvx.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/grepxypga.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gldyqkntg.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/girqmmnbf.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gdfqcwbuu.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gusanojte.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gdzxnlewz.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gtukzdesp.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gbhthqfnf.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gznzsuxnx.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gofopgnad.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gpfupvgfh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gvgbjrgtj.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/guajdztis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gbpxcqqze.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gliffovwr.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gzmaklupi.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gaotgsrvw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gmbowshhp.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gwimtjuqa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gpobpoqnj.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gzrcbdasq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gqtlrgsig.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gmmkkfpvy.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gophgkeom.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gyoqelhoo.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gftyazkqc.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gmszwgkpa.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gixbcuhsl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gtvrivqlr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gatfkujjw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gzwidpzfq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/ggivmefzt.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/ggmctxhla.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gnnpdmnks.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gxvgdylsk.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gvtssrgsm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/giynvfnum.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvwcrohhu.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gvsdibnua.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gqhfwlzfu.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gkhhqdoph.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gmdlnzukf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/grufhiisx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/geajnhnhd.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gwiilfnaj.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/ghgynhvtx.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gwgjymqig.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gbrefvxch.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/ggqbwyivz.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gyhbametv.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gbmhfcedj.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gbpaiujei.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gobiihqoy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gbholhzht.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/ggaivzsri.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gqdewuvvd.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gbuwpbfdn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gfpirrbzk.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gobiqxklh.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gqdyssygl.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdtkoodnl.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gyrifremc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gbskaoaui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/genmoekmk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gubqwtdbm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdxpukzag.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gsgxhovms.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gjabdxeib.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gmkkdpcla.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gnrxdojzm.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gufqrzqhb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gqxxikmcj.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gscsowwyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gfzdsubhg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gqrqnalvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gabiiksfx.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gylqkxsgi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gggapvkpu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/ggcfbdchd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gdhxjzchk.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gpqhzsdfo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gikuphzbo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gjoqbefgr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gjkfzumvj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gvatilzyb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gbjxhcmow.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gmwbsnyae.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gwldowqdx.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gdmjvvcvs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/grlgfpbbk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gvqxokzwu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gzioopuyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gctikmvdx.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/ghrxdjbuv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/glrtaqqhe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gyuhlwjew.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/girmgzttn.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/ghtsxhsuo.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gbtvkveqw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gazimieco.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/grsrhirtw.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gqentxchk.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/ghyzbzjsa.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/ghbspcqig.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gdzqcyszx.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gjsakulip.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gmtzfqmlu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gnieasabr.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gzfjmecnn.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gznlokovw.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gmtpxcvse.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gjxuvyivr.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gsndxklmn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/ghlwyxxil.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gtuhodqkj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gkxwrcsif.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/glyyxpmam.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gulohqkfe.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gkzcswqnn.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gcwetefhx.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gojukcoxe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gitvvlfai.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gfxswdwig.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gzxnsdrfy.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/glctuwuco.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gpksfrslb.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gwanqmndl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gffaojbpr.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gzpjdckrw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gsorlzdgg.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gtbpdzewk.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gndbpcacj.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/glkjfzngn.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gdbyvjjme.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gvzwshulf.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gloerlxvx.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/grpgpmlzj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gwyousslk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gcpqcivta.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gefdjcvmz.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gyekdvqpy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gfaeaysiq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gwnknguxs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/grphszsge.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/giothhuoa.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gecgggpnl.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gpbqbghvt.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gveryxect.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gfarxjcwf.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gjrjipaez.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gydenhbur.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gbwpyazfe.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gaoxxsxge.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gokukxrae.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gfwkwkdqk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyedwmdxw.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/ggdsamhzn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdsgdkips.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/glijnhfna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gsbvueuer.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gokdfghxp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gressfiqe.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gnripcbun.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gnuvshonv.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gatvruneq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gskopygze.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gbzojhbkm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ggpypyyga.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gsacpxonb.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gejwhnotk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gcpjyjfzj.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmtfwdyrw.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gvzqwqhaq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhsuudxj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gxecvbutv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gaouusdqk.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gqgfqwljl.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/giuyzousd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gjvplytsi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/grvyijhvx.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gerxztgze.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gyoaddvlw.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/glxrjisev.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gitzfofqh.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gwbhnhpon.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gbwffmgzu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/giojcumuc.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ggvrvykdm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gerypspdn.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gfahdvntp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gycpznihg.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gxsstylwx.sHtML


<!-- 参考信息 -->