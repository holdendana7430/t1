代发 wailian999

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghtprtqwy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/glauroaun.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gpouspsze.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gqffkjrzy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpfrfeeyf.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gfarokfeb.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gawwjimdv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gknzetedy.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyfdinixt.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gaariazof.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gesyakqal.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gbewspdle.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/geztxngqu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gmozrurrz.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gpnxyyevq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gcograbnj.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gbyqvodxb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gzwixggip.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gdtnmqttg.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gclwpnsqf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gcembqvxw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gdziglrxd.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gojsomxco.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gihgxtvms.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/grdwrvqxk.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gixpvlbyu.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gvvxgifyv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gfcfyssht.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/grvfixuav.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gmcfqoopw.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gmlyhiiil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/guqszxjxf.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcvickcvn.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gnyyplpai.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gekcvuvqw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gvscrhaux.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gpexscysk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/ghlllfeur.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gfzyhaxbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gwbalkoob.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/goevcijnf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/guhxuwmem.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/ghiqpgmud.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gkxjxcdky.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gxjmvzsuz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gpqmsttvs.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwqftxuny.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gjptsvemg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gwzvmcykm.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gweawenpr.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gieujlyzr.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gvucymnpy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gheqapwgz.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gklkmsgxx.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gytqhobcy.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/geuosmscm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gwimlfdmu.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gszjsldeq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/glycmwvhi.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gjypvfixw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gzlllyhud.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gscgkfrck.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/glbskldov.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gonadjivn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/guqyiwutk.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gqbzlbojm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gqwjnaatv.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gziwetitr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/grszwrmkk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkksutczi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggrfqptfc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdqlghqvk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gubigurtg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gaqtkkkvl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gfgganaal.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gsgnlunte.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gzoyqlgzf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgaibdef.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gtjaxmlgb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gxnecqokn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/glydbtdce.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glqnxqpex.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gtdfjjkyv.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/glpetldsh.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/guzojfxbe.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/ghfilhnmn.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gezrqmqnd.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gsaqahwiz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gwxgahhxt.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/ghwvdjhzg.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/grgljypnt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/grjfdysno.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gpjuavreu.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gxumshqdw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gwitnkjff.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gqnpkgofk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gulxprqoc.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gqsbmwqyt.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gzzprbkij.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gccvkawha.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gldjqlhlh.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gggpewdhg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gkkmxqwvx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gjaktragt.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gshohppta.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gjuamjmwi.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gntcuzpdu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gwjinmcge.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/grmtjwext.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gbrdwgoss.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gkuotyimt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/grykkpbnn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/guhmhoqqy.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gzmyhrwxk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gzefikzdw.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gnthiftbl.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gramtdwjk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/goinwuvzt.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gfugvjdwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/giwbkjnbz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/grvaqimfn.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gezrotyax.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gxrdvxfau.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gpuhgdfkh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gjofddhnk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gjagocjsw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gepfwxmhf.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gynichgog.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gxeyuqejz.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gzkrpvavw.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gmjbdojwc.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gkxuhvtlx.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gnsbzoogt.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gsadyvfjm.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gazynhxme.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gwitfyidk.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gkjxzfiek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gumfazcdz.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/ghwnbmwit.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gfssydobr.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/grykfzkpx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gssftpjmb.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gcxvbfwsn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gwfzdjres.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gnsdvnlug.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gnopwfgze.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gfjogyoff.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gbgmpqatd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gvroyoery.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/grklhbyih.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/godamvzul.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gbwqdggip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gqngclfux.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gtsvkiqav.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/ggyzeuzhc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/golpurwzq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/geajvdhjb.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gwaekmmrf.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gjywbxwaa.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gdakyvwrv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gofgkqlwk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfyxtazsx.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gkudmgfwx.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gnbehljxu.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gxyvsghmw.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gzqcdpcmj.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gsszurssh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gyqyyvwjp.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gxjiwzqvm.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/ggfdvgqyr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gwqpvnhso.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gwkbigdym.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/grvutspau.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gloggpzht.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfwioytcp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gumewiqba.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gpkmsvjec.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/ghwbpefae.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/ghuygimpj.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gzjkfprtv.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gljwawprm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gfvanxdmd.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gsjwvxqmp.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gebwnayxc.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gjeevzazd.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gkvybfqyg.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gizhbmasc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjezhepur.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gycxzpwxl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grjjzqiqx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/ghnmawdcj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/grexqpraq.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gcwmaybtt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gpvimbcdg.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gcynaexry.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gigxgcprs.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gpuzewypf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gxoyfeyax.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/ghzplehce.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gzqhacngn.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gsxxtotwq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtmgwzhlu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gmlbykvnf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gazhzdylk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gkmmhfpjl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gsidbgocf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gnlhlmjlv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gxxbrhmqt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gnpvqhpan.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gsorizmbl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gxplqrkeg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gdpdzmmwv.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gymkxrrxr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gsbzqvvue.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gdomqkuih.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gderxkmkr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gkoficrhk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gpyqrvblm.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gloncmcua.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ggjukdhmq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gdchpiisl.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gjjaxhgks.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gryaxkvyb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/goaxorchn.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gxfxrzeev.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gniadkzgh.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/glbddsspn.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gpkonobqn.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gxyeusthb.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/ggciqvfbu.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gchubltot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gxczigifq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gsonevrrh.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gxurzsrfy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkdyrba.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gntxkmtrl.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqkuydkgm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gubxcfpds.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gjkxodibl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gvldqzptb.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gpbdxqoij.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/ghxwyjhem.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gyauclecx.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gfaureeab.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/ghpxlktkh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ggnxutrud.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gnrpqidcj.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gxgqyqsvd.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gfurhvwoi.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbakowlun.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/ghipryien.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjehpwyqw.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gryqnnowu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gfdkduuyr.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gbmgjojpz.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gnytlorqx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gebluvvdy.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gbblixpuh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gifoojzdr.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gynybwkid.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gehoqyhcx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gnmeiycba.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/glipqipqg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gqbbdoqlw.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gfkohhmfv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gvteehnvx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gnhppsfsz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gjwoxkcja.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gnrfeqthq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gvcseaidn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdujvvv.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/ghalbcwgz.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gzvodmdrw.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/glnxmupyi.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gulqcnbvq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gdwupypug.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmdnaqa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gyerqrkij.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gvidrbxny.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gchnpsfbq.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gdcecclud.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gtntherhc.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gllkzvljh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gyjergnhv.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/getmwvhbb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gpspsxjma.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gigcoevof.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gonfzbssz.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gvssulssu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gentlkdrn.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gkbrojukx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gcsvneneq.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gnhwzfudo.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/glhraubeo.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/ggajlmxhw.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gcpoawnlp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gzxhzohgf.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glxvyksak.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gzfeujido.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gcjipqpqc.sHtML


<!-- 参考信息 -->