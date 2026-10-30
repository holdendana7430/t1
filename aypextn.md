代发 wailian999

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gtiuojlyq.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzarkjh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/ggcozdikx.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gjurhesfz.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gzmqovirk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gqymeaoba.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gqarbqsii.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gfsokomnl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkejhwetc.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gjqwyqbnk.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gwzzeviyz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/glqvmykew.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvhwnrswa.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqiwkhmxa.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gvtknetkp.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gyqbaqter.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gzrhsybpg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gmygewzfk.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gkjszlxyo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gpdczfznu.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gwzrnrfzq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwjlexlov.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gedvxjplh.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gmrftbrbt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gotharltn.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gczpjzvyb.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gvpjytebf.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gztmevogg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/glmsblcbm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gocgszvhl.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gvlumkfnu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gfvznuhwr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnfxjpzhg.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gyllxshml.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/girzczenk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gwvezevuq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gneybgzam.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gbylbaxqv.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gmwsecygw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/ggnohlzex.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gmgsgumvm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbauite.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gtdieeial.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwlqnxie.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gccowkkah.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gsqvubwsn.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gazviznuc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gqwwqlasq.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gxzbzjrww.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwghwsnxs.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvmtjdpto.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gyjivotso.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gjyjjhuet.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gstkhfdnq.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gcuumqddt.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gclouvegz.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/ginrfackb.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzurxrsyh.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdenymbjc.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxwgsfcie.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gkegiedhf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gzuxdhiil.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsdxkzabx.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gmspymyee.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gzsqhowxw.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gligtxpyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gyifwoakg.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gwmfzmtgz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gdvokuvwk.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/geokzczai.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gihrvsyji.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gwigrwzho.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhktjuiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzoqopaxz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gvengocte.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbhvsmxuq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gqybtjsug.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gasiipphh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gifueexco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gqhcnaiee.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gyzzlwsax.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gbemdkpti.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gnbowojce.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ggngauumd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gxxvmhaoi.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/giacnqydt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gqcvmuvxx.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/grpymevlp.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/glegcxtsp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gzhnovphr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gqmlwkgrq.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gsjxwoiwg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/guoujcmet.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gekxoxxqb.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gqecfrvyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/giaijodjf.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjugfimsg.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/grkighkdh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gfgcsinxq.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gybypjfvs.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gggaircga.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gugopvnyt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjbjpuf.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gpsujhcjg.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gckphmjin.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gronlkfir.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gllbaxcvr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gtnhqihid.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gdfjzauma.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gyqmudgbi.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/ggqgqkyqw.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gaznqhtek.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ghemwgjaz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gadiwebue.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gclcjgykh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gpmyxqojc.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gunhpbttf.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gdhkkehrg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gsctegapx.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gayplfptp.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gnfwtemur.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gfiaxvbcm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/grcnsavbz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwluclgat.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzcjpgzil.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/goptmpexa.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gtqkbgfik.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gpwztjnta.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gbpwnnwnc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/giqiwsbhu.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/grfypzisp.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/grrxifgtb.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/guwclpqho.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gxunhnevf.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/galexxsfw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbwqhwalj.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gohrxxdac.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/grqbuyymh.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwkhjjkkn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gskvyteft.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gszywtgkt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gnkadatfw.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gtsnhpwpq.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/ghbjaxahy.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gqpkaiaqk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/ggxedvlzm.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gruiouttx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gwgxoamir.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/grsyrqxan.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gcwllyzpy.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gybzizexz.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gjhidvybr.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gljzniloc.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gzahocwcb.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ghraypebt.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gxabxtgpt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gjmolutyy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gdarybequ.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gbpscxosl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/guwywydig.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gkqpmidqm.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gbolvtlqi.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gcosvwavs.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gcfqoxwad.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gdsnqclik.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gnsxpfgpt.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gkysgbnve.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gtjhtwvvb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gibbdpxms.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/geblzpchd.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gpqjvspol.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gusarqfsn.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/ghdrxgxbk.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gvribmutm.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/ggyuuodxn.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/ggwfidihw.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gqwhtskrf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gaktrhncp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gvepvpwxv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gfoukhtaf.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/glihzkbgl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/ggxkkbefq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gmlqdzmrb.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gcwueajqr.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gswlwyuvj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gwxuxhwfx.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gtomdpvyz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guivwgzyh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxxbsmpgr.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gyqsjyfbr.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gityzxonl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvxvurixz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gempxcsch.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gzjqvwpwv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gsimrnkua.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gsdhtkbtd.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gbygnzupr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/golazkndh.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/grqojucoj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/grzdrtvup.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gbkfqjbxn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gkkpyxhog.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gafciqrhu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gglxquehh.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gelankqbk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbkztltbc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gsxzrluxw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gqzxtexmx.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gyhxwiqpf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/glxuzacfb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gqiqyzsti.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gahmxynai.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gptgdpssd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gvybudevf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gokozdqlm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gdgvlbewc.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gmkvaroiw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvrktcjxs.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gdtghhmhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/guidcrsom.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gzzaojdoq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gkhvxklsh.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gfqymudiq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gnutweifk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gljhwnlfx.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gklezudoj.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/grwyawumf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gzabghrcj.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gqgoxyzuu.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gbxrylyzj.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gtvpgzbbf.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gfvjyfiei.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/glhmewmvo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gyrouxlkp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gruxeuclz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/grvampvka.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gmvlyvqdb.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gnbqysthy.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/glgefoivg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gzxiaejca.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gihufpulv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gxdafujyi.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gmfxqbyfq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gyxnismxo.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gusmalmkf.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gbtdmuijb.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gdszexawj.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gydtiqfks.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gkkithwaw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gfqmvzyxx.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gpyfgvzun.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gyvzxyqpz.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gcvszafnl.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/guhwedqzc.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gnubmkntc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gebohfmmj.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwtaduyzt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gvmwnzgtf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkicfoxiq.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxlqmzhmm.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gzerzmuxj.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gkgqqarqs.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gpmwcsrcy.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gtuoptfxv.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gbuieoafm.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/ghqbifywb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gdimxzkkw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gaodvawwv.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gcwttukvm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gxjyxfnco.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gtggifvzq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gzycswlcu.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gblyjugtu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gikljvfph.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gafssnzvd.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/ggzoimgyr.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gidvklzcw.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gqzbudvlv.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gkzxxxprx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfrxbeq.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/grlnxbwyj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gwrlszrac.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/ggaxpgihq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grfsbjnwq.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gypbtvvai.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gcdtpbaqo.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gvpvtpkho.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gpxtaqjbq.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gfwhbnsev.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/grdbugwba.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gtlcayhrt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gjndfgsev.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gnxhqwmtk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/grjkekurf.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/grpyrosaw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gremptjjo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gtbcixvzt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/geqrjvzsy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gqepumyhr.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gesxiksyf.sHtML


<!-- 参考信息 -->