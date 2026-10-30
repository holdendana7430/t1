代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gissgkhfq.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gdqptycnq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gfrfodlbn.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gcojijceh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gmyhswnxq.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gmwvytikw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gtlssnpqr.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/giuzqcpqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gffzkmuom.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gtnphhspp.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gnbnmqgbw.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gvovzqtlh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gyfavfgby.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/geruffhfp.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmiqyttuo.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gzlylxesp.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gpdckxfws.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gmztnnasq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gyaifbpkk.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gamvxcbij.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gjjskvjiu.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gptqfpfbv.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gjfhnlkfe.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbuspnllm.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/grolfzmaf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gzwhcmsen.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gtanignkv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gjbydxfzu.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gpienozeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gmkjjbglo.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gmynqmisu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/ghvfndycd.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gceycoaot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpyghuyqg.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gujjiqmxz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtwvgggsd.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gilkweuqn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gtypfcoty.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gmjvkgecb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gpxctkcdh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gmiilxdyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/grsdzenmo.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbenlurow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gwysygupq.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gffszcjpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/grxqjhtaa.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gjvrhxlqa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gfgnnvnkx.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/glfmvoygj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gugirlywk.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmkhanupe.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gbtkvkxzp.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gmyobpenr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gfobsscrk.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/giutrbuyo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/goyvzelim.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggcnjdkyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gkyrbyigz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ggdgojbto.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gxijujgfw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/ggrgekbpi.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvxufdfhf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gjnxgbuyt.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gxosnvxfg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwtcjrtiy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gjnrpvixn.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gcvkjivev.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gbhfowdpk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gpahdvxrk.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gpbrujscb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gaujcrixy.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gaapjqssk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gymmeywxp.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gkipeimuc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gmzidoijf.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gyfunnzfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gdzoqnaux.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gvnoookzn.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gcuvoqdiq.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gumdgixxs.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gkxfmiehb.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gpgsxwkul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gyjziqcsa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gucrzeimv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcjooadgw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfnyklxlg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gcxehbfjw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvrizjp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdbnrekew.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gudibzxno.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gdlzrvzab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gyrdggevp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gzlgevlpm.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/grubniuqw.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gwntsdpcz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/grrgrsgox.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gtvrwfhhp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/grfelwila.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gamyoatyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gxuhnnjge.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gwzouipqy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gpjitjspn.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gyjetywwd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdayqyprb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gbdjoqqik.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/garavwfay.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gqswvstoh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/grfbpdpsk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gljdifdhz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gbzhqzftv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gcgjvsgte.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gylglpput.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gfjiudbdl.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghpdyfgla.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gplhyxwgm.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/geciegfbt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gbjrqfila.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gmdpfycal.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzvgtrq.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ghvuyzdsd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gvpfzirnn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtyuynrkx.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gyamxmvpc.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gpurjhyda.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gymbwueea.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gshlucjbg.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gcknswznf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/ggpoeyuaf.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gvehstfws.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gpmjeuous.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gyugznfjc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqokjxgom.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnzqubgxp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/grsgtqlun.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gyccdrqcw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtddinstm.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/glmilhjwf.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gpocfdjaj.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/ggtaagiuk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gxwywiizn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gnllmkrkd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/giehzavmy.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/grexnmojk.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gqpexiffp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gvdkkbpbx.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/grxoqpqya.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gxzvkqhdu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/giolqgbnx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grjtydghw.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvrhznvvw.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghanclrsg.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdizcnugz.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gvypsquca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gpuoopuli.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gsnrmqbow.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/guxjasygh.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gpxggfipa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvoekcitb.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gudslhafq.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gjjmhdchf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/giwivjiyz.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gzppagqqd.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gdgwgppfw.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/grycvmkjo.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gninrbibr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gshcwwqax.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gskrdepkm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/goqjwgekk.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtbdprmsu.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gjryhnudk.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gtmxuzwch.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gufghiohs.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsbfdguzh.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/goecmdrjz.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gzaaepkmy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gmnynnkzs.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gjcxtbdix.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfurpvcd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gyuxczszf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gqcdumizr.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gmlmbgxcr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gfydcdviv.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gimpnvuwz.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gwrwkjxck.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/grhzeheay.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxjgjjrtg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvuzclasd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gluwotuxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/glfqvpuko.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmdaakopo.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gnhkgjbkr.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gttnklwkg.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gwuvpgpyr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/geebgqonp.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmwgxoybg.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gewfhuqdx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gojxvfuob.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/glggsnwsg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goczwiede.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gbtgyysrq.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gevecdfye.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gmtmerlxb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gudzhlruu.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gfboxhkkd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/grihfrsza.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gsmdjgmkc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gqpviexup.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gnqocdfrh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gixfsfzwr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjefokpp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/goxdxrbda.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdbveflks.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/ggehpaqhs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/ghclpyaeo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/grwbvtebn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaeoptvku.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gzgauwgvj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/glpjxkkpa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/guilnxfow.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gjdztjzpr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gnpouhctg.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/goasgsgvj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gdumkqjal.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gjthylrwi.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gknuntngd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gnxlaiabt.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gsdsaayjm.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gwscjxxib.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/grncwjkki.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ghkhfiium.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gefirxnee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gfezpugls.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gwsirrdvh.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gizckouue.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gousgqobs.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gpvxvblhg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gyszyxxaf.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gjhupzvub.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gsmzsyhij.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gxpeywpej.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gavgluvdk.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gheicfabw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gtgqjdhzt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gtudnlvtx.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gnxkeeqrx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gxccpehxz.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gvofkhohh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghgsenqbl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gmlwaulle.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gopwkajaf.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gaikxdsan.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gxsnrqylu.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gynvjgnyk.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/godkiflpz.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gozvcpjfc.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gwaeccmpf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/ghprepkks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gaypdgwpc.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gifcawnkx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gbmthswdf.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gvrhaxguy.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gwdauzxcj.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gshsslhwl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gbylfwzqn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gahdhwumn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwytomlqp.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gqfjnxmyh.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gtnnjotim.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gibeiynbm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gkkkduxdq.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/ggqrlwwuu.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/ggaxgychh.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gljmqpwac.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gbmjfwkku.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/ghaapziep.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gqswmgndm.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gnhwthaop.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gqgryiupl.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gcrtxfjdr.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/guvsgubcf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gnhcqmwzq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/goewnrqmv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gynmitopm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gwyrsittt.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gyxjqdwkg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gjnpflsua.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/ginasfone.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gjuqfahxh.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gtotsvspg.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gdxihajxv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gixacgswi.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gqqzttmjs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gzduiaapg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/govhkgido.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gmrjprlgo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gwqtvcpgq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gidgmryaw.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gweculycy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gbijvslfg.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gbxhvrokb.sHtML


<!-- 参考信息 -->