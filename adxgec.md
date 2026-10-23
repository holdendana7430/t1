代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3svmnuexg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cxkmmoxe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vjexaalo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fgljwvvb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxdefi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3apamansk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vsiygjze.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mympnzvy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wdwhieky.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jaikcisv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mejqouyk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xplwzrji.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ezangdkn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bgyfcaes.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mofvdqlh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqiytuf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpcftwbn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rwjgwrny.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jxrvyqfz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3scmjlftr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ajmrciwz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bllvacro.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tlbnkltq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rulgoxzb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3djxinnip.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wydskhju.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hkiwwvai.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xtelsjad.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gyfkmmtd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3opxfnqvy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ygvorczs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jzrakjxs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mpxxzabs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pvcentze.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xqkcggyq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3sdvwopcv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwqgterb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3clbzucnw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwwwfipt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fzrnquyr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rrnfaonp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dituboyb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3exmsrsdm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kbvfgids.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rmhdgzjp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vlcgnyxu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tugtrgzz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlymuey.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfazfa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtfvndhv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hunafatn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mewjvlpj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibkjhnsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qflkpbxs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bctohpvj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3agxdofvl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wullymyu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmolbdpu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3biijqxgt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyuvooku.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ylzoqtie.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qikwysuc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3axqapyul.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oglhejxy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rhsfumep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kclaiygo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnagglzx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mnzirokb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fgliseps.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bjkbicqp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qhpjucvn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vjfriaat.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tssxvidd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvjafpty.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhcmkxe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jlhitzpj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lkfukjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtlglcct.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yyjjohfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mheivtti.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rqnhsygq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pvuxmzjw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nroxrahe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rbxvptkt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ihxlzmwg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tzamwdnm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3eqtqddmg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kdmoeokw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kjdjemls.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fvefgdht.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bwdogbky.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ftesyfcr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gxihhqof.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qnybdgpk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gfuokytu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kviecyzb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ntskyeud.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jaznmlsw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vfiesobj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3apxzswtq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aeokguyb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bqzkpmea.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wpjtxfrs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tahptapv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qzhxeghb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dhuvigzs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pswfhmht.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxdlolb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pkbpbxzk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mqjrywnx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ftmotgqn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ughwjsil.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vggauhhe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3efjbqlso.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rorkctmg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mbvwxlvu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fuzqfcvu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3raavxaff.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tgdvzusu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3thsbhayc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mpcjtwpn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oimjqgqi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dzhycnmq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3phnbbdro.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjlphsrq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gikwtfrg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3incneerx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wquamwgp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wqzhlvii.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ekeeprzi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kowtgmdx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zyqzlktj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lsndoifr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3utwpsanf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3erhkhgem.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mbdpjkit.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3htbbibej.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hafovndo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yzjxjmjx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jtlfctdw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ddftgjyv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gxqhotpy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ejrczfqe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ryezjgza.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zsycyvbv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ujttfctq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xtponyyv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3awurkdxu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3sqkoutjm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3arhvkeyl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ayemudrg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxyakes.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vbgmoier.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ppxcfyyw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3anjwkjmb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bozcutyb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ckzsvfiv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hbsabfdt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3oelbwolf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ovndffqv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ssniejlh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eepvdmne.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3thehpliv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bmnblsxw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zeofcmwm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3unppsxmn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ifdorzbp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3txtmrvxo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tirhqunb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gocjbghs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3njmzsfsu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3snewzzyc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sptjbuwp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pswadznp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3unwuabov.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmzocfnv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ojuldbgy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zygstzbr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uyobgngl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3coilwifu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkfmuv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tqpcomgt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ghbiazjw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mwmhzfqd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rljhiify.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ggrtwnmw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hccznysy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yqincefi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3urnggxcg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gooffqcd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3geyxezfk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evtdvpwj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3quigdypt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qwnhkxbl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rbwtrawi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfvfavvs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hlfhfcxp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltuhkvec.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nenbwlce.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmciued.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dbkdsubh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jknzauww.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wrvfpprf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3iabsiaxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vgltrkgh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3etpiyrvi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yvltujpm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pcmcffxs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dlwdokpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yyybildh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dcoyydmm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3stzgqhof.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bcaweyro.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kqitoylw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ltlcyyep.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ywdoyuqu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xcipmsyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3flbhsomm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3whgobvmx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rzntdlqu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mduehqdx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ngpdflxa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxjsawpb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nvvovhye.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ynfiztag.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxtkhsk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3axpwgrea.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qxfqlfpn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pcpfblib.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pukxaoun.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qswfgmye.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yymdjudz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iqsvbobv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wjirxzfe.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nofnzyki.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nunlhoms.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3orryddlx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xrmixrle.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qufdhluu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pyqmqrks.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zxcrokdg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qqjdjrbq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jpsrlstn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjmfkrn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xjqgwqzj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fzewiorb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yyvcqayw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qhpnutzq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jtywdckb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3naapmfnf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tnplcuzx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wkmtsyhp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qtplueku.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ojwdwwhs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kogxplvc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lctjdjgi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qfnzddwx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uuxdbxhb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rdicatra.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kleyrgxq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gccjvmkb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vrlfcvdm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bdrsdojg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3szayiiik.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtwccwwl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mkitvqqn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gaetqvwi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mzxdjxvo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pcccqobi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lpkznyje.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rndkkqft.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yomzwber.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3iwenqoju.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pdchygnw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iannsgsh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3omjxkges.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3cqwpsbtl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jwxrjuck.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vyseegbx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qjfxfxal.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bopayako.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hojoihmr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3iokijgjz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mfswlftd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nwvqcjal.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vssqbarx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fwzelced.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3afxbwaxy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gxkqrexr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3yfwwqgxd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3csvthjnr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wgujiock.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sgcnmefv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kpobjray.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rqmlnxoo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vnpjflwy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eywnolly.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3olhydwje.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3swzolhga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3usumfcdk.html


<!-- 参考信息 -->