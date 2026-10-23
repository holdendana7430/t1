代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3esimnhjg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sutxsavn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3knqmptji.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zykhiwhp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vivesdln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eplywlfj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ptwqgcfx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oqvxxvck.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mxzfytto.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3koljovtc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmhbzygz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oyvcelwl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rsgmjqgz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mmffkrgf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3biijyeqg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzavilsu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3puyafajw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3baaihpvz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3atbsjwyc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3caajivxs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wcepjqej.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3iljeyprc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxdmyheq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhqnkny.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3oetygkcn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xotwglck.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mexggmzf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3skscfeqi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ymothddf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3bibrxbsx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3imdczfvh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jevjywhs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tohbiezk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bxiaagvv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3klrrdmqu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gpgtfxzc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkllhei.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3awmmcsdi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zfyaibof.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tmdnqmtr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3biwkkbgy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tirppgqp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3sigferdg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tallidft.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rnvorbco.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ishmiimo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xlwdtjgh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqlvbgue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tlifdwad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftzaimcs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gzhukemv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osigavuf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edkwuapd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xonlzjqn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dpfbjjky.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zxagvadf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ckqxnfxd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3atawqqrv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3shqzqzfr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jqbqknlc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pswxskro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wkgblkmi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tyaliekc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bjdkamjv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ysnkedgg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ogcjkpju.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xzhmjzfc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qqlrqaja.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gcamsiwl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3voxiegvu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fugacnmm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kegedmen.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lhzafvbb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rkgwufwx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yzmsspah.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wshzdzhg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zeqfctka.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfgipifn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3irangkim.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnphxfk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vkezhlxc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3syjfemvp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nsdhhqvp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3twaqrckf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jkemobzi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwvjojpl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yuzmcrtv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ckwijsqz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xgwmzolo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3omrkmlxj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dezwcgkf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gxufjytw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qpnmqphb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kofbpqdc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3skjytyor.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ekiawwyk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywtkdxky.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rnstbkkr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xhjzmwoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wsxhjfbi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fqsksusd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qnzljxxe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jkskquvk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uvxfaltg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oafisotp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wsrrezed.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3txgxcxyd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ytghlzrv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zeaakfsw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3klvbyuco.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wqtdkmwn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rknkjzqh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kugfzbop.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ahnihcbi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3djlnvitz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3plveusiw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3imdqgfsf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nqvphjto.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fveavnjl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pgbmojlo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3egpqudff.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wlwnnmdi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxxpksta.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uvajzbmn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3apdxlela.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qfkzjteg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hktjmtge.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yxjycndz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kujtqjgw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3opqzkwpq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3huiuxshl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qsfrinep.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fkitobfr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hwbfhiqc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpjpmcsy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3falruiet.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qqkdhqhr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3waycuddb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gxuosflv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ttnmbdrp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lzaqihus.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ucjpnkgb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3izomcgaz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eptjrbgg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tzefqlbu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lkmyqkzj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dtksuvhj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3twvwthkj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdxbqtav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxqniud.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgzixvxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pazixdib.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pofymqrq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xchdhvyb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yrwnpkhp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gkrluhdb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3omtnbiow.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tqbckosv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uqfjnfws.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vcduuvxn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ktasoupr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yqxwutrj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gontnsdf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yidiwkuu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ozchitlo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqyoiavv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3onhomrvi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kvarjqdz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3knfzyuvt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3apvspnvu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wbkqzasp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ezemopis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xfsmevyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itcxzxeb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxniqwqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfcldpko.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrprav.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ctbofobp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3citrpfyq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iwjnylvj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gjmimuun.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pqxxnpgz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3retqgtlq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pcihpdtt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fpiavmyj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qxqfetiw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cmdzquyd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vreqbfsr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3yvtuyxfa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uhimmqfy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpwxemdo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3znqrzusx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qsrtqpgy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aurexxyr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3allhoofo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rgpkjknr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3elndhzaa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewimwkzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fnhqlqyh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arfmvcel.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qetyixhi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nmhgpvjz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uaumznrj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oozegulg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3tiyxjxpq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3htnbuacd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xpfvmitt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3thcanmqq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dgnxfwbq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3itmljepc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3arbndncx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ftqrnrhe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wwotzpuc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3soyrfjun.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3najcklkm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hcqyvdxx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qlpccfnt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vgrrbgkm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3epwiylzo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xfxpdlhv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufjkoasc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3iemdfqye.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hnlkokir.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3arkqyyfi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3onwyeomr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fyyvojhp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nuuujdlu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3elehehob.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bsmhpboe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fjntxgdo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gzhxpwej.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gkcpxksv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uomkaxzw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3znpjobjw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3anmssfgc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yugkomna.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3saqyqbvi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fpgsdgfx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lyhdkpbx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vefduixf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vhixgiat.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3uzivsxag.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kzciqyek.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wifmiyxd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ageunapr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wjfxuety.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hsaozmwh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3synhomnh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3smdybhvc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hryfjewn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3swmdhgus.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fqwrsepv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hzgsyqng.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xqbrfwtl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3uotbhejd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpsuhqll.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3aaximboj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3doopmrsf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3djqiuuca.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3olndwsvv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ncvcoaaf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ylrwwdus.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vujvaejn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yqyiwhsa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3itwwknew.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvwplaay.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkajwzpe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3omnfhyna.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcjfibiy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bwmlsowa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ykdpdydy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3duzymbzu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qducbskk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3iulwiowa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3phoxcnjj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtlhgdwj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3sqctsuja.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rkbumkvw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktkfmzap.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cdcfgmey.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ahhaktfl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gmjwdsdu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zdasgfds.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3eypxmols.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dcojvsnp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bqgsnilr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmufhuzd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzhpypox.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hrbvvkyo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qicjcvpk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jqndwxbu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nlwcoevp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xcouddkt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ydvagtre.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jilznkev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xpftldev.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ccbpcnxv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3iagxnana.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pvpogiru.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ckmhdsqy.html


<!-- 参考信息 -->