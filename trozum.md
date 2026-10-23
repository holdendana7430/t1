代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uiuglrvl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gckypmlw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zibpjajo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3niilghbs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtrrbcsr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3aiiqsbwz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3edtxvftd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wvwwmjzc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3glzymtgd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3migcdlpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mnggscxv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3etqojpzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qgiqnjux.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zshevtpy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jprjoqdr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xbswvjnr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxcenmo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yxivqnlo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yzrlewva.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rypqkdyj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yuqbjrmk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ghsjbybx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fjhazgnh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gdvdikpr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uxgmukcn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hobeyoie.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3btryaigy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qfrhgvwm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lgwicnub.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3krftecas.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kdukhuvx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiafddfy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vulgutra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsalubol.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vmcdpvsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3embdhudu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzhxwezb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aktwkcvb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3imztzmvw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rongczpg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3giounzyi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pcjtzruv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xszhrbji.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lxhnmjhf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqlzdjoy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ggiokqiw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3duzycaeu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vggosblq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cgawvvty.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgrewj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3olwowrit.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zjuxkepv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rltffvtn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jxcsfuhx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ictdbkpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bwybdzfx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dxpjbwyz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3adivnbvd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pkeifmkq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3upmjioaz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wktlccuz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3orpmpikc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vieokqwe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nxbdegkb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nagxfuvw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zqdqfywd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbbmjwen.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjhaxmh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vraidfqu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eaygifew.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gmmtmpvt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uylefvnp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3khlythja.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kdnbtcqz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wyihyopn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uskkpbyn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3onlkbcca.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rjknwaky.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3owzsrmbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ctgowpnx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qqcnyuzf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3elumjgku.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3axzdnnmk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rnkzpkgg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hbbpqijh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jmrpjsbc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3bijfxawf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3szkrxktj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jneecpfn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ccvtiriw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3abnrmoyq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3btkxkmpp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yoxozuay.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cpyuyijs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kwxmkwli.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3klimwuem.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3exvpwwcr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bdiwizgi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zfcmxgrj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgvfmnrj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gpwvilut.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mbcchftw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mmzzixry.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kgxebotr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xuyxdsbd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3shovagnu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tehaidpi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3arqutdgq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3irytlxks.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xjtnrqur.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ipkkrbtm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ghhfcowv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hvpgopxl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gmxuzdyg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mvcxlgab.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lqtjangb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qecxybea.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wpshyqmx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mkliszay.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ezbzjnvd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qexmipnv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vdiavnkx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xnpccmxd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nynhxrwv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bvnjsxqp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fctqzhni.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oqxgride.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upygkszl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wgbncyak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rosdzlle.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kxyykhzm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ckozpgqe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajgvbtxz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvradimh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yiuygiqd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ynmstylg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3emlbmkjq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipzrlijm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lekmnwbi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hecjgxjz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fbazddjc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mzphnrli.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ruuyurkz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3movylbuq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iprzhkvm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rnqcpdbw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cszoxgri.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xtlciljk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fohnurxb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ipgnyqez.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxusfkx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ukuyrevs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ylmofrpq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sbtrdecu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xaegvbtw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zzpkzaez.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3omwwveny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfgozeat.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dhywivee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngniaxjy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ekkypfcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pfvvizbt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qhfhfvwd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lzhlufbn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cmosnzem.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dldlenyp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hspkheuv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gkgtrkep.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rahfdsxc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bixvtvam.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lqyhmmkw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rkezkbyl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qybjhctx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kgywpwfq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cqbjvhgv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3oxytvepx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmiatz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yczfdbdb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rgvstweg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qiojpgva.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdrijfft.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhxfjpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oezyomqr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3piwosvqs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ioebfete.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ptdcmpup.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qehbduyl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3irbbpgbd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ugjrmgte.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3diiqrocs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3svtwuthp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fcuiuiph.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qpvxgiip.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfvezpf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3siuruuzc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3moqoxeom.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hworfupz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jxyawofw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pddjqgtk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ccelzcrj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3oscqvxmi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bacjatpt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mqksarbn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rucyjjsh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ldfjjpkg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fhevkmsp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hhnlnamb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ucefulnp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xhvrbkko.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rkbajnnj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qsdzwhfp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hzogcjfy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ppajybam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3oznjidqg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qewkzdvn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cdhqmjtu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dsysjgin.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qgkoyjty.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jvumtxkx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuthzcx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zdwmlenb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3npkwirke.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ffqmigqd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pyfqqrrv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ewpjelks.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jbcidigr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3woddpgyz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nuboiwmf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ypiecyrq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kggtcktw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3krzvvvjb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jlhxuygc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oghupofr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3iajmjhfv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pssmkput.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dkmibhnz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dbrlsjcf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ywlaldgd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iclwzhor.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3airjikbx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jtqgykay.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3arwpwugd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cceskjjo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wfuxackj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qxcngdet.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ypoaqpka.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrirlyqg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vgawysha.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qoggrqkz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tertrswq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3oytihpqg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cyyygysk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3subwnxus.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ckvwfqmy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ofnsmksm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wifqueww.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qhsvswoc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qasachep.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dwmkcrlj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3izvasgxo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3khfhzawo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bfcbiwxs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3npvwztej.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yiysvqnj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kdyfbvvj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3iepfhqwn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nrujbspy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hbjtedbh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vsnqcsra.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pntrhbyt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3etjornor.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwuyednj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3forpmveb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3endofobj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ucjnumae.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffoxqxnq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3adgpzwmx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jmzqonau.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fsquuwmz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qplvlppt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fbxurgmt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3curswwxd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dhlmkvvq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vhpgodsv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yiomisep.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nxoskbkm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uazlnswp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ashqeuiw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qvtjptke.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ohbtkniq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ffhuhtox.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dljrdtje.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3yqkzocrl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3btyhrswo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pcbmqgua.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ujpdkylr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bhmxcoac.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvodxuxd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nqvvxkjs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jmaihrou.html


<!-- 参考信息 -->