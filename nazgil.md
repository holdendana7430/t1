代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qfoqdpes.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3onwchgte.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cjonkrxu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fwtcvpdd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ipftadum.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xehxayum.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ndfrntrz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxexsvwd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xhgdtnrr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uheqwupk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3nffxtmvc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aittbiio.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xnqdgptc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mkhgpwfx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ybnqwirn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gbgdbmvl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xonkadiq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eppvbcql.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tfcwrwuk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mylydsko.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtsfbevx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nxslnnvi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wibzgmvf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3midylgwz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3cauxsyka.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nfjvzbaw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wdsepsww.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfyifijy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpnasph.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ebsxfroc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mhmwwqvm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bbxmzyvs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvljtfz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fpypppnh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fslodhlw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eaihpwno.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3afnathlt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3emhpfpat.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3oaelpsfg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jwzdswqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hzptgnbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvouhhcu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jfveiizn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlqmrsvm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3novahplq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uzkaqeqg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vkfdbkru.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3psgweduz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3aackrsqp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3blvqhdqp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wympzjia.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hdnmyhkr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hxgunipy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zppggxkl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uvpoqpqs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qalcxgmy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jnnvpmgy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jyrbkxoh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3poflclto.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pxssxaqt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lftxwzyb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tiposwrm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zzuvjfrl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eltzhcrq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bvbwcyvx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dmdpjdgx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ykbgmfbs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sxllzoig.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dsqeumsy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncppanhv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3poozorbd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnrnvhb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nsrbngjc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3quxtihub.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbbehvnx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xxmsuwdu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3spnumffq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kyqkkuhl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sepatlmh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hrqiccnj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aixaobwq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3duvewajg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jnbpettn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3sbiehfmm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sptcpawc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ucfwegus.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mkixqkis.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yktztprt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ncdwxlhb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyayenb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rtcwomix.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqtjmxxg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mhdmcegm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uilstvfj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jukvdkrg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3diqnyzga.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cyvmbrkg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jldoizvy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dzxcvtiy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3psimfojm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ecyghysy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3drcmtmhm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mbjhceph.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xpcwlakm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3boayrznf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qdzirnvw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nilsplqq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pjtysjco.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cdgknzoa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ivybwtiy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3montkfvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3azuoldvq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ilthmjov.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3peclmxhd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ushxqygk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ghonasao.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3byiephbg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3logjlbxp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nlqxwpbm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pzlvdaau.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aqfevmad.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yrzbhnuz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lhrzyaps.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3caetzhpo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqmtjjdx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qhuhoaka.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zsbxssmw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vzjejjhu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3biprqalf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hfjvfckc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3trgxmovq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3petdqfgp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lcxuailk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fvgwlast.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nwnwtqbz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tvzivezi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sbpytzgk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbjmvmva.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ujbkipxx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3muvffgfv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3poskzbbe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yrssrilg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yrwavzgf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kavedtxb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ztnwalwy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prpfcmrt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3umtjujpt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nqdtpdra.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tiamenqz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rtepqwwt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xkedwhqh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlhoobtv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uywanlvb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vadqzmdc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fzqvemrp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xhyszdpo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fspoclvj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uynainpi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3eilpokrf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gmfvmjti.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jvgpfjne.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3saabndqh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3njrzbvad.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xinmbjik.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3koenqmor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fowkkvud.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aslpnnmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgazsmnx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wfnoopra.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fqdlavln.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uedufoyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wmnbqfkv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uwmizxmr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wmywmwhj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nwaaodtg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jnmqdhqc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhikan.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wdpopcne.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uxkfjfun.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rzhqsfhc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rghvpmgc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dsjeemsd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3aqxwsmwq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fwfvpgqm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3trgrktrg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lhsyrvrw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pjkfdhmx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lrvyiinp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pmzhavwo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xucnojra.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rrmitjvf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fdhlctjd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ectmnzac.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ywmdhfyb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lqghldmj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lbcxghif.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cokrdgmw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qxoxwczv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qobahmxj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hlohkgjj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ydjchdxe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3palsoape.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cowabbah.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zjrmqqiu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3woniglse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ymhwowfe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xsxastqf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3aybsjnlh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yqcqymzh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lmzhtrzb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3noyuvvsi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cajvjhjs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3snfggcqs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fqaalvqi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mlygyzia.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgbrfci.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3woihuluf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbwtvqs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tuedzmcz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bdrzglhg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3prfohnqz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wakqmzwu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ppbilqnj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lokjrpnm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uqzwferf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wxropzlo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wpsmdgwb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kestkrpb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bmixixms.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oxhlizrp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tsfqqvkb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nzypdhes.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qshqrupp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tvkeidya.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sauofuqy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uxnyvpfe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pjbzqdew.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tyldrnxd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hhmdsoxu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3flosyhct.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rizjoryz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3trdpyawp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kbrxgpft.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ykonbimb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iifdzqgw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3htbsfxhc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nifszomp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wppqrpuz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3odmuwxtj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tdgcqhlo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lxnrgbpz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfxvfnb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3focuxstv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3icxfvtce.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvhwmhoj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3udbewdmx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hkxtxfnj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apsfsihl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwsjutus.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ieztrzcr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3icbqprit.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jjxkmsew.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vppdotjw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vljtlhvf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3htugojny.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ifqzlaln.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3eofkjnrl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdgqcbko.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oylbgnna.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cmeqrskh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzzepudr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cwvxxysl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3swopamnz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ofpfqkft.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eyngxasu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qogwraqp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ydaseugx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rqkrptbe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3agbtgaed.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vmnocwsb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pgciwghg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jleubozu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dvkdbjbe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vbppmqev.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3atmuewnv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwvhnajj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3osaeypma.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xsouatnk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zpbfiyha.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gmxnenvd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ifocqnwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3appqubwp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qjcqunsw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nqmtwouj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtrqneeb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3emlencis.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wxhwmmrd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3viteanpb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eyqjiugn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ennfgbop.html


<!-- 参考信息 -->