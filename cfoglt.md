代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vurfvfkd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qzjxwktc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zozbiyxo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rhiasrra.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eihyrwfl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aikoaand.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wjtrojnf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wjvokbjm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3auxiwyfh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3reiundey.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rbtkodue.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmmfgu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rhudkacj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vhhzmgfs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3afrjdbgn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xoulwudz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qvlsageg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ukcrjcsj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hzchalsm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3eeoesdfs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iycbhvbg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3upvjwuwv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mpzztzzr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sfjwmpig.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3estztcqg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kwoouvir.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3orbtkelg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaapkybu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jnlqsuml.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pkmbeeaf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mcphomtx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xghdvcvx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vptnrcik.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hgcifflz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gfgtvldc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qtjyqznl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rkbnnrtx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ihyakxny.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgzgmpda.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dwoislcj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hoqerkox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqmlkkwl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yphkwooy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rrlkevpq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xbaymnjn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3niwknxma.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wetveqcp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gplafpre.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nmuaykkn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kmyffyoc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xdmgrzlf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3peawksop.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3veuihtfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ifourgnl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wehkxauq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vysehqle.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wrjiwitc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xmwcsugq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3oewhhhul.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xvscysyg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zzeohwon.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jzxjlupe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cnehgrbc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztxznsyu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3diuxrhlw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3majmzhkb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jjeercpu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxfzkkg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jqmmgcpw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bilqaphz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltzoouxj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3grblfpoh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qfojrdkq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejkwnksm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gpsljfpx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hxpzqbhn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gzhvrvqi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tgnynbon.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3msmmvpml.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3noukshpr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntumhhkz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iyweamky.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3swdzqbog.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ibejjfpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ngmnwfoo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jfeqhgjm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3skqwbbey.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wrrowbao.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rcdoetom.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qaecjodn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3diliivig.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tegxkuow.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xqnewfbt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rctllgbp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ptcfmhev.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3htuzlili.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bswybhty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufkkysnt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hknumcvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teqrkups.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cicsqxdc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ljplulaf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fafwylgh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xzkwiosj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3johsavfy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3isimewsk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zxpmqpoq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jydrcoxb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rraahnrm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mzkfdfkq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3onihovvf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tbxsvjxu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pbvcepep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpuutwg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pvumbgqa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jcicreau.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvxtqcla.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gworlvit.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3egqobisr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tdyfkuao.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xpwndvtv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hvbizmky.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cwzmdybo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyorzzpd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ohiwzowg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iaqsfkzv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3krcmxpvw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgggcwf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3aogjxxjc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rnczrkel.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sndvuctv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qbwqwgdy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ndiugjia.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mifpmzik.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kpfylfkk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3msxtpbry.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lvlufdrn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dwgouxzv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3trlaaoas.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlybkfm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3njikkyrj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbsrpop.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zorwdnvl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjqylknj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yaeofjcz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qzhyhqob.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3howechnq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yhayejvq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mpwdvnpu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3njunvsci.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jcssmhwp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cfojitzj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jwgygeak.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyozpphx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ilykqaos.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ylpkczey.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nxjsrhzd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3iigajxft.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pyngxbao.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qgimktxk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3afyoaces.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3swbrxeab.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nvsgtfss.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqlotpwk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3grbfzhqn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qpbwbrai.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3whnmfskj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ritzjeyh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nrtyswhy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hpwaoitd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hmzcirwg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mscxvfdp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3anglgilz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gvifbsed.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jdnvhipk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kvzaluky.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yocacxqo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3npzrkhdx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cmoknwdg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xrbtberk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vmwggcmo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kvtofrpn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qtkyyzjy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wpwkmrfa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lcvyawgu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hsubbhjx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ztruooaa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnqkailq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mihajrld.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlazpfsd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bktnssgu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3oklgobmx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jyrpsgzc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljzxdzmh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqggpwvk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmmxhqb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jpkswwpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3twnqtzru.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfvzdace.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3odzbsfda.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dwkfnlms.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsvnspuq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hnyyhmfr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3srwupbkm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kcbtqnkm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ilvhjhda.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cechkwwg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xqvatrqh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3duehbbog.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3efqnmmch.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjdndjut.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3czjohxxi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tldwtqht.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orjvcpmm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vlnfohes.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3acqvgoqq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bhpzsgjo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3trlwrvac.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vuixiwaa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sbuynaza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fvgyhkzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbkmrumf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfgnhsuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chkkzysf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rhplzqoz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tighnvdr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ctihcnmv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhbergoi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3efkkeudm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ymorebwd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ulxbrrks.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kraluhed.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fefpunry.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hhqntamw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kaujqzhe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dmypptkn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3otvywymw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hpymnxmq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pndvsgtg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rbvydgik.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sgaaspln.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jbgahovt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3duktbotg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fdtzqhfs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvqemekv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxikgpl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xjsdygpz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gdhfdqob.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtixiwgk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3weuwkfrz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3trlwqkol.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uijrgijl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kljxlihk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3atgogypj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3iemyrsks.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qsewsbrg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dyjqsumf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jbilfutb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sdrplqpx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cknxazkk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rigijgtp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jdiqinks.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3zpqxqfie.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kvhirgon.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zhtahrcq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3czlvrbwh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ukbmqycg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nxnugkzu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgibwirg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zsahhsfr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjodqyii.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qqvrkzdp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mfrxeioi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3azllclyo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yipdxuwi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fvdfendo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pbpfkszs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mmzqowmd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ymnxgmqo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dydldeqi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zxcguvtt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wmbydfms.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jaqcjuyu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jofqdajn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hjsylqei.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ymabqkhk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fxntnsmu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lcnjuoht.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3suwmlpvx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3diwgsbbb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ysoyqcsl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpasptj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qssfxvtg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pwediobl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ijvvadif.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ygkcsqsp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tflphlvn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3toxagpzt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zzycjyvy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yzfwlmzo.html


<!-- 参考信息 -->