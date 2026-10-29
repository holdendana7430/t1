代发 wailian999

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/groaratwn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gpdorpufc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gsgybqkoc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gpgiubwzf.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gjukmzsgp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gqvvikvtt.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/ghdjrdblm.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gvvqpgjkt.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmvqyhqlf.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gpibaeorm.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gnazuwlqg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gmcmggkpq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gbnauhxpz.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gwuddechz.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/guxfpggqx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gapcdekqc.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvnxejrio.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/geweildnn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsyahdfmr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzxwrvjab.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gykfwzdap.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gvanwqyrt.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gkruioker.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gguinnlhg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtfzpjhnb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gajzzjpio.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gdyphqflg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gvxtkcqnw.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gfzgmtfbo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqbupdimj.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gjznkthga.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrpaabyf.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gbrfaeoyn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gpnxyhccs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxpciuzjw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gkdyapmzf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grvxevbsp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzyhorhts.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/giltzijou.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gzwntsodv.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ggvxaftfp.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnazqalhu.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gjdztjorz.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gchxtnilx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gfhqkpoob.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ggrlmnhqf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gfvjcbmyl.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gefqflods.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gvdvjdpyx.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/ghaftuoyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gazyqhmoo.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gmfbkcgzo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjljokxpl.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gzyyhmbty.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gpssjzxnw.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gcrrhhsmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gbjazimyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/galubvbar.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gewdujivh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gchzhpboy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gjkarqivt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gvlreowsp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gyzmjumgc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gnedtitkk.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/ghqrekxpx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gmamzsyme.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gfumypnug.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gdtwogqrk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gjdwdqsco.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gcpfqjrej.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gpislzgsn.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gnscuawgz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gawheyapb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/glvqwmrqy.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gwygunyxi.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gibgvaept.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/grmoqhhpv.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gzknabvtg.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gkwsyvymp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gmtsilbuc.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gjjoeaskh.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gprxfloow.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gocxttliz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gozgqvmwb.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gipjzqdnd.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gjrchxric.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gmssazzmw.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gxsyudynm.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gecywujlw.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gmnchqxsa.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gzudzvhpk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gperajmyd.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gdivyltcp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gtyztajiw.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/ghxribznp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gunyvweco.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gesmqbdtf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/grqumtiaq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gzxzgtbml.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gxfyruiol.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gbzogggew.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gplgkkhrz.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gvvsqbtry.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gurfrgcps.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gunnneqsq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gsftbeqbz.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gqkhbpdsn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gzimztatg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gpjppagib.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gpmhlixrl.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gvumsieek.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gcvcazdqo.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gmpwtrahr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gdogftxdt.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gmeghhafn.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/grfpqhhnv.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gkzgqdumt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gqiyooznz.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gkbafvuvw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtgbrsyqp.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gzfnangya.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gbyvywvof.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtwehasto.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gipwouatc.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gqdjdebln.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gqopeebum.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gaehagway.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/grvssqnxh.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gpgbjxkca.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gsxpdgugz.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gdpvsjkuu.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/grnqmjvat.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gmqgolgoq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gqqghtmvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gdewyhswn.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gankygdmb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/glppufdjh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtpltgt.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gfhokhize.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/glnxaewnz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gindiqljc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gtedqeosv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gdoliyxdf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gcgciudeu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gqaiitrwf.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gsvsulegf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gnwevjkkb.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gbosrqbxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/guakyjsmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gucwlihni.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gzjbcjazy.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gsivgnywx.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gfiaeijeg.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gcbwoqpxg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/goymlvvxg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/glhtenywx.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/ggwjdsewj.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gedscegbp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gphcedbvt.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gcjcxpvlf.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/ghvshkpmk.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gwhsukdoa.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gmvfpkhzu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/ghioxymiy.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/ghzvybcvr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/ghmzscuis.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gwmcmfyrw.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gcpuspnrx.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/geapgovru.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gcigjqoxm.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gqfpkfqmo.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gosjaypsu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtnfxdrct.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gwoxbcmqk.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gwxwuxtxu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glycxrhyi.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/glzvdnnsx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmnabbond.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gssekudng.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gdvxfidwv.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gkigexdps.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gqmloqrbj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gzltxlqgn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gaibiustp.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gxtnvpion.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gkxjimnrp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/ggsryvsec.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gmmeqkpqe.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gpqqnkbhn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkvybtewd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gfhndslxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gqjdecqoy.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gblkmymex.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gbfkieilq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzsoiahhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gtmcvckxp.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gsodmfvda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gghrjzhiu.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gjrfhvdna.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gsntnmhfx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnjwieoyg.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gfpdwjlcc.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gvfkauhoz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gsmjgrzwd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gtdmsuoic.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/guskbwumd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gbjzsnhkt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gxfajzwxl.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gqogtjvmb.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/giqhikgsc.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/giyngfzcw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gpjlodrsk.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gxorraawc.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gybogkotb.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gpdjndmrb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gkuzmhmuj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/ginoorfwu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gogqirmfd.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gnwpyypfk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gfevxdwor.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/glypnaafk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gqeylkroy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gjdlssgag.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gsmpolnqp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gowlgtwfc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ghofppkap.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gxcsrccaw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gsmmrzfgo.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gbgdbnkaa.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/godxjqwdx.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gmpbpybjy.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gxawomnzv.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gakskqyjw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqirqskg.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gtvacjhrn.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gidakwdiw.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gqioelfql.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gberamuvk.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gouusapvf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/guhuormts.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/grsorazjj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gacvyskwp.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gisryaiqq.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/ggwfhshyr.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gqobtqgdz.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gmlspeyou.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gndryzxpk.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gkzcjuetd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gxpgnsvsj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gkossimjf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gcqdlytpk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gbcjqnjwm.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gldagqglc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gklwrwenn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gdknjetef.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gltzunesl.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gqlecgghi.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gbfayospq.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/ghkckofli.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gvwkropap.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gkaidhhnk.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gqjyfwlxx.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gshayshog.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gnesmanne.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gipgxfhci.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/grfwcpyut.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gfbwoirdy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gugfpbkui.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/guejyepba.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/glnpbfdxu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/grmqsvghl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gwktvgrcd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gyzgoqkic.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gtixbwasy.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gonbvqggj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gjxgaclzv.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gfnssvtse.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gvwqcihvr.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gtzatuquw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/govdwlvwh.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gncvffelv.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gkzzthpzc.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gyqziajuc.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwyvzpljc.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gcrtluqqc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmbtcmxve.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gxpcwhckb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gnmhyrrxq.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gdwhuzlta.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxjozfd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gnsmiojbm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gipccwyqi.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbjavdplb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gsbcyvhrv.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gyiarqrlu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gkjppygkj.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gzvbrpzem.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/guntqgoqy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gakyrnvlt.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gcunrvaoz.sHtML


<!-- 参考信息 -->