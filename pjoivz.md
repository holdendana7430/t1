代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mowmorhh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kwreoamg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hnztzsmm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mjcyrxem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmanepd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xvlztvja.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3szbqeban.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gvagwnhe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dcrbfggd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3iqdzater.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ftausedb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wrqcbqdl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bxsdghvu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3soiaoudj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ohbucscm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ebiwaxsc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ahceffws.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jhcptjho.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nnltyzwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ndqhvavx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yqmvnvan.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dcqqsajt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eynqeuua.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yrkixmhf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3piretxvw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fjrugtmh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cnmvthba.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3osuhjkqj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sqgseqpe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qxpgmyas.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3majdqevx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qvarjhqo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rfwfkqka.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oeffvmmo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ehscqhyn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jtcitahi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mpjcoufg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xseizjrd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xbcphyop.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3seyytkbo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pisqqkvo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3biealcjo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dgnjqcra.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gthjdpqj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nbhaalcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3msaaomiw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3faeopprc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqfwituq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3viosjyxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bsegnyxv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dgmdadxb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jybrslwv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kvyjqxiy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fusorptp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pyhykevo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyqeoncf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mzgsgykz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gbminqed.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sfyvdqzl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcqqkbgn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jiphxvpg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3eetienow.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdwwbsou.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xndlphwi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eigbzdaj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwigwvcm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3njhudetb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3papwnzev.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3czubrxll.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wxfqjxwy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uxuaizsh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bfbweuii.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xnzlvrkf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxpzpk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3uuonlqlc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhqobgml.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3quibkkww.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3iaknqiap.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qhaefcdj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wkbgwzpg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejauyzui.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wdngowrh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lrwpsjag.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xhlnjmgw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dkqhfrzk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3envcfkdj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qsxdxwsl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ciwpungz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sfcmpryl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbbhis.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kahfgwtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eacmminh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqtmtlpm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gftlurxy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bripmkzi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hpphrqnh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dudgflez.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlxcbkqn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rqcrflnb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lfixuxsw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3etejfnoj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ffbijxpn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qokwffyb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcpsxsca.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oqvrfigo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tidmefmx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3apssdzvm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ajpksumb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltgxvdta.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sfncwkos.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tlvucgap.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3afclbhls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nhewdlrv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3djhqutnk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lfujxqup.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tpamfjcn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qzfvghku.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bropdyrg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zonbzied.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rdjsogri.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yogcbgkt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kmnmjuzh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3trgikycv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xrcqhvjt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3falepnth.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mypvryms.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ysmgojbp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3axbnogje.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ulwxpekx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cooccmse.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bsfpmcdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qrcesbsi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ypknmrsj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yojeglsa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tysnirng.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cicghfng.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrjhanoe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ysdkbzyw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jfbqonkk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ulikoytj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fkblplwp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hgsweeqr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qtkeapqe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nlirxmbw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ocvttovj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bcmvfzna.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3prvqsrid.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hhoxjnvu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3icjlrrui.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iqwbchiv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ubyrtojg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wdxdbztk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3unmulwnv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbgrbopw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzjwqpec.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gfosapeb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vftqwnyb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3oktuvojt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ewlcmewt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jzywxuep.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3awjhfari.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zpqrwokf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3onelsmvo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3anbigkxv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xgmlxebx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zuhbxtja.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lperngdd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rpstzssj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hmdckjxr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uhaccpaz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3minnvuwx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3odazjddl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wzamcoij.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uhkdpmmr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbkstrrq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3afyffzhm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zpoksrbn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pdkstwdx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3syzzshbs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vlbmsrdq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xcgloxoh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bekbyqpy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zlkzkpgn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sornvkwh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jkksamwz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrnxsxu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3znwneloy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3goipajbk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqqfkidu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxzoysnh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzsbwcfz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3agjnyulk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxblpzv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bkjcymoo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gpchbety.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pevuothx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hbfdsnxm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sygrybmg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mcpkgqxi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eukypbhm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uwmteuoz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3byivvdkd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iosmsnsq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dhdybcqu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cptfdewr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jgflwmgy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ccgphdzu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gsnskwzo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yzcknwgc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ecrwqphl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qntacyvp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvukme.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjrtcry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyeoeroq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvxottoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyirvxrg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lnbrezoq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cbkuxbnd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qyfcozba.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3naytsrra.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pkdzueop.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ibevucsv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zzlhczuu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3isqefspc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rtvkmkll.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rilryafq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3alswhfrn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3axgsuzvh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3slagvlkt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dkcrmywr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zyrebjda.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3eyizdgli.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vroausqq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oaopimnx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3muarykgw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rhpcqjrt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dectlqdj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3szkvgpwl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkghznfo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iamylmmk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pcvfrgnk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fyxdfkgc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qnxuenlh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hqobduoi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pwocymal.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ajuvshln.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qqwlrviv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dekwstgq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nmxcapay.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ssauaxvw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pbpylxsu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nmmrvynd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3oiwjqhiz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3buqkgsii.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3teuwqsex.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xysiqdxj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bvxjvmez.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pzhbuxqx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tqzxspal.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpgzcu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sepgrxis.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hjxritba.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3olocnaio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxmjtae.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zmisyzzq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3epqvpuzr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3territww.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ysgzilkf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zqjappir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fyeyexbc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ddxluozo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3etxvjwco.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3eumoszvj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tqxjomwe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zncylfqr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uufzlayf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3krhmqvny.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ufcbjfma.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwqdiq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3wlhduibw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3olkwxntj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ogksehzo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3oncqsmhv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3iwedcivd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vtmyouys.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xmiavawe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vrbepfpv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3opighoqw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mjrpregk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pkufqyay.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fldwqgxq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3srfvdjvp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rqfzqfgo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3keuazpqf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tioevcif.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fptutxeu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oefbhssr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zeiwfuon.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vwtllaym.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vywoojrh.html


<!-- 参考信息 -->