代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nqbtqpen.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2baxggfmi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hmiqgatc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nujoqgef.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qxllqaab.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nveqzfok.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2esmmfwiu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2embfjhqh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ubchocok.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ecokrofi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qllqabdq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ejxpxiwk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ijfakrif.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dbrcmyin.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dshrexnr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qeubcoxt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aoslucdh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2odhsbcha.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kinewodc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wwotvnsk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tjnolpib.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzrfanw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2khrhdcnm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hexjerdv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgzvoz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kjsbsvyl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zpvhmrhp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwoyfvvk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jrnqlspc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfewbtif.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eeyljzcp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gnijqpfr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vvvdudag.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bpaiayug.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2inlnhowo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dgdvjnep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lktorwbm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhhlzqks.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wtwczplt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yyifavpa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmmnttf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ulzyxxoq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bztuwlfk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sxpnplqj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vdltlsiy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lksljdow.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwaicq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vawbxaov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jkshzede.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cbrptwjl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zdiiqkph.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ddwakipm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2izawuxvl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zovbaiuc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mhnhteaf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ggrsqvrv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kvdiomca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztgdkemj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ghuqrqka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxntzijn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2liztzenw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iiwsdbcp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2clalrhrs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tcqckdjx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ackdokfv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2opfbfowj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gjtderry.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ecdtecow.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hmzyybof.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gthysmcv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gtajyhys.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iklcgqls.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qbryxwlo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2slmvmdza.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qyfxrvgo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dqckzxvr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cyyswmdf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fbdekzzx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pjlckhwm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rmzcrecf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ejclgsaa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gjtijepi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qtwxloxd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2krhiladj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fvogcgjz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2foasurzn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2leiypycp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoixezo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wantvndn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aasarikc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bjyhcdjd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zgkxukkk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gozmdgcm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cldmmpum.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eictjqbp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cvhqcljh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pfhakvlb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bmfkaduc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fcxxjguj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ttziavzf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjrzzsga.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xrsftmvk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2aisohfra.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fsrthybe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uxyeyygb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yygqzlao.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2umtgliky.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2astomnsl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2utxygpyk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ajomygja.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2znkorynk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hftnpbnh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2etvbwtur.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ubcntwye.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zphcbqbv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhfyrst.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rvvpyuqf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qoxorlow.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbamdz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlmhqoq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bpbzrauf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewkkdozx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2skihvrzq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gzszudjn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uilprogl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mnwpgmuh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pmbxfvyw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gcsbdkzb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2aiprlyol.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lpluxqvz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2muviyuvy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qxdbxcvh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kungattn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zxhtunla.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hjaecyin.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hzkwywvw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mxiswdmw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pshobftq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jksssepf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2acgywlqh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qyjsjyvt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2giwvzvcy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cuugxnpe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dllxiwnr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jfprpegg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2sekyuczg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2edjnwnpd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2uuacgjfk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ggypurkj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hheandec.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pjklwxki.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2emqibsyh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wyganqvl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdtdclkp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xhqswsqc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2djznggdz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ezysyohv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2whdfftai.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eofrjxlh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rwqbtbws.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2domnoxfl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycnmhmfh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zdyayqjh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gatyqpsx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ufzvgflj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rkqwobcl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2phivqnbj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2whzatfeq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mznltlah.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ruffbkgv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhbixwj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2leuflopu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xozudnsg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ptayobww.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lexkypzb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2egjcjdhj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2harhesol.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ssbyjmhz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ypmczxso.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2njxjqxrl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qzktmohz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shaswcjx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2agnbjevj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgdtxzih.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vnmgbhyv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2aaudfjiv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hpyzpego.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vacuuumw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tzuagkbl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wocgynus.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gjeqggrw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2artfovoo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bjqusnlu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ajtcfzjc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pzregpqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jnkeydkg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wufogoms.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qqkmxutp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fwjrgbst.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rxypmgiz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2amhqnvqz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yhssecfk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yqrkkkhu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rbtrcofj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zwvncsdb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nhloptpb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dkrrzwba.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2moladgwm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2omcmwppc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2svrtbmti.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jnyzkcqz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dfpiudhy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sgbwypkv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lpaituqf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fealboxa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2yupkcbjn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ufyvdztv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqjylau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bnqoutcg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uoancecx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tfbmzwme.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zynrfmsu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jewdbptc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfhttpc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2smkdoonb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jvwamfjg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vpxswane.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjmujj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vexfmjcd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hnqmfjsq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qcmvheis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jlqjqosp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dmsppasr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gbckotdt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2deevfszs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gkbfovdw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ydrnecad.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gkjcfhjd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dgudzsjq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2piqgtrxw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eeaqtokf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jjbhsfpg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hpybvmhz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2malpznug.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nhgsfoqj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hyhpjrpk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yashhcav.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2blitmzhx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wtfhczwt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pcjifslh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lkuyxljt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ngwjcvob.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2oylsacis.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzpyzsc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qwvbwozr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gpphchvo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hkxffwmc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2splwmtvl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzkqol.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dptnlnjh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mfbzoewr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pjaqqyvm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vlexhjlu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2njcqtjmy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zdsrdmez.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tucsyumy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dgpmbuvk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tznnoacr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bytozwff.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xsnxemiy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2knjghlec.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhyeai.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2xfvaolza.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxldidv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2asqcakgv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hikvfdbx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2oacgyigw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hrcptnxo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lrhhibfn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztarupez.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2tjqrbjbz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bagqagzf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2lmhmaxfu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aeaupnrw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gmtjcqtp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hciceauz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qhpnurwn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rcmqfxav.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ikjyvusg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dgcvbwgi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wnievgfw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hevthoio.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fchskvtn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qgcgdmhz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mjdaodvg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2usszswja.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fjlpmuvu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jczvmaqo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2afcqgias.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlftcmtl.html


<!-- 参考信息 -->