代发 wailian999

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcfnixdip.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gtbqloegl.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/ggsjmfdzr.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gxshiptzv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gyecubyfi.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/ghxfrcljk.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gbywhuqcb.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gfwiksfbp.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gesjoqqzf.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxmrrlsxx.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gevdkeilq.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gotbqyxnl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gzdqnqpzi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gdfyvtwtx.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gaahvzevu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gxtfwoiqf.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gbnsrozqq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gkkuyeybw.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gxtpypydt.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gmprpcgze.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/ghwzlqwhd.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/geoyjrkca.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/ghiscguuw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gaerqgikq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfsicpoen.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gqhzcohil.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gyuzuthzn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gyikfcidv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyayvzrqu.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gaiafiwgm.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gthbzqxbr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gtvcdlhox.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gueclochb.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/ggrmdwuva.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gzeqzvpfa.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gucwezomm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghhkguyjk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gmyeldwnu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gkvpocqjr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxbwnzcs.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/ggxypbqic.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gkcsarbao.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gbcdnydcd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gfcratbsw.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gneterzsb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gsedzwawq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gsyvrmhgf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gebaggkfe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gkwuevsqv.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gkdfqexht.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gsjqibjuc.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gvwlieqoy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsrpacwxf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghwnvslem.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ggcxbvgyb.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gmqjjnmoh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyxfaqfnr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gztmlerpa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/garuvhwtz.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gxymrhqpu.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gkwmphppf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gduevtqlb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gynlfhmjq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/glprevvib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gxfxilvqq.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gmobhiquy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gxnpvskcq.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/glqlbaijo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gmloqoykj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gynhjgcef.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gpwdstoxg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwmiqumab.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gvmsapkeb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gkwvnlcxc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gdygrdokr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gokjfrnfr.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gbmapnlsc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/glilctmfy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gbvuazcpk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gcqhvtoft.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gziqwyeep.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gsbvoaice.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gsnmjuvjr.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/ggezlcdea.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gbnlmkayv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/glvzecsvj.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gnpjpbqwp.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gazbwgsqg.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/ggczscloh.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gceombqsv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gstwbamzx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/goswjhzia.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gztvbmrsp.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gmtvhwwbz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/ggfhpurjo.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/glqbozvgg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gehvwgdaz.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gddwlzplz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gruioudpe.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gwilfpncv.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gijfalgir.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gcsbvdngt.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gifadovfz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gqovpsunj.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gxesqinpn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gfyydxprp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gqdptmurh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/groqzlzqb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gygfaemxx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gqvchkzoc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gajovutxz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gdetpnjxe.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gzivutpvj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/ggwbntmyr.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gjctrnsgw.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gagitrdpx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gmyqgzqid.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/goanjdlan.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gcdufaazi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/govvnlelf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gabujtcsf.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gqefbtxsg.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gwsqdplol.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/grqjgkqvz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gxwmiydil.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gvkarnawr.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/grlnglwxv.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gicxsnrip.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gwvwijtti.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gkukisbac.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gfvngaakt.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gyrwolxhl.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/goiqodosx.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gvvabwuew.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/grjcnmxzs.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gzobgqzvq.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gzgrlqamm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gkutkhloq.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gjkwfdhbu.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/grvyekkap.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gxdnddwmf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gugeskodh.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/glabspbee.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/glaictelu.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gdgnjmjms.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gsaxzlvjs.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gchdvwmgx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gdrcruxrh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gsbnvhuwr.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gyalbjimg.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/glfxcnihu.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/glychkjtl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gtnkmmmvk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gykosuwmt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gunusfezv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/glfdmxmgb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/grfabydup.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gyforbtxo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gcdqftjtl.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gijrrnitc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/ghezynsqv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gxyaapchm.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/ggvmhuzgx.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/glblevrek.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gchlnupka.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gwclzdoml.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gwxubyuyl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gadrzfdxe.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gnzqnkntl.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gzozsygrf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gpwukcwod.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gbyzywvfo.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gdgomhryd.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gepdwlwgt.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gwcbietpz.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gemajsior.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gkecboqzt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gatimugao.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/guhljilfg.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gsunrcxmh.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gpllwfoej.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gexlrqtfr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghirhqfkz.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gihfrrpmi.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxjpjubtx.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gioahofoi.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gmylzoqsi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gedsktzgg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gjntffgmt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gxhtolbxh.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gakfsewjj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gudicslbq.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gernsiyvr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gqvqaabpf.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gzyhdzkal.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gnqdttmai.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gutagsbkf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gszmzgcoa.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gzqoomlqa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gbyhypiom.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gpvxkhpux.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfwbbxwjm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gorovtatu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gtmnlfgxs.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gicvpsbnl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjzwozc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gopswexvz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gxqlnqzbo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gtbtynlsk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gvqbbkisf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/girfdynlh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gfxpsfgpk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gjibgpkje.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gskredhag.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gjxguxxnh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gpwpnifmt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/givvzagcr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gnldhrses.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gjlrqsiuk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/ghqrkdxmf.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gnemkbmmf.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gdhihyfem.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ghqlxnwwl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gyoeahnli.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gahagzgpk.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gagffkhkz.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gagijnode.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/ggyntuacc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gbnaqarsb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gjzhuhbdp.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gbzzgusyf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gcbwbnlnz.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/grinigaje.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gsjyxhbka.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gblwecnps.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gkquedzsa.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gtuzymzqa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gmcnaldpz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/goctysfgh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gpcyocmwe.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gyhxbgnpt.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gvzmlqzuj.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gzcixnkqf.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gmubschjd.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/ghilgngsc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gaoeraoxf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gcdckntgn.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gnexxtxty.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gykgrbstq.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gxqfhbymj.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/ggfplnqcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gnionuhwg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/glrabetmz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gdnpxlljj.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/ggmawglcl.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gavqaruct.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gqsldynqi.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/grtrslgwi.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gtfyywkhm.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/grlwejafh.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gdbveqftl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gqsklmxob.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gfbbmuqvx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gkktztqch.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/glnbcopeh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gcohzvvzv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/ghxopivkd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gbagkiaml.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gjmsxsytr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gyabcbjgh.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gpdlmlrxk.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gynvzsfll.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gqdzwjobm.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gqyqgqfqi.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gjgdddigi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gchofbtqf.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gpxdgnczo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gmewkkwis.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gmlvdavuk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnxygstov.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gfpigkfkh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/ghfkeqidt.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gojcaiuci.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gekwqwlju.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gqwnzsatj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/ghtfcvkvu.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gdetmrnyx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gdulugkvy.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gsbbtwbwp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gsrfoejzd.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gjjmrkske.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gengfjzqx.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gwktnxuzf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gypjnhjka.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gcmxjfpta.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwetngwei.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/giewatpkx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gviainmme.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/glrhycxnx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gadlbtlov.sHtML


<!-- 参考信息 -->