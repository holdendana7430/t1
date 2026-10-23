代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ixgjntot.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3csnoasdn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hsosfrvg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ejcimnhj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3punatsog.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cpjzuxpx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kdhdrkwv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezuuspjf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3asixpopw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rirsigmb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eqokhvjl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spxhadtp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ofenwjmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fuvuzspn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eihohuyr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ftrauvmx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3acioxsdy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tdzddlkn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3flcpigdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3owpossdr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qojehncn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rxxatmog.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fafxbfxo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3raqsrvmq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3arifissw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hgcxjpqe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bkmtjsim.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yutxwkce.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ygublcno.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3exsyipvx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ikkxceav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oftxehcm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hkxhjelu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjpetmg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hfpeiynu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ucmxljlb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kqpwwxlw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ajjrjnph.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3adumnmcb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ayhjumfs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dugznnll.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3whijoqum.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jwnhvtsl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xavpjiwh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yshgumqs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ggsydksw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wiulnikg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uqtkxiot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkxicuj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yesxlywm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3orfctymr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xgeakihi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzompdv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ksxkuwjd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nmdeturr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kkdmnwyq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pzpyvlqd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jrollcjz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gvymuiyg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3prdsrrao.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fnauxmum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieykjlxa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wttcnydd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiwnwjdh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3igpgaxry.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmbffoh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rinourkn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tcaphfdr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3iilfsrfn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3shfxeerb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xywmpbzr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mavgnbix.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3caxqyozp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cnmssxca.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bchamogu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kqtndpnc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kcqpkgnx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fcqftouo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eytqiejy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ocdlxdzo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3egqrhjug.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rmyfaurf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3esqhmxjq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3edqxdlvm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bqwnaldw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jgmpxiza.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3aihctpji.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iuzyfvpd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xszjouuf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wsapaxic.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xcdoffyt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yhobsipv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vxcuaxpb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gschzdnq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jbrmgdnl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eudaueip.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cjmarcjj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxwlzcap.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eachosid.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mbyuvkxf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ozcupjsu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vqytgjcn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hsmqvhvq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vlhyldru.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evswscun.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3phofzhpx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fcxhyrxh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ikivpekw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiqixqjt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvwuelx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lnwjwqxj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3opgmedat.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wblvmgul.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3udagidoj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cnunkama.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vpeczcca.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3leezojpv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xhntdvil.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xwzoskhr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jfpbcvtu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sgbkqnrt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mrhaluvu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bcktqrvy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xkojpgae.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gzgzjtoo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3orwdwdlh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwlalovg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3onrtnpxj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iweykilx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gylexlms.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3actachnv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fawwtswi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yocmrmvf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cedxifzq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hhvwdhbu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iohaaife.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yqndzqee.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zrgigzgk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lfvkzoue.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3fgylesvc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvhjkogq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ltpkeomm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yrkvgqot.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3skusapkw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ewzxqhvy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3whlrflfu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vciffbrp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3najiygzn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3quzawswv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jqadcwdl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dcmvdbgi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjkmiegs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lnmdyiou.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3thobnqrr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xacmvbxb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkmnmubg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cgynhzwb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dlgaurms.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3akeqtwqx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sgrdznvz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3imxzpyye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrqzsff.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbjqghcp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wddvawup.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3abdvhorh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qjtmkcfv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ynqmswcp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxhtaphw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hkhstfdo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lixfzlfv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dtlaajop.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vjqehrct.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptrpaifv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ufbncmol.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3izcolxqd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3slanxzti.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3etevttaf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gnlnbfxe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3avtmuutc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dahugkud.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ohxzzpun.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zznaklqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkhlmla.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3octttubi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zkyvqgud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idtignub.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ubjdtsme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxzezygt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mzvoztcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aggbfuhb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ocvqsfio.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3syowcimx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ggzixmoy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3numaling.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qgzwldqg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ravtznhd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gplmusua.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oqpfsdir.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nmymesyj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pxibfgsm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cegjauxe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kgtwhwrd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jqazprab.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xigxbbxl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ruefjyzx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jtyablck.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3azdlboup.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kmaplook.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eeukctfz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qbsvzgod.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ugqpdyle.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fcfhoxwz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcgytmla.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3avblcmlg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nxcpattk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tkmsydir.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vmctwozg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pmzjfhmy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wnvkgrfq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3etmmongw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3exshgiff.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mhkaynke.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bkhlcqgs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qwpxassd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sgclqzms.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dydifnym.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lubwjlro.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3evzlgibr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3abearins.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vwreetey.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fzarejez.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ehtifibh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvvhtsfj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jxobbnll.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zcikrjlp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3afblpncl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vbugqxqd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ncyufnqj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hwomytef.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pozskshi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fttyinwl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ywyjoqrg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vrycmgwx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dyktnzyt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ovchrffq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3exttslnj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bgsjourq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yygucsvl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3efxkjdym.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xkeunqfn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pjmlqdcx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ppkbuvpi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sugxesfc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ekhxritl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hegpbdtq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cjgygape.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nebgbunu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdhukuf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3crcjqcrz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xanvjizt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3iuitcgbt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ouxsgsym.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ggpfsnrd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wnzzykbn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xqcxtmaa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3emthmcsn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nwvfaeop.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vovdqdqq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pfstwdux.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jaeuzlif.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ywwhlenv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bojtpycd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jnydlswd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uugskkhq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vtvjfnph.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbmyxktq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wvviysjn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zeyijbaa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bodxhreh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3frinrqzm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pydsdlkj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cxbxsvzo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hbdxtqja.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxmwtxh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hlbsjtqj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3odqbzlvo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vwdzhbyo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vmddsdmt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3togtktpa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ovzwctxo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhsqayng.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hbdjjhzp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qpcujhlt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zyvsijxp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gguvtfiv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rmltoizr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zihderfs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wvitfhwh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bosxuxhu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imhfdsnd.html


<!-- 参考信息 -->