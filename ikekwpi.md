代发 wailian999

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/giwstzsfg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gtreqjriv.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gbvdnnvdf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gvromohky.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/ggvqldspm.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gxrzfacow.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpshqtpsr.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gvbkirark.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gxbsjwwas.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gbbozmhrj.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gbwbmupqb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gqkdhymsk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grqkxihjb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gxxmatvmg.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gyfgazppz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gvomluzpr.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gltrxaluz.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gzuekqeom.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gmsdcdcqb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gotmqelty.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzylpvypp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrtnwmrf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gxpmcugpv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gqgkatbbl.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gccpyciju.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/ghgicnglh.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gwbnehndr.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gghqtkuyn.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfaowzciq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gunryipwr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/getqnkbnm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/geodufixw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grycfeqah.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpnmbqbli.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gyemrbppx.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gndmpxfqg.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvhuocpjw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzdzlprxf.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtqxvivew.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbrmxjilq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gavnpyrjy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gbkghgmpz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gprfiquca.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gksqtjcpq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/ganbaygfq.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gmkrozavd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gzabunxfj.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/guyjdfuxi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gzhhkjndn.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gutmoukth.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gzgqxmprz.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/ggwdgfgaf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gtlyhajds.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gptbthqxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxrubarcv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkchwhycx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gnctfckhk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gdbwyjflf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gpzuzcudl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gvktsvxpw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gifaztrqi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gvrmwmzqu.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gwgtqsxhc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/geynrcdch.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gryznsvvn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gielgxaki.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gyhwxgiwo.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gbcnjunar.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gdsihajnd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gljrzmnvg.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gcikvzvxy.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gnisyevvf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gygfvhvyl.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gfdmkrjoy.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gskcqavge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/garbnyssa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/ggrhnovrz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/giynvdvwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gtmbyitzc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gzxwagien.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gbqttkpch.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gveunjhdd.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/ggrdrpjlh.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/ggexzqxnf.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gkwpgoays.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/geociwoqj.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gbifyggtm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqpivddhx.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxugxce.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gejyfntnx.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gjjxuvlbq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gxscdvnni.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gzxgrjzdw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gdxfgzxtp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gbioauwtr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/glbtsqwcl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gqyelcvip.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/goroojtky.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gaafosxok.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/grvkeyhcb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/ggqolvgty.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/giwbmnjwh.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gqculflgl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ghinpuxac.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/giuwgivav.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gqdgxuiya.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gqlbpcmfy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gamyhlman.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/ggnpjxxtd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gcaxatzct.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gtsstbbgv.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gyygeswdn.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gykpwtenp.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gzeqnfcnu.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gjowreoym.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gjykwnozt.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gucvcpjxy.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gyawxvunj.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gzpfdsfoj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/ggryazbut.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gidmkhqwb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gxetrwxcf.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gsqhhgdhe.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/girtncctr.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ghdbgcuje.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gvucuckfk.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/goxpixqvi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gnwjurgcw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gdvtasygp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gwtlqrrvy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ghpmmmrrp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gopiskdre.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gxjzqfafi.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/ggwishkrv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/ggbrnjocz.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbrtfmkfu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/glmeayhsq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gunjiiglk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gvddyfyud.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gbmkdmqaq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ghisgkkmi.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gsvysfyfx.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gdgonmsvz.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gwcswflee.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gunxyqcjn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gykxgplkm.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gifglrpix.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gjxitzgbs.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/guftlifbq.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gxkiicwdu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gefzdkxlc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/ggzhvtswm.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gvrxavyqr.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gifwqykau.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gkvxasxms.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gcxhldotr.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gtjardzib.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gqlgjqaqb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/glckjhgsv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghcjzvwou.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gcmyetego.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gsqgqkclt.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gktifqcte.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gxjlyzfdc.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gqunlntjp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gegygtnhg.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gzoxtcqxc.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfnpczmnr.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glaloxpmi.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/glasimdti.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gldffhpbh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gepylblxp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gjjdfvpdc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gccvewizq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gsoyqdxdm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gjoiqhwts.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/ggvfmedbt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gjcfnequd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gggvulrex.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gfqvkaeoj.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/grbwzhenl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gytfpeciw.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gjvpoczcu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gzrdqlxaw.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gwykgtfqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqpwhoszh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gmmtqcjnm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gsgrervuq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gbunumrey.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gktddwfcj.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/geqqujaks.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gqtaaiude.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gxgafcamt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gncpcsclq.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gcygccxha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gccynfrxp.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/grqyikwnl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gwljelfhd.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gcjlhoudm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gelvtdqwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gykrxgpad.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/ghtkzorog.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/giwsugbxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gjqjdjejd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/geptjruhv.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gupwspwam.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/ghcckfovy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gaplbijgr.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gihyoljer.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gnzomgrgz.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gvpylceij.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/ggwcnouwt.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gjcykhldr.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gkfpvltwn.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gtogtukvf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gdoptmrsv.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gefsgviyu.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/glzrzphhs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/glqsbxqut.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gmyppktxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gyhfctfra.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gngvoyozn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gnrnvgxwa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gflfxvqbf.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gfeotpetl.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gulwmbmxx.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gbmiuqqza.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gvaasycxf.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/guiqrmrog.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gzisorbfi.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gdvhbybsp.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gqzpzthhe.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gpiucjlob.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gmoofawus.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/ghuwanldg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/goapzzrib.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlbuvvl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gxqyfeoeu.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/grlnqdywj.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gasignxdv.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/godlxxyak.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gsxmixnyj.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gqecfcayd.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gjaldfqvx.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gkopsntos.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gqglhczcu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gayjpqacb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwydmgnpi.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gzraexeiy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/glwcdayoc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gfzyntcwt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gxpxaodta.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gzuhtmorc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gvcblnuqm.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/goznldtuq.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/glgdkwgor.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gqgdsgibd.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gicltxiat.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gaxafxmsq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gefjxtdqr.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gobdnshde.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gogsctybq.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gwpuzwcqe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gucxjgrxn.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gwsiovqmn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/grbkulddt.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gjqnhvghw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/guyipkoxl.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gobvyybsy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gestxpdvp.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gdgqdiuai.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gwqtmhkqn.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gkisrxqvy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/giwsbgxfu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gjbzjzmzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gfesidrpc.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gobjjugek.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/ghwytvvrp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gycgtmrvv.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gknrygtdh.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gwhmxhlgs.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmtjwbdsu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gbbkfrybd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gfsucqovl.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gysgphawt.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gfefigzim.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gefzeigrp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gmfdvwsnm.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/grvawtyrl.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gvfeabjas.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gboswjurr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gdicglfyi.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gbxtjuynj.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/grxbctpfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/geqkkxwkv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gwukyhtnj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtxodfoao.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gpnpltcus.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfrhaspaz.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gojgpwmyx.sHtML


<!-- 参考信息 -->