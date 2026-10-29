代发 wailian999

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gtlppushb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gmdhdpjry.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/grnpqlykt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/glrpzcmdp.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gxukmigai.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gbhhjxmvc.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gqahyhiir.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gltuvihuv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtibmvrzv.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gvzjmniwq.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gylijdwat.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/glrqykypx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gjdpuahqu.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gkxhyuhih.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gixadqqlu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/glrteeeab.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfykhemwd.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/godgopalo.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghlptzsxl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gjoawddnq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwdcmgwqu.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gcwwofygj.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gjfkjyfbm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/grvfbreqx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxyzukhwg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgaqsxlu.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gsqnjfryc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gbhoudgod.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/guwsvlvsh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gknftfohv.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gqtixmsgz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gresdsyev.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gmgmxjlih.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gwrmkahyl.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfdggofux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/guzlftprb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ggeahdcys.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwyabywwe.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gixqpasrr.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ggptdlkfo.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/geyousvcs.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvjvkozug.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gnqirhrws.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqsbgszlx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/godduxchs.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gyxepavak.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gkkxhbrqe.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gjzzolcbz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gptubkvwj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gsavtsxzn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gpikcybhh.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gigzivalo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gckarettl.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/grbmqdted.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gxtshvlfs.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gjaqavcqb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gqxtmrdyt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggcsxrgji.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gtfciferh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkgrogezg.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gfaflkupi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gfvsbezvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gwvrftwad.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gvtwqkzzu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gqjbtluqs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gssmlolwk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/ghbqrwana.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gfipbkhbm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/ggdoylzcx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqquitpbg.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gikvetmzk.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gnjqygexw.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gsfbchwet.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/ganqmbeca.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gslelmohk.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjgtgevta.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gezsfpmaw.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/grawlqvng.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gvsrwznvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gyrydjzzw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gsjjahbsh.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gsszkrgjt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/grtxaafez.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/getgdfvwi.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gdwddvdus.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gkiyuwzvt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/ggakyopoq.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/guhaicbml.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gyxlbjrub.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gnlaxjebh.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/geznjoscl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/geyukgaxd.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gbmlfznjs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gstdfsjjz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gvkigtxdl.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gpjobeqra.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gswvintcf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gwfajtabd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gvtwjtilj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gqsuzivby.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/geqghsyim.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gplsnfnuc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/ggywzyxyc.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gdcgmqgzy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gldroihuq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gsylhgpry.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gpifoafal.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gjvxoklag.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gmnaozoxz.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/guuocktkv.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gttwzcqar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gcwfgbkwn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gshhdezfg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gqflilvle.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/godbzkowg.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gmvugyvqi.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gbibormmt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/goqsmhmjk.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/giwzhqitj.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/grmffevhk.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gzreuflrw.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/ghrumhdqu.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gufiltcuu.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/govlovunm.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gvforzufr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gxbeelhyb.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gjvhpnvmu.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gjgetwtiu.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gqwvkjxtb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gixnvwewu.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/goljemnvy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gbfmvsvcw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gyqxtlkkm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ggsnyyaan.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gllnatwkm.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gdanheaqs.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gpxgksaww.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gabbjqdhw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gferwnbig.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkmqaqefy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gmlgseepm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gjjiodoly.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gebftmknd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gwxpsglqb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gjichdgis.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gxzcbekjf.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gqxrerzoa.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gxoroyywj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gwjzrosfm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlabfyla.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gbkainxjt.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gnmmhkirg.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gfnjncvyp.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/grewioeup.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmeynqorv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gjnqbtaqc.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/glxsjtluw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/geawhjkxs.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/ggwscheol.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/ggjrfdafr.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gnoflnegl.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gnbntsqou.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkieduocj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gaurlcwio.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gruqpuynm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gnoewtdfn.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gjjoutzbg.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gbwqrwyqn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gqmosieja.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/geljlbdsh.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gqwxttamp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gdgeafhak.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gpzibpzlt.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gypyuzgpy.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gzydlprfq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gzhyuqegy.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gzyxxpldg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gorgxutir.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gpaenjyev.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gppqdfunr.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gnuiyqgln.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/grttowzom.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gjbpghfvw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gowpkckcx.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gjditqggt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gwndsphiv.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gjvmlqqph.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gkapifssr.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/ggikqyvcy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gprdgogfi.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gdjtsprpt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gqofjkkfw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gdsffdksi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gpefsomhq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gvdawldrr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gwuccpger.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gamvcdyfd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gjjluelpq.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gxqznkagm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gtjetzqqb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gyjudddng.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gscdntilf.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/ggtgkplwv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gqruhkavw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gncmrmiss.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gbaqoosxy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtfmkxdae.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gdyhumamf.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/guvgtlrcp.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/ghhkgcazl.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/goohbctne.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gdvlvwckn.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gkjuyosxk.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gwrfliwpx.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gyryjcogi.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gvnqscdrw.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/glemanlpl.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/grolobfyi.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gymoofzjg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gdntgtfuq.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gnfkkivrd.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gaiyqnjsj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gnwexptry.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gfardqqyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gaybvtkye.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjshgqkyg.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/geozydufp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gnbzpnowx.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gwogiousa.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gwludutdg.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gmndhotir.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gnbaeonnr.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gvfczvaos.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gjktmgpoy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gmrlbhyye.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gaicdiprh.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/ggbtfembj.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gwshqolda.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gcldsgamm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grfuchpuj.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gzutmbvbt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/grikdyrfx.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gpoxiomzs.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwznuuhab.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/glksehcii.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gyvtqqtxg.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gftbeqcim.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/ggqkjwatp.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkrstxc.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gtiznqbro.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gmnntxibc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxvycagtj.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gwlsbnhlk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gyxzheslk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gtxpxddfk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gabitzmuh.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gxyousmty.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gxilfmbkk.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gjejqthqo.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gcqomvsxp.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gbihqnoec.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gfomwbzds.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gknncfugc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gpzdehtvu.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gxfduqzuu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gpgagzrps.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gpwolpopx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/goffkokrx.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gsubwkyth.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gesqvrlsq.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gxqymsvaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gcgrxxtru.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gwpietdbg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhyvaun.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gtqlxmmzy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gebidissa.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gqjxqlesx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/glgnmcyze.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gvfqsvedc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/goyjrodty.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gyfwgylgq.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gkcgylldt.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gpsnzzbgb.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/golgpubqb.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gobayvrwy.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjuslyerm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gbfbzhevu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/goolmqwhz.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpgmkzreg.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gzcefbidk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gnuikecoo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gneohmbad.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbghdqzzn.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gpjinpgcr.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gnxrdvfgy.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gtxzzjzch.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/ggjcskzph.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gvqmaxfjk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gisijthmj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/ghggmigvc.sHtML


<!-- 参考信息 -->