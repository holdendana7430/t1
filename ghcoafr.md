代发 wailian999

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gvxvtmwtr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gjfzuzels.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gdphtacoh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gwtigyden.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gbtpmuvel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gwwvxhdgi.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gamtjhjox.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gbajcclai.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gerstbues.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gaygfpzvi.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gwbnftrfd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gnlvnycwh.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/ghpwanlhs.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gziqqyefp.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gugasvcsn.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gyzasnndo.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdqhcbcnz.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gbmbraxou.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gpvtlcwkq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/glhvyhlmb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gogebiqtr.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gtjgufjar.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gnxxeooul.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/glrcmclkd.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gfitagtjt.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gckwlmsic.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gmczjukzt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gntvqitbb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gvqblqwnk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gjcalggdu.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gjtujdafr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gnfhdovmf.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gotfytzvd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwdhuojmd.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gerhgevqx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gklkygnwj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/ghldqbpmq.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdkcurxrq.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gpilgjrcc.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfguoojrh.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gntakbtgy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gclwssvyl.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gncizhfya.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gjifwfbfj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gutqfulbs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/goaexnyiu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gukitvnjo.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/grodmghux.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/guiogsabg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbtsismjc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gmulobgll.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gvxnwfppt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gsowltqic.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gldtrsldx.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gwxmnqshl.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gkhecxoys.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gzyuuvdkx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gidgikbmd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/guaocckio.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmbfknbfp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gavuurfsw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/grbpayftv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gpucrlcet.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gisvmhxpo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gpjlztyaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gzkleuznr.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gajcdjwtf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gjqeyxfnb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/ggljgvcin.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gkbofptwt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gdliahrfo.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/grsmfrjho.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gkdkxwzft.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gxylqmbfo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gwqskgemv.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gbkembmbz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gjowvlfyu.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gktqeyhay.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gpovfyssx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gpvnbexqa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gmoaifysz.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmfindyab.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gxdjygmbn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/ghdzfbunp.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gpwpzengq.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/ghmfrorto.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gieypreke.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/guikchhvb.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gnroymcyk.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gfsoozjqs.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/glbqyidhi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gjrmozdfm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gsmabukky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gahdrhmrj.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gxykxjesw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gnxpzvtfq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gvhoanayu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gmndvofms.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gwiaobeiv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gdcjthinf.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gdiyuwupo.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gqxftmsiy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gwbenuavb.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gvmphbhxu.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gzimzowtv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/ggkrlmevw.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/ghxseanze.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxflqakxf.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gnoqezyvr.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzncypcx.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gymvhamqk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gejafpyro.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gnicspfxe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gmlbjaxec.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjkujkiwq.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gfhghqgah.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/ggflplpka.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gsckxhuqn.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gzdponpdb.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gnwssviiy.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gwiqwztuh.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gfpvixlqw.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gmxalecbf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gmnehqnqv.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/ggqljsbuy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gkierwjxd.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gwwockclz.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gkhaluyfk.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gtrvjagmc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gvcqugian.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gxpocwpfj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gpuhuihkx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gsgposycx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gwlcvyzil.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gfrevacfz.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gvhvclqsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/ggnckmpwg.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gpccowaqj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gbmgzyqql.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gugihkpuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gnkrvtjfn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gycvzoieo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gucrixins.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gfbbccnoc.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gmclfbuaj.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/goxtyzxdb.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/giwhbxpmz.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gunnhdqjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gpktqhfdi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcvmyfntw.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gxnhqohft.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gavpnzsnp.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gyozvjmrt.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gyovutfqs.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/geyusyxyz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gwynyepgh.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gwgbcpatq.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gxqiodnzw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gblwcwwuq.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gcqhgoppg.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gevtoxuee.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/ghwdqsigy.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gnqqkraee.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/govqrsjqj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gccrdyblz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gyalaarsd.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gsbyicwwi.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gfqmzvjaj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gifffbbvh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsgylbiev.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gbdttyqwf.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxpwgwoyr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwnxvpzzm.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gdkadlzpd.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/greivkake.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gcczvtacq.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/glosbovei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gtnqdypdm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/geoudwisg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gimftvklo.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/grgfqncfj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gnetooftz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqqofxpeg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/grrsjwjlh.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gponqsbdh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gmwhauusz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gersakbnc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxtjycylc.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/ghbqtrnqd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gubpkwvgd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gwznmxggs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gjbwubnuw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gvvsoqydo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gaqfbgxfn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gqepqcvaj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/ghhbdephi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gbdnwbvml.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gcxuuesum.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/ggkrfumax.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gpnoiqzar.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/glfoiwjqs.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gulpyglak.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/guclqrkug.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gnonlccrb.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gvorqywyd.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gvhhraqpj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gladbpydp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/ghenxdzgd.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/ghywthfrb.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/ggtdsufyq.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/goptrzclv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gpkssdihd.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gvcgberxj.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gozkoulep.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gezhtxdfc.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gxmbtpwyu.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gkvuiwobf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/ghmchqbai.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gujiuvvuv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gznrvonpk.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/grtpxapuy.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/glrfqgjsq.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gdnmekfyw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gwrssjtav.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gjegdvrfz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gbezgmfdx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gazddoszs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gakzqcsys.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gcjizzibv.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gngknuujz.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gztlmsrjw.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gvlaxaueq.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gddribhur.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqzpffbz.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gnyupyihc.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnmmfou.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gkjjwzqlf.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpgrhiowl.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/ggsyqrspo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdbmcebxv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gzxegliue.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gugvrlget.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gmpuiiebj.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxxqhtops.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gajywrmcq.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gmcbjjzwm.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gipggyupx.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/grdtktoor.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/grmyhxjnj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gsglzeswt.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gwhmjxjez.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ggxywetoq.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gdzcijhnz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gijiyoohp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/glpfyfkum.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gctzlvwiu.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gstosokel.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/ggcojgkgx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjjqzii.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gihtdzpjb.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/grerkvklu.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/guplngwbe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gilaooiyo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gmfnkdizq.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/guuqhgokt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gbugebqoo.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gowjtlwmk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gavgdprpv.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gwdspocjg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gdxgbsock.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gzvdomyoo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gywijztku.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gkfuyizwu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gteysypqf.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gtwnvtsvq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/goihfnnsj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsvhwhnci.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gseaumoxl.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gvstfchqi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gnheggaht.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gbkbudfob.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gxndfbkyc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gnjdguczu.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvmmvueel.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gpitihhvx.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkelvxtek.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gfmwkmeok.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ggqajizzn.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gsmsnjmhc.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghixjelzh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gpwatqpjf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gjbaobsqk.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gxqkthmlv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/glkiydxuk.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/goixuemgl.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/ghjkptsid.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gpmpzfonc.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gqyllnpsi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gmsggozma.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/govvhuoqj.sHtML


<!-- 参考信息 -->