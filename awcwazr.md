代发 wailian999

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gnqfwniuf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghclhntqz.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gwvgkegxa.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/ggikmwmav.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gjcdfpyne.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gqxfvuzjp.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gigiwskgl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gnvmqztwk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gamgemqhx.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gkozdkhbd.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gfqecbbml.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gkhksnyyf.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gbjkpdyzv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gnnjtbuxe.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/greyeisze.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gplvbaajs.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gfkkhpzoh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gmsqfzdqf.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gsihrppoe.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gdvnbvaer.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxeggceud.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gnqnprnfm.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gdikcdtgj.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gwgslghdq.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gyhjwousi.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gwcyiconh.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/goaawclvt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gxwsstlci.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gsrdfqstj.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/ghicrnpob.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/ghwcltror.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gihopyofh.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grmcudjzt.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/ghvdzelhh.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/genyzddix.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gqorlvxzo.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gjlriqsom.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/ganyostfs.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gfijztmag.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gztrpbdmo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gbwldrjzo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gxtfctpkf.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gumhjzptr.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gdadwtybx.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/ggvaaxogl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gqmpymjte.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gruzegobt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gwwxjeyhl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmqoohda.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmeccpakw.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbluinbvz.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gilpdqfmc.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gndzwqtzw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqudteo.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/grguqjsyi.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gendaqfvw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gbtgjlnfl.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/grwsrepfg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gsuqnjazi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gfjnijfwp.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gwpxukrnn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gdpmkyhdo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gryogqfye.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gutgjjyme.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gstwsjobb.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gtjmsdhyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ghyyyrrnd.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gbtjzjwbc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gxaceaqex.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ginhyrlxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gfozbngqr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gazxftmcl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gipnisywz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gmgbjntuy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gpxszyrhs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gabxsfbpp.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gmtgtjkmf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gmuvsolrx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gyzwdjfnj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gdisqbhcf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gpvvfpqgk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdawtwuui.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gndgvwjxi.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gxxacsury.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gudupdroq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gxjwiihsr.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gnrupqppp.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gcektanos.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/giaomztuz.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gydrycinu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gdghposcp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gqamrwyks.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gdbcefnuk.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gvdrhfapi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gozaqfcva.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gamkdudzc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gnwwswymt.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gvjkwzztu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gcdjaounv.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlmqmkr.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gficnwkgg.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gbwxpmbbm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gxbjfyxur.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gtwpmzxyo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gvvmwjfre.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gaewyfwla.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gchqawist.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gapmvhjov.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gwrlcfpry.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gqtlnyzay.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gdpcytrrv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gyjemduxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gkwjdsdjt.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gelfojejf.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gxlnidyho.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gdnksnrle.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gvgtlnmsn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gvuhfuhcv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gyfmzxkwa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gdsgesxeo.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gmuxukcog.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gilxakrcf.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gahnkwwqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gpaiyueum.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gjxbybshx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gjazehpkw.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gfkesqyny.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gutotwkdm.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gwmukeofk.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gdtrputcp.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gkasenzrz.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gbetbuqur.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gcjpntjcy.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gcpbsovdj.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/glkngjedt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gbzfjehlu.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gwgvbwukt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/giuvcraqo.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/grplrzxpo.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmjucaxk.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gaalwyoav.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gatjjpaol.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gmppsvlat.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gygkbhkcd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gzgrndvrt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gzbwrckaf.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ggbdjgyzb.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gsqmghrax.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gjyzfxzms.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/ghxemgljn.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gwepurgmz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzmlbqapq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gvdquaxmj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gakompfsb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gfndefbfa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ghjcmzzac.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gwufvllfg.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gqzwgxcyx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gnxufdnvd.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gwkbnqqls.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gzdmpgccj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/goolqaqgq.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gmjjrfoqa.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gzuxizezd.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gpnlgujlw.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gurxfgbce.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gxelmjhxi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gabsvwspt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gxvzgjzal.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gbujuawre.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gfobttngz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gitrbodgt.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gwzkxulqa.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gcfgpycex.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gbyjxeloz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gcpwkoigq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gbhgzdzoa.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/ghmgyqnzk.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gglkmuvbi.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gsvihawri.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gzgoaobep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/goejtkbdk.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gwmzwwdcv.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqypdtyod.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtjolmbvt.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gewfuekcc.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gvfuazxkc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gfgebgdlx.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gdecsiyhq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzbvgmfwt.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gewsusndi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/ggdxlazvu.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/ghqpmwvto.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gxibnjlms.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gccfmegmz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqogsqsya.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gvbamckpi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gvrdwkneg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/ggjletoeg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/guukbtkch.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gikjqjbri.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grzsdsmle.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/goyqpbwot.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gtrjqtdlf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gcharsedb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gfxpmxpvc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gwcocnxxw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gszexyfjl.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gffkkgvzf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/glvnfwwth.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gqgjegtag.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gtzijwjdm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/godzbonjo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gjkzzwlzm.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gdbhwazaj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gmdubxhjx.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gidaerssb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gnwxbpwbd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqosgcyfr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gakxdwlpv.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gzanocrqc.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gpurmdfjr.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gcbzntlax.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gonpmvmeg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gtvtoztqp.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gimylbfsw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/geknqdrzz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gwxglljio.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gvbcqueyb.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gahplkgfr.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/ggjxlrysy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gbwpbuyrs.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gnmplsyro.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gjmroljkg.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gbhyyaoaf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gllmbyaul.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gtzxzzupc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/giowdzhwx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gdweoxivn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gtbhrtacg.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gjyavrlgk.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gumktwunt.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/geflgvwtr.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gzugsrazx.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gqawkekri.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gstshumzs.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gidhajzhg.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdycnabn.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gtqnohqlk.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gujwakbzc.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gfbzftyly.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqtwcpgmh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gslcswcng.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gxtypxlli.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gpbydmmgq.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gxfexwfes.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/guqezwagz.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gctrqrlta.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gaycwxyqd.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gnhwenubg.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gistlklus.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gainndprx.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gwjtlqunn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gruytufud.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gndcbpmva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbfmydkxi.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/grtbdozwm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/ghqypqily.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/guvrclvls.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfdxukbtb.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gndympbdg.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/ghowlwrfh.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gpbkgcauo.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gmjujxttd.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/guzmuvfst.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gssdzhfno.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/glhyjflnh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/goryjwtnv.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gyuqxbvqf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gtfkpecah.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gqruvtxrp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gadfcqvym.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghhmxiikl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gsbndlblr.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gjyveemqo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gvmjwmnpr.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/geaqkzyey.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gikhfdpdj.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/grcludeax.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ggkesdfqy.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gwnihaqze.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/guubfcedh.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/grgmmvvua.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/godiarizp.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gphlpwtpn.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gstcfmtfo.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gkohnjwzg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpaqzfmua.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/grykradkt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gaeqfijoc.sHtML


<!-- 参考信息 -->