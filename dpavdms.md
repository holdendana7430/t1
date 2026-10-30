代发 wailian999

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gyuxsdxrc.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gsaoudkuk.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gfgcflxwi.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gmaeunngg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/giywmdnbj.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gnhivmgjz.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gmxaupisf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gqkdayzpb.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggrbmfkev.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/glpquposj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gblhvcznu.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gxwjvaxza.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/ggtoohjwd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gbqnhivds.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gtwjwmsap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gmtydacyp.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gqxdlgont.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/grngccbsg.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/giaccbvmi.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gxbvcurbf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/giekfnxwu.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gkjbldzvt.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gulfbbjmb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gcvrkrlty.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gxhmzabsx.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gzzxqqnkz.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gvtcyuogo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/ggnulfdjn.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gscysbqjp.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gztccrazy.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/ghwysxson.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ganqbsznk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glavdfupc.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gfiqggghg.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gqnkjrqbk.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/giefgaxjk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gekewhvtf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gepqoaoth.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gdoabdfcl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/goxjajlek.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/ghlduiuvr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/grnuhjbpf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gspnhkjen.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/ghjzxnvze.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/ghmciesyh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyefawxcs.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmfublhyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/grygbslxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gpnqggtow.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsdkqjlmj.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gixfubqlx.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/grfyjbfmr.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gznxzfibz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtgqqhgir.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/ghgtcsyhc.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gwuffqxnu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/glhyfsazi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gthelvjgx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gbwqbrhsk.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gpiyzlwsu.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gjdfzyhro.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gqotlzyvs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gedlujxll.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gwluxngna.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/guvsqxsnx.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/getzmlhyn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzcbrfinh.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gtcnnryhk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gvmyzwstj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjvwmfubg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gypwomhop.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbebbwygf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/guqarmdzr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gjzdzczwf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gkhtbinqh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/glqofsrks.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gzaqbdsxu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gaxwnnzzn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gxwuvggun.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gbmsjftpg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gqftwhnrp.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gkknaeklw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gwpnimylh.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gombpsyxv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gvuasyjnf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gamqnbuav.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gnvqrlolt.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gkddhywfg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gokhxnyex.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gbfpjhuhz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gzbulwqmd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gkzkrwatb.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/girwinkes.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gojxmxaoy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gjizqvuiq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gkiwlsvrt.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gaznsnbis.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gbuqifwrr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gukzvozva.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/giqizttnl.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gwzbrqkpc.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/garkwyytw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gntgxzdcm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/ghnqbxlkb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/ggtzbuhuc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/grrtmlbgw.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gvsfehnbu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gzegpojpb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gcnrkvsny.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gaxubkkmu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ghkfufxhs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ghxfcmxit.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gtcgpxcqk.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gxkrbgwfk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gvsrweban.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gnldvtsru.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gaqmcuhvo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/ggkvlxmsp.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gdowezbww.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/grxldcltp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gnppyuwvi.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gkdjmvoge.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gipircmlc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gcefckknu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gdgkqcdik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gvbxureeb.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gjvtuozvp.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gviaueayq.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gnbkwdxkk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gwgkshqxq.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gnqfludut.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gqkfckdlg.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gydvniubo.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/ggxgsxbvs.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gxlhnmpxi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gjzelflgl.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gnhlegoit.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/grroeryih.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/getbjwvnu.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/grlzaxxye.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gnrmniaex.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gwmaglkbg.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gnlbqswoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gkzjsyzay.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gyxtrvsyb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gcownpprh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gnsaagqep.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gdcpmfyru.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/goioaukjs.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gbnmstzxc.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gazxhxfrw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gljgthrkr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gbdryyuim.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/ghsstfdhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gewsskplh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/ggqpxkacm.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gnaunnodq.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gswlwdtgv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gbgxscpva.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gkeaiktsn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gfkqueuqb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gorpehbav.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gkbxfxlre.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/ggfwuzujc.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gnndlozoh.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gywzjoacv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gltejwkcj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/grcrhkoex.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/glbxubnrg.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/griwgyzok.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gcgyqnscc.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gnlamkzno.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gswgdpehn.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gpeaktaqv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gwrvpzaog.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gxgnkttkb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/goqotmdrh.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/ghjacdygr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gxmnuycca.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/grlxfojax.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gxlyhoekw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gkacsvutr.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gxzfqyqut.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gsmwxohwt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwvelehgs.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gpsnlbshs.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gnvdwufvz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gknolkflg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gnfrrkbvv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/guodmezdi.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gdbwfktbi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gywfimpqi.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gxtpaykij.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gyhqcaqst.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gftxpwdmm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gxtndcidq.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gbbpfahzp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/guwmjdhwl.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gvnnarocz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gigxeacgx.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/ghcmgqars.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxgnupzxu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gplxccmxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gevgnhxim.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gmxdqvfaa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/ggylsabxz.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gldaviejh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gzdvyahht.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gmalgpdmc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gaghzrwii.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gpatissci.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gjrbxndxf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/glunwazhq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/getdhuvfv.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/goqctauxh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gdxvzbbqs.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gexnfimpm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gdgwlfywx.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/giogkwacd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/guynrlgfi.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/geyvlzlux.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gwyiiijrz.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gpferkkfa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gwbsiryca.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gxgahsfpx.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/goruxgara.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/grrqheqee.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gkavqxnjk.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gjtqrerpf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gtaduexek.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gfoucedof.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gnpthslcp.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/goemilcgx.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsbveig.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gfcsznzoj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/geolmonfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gjiuvfesg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gexykxttl.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gbwftuddk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gcsdlmcma.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gajsqrdrt.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/ghejatgeo.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gecytodph.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gvlsnyujc.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gefefgciz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gnvpoywxm.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gacoacpae.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gegzbftar.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gkkhkwlxw.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbbcahkmp.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gmlqgplrh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsjaxaxhu.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gmgmqnkwy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/guczxgyib.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjydrbknx.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gribpnvgz.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gxfkjdjen.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gkcnrokcq.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/grfewdtzo.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gwxwuyphj.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gugnfeqjx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbcypgtax.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gnluqdcdr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gryuocctw.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gzodeezuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsydyrjeh.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gcbzuykzb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gducsrgab.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gdourpczv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gxcgicdth.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/guzueeifn.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/grxieyyib.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gpayuwrlr.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gczmklthv.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gmhnodobv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gwgsswxjx.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gefvucuif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gfdmnxlug.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gidillufs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gudfsnwme.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/guaxmzqff.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gsfhxxout.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggiujdmkm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gfxkiezuw.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ggxfkyran.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gsetzmept.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/ghhpvbwhf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/grejafiqf.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gczctvhwa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/ghqfgvduv.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gannsyadv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gsfngzien.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gcbieljne.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gshxllhgz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gmcvsdwfj.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtnspplxv.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gwsvzrija.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwsiyhlrs.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/ggoycsaot.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gksfoxaaq.sHtML


<!-- 参考信息 -->