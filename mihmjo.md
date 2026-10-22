代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2onmqcnbh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2thssgmys.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bbcthixi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xeveifau.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lzvrlqqi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ojhytntp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2slmeejht.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tpseivtg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fvnmvzhj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2awxatera.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2njxkkwml.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2olnxeoqo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mrmvynmu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ukwolrtt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ylnommhc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2knzzracn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hojvaygk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rkjhnfme.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2icmrdtbb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wimjmdvt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kqfivxpd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pteygazb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkwuwor.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ljehalfh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nwflongi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2omrsywwn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nbywughx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qqybnljo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qdgreksl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcwcvptf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ykunwetv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2csgwzmsk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hmpszesf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iazwfnhw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ojugdofw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2slgwwlmx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nqhgfxvy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jupgessr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2icaavfko.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2syrnftdg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iwlmqlgc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwklfsmi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kywlufqu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2awwcuzmn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gvwtxyxn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iqwuhmew.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2iddxhjnl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2quhsfsps.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nleelpbu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uvnmkhev.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zabvadav.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dnubdibj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nvqxmzpm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2swxkefrd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2teivfjbm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvwybva.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yfwegvkm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nhrnykio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xetnstqu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hinriqwf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wkopsbfw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kfqgcpld.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwhgqbnd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hboiasqw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ktmnmprn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2duablref.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bnsuoaai.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vuzfjmca.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dcxnxmkh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ihcesgif.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uirufkov.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tsdozmyp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nvidtcwm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lofasfes.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oemfoimu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zbidzrnj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cblfvcqz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hdbhqnqp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbumruve.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vnvigera.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajrwfbi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vouibgvj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uhxflfvc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kqfzgzfw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cvkocjyh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mkovrbvz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2leksxhal.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2emdgghwj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2icljgnxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pngiikls.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dmjpfeja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byoewein.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pyjdnyqr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2enkujkia.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bhasktpe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yevlaawq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2phijhmgh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zujopfva.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xwqsxitv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2whrvqpec.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ogqjnsrn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pmssexja.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kftadcvu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwpcscew.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qaxosxmu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2flqcjzgz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gpkpbkpw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vialqhkl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iadkvact.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nplwdshi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2sylhjjdg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2meoevpqi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iqcnfjiz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qzrrnece.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aoqahswn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhgqhap.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jrdpxmcy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tynobrfo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ycahkbrh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqdwijv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dbjtfszt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zacykpyp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ennnkqyf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mgfdhnpo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ehknjcam.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fhlahwhc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qpstqpwp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jdearsoe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zeawjxcy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zeqesyzo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2iyxiyfvl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdfbefk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdegsq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qdqowgqd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jvymlphz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kssflpuf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2drogdrdl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pxawhrxb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gvkzebuj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrsgldh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cgrngfwm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2biguwcla.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qpqbliic.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hvostybr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jiulffcf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kremlvny.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dqrzwwkj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2psmcsvcc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lgufltrl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fshtzbhb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cyfarcmi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xwiykfgm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wngwcksu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wppmupra.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qamuwyuh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wwsxdepx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dnyfgpib.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2twlboton.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2masrpykf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nethswms.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2afsxokcu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lfjyyfot.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cynbpeuc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yevygftb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tjpkbqeb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qajpnggm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbagvggx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gxauruhv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2djtjrmgl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hftryxqd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2eygdslnw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vkguourl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khocgamo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2sdglcbui.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yojdrrvn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zuddssxo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wkthgcuw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vzawgfjy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hiiylxlz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuhirssu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ixfdsult.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2uddgnmwx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2imlsbwdb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeczsgqr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yulkdizn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvjadho.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvkykkzd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hisgamut.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwciybgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tljmxazo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2waqxppoz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2twgbtehm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vggoarar.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ggubdagi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ounirqyy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fmyqnvht.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wvdmqwcg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ebxkoose.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bmjirpdy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpmbie.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jjhzhozl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uwphexvq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skncfctj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jsavwdcf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lzpbbyeh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dtheqvsk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ojopvuby.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bwwtdpce.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2calrztkn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tczkicbm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bkyqllnz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2esedrygp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkbtlpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnauzclw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sqhnnhdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiufklab.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2auclagsi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sfpfaoem.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hflblkrj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mfgclnle.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kifafxze.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gsmscyqc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2kcmheebn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ltyffzku.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nokukoyd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mphgpeab.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yypbppax.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vgdngeap.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2sfphlbam.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2urnchlod.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kldcszty.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lcjwusjt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dhtigjdy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mzxpvwqm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qtpvvfuw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ekwiogvf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2aqnyvjus.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2prvkvjer.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jjbefgsq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrswtwu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yzmrxwjb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mcofblkp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nwubbdlk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aflevfla.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wbkjvock.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dhidodzi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vprkfpfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2djfouwrj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jiikvajj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pblcvaxk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vxwocayn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2novzfogb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2faugblcs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2regiovyi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gmcrxoqm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjmtbxz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2swbdouvd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2sgabswjz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2aheowuzz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mltojpdu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2holzmizh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ejxqkibv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2moxkvcqn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ixvgwmoh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmyuky.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2djhgnevz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ssqqjfxx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2upztgbxu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yymuftbj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2agxfuova.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ewwtidtw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lsyldbnl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lrxjcgcx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gmywfyem.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sfwsldcw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnfbvtz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2azhufgco.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kikynigp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jdpnwjxz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xgwwpfrk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ebwxqwjq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xlkwdhqz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2udxaxggd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqtgdma.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2oshnpslu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2msnkzval.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2yzvkbqaa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pvizbplt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2iahdozdl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2omxogudj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qgeecqrb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uuwoynot.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hptcbaop.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cbrqivnc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ihzmzyns.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wlcmtloa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2batjmxee.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbrghn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2iswxxfae.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hzcgyjwm.html


<!-- 参考信息 -->