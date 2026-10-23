代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gqaqhual.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tiosggrm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zmalkhps.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3btwkjtfv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kjrrfnep.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3siqtwugc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lqrzxwho.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3eozbcpkg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3edoshpsx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3raulldqg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3omibdeih.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ltlptjau.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jrndhrvh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uhriyjer.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lhdjwoxm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bhpmxuis.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xrbyzoxo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3umycoowf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3soxbzhlq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nhvqcywz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3egnptxac.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qwivkesv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3owxmroom.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgwsvvmh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qkdrjuzy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdgyopaz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zfiyriam.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3klzsfsux.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ajzmgjlz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3prpqqqtw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bchufwqm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yzbvpfqq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3eccitsap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vqlnwnor.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wabwclav.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aucuniss.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dcintqgw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3eekpqejb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kinxsilx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iwrzmqds.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqbdpx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gvogtnqg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3iultdnah.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3epftmaeh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqfoazve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hjfgeqpv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqaijvyb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3djfhccdh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kkkaufwp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ptkqopox.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ulwoqqni.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3foszfdjo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hrnexweu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fneaxxdw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3umuncuxv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nmxqcuge.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxvjuewr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cggzdbcg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3krgsvzby.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3osxbfhvr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tbgigyzx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yxceprwz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rhysjlvx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bnjqdwio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bglerosd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3slmfjydh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hmjqjumm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3giugpfut.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ymweqcae.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lcaklvks.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3azjpyenk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kzpcgtzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3plmhpywj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wnmtsmvb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eljsgevc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mthivnzm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3koboezwf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lgkrloaz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3skhifrsp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zojueowj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3istinvna.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3txzfnpdq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zkhvpjrb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3anmllcvu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3umwxbrzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjbqflru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gvolymmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmpwdjkr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icxjcsrw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dinahqhr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ayggopyq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3erywueix.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3agvyfwkj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bqgrnuzk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jkdstihx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kkoozsve.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mjdjksae.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tdashgnh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mrayomgh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qmbkutyw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fnfhykxo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cvjrlqmr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qesijyfb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpryku.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngqyfmri.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qzswxzug.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehlqsdeq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qsetylnx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sfdvezsi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qtviluxg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ewnqazru.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gvhznhjs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hjznuntq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbhhhqd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sipbnsee.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ruoflpfs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zqcvsicz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3unpgypfn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qumywkbn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkvcmzhj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3adpjirhi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhnjuals.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ukprmdwg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zzcnoqof.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hhvlloox.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywwatuxa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dmhhczgm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3micikriw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ynpwvxzk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hoenawcz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zuyflmat.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3idvfonph.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmkzwnls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cdhevkte.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zsowkjgx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jtsgyjft.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rquldmjc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rnnqiknw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3juuxpbmu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vlywwbio.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nhnlyass.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3svlembuz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bcoqnkgu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3epaquddy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bxbtcmwa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iunuelxg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ffsrstlk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ibjtwchq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gfmeelwh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxwmkhrl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hnypzcjb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fyykybjv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yjdwlvdi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hovbemne.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ofcazprx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kesrhmlt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qdwubvkc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lxsheasv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnsomzai.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uqzmttln.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3otqvdunh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dochmcuj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmgrmhga.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3idqowvim.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3azasfpho.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mlasvotf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oaachujv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bafkamts.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ekmdbdkc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3llexnphg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhovxxxr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3crslwiiz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xoryeyih.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tkuvsmwm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qokfpszl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lozutbwl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wcvidneb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ahyqtdgg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bxejtofc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vmqomjzu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ctquaskd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbfffztq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nregqaza.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vsuxbzug.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jaxmedyl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3btkacbcr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3afzkyhfi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pwmbejuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xktciedi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ktcympvx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ymiiryfw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pisksaur.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fkrdqetz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3meyywwge.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ypjgcevm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vtjtzsxo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3meppfmnl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dfwtenbw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3szcehcgc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jyukhauv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3doagxneb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vngpbwre.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrdjymw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tsgykhng.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3umlsumcy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghzdvmag.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eoouqdyy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xwxxmqbh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fmviopfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysxgsemn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pkveqwpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckjlpxnz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ekwmerqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zeqftxji.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pwjrgkke.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ndtmcpeu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3chvokdmu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hrlhikrk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vhqndgtp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rtfmzvyz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bjlsmhsj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hvsixyxu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pbfbyklo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kapqrnek.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eonqmlio.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rhrabycy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3porswwwe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bowcqqpd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tjpxmghy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rbdiamvo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sondnrll.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xczgzekd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3iitzccke.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3iqkedtcv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwzaqksx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3kjfcrygv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pwsfwozu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dfzdexyh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ungwezfa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3paxlntww.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qboafwkd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3csbspenz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nanwrkiw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3volgupul.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3sshcptbc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pulhovjj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qxvqixmb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dfehrowd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pefijqbp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hygrrvac.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ngpcbcxw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3atuifvck.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nhdwvcgg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bseysnxd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vydxcdoq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ipoyxwqd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tztsohxd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gajnteoa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rjpchztq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hevvtzmp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ypibgstp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bqdzuoht.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fjndubfa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbbaaai.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bmateuqx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3trwmqecb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nwhxnabv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xnubmmwo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3axijamtu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hpubqiiv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vjsfhnvu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwwqfra.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ydpmfmvh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3btwxwgeq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dgusiwga.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hemtcrop.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pclvvxem.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uscvizyb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bgpjhgnp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ofjkqptl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uaodctmg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jwrqeqxq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3etkzgxdq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oifyluyz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oddobzid.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ivstkone.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mjmyizgn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3raaskaxw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ivnsufjc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qkakpxcf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hytgiszy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3euoyosqm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zwgpetmm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dleimerf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qhgymlwx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3utrrgqtb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rvzwhcmu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zfsivnrc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gxubucta.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pgxkdgkt.html


<!-- 参考信息 -->