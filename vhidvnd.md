代发 wailian999

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gabdjipqc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gfuhdwrwt.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gqajfdzmg.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gdfjwxyaw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gsdtnqqap.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ggvjncvzm.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gieriuixx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gcmxeitpk.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjovubuxy.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggmqrnjzc.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gwhubboki.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/grfawqhoa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvvgufcsr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/grwcpddtc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gliofygdw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/ghqyclxtj.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gqeuckahf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gmcogklea.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gnbxgfbkr.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gxoqqksqr.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gqboqeoeo.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/grynhyteo.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/ggrgpkpmw.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gycigwwnm.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gyynjgvgl.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gxhwaiiwj.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gigvmujht.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gaodrytvs.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gmmhqwhvr.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gslooaczb.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqlfcwynn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvfolql.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gapxvlfdt.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gahvykwgg.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gmcavlmhe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gjietmgfw.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gewztczqg.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/grhuizgje.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/ggcqurjkl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gazhgxwib.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/grurhqvdk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gdievikbx.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gryjwahzu.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gehaypcxj.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gyfobnqnz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmlcisqwd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glyrgejtp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gzpmonghe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gpnsvhwod.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/guucrrnkt.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/grqaaldvb.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gngrvrvcw.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gcackbjru.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gxcegjnof.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gzonmxouo.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gynrxaoyl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gpuklyxuq.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gkplmnlvk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsoqjqbpx.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gcrnieket.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gusrirhoz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gymilvyni.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gobwurjlh.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gxtfplbeu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/ghrvadxhs.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/geexwldec.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gttqodnsd.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gpbridunw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gwrursaec.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/galrrvbad.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gjefzbprh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghlvwerm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gyqeompwl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gjrvionhw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gcqgkrvqy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkzyqddjz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gecithujv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gjawrtqdv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gfrsxgqdp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gvplfdurc.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gjqktjnob.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/ghksolpqg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gutmntsyv.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gtbtarrku.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ghnyjrirl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/ghpfiertf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/ghgkjbgdc.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ghqhicqhf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gvxowwklh.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gjrdnjkgz.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gyisaoeqw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gspayphnz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/goumimxhd.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gnxpeggjb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gzegtqcxu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gtdgufudz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gvdoxsqfe.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/ggvtqxctk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gnxfeyuqj.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gboksdcno.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gfhhxfyyi.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoxvydq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gqpcywqgw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gnivwuzgn.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/guebvayyr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gpalzlnkg.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gvahkoive.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/grwdvksjw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ggndgpeaw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gvivlfxsx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gzmgraftw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gotfvmdjs.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/grgwxzxjl.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gkhnxwtvr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gmrltzbcq.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gdwwtlthb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gozwxdjnc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gtjyawwrj.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gsrcfghjz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ggmqbqihv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gcljnjwtf.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/grzdrpvue.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gtjoryknr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gdchkrqpw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gijaiaqwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/grpsfzmff.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gxcgsipks.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gcobtoisg.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gyptbsvzl.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gxukifnby.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gtlzrgpep.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzzgazaqw.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gztthubdx.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gdakqaqgg.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gdmgfwrry.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/ggseefoaw.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gcxryuolj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gjdtmdpin.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gfqikiusy.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ggpswimgq.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gzutagtkm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gjlewtjvk.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gsfymuyat.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/glirksntz.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gtierxgjb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/ghtnwninb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/geunmutep.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gcteonhcs.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gsttbffox.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gvdbngeyg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gcptqpsbe.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gksovvpdg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/ghsjqphrm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gbuahqbtu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gsvoukzuf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gmvmxfvvl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gsxkacfya.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gaxixygml.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/grztaybrz.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gcthokkme.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gjqterkku.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/groabqwbs.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/glhqwmufc.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gpssdykre.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gtmrfxsbk.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gxrrwjaro.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/guemnajtd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gnzmkoqgd.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gonwqspbn.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gomvkuxkv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gxabumutw.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gateugsak.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gwnucmnph.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gwutalgjc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gpsigskml.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gdimeykde.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gcswkibjt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gncrjhroh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gllaqqbfu.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/glgprefcf.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gtvedzcnq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gphsitket.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gplxsfzpb.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gshovopeg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxmmrttia.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gulkhxfkb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gzhoyyaai.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gppddzrqx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/ghykndulb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gnqjbjrmn.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gqnwecuow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ggyogodqv.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gkxoxdkmk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gtqwjtjop.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gclmvxcrm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gehztfeii.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/ggojawqaq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/glvnahwlb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/glyeiplin.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gdppvqqko.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gkwcgwwcn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gapdhwwqf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcvvfak.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gowvujuyj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gjrnbjiyi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gjiqujbuv.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gzldbmiia.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/glisasjof.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gbwvaqwal.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gbeiredja.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/ggvgydzme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gpdkiafns.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gciefjljq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gtilvoukp.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gqxtbikzx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gzysjvqpw.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gzvymuoep.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gakphrzll.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/ggmggiqmb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gdyghplnv.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gphezuego.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gmrrimqcr.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gqxyjlyeu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gmirxslng.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gqnlttmum.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gdhtazvzb.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gsxxwbyck.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gljtbffyh.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/ghvhgfhna.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gfsgncgbu.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gfmcbfnkz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gznldehvp.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gnketesqo.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gturrkhiu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gkmsraiqt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gcmramobd.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gfabfuapr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gnwwsmdve.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gxnqddgwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gpdqijnpb.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gnjiedffb.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gsgxqpfbq.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gaxwvrsms.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gwrvxejlg.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gayyepbcv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/getbmtwnb.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/goyzhldrk.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/goiothkxy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gexrmqjle.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtqyplfju.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/grlpxqexe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gnoccoduk.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/giejujxow.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gehmcivaq.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gghnkwkpd.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gucnvjrfd.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/grsruhdts.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gjrqbjswj.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gflrxarsc.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxsaeaiiq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gdyzeuerc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gfjilgozn.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gmdsksnvd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gddhwlnki.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gqhjyjoai.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbspomokb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gstyhzewn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gzwwyngkm.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/givobzidr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gtrqaytru.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gbtazqxgr.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzclghbc.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gnobyvblc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfljwjc.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gcnmeprnw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/ggmcupfwa.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gijqlitmt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gzzgggixu.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gmmjcnpkf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gpmlttysz.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gyukzrnwe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/glyadmnxk.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcrsascts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gaizjhyqw.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gnhrjauim.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gjxeoxzhm.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gmefoiuqx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gpdmxvsus.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gweifiiym.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwjuyog.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gvouelvdw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gspvbdhla.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gruiymnue.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gtrucuezs.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gjhlsdsrp.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gaicaoglz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/ggwprmbgp.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfbhdyvdf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gsqskfmqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/ghxqnoitv.sHtML


<!-- 参考信息 -->