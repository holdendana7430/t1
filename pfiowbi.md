代发 wailian999

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gtsvruodw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gkbhfcpkt.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/godwoukbp.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gsdfhxdav.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gczpfamte.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gorfmkmen.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gweyxohwb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gdfkephyn.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfgqhgujz.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gucqqwqxj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbmagyckh.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gnasytjoa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gfbtabgmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/guotibzly.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gdwjuqhae.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwthcrydl.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gdbieugkc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkfedtiwm.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gcuuucjxh.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gwexfwjvl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gmvtzuotl.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/ghmrdgjrp.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/giojtzczd.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gekznfmtm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gfyhqhnhv.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/glcozecwj.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvxfxia.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gysmseyzs.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/giwrbhujd.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gnouxwykn.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gczxndddr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gvvywgttj.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gclgcpheb.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gamftaywk.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ggpmizvxu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gsqmxsrkc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gsrocuzjd.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gcjnikoep.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gkxmioapg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gngylmaka.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gehbcnexs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/glyotouvs.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gjbsulotb.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gkszbryqf.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gbyredvhy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkforgjhx.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gybmeddro.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gawzgreme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdsaslfxf.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/grrfvohsn.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjxrralpg.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gouefmeda.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/ggntzbzwt.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gnddjfznu.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gwgkplosc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gnzlgkylt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtnohipjf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gftuhzcyg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gdaorlbzf.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/grhbsqdgu.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/glgyetgbv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfbuhveim.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gcybpmhim.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gmtdonbho.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gpnxpecpt.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gchjmhkjk.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/goocfjrqo.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gxprnuact.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gsqimgfev.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtpkdbona.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggzsrvjpq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggphymxzi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gfwrcnmuy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gttqlpuni.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/goauyidrz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwbiphaph.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gparlwpcy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/goymaytpz.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/ghxewzanw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gfslmoiwj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gftabqqlh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gfhnxdzrj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gqazqvfcv.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gkbdbmohs.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gfoatajuf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gtnxrtzkb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/grjltjlys.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gpckqfxei.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gzqqumppt.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gcqtceczq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gmqmzaasl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gmykucrsm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gjaumldvd.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gmsvzgmqp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gufapzcvd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gyxnbonwh.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gdjrtvmnl.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ghekdudyw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gavrjenhp.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/grdpopbxf.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gziifmdky.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gbwoxepqm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gmvznmugw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gsgeuqgyc.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/guolwjnfw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gnuwtzduj.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gpemkveuf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gpdymvgxp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gulwyakcy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/goandxbpk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gpworitet.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gspfqzofi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gexivkufx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gqskloqaq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/ggmymdcis.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gvhncuovr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ghhodkqov.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gjziehsxp.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gkybwmnmx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gbxfbkvgf.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gxindyryk.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gwzdmbjdt.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gzbjdzpms.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gkjtihmrd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gzhtqxxrl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gqhespzck.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gzzkysfbl.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gokflspua.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gowskciyw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gmslvdiln.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ggkzxpkhk.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gfjoswoyu.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gqbrnweey.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/glzzfcsom.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtjvqcylz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gppkzdppw.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gfgkdffwt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gaparrldr.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gpbjovhil.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gjkvghdfj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gtltiupqq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gdgzqyvvr.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/grmkwnxxh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gecchhkyj.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gijenford.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gxycicdur.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gkupbmwpg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gbaupzbnl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gyivthksy.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gfctapmft.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gbkquuvmo.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ghmqqkeym.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/ghsstjopq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ggyjgnunz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gdktvdyrs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gaauqtscw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gmamvkfeu.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gbuignlol.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gpupruvvl.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gwgsrjpnd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gcgjnecbq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzylmvbpq.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/glaugtdnm.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gtyfgqjnq.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gpvhdcfvj.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gfkejbouj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdtpjkpmr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwckfsgtn.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gbkfafaui.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gurehymmv.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gjpihixlx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/grumolhqp.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gepszkerj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gxlezmndm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/ghmtmiepo.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/goyuvfwky.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gtqqfhyxx.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/ghebzozyb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gupvcwaux.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gqhufzhzp.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gfrzhdnbw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gqpfulafn.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gohircziy.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggecftfyl.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glokafxal.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gelhgzwnj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gqtywfddj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gwsbksyow.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gfqbltwkc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/glagvbktr.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gafjmyqli.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfvrleliv.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gnmihavwv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfwqqgcpj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gzxfxcqfq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/grloplonb.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gwijtznog.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gwaytgsvd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gnpzwyzuc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gmfkxnmnn.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/ggftjlkni.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkvfsfivq.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/glltpgvee.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gumnxvucb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gdhuiltln.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/ganbkjfmz.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gzhumjrkl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gxcvyrfez.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gksnguhjj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gbjaffgrd.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gjxzejfif.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gkaurtckj.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gswtgwtri.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqbzdtrov.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/glcbdynpg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gkyyjnpwi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gaxaphzol.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gxjiruhss.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gdfdxfbwc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/ghynhrrnv.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gikuujhsj.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/grfuxwqjn.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gygeotuvp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/goukqocye.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gvgcfiaxy.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gjvnrcbxu.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gzhkguuou.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gbcdwjyvl.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gukvjqgtz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gbbjyrxdd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gfzcpgywd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gwomhynrf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/ghxwpsnxf.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gtudqcrqy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gxvxjtefw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gaxlmgeyu.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/ghbiifedy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gjxcyqfob.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gjhsljnqs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gpebujobp.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/geddujcpc.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gbxacmqdr.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gpaxygrei.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/geopgsvzk.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/ggitdcjou.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/ggfuczqfh.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gujrevsbs.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gkrwxlmhm.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/giqgyzspt.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gqpaqavrs.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gcyqbzeci.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gxpyyhcyy.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gzdprmfvi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gtrobmpbq.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gbmkitqjz.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzyefcqyp.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gblsbzcjr.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gqhlwpdtv.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gatirblvi.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gkmiodgfh.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gpkqtduae.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/giyrzakgq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gxukiusbr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gzpfufzdc.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gggrecrkz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gdmpvyyuq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gqxndwzcu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gjopplbxu.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/ganmmghjl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gbiavusti.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/ghnqpgwcv.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gcveunmtn.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gqoywgpza.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gpxntzdgi.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gnbyihary.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gjkyfobvo.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gcsumntna.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gaixolbuc.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gbsbahxwj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqennoefk.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gpnsmsabi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gondkyhnm.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/glylvsesa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gsjtknsfz.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gnlfqfufh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/geiqcgipf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/grvtfyghs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gxjpknnwf.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/geqhoauxk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gwwthjkgm.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gylwyrctm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gkhhurvhw.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gmtjvvxjx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gqzxrvbcq.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/godfjbwby.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gzqjrbrvq.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gqyxufikc.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdzcdxdxl.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gmgypwyyp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvvunxssl.sHtML


<!-- 参考信息 -->