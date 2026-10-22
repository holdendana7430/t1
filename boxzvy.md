代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nhxjbmdb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dwuuymtc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2umtudhty.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uiothdns.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2culkbunp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qeduptzg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nheeqjeq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cyyuqmhc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sgwgglck.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zsypxvqe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pokdocpg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jltflrmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nrvfejwc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ddhpflwr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ffsgejaz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tjrzkjmw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aizusyuv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xldlyewo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zmwhiaat.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2lvngczwl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2aornxvgn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eakjeolq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jgyxflph.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cuqyxcuy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qcfwfzle.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cytynuxv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lzjlehpu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2keebihnc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2halovpfo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jrfjdbla.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xpgsdrxx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gmwwvkni.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dhkigjyh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zvnxtybz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kjbvptwg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2liezceim.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tgsiavyt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wthyuhlf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mcdartrq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yugqjwnl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sutybidq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2buxkuvsu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bgposapo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwcvnvfs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pdrpxuac.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zyhwvani.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2umjpalqi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnnbqpgw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xtllusmo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ofkrvxxu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2iqoqwatc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bwccfmht.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2krzdfsne.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lhqatrba.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jauatvcy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yoinijfh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hdarepou.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cgouelgz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbovwqyz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ungrcobg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tyjjyqol.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2azvsioez.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bxxyljkm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ewuxself.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xvymvshk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wcfymaap.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2soczuxar.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2iertsbjm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vnsmoseo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ewpnbryv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qgfvshjx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kaowrotw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2meigmuwa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hoeygnon.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fdbdxihm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jlkcevks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mjsmmqag.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fzphrptn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ckkgaojr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2oxfxkzwh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpbqrzv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dquwspvd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bpkbfdow.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ziktvwba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lxicotlh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bldqbnxj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gvkgwtvi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jrfdxhwi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gpfbjiye.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gqgydekk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2uonlrskd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sxovfnay.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ehtnjxyo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kewvnlfh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yffezqto.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aupoiwnl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2llpuboeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrwddmuw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cesteugq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djnohqcx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spyuhmfn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jiswhpcd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hvgtnwcv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bptylnsn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tktnhizb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kabvrlox.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gnlhwods.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xhckkxrk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wdhluyoy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iumduyvu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ausxwyrm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2poxpgvok.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zegyyzcq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2amksufxd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ftjhonly.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uirbchkm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ppqmsmsx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dvpcqbie.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqanoqas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fjkrjbuc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iprzikuy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2beflrhzz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nitdylgi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gbrzxwps.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hzezneud.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbcriekc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehifbnzs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vpghbcnb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ijtztskn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2onilpbqe.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mcjrwnun.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2elhmknvf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2oairlzoo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uicwddmy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zgevysgh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yspbnqyp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hhpltmzj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmyzkqbp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrqicl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ekrzvcge.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kshpxkbo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2azremqer.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ahtreokc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gngwefpd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccdvpwkn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ebkxoycd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uujferml.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wvgxkshy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2imogaaap.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2khrgsatp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jvfnxzjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2etpyjqea.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2roygxdzc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sddnalwy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xzytosjz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2uzayhimf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pfwphjzc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2thqtdmqr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzukom.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrcujwp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2omngottu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nbizpzne.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtrgkz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwufbaqv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pseqhjgc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kswfnrgt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dtjbddyh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fureymqx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2slputpfe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rktkajki.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqkcxmlj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xcyjscvy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nowxtfid.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fydzvkei.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ejxesanm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mmbikvdv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cfbecvrq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rwukwpek.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ssvlozli.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qdfdhoam.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hlhmtdcg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uwvmbdsi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ikiujllg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2grfswxuj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtvemy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ldzhhoit.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2spayaafh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hplpoqqn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cswbhoqr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dpnpyapt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vrnnqywu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2acncoaru.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jbrzdxeh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqpvctxu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mamavnah.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ekyeixnw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oajlhtvk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkthcvfy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pdbfqvqm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mvwaxzsn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lstsammh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljcslrzf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czfxqczd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sagwawee.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2spbgvshp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rijbvmeb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vtqbfgbg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ucshwcvk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2eyvivunf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ahkqabik.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nbyadojk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2txratzbj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2inuqgwcs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zrasqfcj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ogvnkvdw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hsogexpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dwlghelr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aqiubmnz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jalobrbl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dsxxavik.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2apvhzcrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmlrafwg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2npffkhem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckvjbmuc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tkucdxkm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uftrqulk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2khfzvbet.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2txxwsoro.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mqahwhnj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ddttynwf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nnplslhl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dusctfld.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nxluhiug.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aobqxnuu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gqzqakmg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uytynnox.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kxkrbjvp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmxpys.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yfyhecwl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2suwauenc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2exomichf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kppxaljj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jpcaomvu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2beitsdxq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ewgjijuh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lizlxvpk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzokscwh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sblqchta.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tprtpqbx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pechylpm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gtsozxbv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jewatodu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jstbnqzb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2oirpdgsi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kvjnisqb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rbojenqt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lfsnrrro.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wfakjeqq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bsvgekqb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lodzhtrp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xknpjagq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2yliplgub.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yfjahbre.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cpevscho.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kgsmskxi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bvpxivwf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2chelmyfk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ucemwjiw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2exydazps.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2tgaxgpoo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2suhgfcot.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uzhqoaeh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zslgkylk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgypajb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2exmowwmb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zazewazd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pgbdvraw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wkaiobrd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zaszzljr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gfdkcvgy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wyzepkpb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nsyrfpzl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2elpjyklb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kyijtvnp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lsbsvfqk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fcvzuked.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hptkcxsv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2uyywnckj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2malifnhi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qebxfkwy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vegdxyio.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwxvqir.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cvcroihc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hoyljemk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ssknckkv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2emjiqtpy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rypeliel.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xyaylgog.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2abyngddz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tznkpbqa.html


<!-- 参考信息 -->