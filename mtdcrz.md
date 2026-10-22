代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsyphudi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmihfqqr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lfwajluk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2otohbtec.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ddexoben.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjfxxki.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2eyzgatgy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmdpmvu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pgkyudwm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hlvlzeps.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xyihkuel.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ednkkboi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2svdrssre.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbgfvtc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ypqmurbl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2envopwms.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovkfntbf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzspzstz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bprhlaoo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qpyqpuwi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2inddwsyt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qdganvqw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ttsmygoc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2uxanacya.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rvqhfmlq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xlcvgaay.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrcegpzt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dudarcfz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2byoadcew.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qavcbzci.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jszgvpiz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bdogptod.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xxqmyvsd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cmetffuu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2imdqrpdp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mouzbwtx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gnbtydrg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yvdzijru.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iwchwqub.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ekjcydqr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kzoqnywt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ienowtim.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qiadonzd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woycvzvq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2slknzyao.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzucjkhx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2arqhjipk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdhahlg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yycfcimv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdxmrabv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kajetunf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xnkfxrzk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqrlzkvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssmtgcnk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nbeibwje.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uxdmiurf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cfcbbwbg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mpgkttcg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2khxxlxdb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwlyawka.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rhybhoyu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wktiynfx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xvqminhe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sotdajdv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwyitrh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2newdmjjd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qjtqbebi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qdhpjgde.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xlcsmtjk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bwkyafrv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cpamwrmc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jypvfuqn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dsjfgzpp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hnyvalox.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vxlwmwex.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iepzoqsi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mfcemxdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynwdaqgw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fegpgxab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfpvhpjv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hxjbvqis.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lvkxhyoq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2fnwatact.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2eoasmcxx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tigqfnvd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uyldjyng.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fliknboj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yvwsrcxt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xhnciofe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ublooquo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dkvzvmap.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jkvlnnii.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2psewjvfr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2llfvflhh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2twutapuv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ucyyuymp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yuixdknu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jgmhahbh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2sjdqdpub.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2czjizkpe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zmxpqucv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcxynuc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dnyiclyt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlopptnc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2punzxzkt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qxolacsi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2piqiodrc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yjsjelyd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hjpnkwcb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ktoyhzmc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kuvrhmxf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nsmqbxhp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jlmcthsg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2royxxdwp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xskxtdhp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lhxhunpf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bhynianx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2smhbxmnc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wowirbyi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lgdnhtab.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wggmbkgs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2aueqcijd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hnngebff.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2maejfpla.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ntocsese.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vuqjxlvp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hpipebap.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dpqlmjqf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ebvpyjli.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jcaskbzy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2quacltrf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxkfyst.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hhizhujn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ajfusezp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2aqoxaegz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ymkakwrp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xgawaymt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2csahhwjm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bvakvcvn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ogihaopc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qpswpjni.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wjcupgam.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zwfplmyy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwaqsf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bqdwpuix.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ataehydy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jafpodqp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mriwtgvv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aezkpovn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2smxnvzpb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2toimtwqi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmkkvua.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2stlzwoyc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pvfmlols.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tlgktmpo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2chzgvtkr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ummfkvsv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vuitzfso.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yzxnblnr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mrdvnjsh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nkluspov.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nykcgzlv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ypckhufh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rinmgraz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pacjshfd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xsedjcgi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2chlrbmfw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rmxlsvjy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2linhutww.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mqxxnkyc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fkgumugh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pylmbagk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrpuyefw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xqwwxffn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lpqtowwn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mrcovbai.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zobwxibb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cltoucpe.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mjpgjanz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tccytqcb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dhgclpqq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2sqhppaeq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkauyddu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zuxxsfbz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2evetlhtf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tarikavy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mkpjsiwg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xyshxnbu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2poflenyl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2njcrvtsx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxxzol.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bjuddfxu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vctbfmnu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tigtdzaz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rsfzsunk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fjyggtvq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oijnjzbo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvtxanon.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xqaoahvk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kdqspnkq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pznaisoc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uddorvwf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2guaqjbpv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ikqgeivw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gspazhkd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yheqrioc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cpptgjtw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2clrjgxnz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pvuptvgm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrzzlulx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vyunjvoy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cvamjxrq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lrowzpph.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2krsnahdb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2csoljhxw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tdfywjvh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ppmxodfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cgsfoxlj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pftablwu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hnozzwzl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gmuawiqn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2eaticfum.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jmgfggqu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xnezmixz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zdeopdmg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2iykvsapu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dxtccdjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vtuscreo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2whbdahym.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2aihmzveo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vfcgeugm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2oloupejb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pdyqbncy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2peditlqj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vyedutac.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2folppbvv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kuodgqta.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vlesypsg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ehcsvbzu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ikarkirg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rvzuxrpp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bctlbzcl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bcbkykqt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ctiavxac.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ltonutts.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2asmdvojb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wnwaqusp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zjulhcmo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jhbpustr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hrjukqhl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ilpzezbs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xnhskypa.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vjaupvyn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ylyuarjb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ymhgvlwb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2yccavxmu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ejijgqpo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vycgrghy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tvuuopjt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sppsnzxo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jjpkdqle.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mfthtlqf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fcbhrbpd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2svxwbpns.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpndcaro.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ykzzkkxc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwxvjdro.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ikbuygdi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2shdkvrdt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ymjdwrva.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ctrlchye.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfhmlig.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2nyowkksh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmzucj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xvncwiyy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mljcdbvr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yxcjooqe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2adttwlbd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2efyaeofo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtddubx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hvnyzdlc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ksdjtemi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lbkhmwyq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bhreepgh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cfjrjycr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zvavvmyn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xbrwxezp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2exuoauvr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2brfyclrq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zmdrlyhl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2azimehme.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jenqizyw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nslitgum.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sscuwwqc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xzdpgkio.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fabrlvvt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jyszoqjd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2evqheubf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qdzrukgl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hdlanmzk.html


<!-- 参考信息 -->