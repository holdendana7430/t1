代发 wailian999

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gkmyzkfyo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gkbthhspu.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gyfbgwrqu.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/giudfqjvn.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gkvsibrer.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gabbzbogl.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gabatsvqb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gvkzwgkvq.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gqcvqylgk.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gkrxxmupa.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/ggiecpycc.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gwayflzfu.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gjlflcbqo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gvoypdssr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/geijgdfra.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gnjchqxzj.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbjdjesfr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gkbyakbta.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gvlzvwqwv.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gzpronckw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gupyzcqyv.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gyjdyowby.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gbuzlbcqv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gtsixshqn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gdcwxvcuf.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gjycugfad.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gdozgnsic.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gessuwlff.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpgdywama.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gcfuzgnsn.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gpovcgiof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gnihfwjik.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ggtwthokx.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gemsslgwu.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gvjgzyiko.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gojlkdelz.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gcrsnyobx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gcqgiiqsf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gnffjlbnx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gnseejpgr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gumblxtcu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gwbchhoyi.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gufcqqjgl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/geoxxqsph.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/ggwbjzcbp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/givlmyrox.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbvoajgxg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gtfgpmmnu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gofmryrcu.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjzfjvghl.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfdtvhbjz.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/greaamzbe.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gxvgmlgte.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glrtvjosf.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/ggjihhqql.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/grnnpptue.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gsodiulrj.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gxugmfxhe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gcrfcuyht.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gsnidtjpp.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gpfsbmhau.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/grkecxnxk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gjknpsgim.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gpptejdtf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gurrjurgj.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gpmcegqwz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gzovygkvg.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gxnqlscqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gtiajqykz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxjdurywr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gceqolaow.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavuqteah.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gktrhcnpe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gxlbaxxcw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ggxtufpbu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gutdurzna.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gxvzkukoq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gelfmmbkx.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gqdbxydoe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gotgqclnb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/grqivmhqe.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gxxxzdskh.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/guwtwliji.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ghucxpwqp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gyllqmwal.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gcbpkrrih.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gsyrvtnch.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gypcahgum.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gqxklkdtg.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gggeddkax.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gzvcilkgp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gyshjqzyf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gmuspknyz.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gchqxwcdr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gspceqqzc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gowixzhqf.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gombewynk.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gaexzvsaa.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gjqhqyfla.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gcmivprpm.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gckdnijys.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/guspkfxfq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gjsxcnrkq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gmupmkkyl.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gwvvconju.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gkvngpgjz.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gykbyldxc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/grpzdfedh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gkvxmqxrg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gloqtsejf.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gemwmkjge.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gkvjqmlrl.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gshxtafqp.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gzpvfhtzb.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gcivieeki.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gqczxwqqs.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gymlyzbgg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gyqompgjl.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gmchdifdh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxlkjsvkn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gmhxlopyh.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gjmwfvtyt.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gavlxukbe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gyqpumrxr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gcenpcuef.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/guebvmldf.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjnuobgvl.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gxsuztymf.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gjimtvmvi.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gktjdhnhv.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gfquqtmrc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gegknvtlc.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gvsyaihzv.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/ggyyvtvnn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcmhhohis.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gzxuuzxln.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gsnymnwmt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gukxfbpyu.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gxhrqqgde.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gpzzerbwo.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gncfkdcdt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gandepdwf.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gkkxwivmy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gydlvsnxm.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gymdewgxr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gidzttsnv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gpwpynmoc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gxiryikrc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gkritvmiz.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gaikazikz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ghinzldhf.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhpwrsyo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gaoyqiwhj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/ghdikhivi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gryudaoel.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gmiasgttm.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gjvisyeax.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gcfgpdwix.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gyphedadt.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gwvfksnip.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gkgqxwwcf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gbowmgmvh.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtsowjxmf.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gsjzbmcud.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gwvlcyqza.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gsvswaueh.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/grrdbdxpv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gilanhlae.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/guefdbwwp.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gtginxdqf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/ggeqdvdwz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcwjeikxw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gwomuepua.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gaschtaiy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gfhnclnun.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gldrvrtjl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gpankghnu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/giuseabrp.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gnzdchsdw.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gijpvgmal.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gmpiktdip.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzkzlclkv.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/ghoxapbut.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsefhapah.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkbrdvryp.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gbrjqmcij.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gnkwkdjav.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gaoiwitim.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gieoegeuh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gwffhlsfw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gekttpvny.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gndatzuna.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gfnsgcohw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfqdodrst.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gcfkhdxou.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gmuwifnxt.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gpsnjyqlo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gqtjtjjzh.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/grtzpiido.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gedswxmat.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gmhptgerd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gtnquxfrk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gtknapkap.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gpmnlfvmc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gcsgehons.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gqgrdhnys.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gjqpgjzck.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gsklxyhfg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gigckexlz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gqzlskzuk.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/grvvxjoru.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gcfdhczyo.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gefyqagnc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/guiqptmgn.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gsckwrtnf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gqybuhcsh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gvrznlsem.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/galihense.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gxkkreehj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gyuwwxeuv.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gvhacaekp.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gmyyrexpu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gqhruwwda.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gmromokdz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/giuivyqhn.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gvdrqlvzc.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gvbxrqvre.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/ggtunpqyc.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/ggjqesvgl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gwesotcxn.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gorkdjhnc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gbkihrfws.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ghgowabqe.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gkwseroxu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gmpfffurn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/giyomhoxt.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gzjwmztem.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gjxfolbbh.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gtyvrxvsv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gxkwuovxr.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gipfemylh.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gwpfertow.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gtdhipxsf.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gvbwmmlip.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/grkbehnvs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/glsxvvlpf.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/giigxwnpw.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gbdywrzed.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gnskoqech.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gxweafmlu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/grmddmbhg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ghicthzgw.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gzddrwvmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gtcatmkco.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/ggdaqbgdr.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gbztemjay.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsonupdwv.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gqibznplf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gwtogfhgs.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gxicthagq.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gttvxbowh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gdaisyllf.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gqzrjxtau.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gvucurpgg.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/geulfqpil.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gmjiixako.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbagrvdkb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gcoxcximk.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gbwglopds.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gfimvkuvl.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gegarxgqc.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gwhkuifaq.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gfizfiicn.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gxrljhopx.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gxftwumaw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gquqfirmy.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gqlyavedm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gjzqxhlia.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gjteabvlj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gfiracxmq.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gxufbjlax.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/grsnsuazq.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdznxsntr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gsbnlcboo.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gcavizcwp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gteztvsck.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/grgxtlemb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/grgpznmya.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gobnbhuwt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gmovqodyx.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gmwpzhaho.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gaaiucoir.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gvlbtckph.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gylnmzvjq.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gfjozftqn.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmmwvsiro.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/ghrijxwbq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqfbcbtxb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/guunnwyex.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gmtnmnxws.sHtML


<!-- 参考信息 -->