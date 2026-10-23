代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pjioifbm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rbobfltd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dtpnygcp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wcjqavow.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dhnnzqsb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3catxumjr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ejjkacqe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nsofkzfd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bdszzkau.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3iufnncmc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ewgwbfug.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ujeecwit.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uzcoodmg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ravawxru.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dsqjfbhn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gwwrfbik.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jtvcbfjt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pkxhqxif.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xloeuhco.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hirxgblg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3npbmyurr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3msxxylmk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kcjdnonz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bgzaysxz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qkrcbusy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3huvurrea.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ndujvyib.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sjohubmd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iziktivi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3amrehqbe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yubvwyiz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bdzndutt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3esrqwnzk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lwteshxp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pryncanl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjqgtzob.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dwaxmdeq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xxwwaknk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nnrclhwt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvnbqsox.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yvgfnpic.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahcosoiv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hraddhrh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjqnysf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ccqeipfd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zidoifoa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3quzblebh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzzjhpb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zmsssevm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilsgphrx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jejjyznp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3sdfxnpzt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qowqkcma.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wiesikty.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3utsxdaby.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qcdqwvlj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmqpwwis.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nqlrmrkp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ejnuscmc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3epvuvqoy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbzmmui.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sftvrpjr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdjvyv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dzbctfjf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3imnqfzfa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lbormcyd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhbqmph.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3leodnvvn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gceiayce.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3srxlndnm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ctejcszo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tfzzltrx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ougawyej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuiffbps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3togrblug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vapxrhuh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vjbgqsex.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gytpjuky.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3uddftcpu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjzgyneq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hzumqcmg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxvotxv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rvpjoszv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rczawpxm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mlrzihpe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jijteanu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rbriazfg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nqowegdv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3gylnjbbt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wppopvcu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xqokbbto.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kxobudrb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3upoyodog.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xabwtoqm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ethmrngb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mixhpoxl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dnzedsyf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htocvitl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3twadnrye.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xykionls.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zedllglr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vwdtmoce.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bpfzgefr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hnyizspk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3arvfahup.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yihjyqvt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vricxgia.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qykvusot.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzazkbmv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3aszbddqv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tpayhhuz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3srlcbded.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3teiipran.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3keovjecq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ovrukifw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3poyvxaey.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fbrkxxlv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3whfonplp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3begnkure.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qaqcdonl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxfpuobo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rdwkgvgh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kwpksxxs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tokafvjd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yfbfxomt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wxeiamzw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3txjpeoby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zmgncrwy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3nwxvwtmd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ezmdkihw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wzuijymv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zoatatao.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wbjqkygx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qkuhdzck.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mefyxwvu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ugmnzbxp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gnvfpogf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zqnrqcpq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ninfvhuy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fzmmhjfi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ntpiamzl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kbtljvjz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ygtigwyi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlwpzon.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ndopdqoo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qlgosdeu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3npusxcio.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oadqacxh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lldzvusi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3beubteqd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lasnftpi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jyjfwptq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hpzkuqii.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3gkgsfwnr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kiknsdmm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bktgbobj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vwkqlxvf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3difpbrra.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tedwebnc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljiljgmq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nsuktuft.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dfycfokg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkfvwiom.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dkplkwyl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dkjnaujx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqywxwcb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3trntbuad.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hprthbut.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vjymntrj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ypjzosqa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xmmlfist.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ovmxfznj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gkhnldsm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3eykyysew.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wxjqziny.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbhgxwlr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kiontdtk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ivtpindy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jymuektx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rsibvtal.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pzyhdbqw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rsidzixm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3feolulfb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3syidrdlu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xizlnstc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dznrihlu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3olvmtimr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqmjdkd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yzfckcew.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tllvntbj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hnawvubf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pssfokbw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kiwxwjxn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oskjbfwk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bvcqgfdx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yxdlshyk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3knrcfitr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3akenxjwn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xuaotuov.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gqqaonni.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lczcjwox.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gwplcepy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vbjwzejd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lgnldtsg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kgclknke.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vaxnnrnu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zyszarpp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bycfvdrl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eugedvah.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zpggfpnw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wgycbeuu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3flvhmmpv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhnnnhup.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aolmbhhm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sqilkrzd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uppiaqmd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lgqqihgi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ctoczebb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vjetnwqc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vqlnsyfp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3stamsamk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qhmwbqhi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fijqeujg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wegvekir.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rbhjeizj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rhqcdxgn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ntpkkjpr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzmdpso.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rmmscggv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jpzvtzth.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jsgvvmnx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ixmtoqrc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wibenvny.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hsghbxei.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3znvabyjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gdjnllij.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jfuifvyi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3eljpmtyh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kaoogewp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fuzyuxkq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cpamrenq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rwwwrxfm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3msgsuwuk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3toknnqiq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3feoxunjr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cuqbzked.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qgdtssfy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uawgzjhl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yxeginet.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kprrgcgz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mdcuwhah.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kaywntqv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cdkultrs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nwubzmvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3nblagfmf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vubhhunk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fchgexvy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cupkkfhl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ztczmevb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3olevviyo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmrzbfeg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ewwmnion.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rmcbwwxc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jwmnqdcx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hgwuxysr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nhgmhzwk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jtgbtwnl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgopykop.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kbdsksjk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qyarvmnu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pmrkjylj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rluddkyy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3atlkkczu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zyfvhteh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cwsaymvc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zyeprzai.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bfuxigml.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3eqxzegih.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qrlkuqnv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rvvqhlaq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lyffrguf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3larpfhjn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yglrypxw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uanbkmxt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3acxdsygc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cgxrmlrs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3akronosg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jstbhwsr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mobdopat.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3apgcfufj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vydjwfmo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ujftfuju.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rgapwplh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3khcppqtu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oenfscja.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ilodqhvm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vrhclgau.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nkibenaj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mwpecqpd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tkhwgtij.html


<!-- 参考信息 -->