代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3twxtnxto.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ukmpregm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqzxjzwg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3outpzfhw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3torwrckc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3asmvqamn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3quuqwaiq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uotuctwd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wuohqjgr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vscarqvz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qbguljyb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xunkztpp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3twxrydvn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ogjmwwua.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3efrteewu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mjaepdwt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vzxurxfa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mvlqomzo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rgbirxzh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mbdojple.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ayqjieuk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eopwtqzw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hrgxolfj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jwvxwzxy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ahtmmxkf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3twzvblos.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rttqsoky.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hnepyhnq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qfntbeql.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvtxdnfk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xuuakmlh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3smfyciuu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fihtuqii.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjigiuo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jdpwasxl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dulcdjjc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3aihzhqpk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vmqiiphk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vbxuvyuf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hfbobpkz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3trwecpvn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbshuir.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkfpatjz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wadxqvja.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zilalqub.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bctzlnux.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ptuuhotc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xrbsmmfl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhcemofe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvjrlzdk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zclgvpdz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lkypnehc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eoxxflxv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kokoqhdf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vagtuabi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ghpaacyq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fudhcjzi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fxxhrfsf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tglfxqmy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ehcrxbcw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lisysubf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ejlpdojk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gppjjivb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lpeupasv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hghojoaw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tzfxyxgg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aczfgrsi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3chmdynwv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qzyoccat.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jrdmsyxr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ptqkezkb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vifcvsko.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dibhaeff.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ukzhxsai.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lsbtvxwi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fywskgxs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bcalguba.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iyorqosp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhpudytg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3oogpoldy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsqospo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ioctdxrs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dszpmece.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3llhghytw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3etlvahgf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ooflyepe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bxdlknck.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zdbxssvx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kcrmxsmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byueikxi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3candmjkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hosiwbhw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kdpbskrb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tpxzjnya.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3viozywwu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ndvkjyrw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xmilgxml.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ynvvcawz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdaqke.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lfywxtfw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3birkijtj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qurbbmxe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ihkmxzzh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nrkvnuoq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lsannkbf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gzidlhlw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zovuzhpu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxkrvdu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjtklikt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dxxczctj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ecadrjkr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xctzwwrc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hghucsya.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ebmezyzu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uxemqqwn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zjosoqmb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gkehgjka.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrgkjtg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pqmrjfln.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xgroztrh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nvdngtyp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzktnho.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hzkfjekt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ayhfpejr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3juzvzdfv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rctncfag.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ijqzehmj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xlanjneu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pfvvfxzo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywauupdg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xztapyjb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3izultixu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ugyhasps.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bxfnfaap.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pbtsyllm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwklscyg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxyximsb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rdocupxj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yhgfoavi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3amrczzxr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jsemmnft.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kcxhxczo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jdmoyhbo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zdidtamb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ueeyfksu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3thdauvxt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mlfbcgtk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vcroskbo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xugearjy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bswawcna.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ebrkvhvi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vavthwbl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmurexsm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hwegbces.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwosnr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3oofohgiv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vtnbpxxq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cwojectf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3osjfgpnl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3inrxyjjt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3agnofmpk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zrdopanx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tcwreimx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ctinbsoq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cqraquqo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rmlgedot.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vbucrxoj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wdnbxwsg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bcqltfhr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zreuityr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nnynqobm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3svlfraea.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ynwokzts.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nngjnduo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3clknlzkc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3frfbrzon.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3weitpkdu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ufezdwcg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3skxbsbfn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3crkddumd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hcoupoep.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3nlkqzijr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zhwlpttt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yksrdkrg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tuvrtckp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3drxlonoc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kgrmywya.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3upjhgjlg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rjsjiahe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dklrqjqu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvpmoo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jgosxjnz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctsgenjg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pjkxsudp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ngdqzvpi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rmrbeglm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ajkhmeyb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3noxcfyee.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wmqlmsib.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3njixoumt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kbgxxumo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3udzienkb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jutitxbb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3itpjulms.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3klnssewj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lbeirngz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqisynpx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hchbnktr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gfhuxqne.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dgsqvbza.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hotlufbo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3quwcfyen.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lztgadxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kymbysul.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oojxlskc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifvojrpk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zwtnjwyj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kvtebvzm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kedotdzw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tczehibu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xgiuilbc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cjupjbnp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3puuzwfos.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dzrezfdm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nlwfbkcv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wtptssew.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vxudyqfw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kpckoyap.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3spbytzvo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ecewsuwk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wmperlws.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nwzwfwiu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gveqnizj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iveoriqk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xqyvlbzs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hclguqjr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3oobxnxvr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmtiqjf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qdbumoup.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3leittziy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hdgomncy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrpujhg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3krkhntnl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ubjuljiz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ytoscodw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zemshumd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3behratnx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ustrpdkl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bjpyyfiv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tphkelvb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vslbfysv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rajbabur.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mdlnqeud.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cfcvlron.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tuoqzaay.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wbyxilum.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fnqttowe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ireupchq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3morxuany.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fuvmqcuz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tlidlagg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3iwxutgcm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ubmiqzal.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3witojchx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ltexzlnc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tpqnmynl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rldzxtog.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nfrocfrt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gugbytbt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wtyztmrn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uibioewc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kcsnxwog.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ibgnpwok.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ksjemrcm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bhaubzst.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3drymnpnp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sijnxztc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3olfjcnai.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3grcblhdl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iwsrrcas.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qdojvfyx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ojrbsebb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hyxdqlsg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3abpoctua.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3arepmdcg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3guakmbie.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3aywxapwk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuofsqt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cowjezhn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ulmjkowo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nsmadksh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rnoeizmd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xzfttqvo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hakphjiz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nqhciaml.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwpsjmq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3sipgipbo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eofqmjtu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jonltefa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3nqtfvqdv.html


<!-- 参考信息 -->