代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3akuapgcd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3flycydsi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hrxgmlar.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3getoiotj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmibhbs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vcehjljt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ecwtqhmz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hccqglkj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3alwlaags.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jvhfqood.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lzgyxacl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rkxoansb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ptjowzii.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dbxfyzzo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3msedjvdb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3degtkuxv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yyzpynxd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hemwgteu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pvbllypx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kvpsrtle.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xcsrjlse.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gptkdfcw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ekgvmovi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zfreawyc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ixqctzsg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3euyodqnp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ykqvuudh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mfbvjjcv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xdjdewwu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3orlhbnnf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ghuhwyrc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3itmxtaci.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nnjiuedx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfwcabc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwqxmuow.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rlsslwkj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zdqtlamj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tunvdqtx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ygzpyutl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xggccvnu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3epvbseze.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtblyzmn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xyfjzpmg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lurgxxdq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mhjkbvuo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mwptdjkr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pcwjzcpy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yulmjevc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3knrkzpad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yhnocqvc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oyeuqllh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3txvcocbm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qgosjfyc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3izbzoeyr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3suobyrmr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jdaqlzkt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cofxibvp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iswnjpwx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3knncthmo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpvnonc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zjwvkdsf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkizhqef.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3iszkiyft.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aerqlnmy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qqggcjvv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kgxgyiot.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aiqzfwyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jwxtyako.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hxqbwfsg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3otktxznn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nqzztokl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rivgrawu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zufbhrmw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxyyvnlk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zftnuaab.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3omorcagc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tayisoeu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqjgnb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3drdeumtx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3whzdmnuk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sobuufvg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zjkylukd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvocrzj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fzzgeacu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3qlubeolv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zeyrjvkn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lyexoebq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qqybhurc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ygezbvfc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vkbvrhre.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3odsosmwh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ottlhqek.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyfsak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbgvjqig.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3frzwcowr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvrhulff.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wlvrjxkc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jthjkuih.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3edjmumez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ltralwrx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yjxuhasl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vhrywtby.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jjgilffm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vnnycgfd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3safwhnye.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pprojtvv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vffdrghr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3shzjuolx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ksbjgjcc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3johllisg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yxbrmojo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3htjncbev.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3faypiuku.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zpnufrva.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ypvjuaks.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ihzmuzge.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ucnwowwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pdfjjkyv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dupbubtc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnodvetf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3okszhgye.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aaqfrwfd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gluotzty.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qttotbub.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tqqrcgwf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3juaussob.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wprjbrog.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnommmpm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fjfkkijl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nvzeloek.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uvzfoxhz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3agqjxdyp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yimorwyd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mewdultd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hrnnhrqy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wiignotj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tvfkmnro.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bthhikwz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yofttjbj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3aqvnegap.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhftdonl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wozbiyyj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3exciqndw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qopyjtci.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ojcxdfte.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3avdjqaqi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dmpisykp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tkfcnugq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gqdglvjg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tltjnbhe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fffdxbjq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3reunztxm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ormjzjfu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jzyxowai.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wtztdsos.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3spxrbghi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdlapkit.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xusnifov.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3agwvnxgc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifuhfich.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ozdzbwyr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gkldtibf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jxxlphgo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3imckcfff.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dfwojqhj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tzqaabvv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmyirjcc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3eledwyig.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ozgefkvi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3liwheose.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wuqdbxzp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sxaukdyo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sqgnhgkr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sgtkkdxy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xjzliigw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yjquewov.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ykvnekay.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tlkmlqvm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtddvbqp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxakqbob.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xeppnlls.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mqodytag.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hxpmnrcf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dkijjhni.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zsyecmqm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhywfars.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hpyxfvnt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ckbcyiyf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pjizrplm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lolqladf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3efrkravg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bjconovs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eozbprmr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zedazcmx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iqhcflaj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3trlexrsl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rbqddtji.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pyouytla.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mhlhavzz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kryxpsxh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aundvosx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ptqknueg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kzildted.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rwbllsxv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dalardqz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wenhyflk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fhwnqjib.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hpcopcup.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fucmljgb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3msivblfq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3frocrhkx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kxcfzagw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3eqybvwfc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqkmduwj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jtbfqjnw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ajbshgqa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bckleuvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dezxehiy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bdubiqlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gloeryec.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xyswirxi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ssxnpjbg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3opetxyjj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xcicplul.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ollqrfhs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yezzuyhp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pxjwzmjh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3itomdgvt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kyhhofqa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3glbtvedp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wdzhnkxv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kaalrnep.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xlrciegl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3spjapufj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rlckjync.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zctigaee.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hiutzugj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bemetrma.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nilblsjp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uffyiaby.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zntrmyyl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3arhrvjvm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yevgvbne.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3okcuckgh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbordmpg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pwyazsph.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cbxjlymu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pmtvcevz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3djbhlkdw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ejgtrqfk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wmtawsjk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yuhkhpqy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ebbpuwnk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qxvnuoye.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kejzjxvj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eisqvkhf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3abyfjyih.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ihkrsnxm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vlwjmukd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3toblqqxl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3inmnmjos.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bpqtswip.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3smhazuzd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxlkhn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cepatzhq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3htyoqtxi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ivijyfvx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pofgijjv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vqnhnyjx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3huywwtqx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lyzwtamo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gehnwnnp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ycgtszwq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jobcyeqo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pezrzoqf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dzzcitvh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3axelyxah.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ahctjyql.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3owsnfqmd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pordgaen.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3obpkfdwh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rwgvutkf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekkhfivm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ebftflsm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ozmlihrx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ggrapaai.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gqvijvwp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dxmqkocl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lmetuuop.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sertpxoi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ylyiiqde.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pbqmpwet.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oyxdxwzq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ywkuglrm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofknhaem.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ovseckkw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fxqsuzzk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3faiephrp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3buolltrr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfobbgwu.html


<!-- 参考信息 -->