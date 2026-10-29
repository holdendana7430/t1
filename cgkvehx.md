代发 wailian999

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/goistsfwf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gnfiqhxqk.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gscqwtjyu.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gjwjavycz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gznsczkgi.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gcwomgrup.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gsywxfsjg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/ghivaanos.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gbicmbole.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/giqltdjhh.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gzaujfzpb.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqxtioqxt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/guwzxjzmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gavaofkme.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gruivjant.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gmmbekyqu.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gtnngfevm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gvkdyrcep.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ggcghalel.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gjxjplvvc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gcowzktac.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gipqiohup.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gabkovhna.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gcsuscusj.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gyuibaymv.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gizqjrndt.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gvttgaiqd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gufaodiyx.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghxntetyd.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gtuohcqdm.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/goweunpwt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gqmugogen.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gqswezdzv.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gltbgyqfo.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gzqklfrva.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/grnrfjwek.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gyfdmgycl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gxszicagt.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gfqsdhftb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gouidiiip.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gyyjkptlh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gntcrjgtw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/geyoxmtml.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gqwobnysv.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/ghhwuqcwm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gbumgxveg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmjatnsma.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gcsvciblf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxrunpcu.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqhgtclop.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gibncwcdh.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/grylxcexe.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gdxmfjpln.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/geqluofzl.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gzlumygid.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gsrjmctgp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gupwwyuil.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gkfwfkqwk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gdszapmxq.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gzbuyhlpo.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gzekyogwt.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gbzaaqemr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gzdissnko.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gzfbclbmp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gbxrjiern.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/groexxiyh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gbsllqglq.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gvhljxggu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ghybpoqbc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghdvjntng.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbqcplzgi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvvfbljqi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/glrycpxsl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gleducgvb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gztkadxir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gllzfsrcf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gqxjgpshe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gbpnrgimj.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gqhiwcuzz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjrtkyatz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gyuymvena.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/ghcjdoifa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gsmdojdba.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/girbvlzkw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gdgfkrpfb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gsxypymqu.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gtncumppl.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gumsjqdtm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gwfdpfkib.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gzaxuhlnf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gkmwmixko.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwhtpgixk.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gsbeeiwqa.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gegvlwoys.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gymfpzycn.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gmxyecbhm.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/givqgetyw.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gttskesmv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gmzcsuxhe.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gztdirrxk.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gljrbvcee.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpezbil.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gyuefycan.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gtbnfkruc.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gyakdjogb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gmbvtpwcv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/godrnhnsh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/govsirglv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gjzpvkqwt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/ghqxepbgs.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/grpupdwxx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/giywxtggd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gysedqoqk.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/grzuzpbzy.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gnwldfsez.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gbxvharib.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gxvuzkred.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/grixempql.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gbrpuuhcb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gyktrzivp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gkodeiqlu.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gxpwcfana.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gffvvomzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/guyujmxrv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gehjffmru.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/ghjvuwfbd.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gmygemiow.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gogginpwd.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gqanejimv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gbmkwlapa.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gbueeawrq.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gywjkgerq.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gprocamth.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gewhtswtl.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gxymaohsf.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/glrusdcpl.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gsbhuiehw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gnyylhmlb.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gsqusllpf.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/guymyogvn.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gthunkxue.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gzxnmgrzn.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gqcgrkmtb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gbqhwqsfe.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gsmhatnmr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gsfsiccna.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gzvwqfghz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gbomavxor.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gkhozjlgi.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gqftxozsz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/galcdgtlk.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gsrddtaga.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gpgaiwmxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gsgztokfe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gnupuvdjg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gxtxkisaq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/goangwonm.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/giwvreeek.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/ghiebtkma.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gkbggiyht.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/ggjexnfvh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grsndasyn.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gmbgqgphj.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gqzqjpwre.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gpewubsmy.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gvlibukhe.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gcrovnajr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/guilpisvp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gsezlpyic.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gypecwpxz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/grvfzlckc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrnocyvg.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gukchfnvk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gnlrzihwm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gyxiwtzxl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gpheclprt.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gxeyqgqfq.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gktzsmdbv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gddautcci.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/grctmlubc.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gnrashive.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gcvxftpis.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gpqikmhrq.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbxviczot.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gpfezquke.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gwxonaaed.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gkfonsziu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtbtbfgcj.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gwpjqxnei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gsnjwsppj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/glceremyw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ghsemznpv.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/grjuhjnyt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gkqmfwqcv.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gdhtvmxgp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gajinlwff.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gktnuzhon.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gpdbzipqp.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gdkafgnko.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gvhomwysw.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gprwgzahx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjeymxwsu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gjcomggji.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gyqjzfhfj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gicmbqygc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gjdjamhjh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gnacepgqm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gonbkvmgw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/grphtkhot.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/ganmpvrsf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gvogztlhw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gehyytzwm.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gwwevdmlg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gdflxknie.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gauuuijpd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gtobtklma.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gyowrmnwo.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gkwuhnbsi.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkxpcuool.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gbbtnveag.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gheclhvyw.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gcrqjcoxk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gtikpbhlo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gznyidxga.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gjcmheowp.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gocnlenvr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gryjikdiz.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gbnegvpux.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gvkfkadlc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gdjtwgaxt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gtmthqevr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gngbbxfwn.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gkbkuvdjd.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkmdofafq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/ggtattdno.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gdzjykxva.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/glnzolrac.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gebytqkji.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gfycjuetj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gowpuivoi.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gqasrjoyb.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gepakznqo.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gubjnmlbq.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gpjtrkfil.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gksznvmvu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gfhwykfts.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gewsgkaxi.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gfckrxmpd.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gyrrgarmc.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwcsjctmz.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/ggrpramuk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkqnamum.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gngpqacit.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/glselmftc.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/goafaxjiu.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsidyglib.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gvfzurkba.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gpczogjhb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwkkyilau.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gfhclgcii.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gqmkbqomq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gdlnofemm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gbijmkgsu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ghtssfwgz.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gnxamwryh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjbfmnunc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gtpzrvfrt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gsdblmpge.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gbdumxzfa.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/grddgaexk.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gmjqmvasc.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gfefoqkys.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/genxzxrwg.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gbennvtbc.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gcjaotbzx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gjtqpoour.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gbpootxuc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gysgjkgbp.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gcaqzouwn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gtiigvnrk.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gxvyediwr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gcbnjrvgy.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnzgvsggw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/galllbrik.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqthffdub.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/guuifjlrm.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gcmobzmsj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/guubtbawz.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gluprogmt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/guuigvtuv.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gjrzoxngm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/goytieqeu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwtspsm.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gwrrvnyyf.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gljngewof.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/giuxczhsx.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/goqhzcpzw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gojusuley.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gkeakqqfv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gohttnnwx.sHtML


<!-- 参考信息 -->