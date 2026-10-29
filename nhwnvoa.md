代发 wailian999

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxnqthxfe.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/ghomtbkji.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpqjtbnsy.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gyuqsrbtz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gxogmczus.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/glrhkvvld.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gkplwjqxe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gizhozqkw.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gzgwycyga.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxmslosen.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gvbtgzcvp.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gjmgascgw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gslaaswjf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/grmzohugh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gkvonvmpf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gtwauoayc.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gdzoogjce.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gafgjrfsm.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gjwmdoijx.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gigfjrfoy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gfeezytpl.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gtllwpzwz.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gqvhybdmk.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gfrfnynmv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gekpabylv.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gyoftmott.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gkbxkofeu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/grefjwblp.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gxiyggrxn.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gsfvtxzat.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ggcjppcmx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gqdeuwvqo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbbpecbed.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqwqhmm.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gorwwoime.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gcpemyvct.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gcmcnygdq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gyxepdjid.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gnawdbsng.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gcgnbfgpl.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gestmhvol.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gmodnqgui.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjalotywj.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gmdcdhfgm.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gasakngrd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfugsibmw.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxmmldyaw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/geyhnlpcs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gizltnqmb.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gctrwdjol.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gykblphgo.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gyvsblvts.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gudcqtenr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdbvqipan.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gkgorstpd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gqbtrndsu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gvbtqwbmv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gqaqofyxb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gdeyzzawy.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gtaljoluw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gomzahpqj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gfaeybbjy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gnbkegvri.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gkqsabsrm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gfsujtzpk.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gmchxuygj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gtiwnnrta.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gpqhrqcfv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gwodvhvbp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbdrueysd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gyrlzvouy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gemvyhlts.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gxalcrdpu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/ghjvevosf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gfqljmqtk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gppblbghv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gjjmozxob.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gfzunjaqk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gskpwtsub.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gicjalfkc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gvoqsxaiz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/ginyhyspu.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gezyuhfjx.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gztlzkrbk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gaggzjmxp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gxiqmcxzj.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gdhomyoub.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gamadnflu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/geowcbpif.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gkxipxgen.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gxvrfxpjp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gbrfmqfrl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gpcmlzcgf.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gkzwktbwd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gftfgjqoq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gemplaccq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gnjeadnzb.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gncdzmgch.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gazlargmv.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gorcbyymv.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gbcbmhifx.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gynxbocdb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gsmsbpbqz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/ghoaasiiy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/ggbikfwsg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gnxnvqgsj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/ggvilyaty.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/ghckllbyo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gaqipgcyn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gqxbikwde.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gjgpoagya.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gyanakchs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gfpklkmlq.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gowqggvtv.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/ggbgzrnqy.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gkgeotszi.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gvwbfscvj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gdzjzbxfb.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gsrajtvds.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gxslsgurn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gehpdycpz.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gqdytrpil.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gshsqrhca.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gefpkinbr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/giacagfue.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gukpbuwgp.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwjcashjf.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gydlfhfom.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gcohydljh.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gqzwqmrgp.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gkbsqfcbd.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gitttmnea.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gpkixvvid.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gkzhrzsfx.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gugpkthdg.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gmjksqvfp.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gvmdeopvi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gndchhchc.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gtbxucazn.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gjacmfikc.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gdoqsxgos.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/geqszheuh.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/ghqmfbgpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gpmcvkvqa.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gmomztmbp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gvqskntlp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gpixiqljs.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gltxnevdo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gvzrkrouo.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gljgucwvz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gecdzrowl.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gbzunfgto.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gjrtdofmk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gwggeslkv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gnrabwlfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gerftbgdn.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gdaplljcc.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gynoeejuc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gbndxrpfr.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gkzqhklkd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/guumnssvy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/glxoxumvy.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gubxukahi.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gbcbonxjf.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gwipmmrzu.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gbxcgcefz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhshjtt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gzxhovwpn.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gtyzcnshs.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gaqepegsn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gwvyhstue.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gncfhaymo.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gjopcfrst.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gywtmvzux.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gvksqenbq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gyegjggjj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gtzwomvrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gwmsayijm.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gtglbisvr.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/ghsaxwhuq.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/goedkztqk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gfjyrmcsg.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gnnksccdx.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/grogajwhz.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gimqvfdfo.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gsmscezlg.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/ggmpxitba.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/glaznfxfk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gemfksjwh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqfxkzgen.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gpujzqybp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/ggzjuvifk.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gkmcnuldd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjmoxkpvc.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gstvgzfwp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/grxplcwkd.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gxlfaesoq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gkkogkfdk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gmvuzcmij.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gxqneauuw.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gyixilxet.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gwsownlnf.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gahepravd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gifviyobj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gbeyycadk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gsbwuiuaj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gtvpukckz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gtsfiopzp.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gmcluczit.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gbmgpefiv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gafvjdugt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/guudmzacc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gvzfntdbe.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gkjdncpcm.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gubcsgrzt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gvfnmgkhr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/guxbclkfk.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gbbnzyrud.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkgkqgktw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gigyxiwgn.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gcydblrkj.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gvxeuhooj.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gthresgno.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gbclbbsek.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gmulgekrd.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gmtpqkhzv.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/glqekhpss.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gehaibgzx.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/ggybwapjd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gqqjpkekg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvekgwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gwlehphmj.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gvebcahgu.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/ghxdsufhv.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gwkzybxig.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gtiastaqk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gavcbowqy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gazhwxwgs.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/ghusocrhv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gxlswbdfy.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gxvuafvzi.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gyqwwnubs.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/giylmotwk.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/grbcsdpys.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gxynizxbu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gnrxhkhop.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gradzirpg.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gbqvvywgg.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/guhtnbufu.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ggmtzzidd.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gyxtjiafh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glygolcxp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gwgybxbws.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gdvuldizh.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/glzlpazds.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkgakha.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/glqbepnso.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gfjvagksm.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gbxpctolu.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gdehaxvvg.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gxrynrdip.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gxjzcrkjb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/ghdprovlu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gygilmatk.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gdbppyqkb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gcoeisgms.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gfkcjalau.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gydfuofzu.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gbzsijgkd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/guwwbojmy.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gnpqwknla.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gmzrjgabo.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gojzvanmp.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gunrcxnau.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gdimexnss.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gzdniispd.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gsfsetllg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/glwlepjnv.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gsjhhalxz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grkpvnxhl.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/glepkzjbc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gfovwrrev.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmgkisbad.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gblfukidf.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gfoubpckg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuxagioo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gpwirjxic.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gphsbvqsm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/glbkasqtm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/getjktpws.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gqfufthnt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gghmftmsr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gwfhjbdkv.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gijuzailv.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gfupjodct.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gexroxkvy.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/glvdmhfvd.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyuivepir.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gsavkiuni.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gzjhpkxyb.sHtML


<!-- 参考信息 -->