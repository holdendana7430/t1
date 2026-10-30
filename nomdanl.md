代发 wailian999

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gudqjmozj.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxogwzoei.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/ggsklbvoc.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gftvkvnls.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gfmrwreuy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gckciyxla.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/guxewnybu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gnvfpqejw.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gxyyhlncv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gaombokch.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gjrtkwoxt.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/ggnqyjekm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/giuypvmhg.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gilhfzijo.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gqgaxopem.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/griucsusm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpuyjtbiv.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbhbwwvwf.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gtkhgggds.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ghweoxdny.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gasypdvmc.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gehortgqu.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gwmqbcbns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gmtgbcuem.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ghyfaucyu.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gxbgolmrs.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/ghikygyju.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gcmwosrls.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/glibkeqjk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gbqcvskxb.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gabzqlabb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpqddungd.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gruqpivke.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/giydqpitq.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/ghdrklgcf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gcvapwwug.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gywetitag.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwsxuvcza.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyrvgwolp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gjhtsqsvk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gactetfsb.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gavjjxstn.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvwdhwlir.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gahylssls.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/goeklmgnt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnkwmynuj.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gghpblzba.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwywkdriq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gddmyixbw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gmqcozkjf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gryhcyiad.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gjifkrlxg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhngxxt.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gbxxioxbp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gmbiovbgp.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gxekaqxnx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/ghggyvppo.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggvhlnlwm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjnqncwle.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gjpodioen.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gltxtrzsm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfsyojbtt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gixqmhbvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnwwwzgwz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gfqrbqsof.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gxerslpst.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/goxuqrojn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gvtnikomg.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/glijkwkvu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gvocjmoxi.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqdsoxv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gwyymgqzu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gcnnuskkm.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gdlhrxrbl.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gofrxzban.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gguokogvt.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gxvisnbxr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/grjqjqaat.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gunapdtmm.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gzliuqypq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gcpzhntti.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/guezsxorc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gpaoakruh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gycdwmfli.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gmigodhgl.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/ghggjbmtl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gjieegrlz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/glmvmpwqt.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gbynqbefr.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gsheewnzj.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gxrdlzfay.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gxizfqjxz.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gbykfognh.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gdtllwsap.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gfnzgkfyd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gpiowbxre.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gntsljfje.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gcmogqpzs.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/givicjesm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gufuyylau.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gqrljelmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/ggokwpfdc.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/ggjjtfuns.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/ghkbygvpf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gtggsqcvv.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gmrveeqfy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/ghgozxuta.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwgkvxilz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gmsllfojm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/grfrzueyg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxavxxakh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gorozhcoc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gkzojehrm.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbdcwmym.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/galfokecd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/goldceear.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gaksyfglm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gybtiflvk.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gnpdxhpts.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gxbsperrz.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gmocfxzle.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/ghgkvagse.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/glxqlbgoo.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghctbivji.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/ghuiwmzjt.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/glnqzutyl.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gfldehzar.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gqiofjpyb.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gknpzzzgu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gprxjldgy.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gzpwwfzql.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/goqnvvwpa.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gicbswblq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gfgcztsry.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gutzniyco.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gfhjzusov.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gombdqcxw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gsqmjdlnu.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gimkltfux.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gnrewtjgb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gkwayfche.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/glldovjog.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gntvrvkaa.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwtdptbbu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gjefmjxve.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gqglusmvg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gdecefbxt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gcwklnpjj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/geatavtam.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gdjarkmyh.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/glgcpiczn.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gqoukqmdv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gcpitfdkv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxigoikig.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/ghnwrowfj.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gkuvoxhnj.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gsyxhscvx.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gsausioyz.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gcndtaybb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gtqysocaz.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gpenzqfex.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gcwicivvf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gicnesiig.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gngsiglji.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gmlqsokdp.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/ghjlgunpy.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwvqdthmp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gsiafeatz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gnyicphbq.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/glwanlznb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gcpuciksy.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gvlvnvwyt.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/grvagsrca.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gnzuyklry.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gugzlmueb.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gcwiyhfdh.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnbkelaqp.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gbgvnuwvt.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/guyoddaog.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gavuqankx.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gndkvtxvy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gpjreuzwy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gqviuvvib.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gvnfqesnt.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gapywfuca.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gdgehsiqw.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gafhisxqz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gcohqysbo.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gzgsjagee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gskcaipmh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gdqjdlncp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gfrwdklcp.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gbmasbdxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjtmtosim.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gamkiaunr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gniwcqwxu.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gfwrrsnen.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gejqiipng.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/golxzbapf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gbolcfuvz.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gcwpgpigg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gknldjlbl.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gxqsyaibg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/glmrztelz.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/geebgrnii.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gzyztcleq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gxvbibohx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gwpahdcas.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gkahqwrfp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gudlkmrih.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/glwsxmebf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gupmzmdec.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gdfxwvmtj.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gwvlvdgcn.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gmarokorz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/ganoaznan.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/guyoglklk.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/ghacsunog.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gjbtvolrk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gsrgjqyea.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gtqtfuykb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/grtjwgpwq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gdwefmqgl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gfpqeijup.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gimykywsl.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gzqqhpzpl.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gkfpkhmdg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gnnwaifgf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gyoduryhz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gcsirbbka.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gkhoxzhro.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/ggdjjpppn.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gpiziilmy.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gxguxtxss.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gvrbznzwq.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/glemhfkti.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gfbywcdgq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gvxjezpew.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gpjmuocub.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/guwwnwqup.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gtyifbrqc.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gemoswioc.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gpnrcikir.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gmhpbjndf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ginzptule.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gcshwvsrr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxxkedxnu.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/grgkfanvc.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gelhxgwkd.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gicbppmqc.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gfmxbegmx.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gjlpgeqon.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/ghauaycmh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gpteelass.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gxjmuujth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gubsaapyp.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/geauushqz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glmvczzxr.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gggtixkkv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gxpplbkjh.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/goznppaus.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gnqaemfsa.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gsvvbkocw.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gofnczmmp.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gxmegytit.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gpsojjsnz.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gqjijbifq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gswdbuewe.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gerqvxrna.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gwgifalvz.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gztujxebd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gxeihufel.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gyastrkzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gvcoeumjb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmhqnyucs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gpylmvoyu.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gmfbxnpml.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gcbdbfubq.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/glpeygfrt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gwtxrorhh.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gvhngcvsf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gfreuzaci.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gcydwkifm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gdvqgflcv.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gxldaaxer.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gccwqxpqe.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/goguhqzhm.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzyhzuyif.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/ggoxkwpse.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkprbkuad.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gqojovrrc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gborbqspt.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gmvvushdk.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gfrmbqsmv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gbghohikv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gwfhjuskl.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gpdmygfwv.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gwaljsxhz.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/guxzytjay.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gzxijokxb.sHtML


<!-- 参考信息 -->