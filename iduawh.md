代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2grzxarfz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zyiysqxw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nyzpqvqe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cargqiku.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvyueqc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jyfhdaxc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2truvzcwi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ptkmshaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2myjlizli.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ddhmjpwc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dtolzlyz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hbgwdgke.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2udxrwygm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sipkrwln.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yartxyxc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2buqepdcl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iuldsrtq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qkbbzpzz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qsmqmvme.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bgccacgy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ezszzwop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klhvybyc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rsqsrews.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsdgbjqr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pkgcawju.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mzqokyyl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fdgqzgre.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cubxzmtg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xvvvfwgk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zsrozmbb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2okfowkmc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjxqfcwl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nyrqvxke.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cmlmfvmy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2noecthkd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kpngnceo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uhudrhuw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdynjdy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aminkyop.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vinwltni.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jtmotctq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wlqyqhwe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2emjdditf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nlualyqd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2foddtmbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwkkcqf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnmfvc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kafnvvsc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hbjknjur.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytejvmhh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lyxutqem.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vorabrxd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2plhiyphi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ygqobhmw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzxzaalq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xaqjgswo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ksnbnssc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fegsrqrz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fvdwxlym.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2djcmqnng.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lpvckbee.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zemvllrn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jtdskejt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sahkmzkw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fgciupbq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fqajapir.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qkmgvfdl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2enzizjuv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aynhpyed.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vndfpyyc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2eyejyloz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lueyyeox.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2edgqlmtd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jremrxqn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tcysftkp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzhhtwp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2awgmstbn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wgxaetcd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cudmsyvu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qgzdhlgt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ispgabyu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sybkdspf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hvhyuxja.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2myfwlskb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xcstswoz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uqdsumea.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bugifwkj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nmjjguif.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bzzqmxob.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2eqliqvvf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nuvgoabq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gqcfwsnh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2whregrlt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2amivqcdy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2srljdcuq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bsmxqzxj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fwaiipjr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uyiitjmj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bagyvvsv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wafknxio.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pxpwrqai.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ntkyfwed.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bilguqzn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cbwyigjm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pcjilzca.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xrpnduab.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2soeonlxp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wbiumdwg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hawsnmdp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dfifuizw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lhhabldk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2okyusmyc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2guicvnxi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2uqxoznfi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xuzbwfif.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hgffatwh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pvimsaph.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcdjuydv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wyyreony.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rksrmxoq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nxtkpklu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bvqwmpqe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zomaepst.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rtabxuoa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vgsztrov.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdgjrrfp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jjpspxqz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfnbkgkn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2siooertn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxkgyncf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zgholvvc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ltwidowe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ygbasilx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jruugbea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upwevsvb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2szzlmjvx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dubaclmj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vtntxdsd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqbpykps.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rcznnsdm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2noxhnnon.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ewriizfx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kakszkmy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2opzwrieh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rafizakk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqzkecaq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkroicwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykbotvel.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uqnalzur.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hnngfqdd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2icrngxcy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2esdzklyz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kkhacudd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hdvxxfvx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gwievilv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ginrwche.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vynaqcna.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wndgsmzu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jqkllarm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dpweiadh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kjykqlwp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2udbfhgko.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rdqpxtdi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rizvbcwe.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zkoonrzw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cnfwllil.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vkxoystb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xdypecpq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eypcvbut.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdxrzfv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pvcpslfw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hnhmxvtt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hzkiolpa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qckpbhtv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ugnwksxc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mqeawapn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2txwkusbz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yjaqvpal.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2aatoczwk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2shboaiog.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fvrtksxj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2phpdwdfn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hcuypzbd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gepcxlcr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jytfjsbi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvdeish.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gwqvhtij.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hovcbumz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2anunwucx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jepvyhlr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jfpeqvtf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bidmcxbc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkoipfrm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bmnzwvql.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bevjlzjl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dkhwkssu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xofroicg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rseriijh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2biwovodo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lxylzarw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eerifpvj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bfqkueyf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bqkyutgx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rtqxrbqb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vwuwvxig.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2iufjwwma.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sfrydzcr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kaotohgw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ttchdpbe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mcpoujib.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fdcbmjtb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ogtqfmiy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yjmwfifm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hxbmpsum.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wctgnccd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkxuhwi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rrwieixm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kvxgofuc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ltmjogrn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2oyesxcop.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wfklcwjx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ompomheb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mgkmzrkv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ezkisvoj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gxvmstqe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jzqbscsk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zrfiorfx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gpgwwgfj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gnavjfra.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hmnoqasn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dnvnpcvf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2toozyfnu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2drioxira.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2krogttja.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2upythrab.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wijhfygh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2whnsricw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rtdkmqlu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2oukpuskm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fjbfjlzh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmshctuq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2oqgvzqho.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xkygintj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2huzrbyqq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mgejaafp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2orefsbzx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dfuhpjzq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2katwftvg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ojcvfhkr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2besgdyab.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nykyxthb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xjfpqdlr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dlufryry.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kyfytvgf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2btodgkmv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jsryattg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bnryqusl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rbcdltsa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jqayhkmi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mtwdgzoe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xtetbjsz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhstumwm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2caislbhz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rezhuhyi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rugnddqi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifnqcykv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2axmgtlxx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2beywhhhi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2misadsiw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxdvotdj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2eierkyhc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rxtgnrfm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qsrbomym.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ntbpjfqd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdkdsnim.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tvxoewia.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wwbtqshp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kswwifdm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cnllatnx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oesfnedp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2aonixbdd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2idmzbwjw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2oemikvhx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dhmxdmcl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2apyrhoct.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qvzuwlwu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bzyieqwf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zvvyoiqg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wnbbrynb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2podicjca.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kjvpvoqt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wzbbxqtb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xmcperxu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vxhsojlm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eedtvbqw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ngsclnzz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2khmpagth.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fdatwyuw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jzvtmcpb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gyoybqtd.html


<!-- 参考信息 -->