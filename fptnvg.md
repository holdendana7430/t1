代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tcbddaed.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bqugyyzx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uxqsxhsb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gedafcif.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jgbggjap.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kfcawhzu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vwnqsxck.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zgjbaoao.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vbrrkchn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhynaek.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxifqh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rweyluzq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lxobtsxr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjutulfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bagmsuzb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qinozxkr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wpchlrhb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kesmexcz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vrisbbyd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wcldoqyz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3amhnocqm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oyxchxob.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bscpzhux.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ezjejqxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwmtqpb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bowzqkau.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ypmrftnf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3crzklmou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3otftkqiu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mmlanjtp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rulpugik.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cyqjguhv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gvxhniqd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uiclqgac.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tfhmpjbv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cezcjgby.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3huwqrfmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lngcwdrr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wrjigecw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfikujav.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rezjqjse.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vddixorf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3eksgfzcr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3veymffzx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kxghjwbk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ixoslhzc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3drfanreq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bknvxvqf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3awrqgefg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ixhdqgnk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vgqsdszb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cqmvmahs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kbyzqzwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rsrjpcpn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lgfjuxyz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ezgnvyar.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lfnlwpds.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3puigulph.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpltjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3faziazze.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3guntepex.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pjacabhp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yezhzmup.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oajcfsra.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cffrwcjw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvlvxkv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gaazvljd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ldquokpl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xiiqdcht.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gwqmikeh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jgpblvow.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fvsfqgea.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cfdmexcm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nqcxzprw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3amyyagdi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bkrllftg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3elvvwrfl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkunvnb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mhsvfxii.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nxeoyhsb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udeuotgm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nikyqlhk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cvuiroto.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nnsipvoy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlevsabm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3iqswujwa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3trjayezr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ywpsvnhh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vazuqbev.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wdoemare.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ueatukxw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3urcemojj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xlmuubbq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3axjpheye.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ajkwcidw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ixxckgwx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lfbphjxv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hpqglvdb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kbuclbxd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3oexuhpbu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgadacyl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xitferpw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3eqdfdozu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rflxqogq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3frgdtpmb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cgesypua.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jnooctmo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3exxdkgpg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vxymfetq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3drhzhlve.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3oaawwlmv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3fozptgrq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hfbcjtyr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wyzpmlyh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hduhouzt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ptsowbjz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jizgtpph.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wfpydhmg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vtgmqlhy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3asuzwvlq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyncsgpm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3caukujsf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iccgklkk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jijxrwjo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hxbgwgqk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nxnwuliy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fwnoykok.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kewgijjr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ypcweimb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3obxltqoj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3utblkcor.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aljqmxwl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jmmfjajx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dqyamnmg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpmcsfqg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pmrrjgbr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sjfffhhq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khepijwp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zxaagclh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pokfvnip.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jrzglyxc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3stgmlykv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3smrxafxr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fszncyyr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wjnlsmdj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ojwvdyqn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jjtjqrjo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yxlyictv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xdxdyefx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xvhmjytn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3egipmmfj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3okiqonxz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oifzehlj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bprdcgdb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3drtwecxz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3clnhdtok.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mhmntkkn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tgskdtfs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3irttarvl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wiwelkfh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zygyhpcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jciejxby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3whofiiva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljbohpjn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dfckwviu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3coegdlyn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ytkkgqng.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tdbwfdww.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3weojtvef.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ifgzwthn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3goglwqhi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tuoaqnwp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kruvrqpg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jgxxxhpx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uiivnrtl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vcwhadmr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3dvnfwtkp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3upbllzac.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xnerezqq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ztecsqhl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qaigsyyx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kjpughdp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ufpksplb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ktyjobti.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lljblhgj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nibgeoua.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rvmwjxzp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbiiwyk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wplmkvgx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wyyaivot.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3acmlezak.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aroxpugs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3aikfbsrv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dchsmpem.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qbwdgyxe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gyelnfak.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hfdyxsfz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3knlqcyge.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ybwgeweq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cgkxcwek.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nogxyege.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixftecip.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pzvqlpgq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cflffnmk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3eavpqkqt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nobcjfjl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zoislsdr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gxtbtzou.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykawnhtq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xvxwqbgf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ioximqki.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hapfvxwr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3maxzfxcp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3csfhnpfl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ldfqmwcw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgeyhmn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sonpjwog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tokldmrd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3csnusjdn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ahsdjlww.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ryicbsve.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cnxfaagr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eokwvdre.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lfmyaqyh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3btwauviz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tzdhxlku.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tkxnombq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rgjzcelz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iasvvufq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3chrwxhnm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zzswewsc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsfdvgr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mkjcsqja.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lcigworq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bpwoqsac.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nndupdpu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3aobxaivz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jupquvrn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3dmrvlmce.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cqnwitlm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bvhyyetu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rukmqtfw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ysqkjkqy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbhfejs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ypiktbmf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dfokugtm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3egnhxbsp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tylxhpnf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3npyfiwsg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hepoqiiy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jfavyshl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3imtgbdkw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhgfibtj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3duhkirqx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xibmuray.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jwqhtdco.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zadqqlge.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wmrsnfbq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lanocgov.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kftjtcws.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wopkcvuk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ijuigqry.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3twxrftth.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jafgqzzv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xsvbxedh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wfnzibhd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wibjqcuj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3advbeltd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3cwomojpg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3etkvdagg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uixwwrjz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3oamaqlqo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rjjcvldi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zkwhuyoz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qlgfnsxf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqrozgej.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zxcilbwd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbstlegk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zcdzrtnb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wxyohggq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3cydciztg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcjnpste.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nxppjwpi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hxrtmsho.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ishqbyoa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fozukdsl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cjzfwjxw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3btqunmwm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dnnuiyrc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lrhzzohp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3szpldmcf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vwpsafvv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qoyxkkzw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3slqkueco.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mzotnhyc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zugesnys.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dzpghygt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3otsjfdso.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gxjiaqre.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3knseetfw.html


<!-- 参考信息 -->