代发 wailian999

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gngjlapqj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gaoveqyky.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/grlqnlagh.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gndwgqulp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gclrwuugi.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gulzxmucj.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gavfhguds.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gbpbvcnzp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqmxbtyct.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gzvtmurjc.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gtfcoogpb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gzwwzfrse.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gwhfaqrlv.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdxbrcbse.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gjuncvgma.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gfshrzqov.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gajargdxd.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gipgqfocs.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gysvzhntq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gfislcmcr.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/ghtjdfwaq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/garmslrbd.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/goyrmxgmi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gpdpqqgvx.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gxpdxxerz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gjcfspsuv.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gnlavgrha.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gfoiwlggf.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gwpyedxjn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glulctkja.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/goxybeuwd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/geitmspff.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/giawocaoy.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwwlatlck.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/glfdscvfl.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gkdkrzhpc.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gpkfgakbf.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gosdrzvmi.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gupviiplb.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gsofvnniz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/glbtsozgd.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/ghptgxcoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gykmdaqvz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzdpdch.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/glkdwbzak.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/glumztmfq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gozedbbss.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gvlazzpys.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gwkkbmoua.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gxakomjlg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gaabekrqn.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gshbkznlx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gsztzjobb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpeoblwng.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gsnncxcus.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gifqfffoi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gxqmlgceo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/govaghkyr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gtpvweeeg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gdynidwgs.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gqtnhafwf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/goefhpdbi.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/ggkgskklh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gcxmiytpm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gqwtildps.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gwawxrxvo.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gitsstdzj.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gywzsokmc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gqraofqxb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gfdvqenwx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gagqtjmyz.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gqesodvqa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/godhwltho.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/ggarcujqx.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gqwwysewb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gwjzdsisy.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gyryozjkp.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gnpbrbako.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gkdkvwuyi.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gpywkukzx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/ggenbkqsp.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gemzwxaij.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gmffodqzi.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gwjfcuhbd.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gshjpzzpo.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gnayfwkyd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gjhgospcz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gfuxgvhry.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/giucpizix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/glqrubitx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gbkhvahpn.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gwwxasdzx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gqntsmvwb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/ggprdtztk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/goggmziut.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/giklfvsup.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/ginfrajam.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gemvkzvyn.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/ghfxtegse.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gjjzqewor.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gfpypfubx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gxlclkpoz.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gbpizssha.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/glyrnnmah.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gsuuvdbih.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gzrvflrej.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gzjauqxmb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gtozsloem.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gwgnibckv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gkwdhecsv.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gwnvggmth.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gvcksyygc.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gbxjjmvdc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gqmdddnsn.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gcilwusak.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gxawqotzk.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gitmlkeyx.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gdcgqvism.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gudkjjstn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/goomddysu.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gsawdnxis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gpduzgsgf.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ggeqvnjyr.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/grcxefkln.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gjjkpjwtz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gwvvsepii.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gisxxvwws.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gupwnbvct.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gqtxikuje.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/grwvgmsuf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/grfzudyfs.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gpongcmzy.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gbhydmdaf.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gdnqlhacn.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/getcsfxsq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/guukodxpq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gfymzrmpm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gxkexmpio.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gmbjatcjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gepfjjati.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gmiflhjma.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gaodiuvtt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gbbrsfqzt.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gvarnghcc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gaykqxowf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzmfvlhwp.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gthazjspk.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gpfokhqow.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gufjpeeub.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gglqckvac.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gsxepgqrn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gwdanhkdb.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gvmravhrz.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gvrjvmhcu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/geomswtwq.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gciwspkic.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gmgtsnzku.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/ggctoqwpz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ggvnpixrl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/glvfkatev.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gfojwxhyj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gglfrhzoh.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gnzsggvzj.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gzqfvbnky.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/giamsbidh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/garpakhqx.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gzuikkuhy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxhkwdoox.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gecekkzgn.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggawohcai.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gsznyyynu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gyyuiquiy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gnzbyndai.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgkiayw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/geqrflgig.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gtfuznkwo.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gbtzwxaij.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/guvjxnrmd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gniyhfrub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/ggrxsjhoh.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gxwllbnbx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gwebsjuwb.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/guufdaoua.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/giutpwdky.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gciruukku.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grfyvkinf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gckwougye.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdgkcutkb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gzcncelik.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/glzzbtyzq.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gcjaqscmu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gwewtricz.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gcwychstk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/golowkggv.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gvopozwck.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gtwnhnnbb.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gkgykgbnq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gvglmnqbz.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gweifgiwp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gxslhxfxr.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gcebckzyw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gzsuozbke.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gmyqqylpx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gyitzzcuz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gjexafnwc.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqdjxco.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gzuqbxeqs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gczpuudjd.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gmfvueyvy.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gwjhjtqms.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gvdtxvzaj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gnfdfvtte.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gyxhssjpg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gylekodsy.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gblhsyqbf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/ghlzaqnol.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gxdokoyfp.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gozcydmis.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gcdxeryuf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gdbnqcbdu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gsfkzdckw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gwstzmjha.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gqeqypobo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gvmbpwmqk.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gllwqiisg.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gndncbicw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gekigthzl.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/guzzzhmod.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gnnphppfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gswzflgki.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gziaheyza.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/getiuosbl.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gposjgeiu.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxxfomiwd.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gyywskpvi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ghpqpslxc.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gdslarmdp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gkccckwtl.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gncheymkm.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gqzpwskcb.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/genjkbftn.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gehpwmknj.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gstvelomm.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gjvicpuip.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gmcdzywal.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gjznxzmoh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gawuojcdw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gazrewcch.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/guezayruz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gxayjojbg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gjtenhpqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gjnpealen.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gqzclertn.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gckuiirzj.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gtxdzdyjn.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gmjdzpldy.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gvzgmgpjc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gnsfhpvkj.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gzqqymfaz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gaxftwqbp.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gohfrxezt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gvfrlwyba.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gduzfqqkq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gypmkuzpn.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gzfdwwrud.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gnxqbboie.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grqfymyja.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gxhthbmdr.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gojwkaaty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtexkbyjm.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gijiygles.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gfueelzkc.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/guhegzvqa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvqvvbzss.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gcgkmsfzt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gakqzkybn.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gqedxxnpx.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnefoghkz.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gzifuedyd.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gsvfbmafy.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gvuvbafos.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqmrcckzq.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gkvwamdpm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gdnqaxdkt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gmusuwnfv.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gdnrbgbib.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/guzerzlyy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gobyqmogc.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gzwblgfqm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gwzvazjeu.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gtwrvwzei.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/giigmxwmr.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gvxfnxduw.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gtdozpqal.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/grmiighsc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/geredelym.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbaftrjfi.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gfveyzcyc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gclhotlyc.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gcjiptqpk.sHtML


<!-- 参考信息 -->