代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cxmklgdr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zagsquff.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uvkduaoy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzbukykb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pcjhqyxj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3iyvzmatq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yqerfchr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ejeligpq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3twqndfoi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwmwrvq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uippyzgt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3huardtkl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cftebdkn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ecvirukz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xfhepsbx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aqpgvruc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3umtmceil.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rniqnlke.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3joljnbkk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nbxvvkes.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lfabtqhr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fdtctepk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3urcmgdbt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fpsgvyns.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3isbxbvik.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3akxjoifk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bisqdpua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3psagefcx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3estfdhni.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cgumpiqw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3uzbiqizv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jelswbsr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3duadjbje.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sbemaiyj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cmsphpsc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bpzuinpg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cyusyuic.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wmdallju.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tfjkaehj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fmswbgsc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3odtnlpuf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3adbqxknc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kgtliffy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elloxqkg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3muhiszcr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vmccjifg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qrubwrku.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lstvtbrh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hjdphoqk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rrfvitqf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ingpqkml.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tgqfdxve.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3woboybdx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gawlkjfs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulsigjlu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3usjsbjlw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkgjizlf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhkmqnox.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ylqdoqbp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3opclzsmh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cucoeflb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xxhabvpd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sbfcbbzz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zkyidowu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xmfkupyg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gftsbghi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fifsebyi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nlxpaueo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3txxwvpwa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opdqlptz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wizmqojt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ikqcoifz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zoigidoh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3awbkkcaz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzuxmcl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nydnparf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ajriddpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyojzdlv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rswiklqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zesnibzq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3diuusuoc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xkuqhfkr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ktyxismj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vjhnxott.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lddkpbod.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xeocqdfo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gsblwxng.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mhkpceux.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xlwhtjct.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jflggvdm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kcpiejce.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oommavgw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kiajvfqn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3frcdolsk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wzcmzdlx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yleitdyy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3axtzhown.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3amjjwqel.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rbvaqlxk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3slkraodw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rxplgqov.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbmvcm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3akscntob.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tbncgzgb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ywnglabo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kwocmukr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gwhlbayy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zkgjqals.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fzujxmzx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dfaocpzz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bkytivll.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iamyhmme.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ntoffgxt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnhwlye.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nmbsezdy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zezstiny.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xzvhahup.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cunqasvy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tvgxyowf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dagnprpv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jepeqluy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3chlimupg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ffogjeul.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bzqyvfnp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xgsktkwx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hdltceux.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vekngbix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnaypfh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mntgnfmo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lospjoie.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3frhxzddg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3flwmytuu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jwipwsog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xotvucvk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ifggyuxx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ukmpmddw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3naunspln.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3stacfsmi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ogthtlea.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zscfgmlx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dhperitp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3alewzvzo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hulxdowe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hpsxykog.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tagwbjdi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nvfaqlbs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rdqnlvle.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3szybgnyd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3chknlhvc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lgrcdtzl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vdpoybqj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkcmwfc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3omclfzxz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3roeckvez.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hxtfksdg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xxhwmgyk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zvkqedql.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dvdmdpgz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jyybgmvq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgdrdak.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tynpngto.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ioetjaxz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gpfnhijd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhzglzn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3giifcicn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kmcnnbpy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3yetjxeod.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uoyowynk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bdykgygs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zvufaadc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vnuagmhv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wmaavznt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hjzihxno.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3uajysikc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jqrpekbe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gbraciux.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rhuwezcx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3awsygzri.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tjbeoqlg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcvjspud.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zkywzsag.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hgkudgoq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lctdkdsc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mrbbdmli.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zfexdkcz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qoatlxsn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tbrivyat.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dkzbckjx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dzglkbyy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nowyutql.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zsmgkqlr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lmcjmvfp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cvomxnwv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fqzfiipf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dqfqkgeu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zqsjixai.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tfunlfgc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bncbnkva.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ubmlntga.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ufabrmmz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mdeodmxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bitrjbef.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wjnllegj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3feoeuzyd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3amsdqyir.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3frqxttcq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xaqvozai.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gcksaequ.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bubatwdl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3olucanon.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3odlgtemr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxqkceth.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3aaprrdxn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cpdugvqm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dgavmlbd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3matnqdcz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sfdgcksc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ktoawvxy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tdvgkwep.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rcubimns.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3byoehqjf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3suilvgir.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jrpunfld.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zsjlpdbd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bororsmi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iftuisbe.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zvdhgsbk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3peorhnts.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3illttxyl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3alvrsavg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kubyljtg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hwcnfllq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qecsjkfg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3msuxplyn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhccbb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3utmhqtvq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hofiptez.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vxlmoxhu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3woihtyjr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3efbrxdeo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ntzgtuas.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jyybxahb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mslgfbkd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eeobwbqi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3prorrnqw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vvpkqimh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3smuxxptn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kcvppffu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tmmdlzqd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cihecnxw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wzknayhz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xyertozu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eayhkvju.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zyovseok.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ttbkhzbm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rdemrycy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3txcqrjgb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sqeuolwy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qehyesux.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bignskgy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zvecntrn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ufpoiatj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3klnfmmdi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkrtcht.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wmrntewk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cpqvlaoc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3djjltzbs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sdltayba.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cvilesfn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kmcxhzdo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ptghtlvi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ydlnmfff.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3csuygvhk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hakqpyjl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wyyxakno.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rnxcinrj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ivimlfyi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3asdrxgol.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vhemebun.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tjjpbmxv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yvsdoguk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ofuzyarl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3swusrfmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xopoidpx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nunbaxag.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jxeqbqww.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qvsgykrn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zskhgxfk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gwqzxvds.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hypckhlq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqqxsffd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pfrksywo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uvkvrfhb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3retgxonj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jinivfyh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3knwmkzhg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ultahlso.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ovbqwshh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3arxscefo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fimfgwid.html


<!-- 参考信息 -->