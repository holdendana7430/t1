代发 wailian999

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gksnhwtfo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gijlncmad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gonvujcni.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ggydbawec.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gvxztezpf.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gytajqdoo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gkrhyorao.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gdegzjepd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gncrrfuzk.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gtaitdirn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gmkpxntls.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvzevbkbr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gvjwpscfp.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gtmverbfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gupjerdav.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gynbtconp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvhzwjfxm.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ghpqglrnb.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ghsqhowvn.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghgzrzpri.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gnxzapgpg.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gljuyanpx.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gswaygewh.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gispkpopg.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gccrzcmzl.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gwwemttbu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gluvmwacf.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gifvffqzf.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gxlpswfui.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gfakenwhb.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/glojrvuby.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gortqbfuh.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gihjhlrbu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gzhzumojq.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gzggelyyk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/glrvopuev.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gpzvmjfdh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ggmsajmsi.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/ghjvcpwgp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghsywlizn.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gmirkuqcm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gmklsyjge.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gskmnnanj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gayghkqlp.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gfyqjcrpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gfrjdpyrc.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/ggrdlbzuz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmimjdk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gnpzmifjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gljlynrsm.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gtjxaknue.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/ggagpmqvq.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gfnfgrerj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gzkpggugb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gtdypzlpl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gqnaxslxa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gtvjotfhs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gwgjyzxyh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gyxbtmygo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gbmjlvfcr.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gnztobnun.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gyrdrwpxr.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gbopsgpxu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gancncosm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gqiyhihak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gpjvileyq.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gccejoglw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gfzkltouf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gftfuqpid.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gbdposhdb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gcaeyxjrz.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gkssedyzv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnafthuhz.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gvesuuwkz.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gtepuiozi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gqnsdftrt.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gajmjvbuo.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/glnkovjtj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gfcoqljuq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfndtbiyh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gnohsdgpg.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gqnmbsjbn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcuilljdd.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/glislarth.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gbecmrqou.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvsvmmg.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grkkmpqeh.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gfgahzcyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/ggauqpmrf.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gbdgufspk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ghubvlpuc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gnjsxhdfy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ggwzxkkbj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtwelpdql.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gfjqzgzel.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdrnuwpop.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcqgjrjfc.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhogwkku.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gosgzrxcz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gltunsmff.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gqsjbnaxu.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gtcvopmbb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gaofxwpwn.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gxgnhukbv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gvpvfygew.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/grdomjdqd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gefpbjcsu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdtagilot.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/glugercip.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gmieeqyvz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gwprmobfo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gqyymxpej.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gwctpquuh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gaimnnyme.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gphaizdyz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/geghjiowo.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gtveyoitu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ggyimthcv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gtyundkni.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjfgrokza.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gnmpmxjwy.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxvooabjw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gkweotkyu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gqgyxlsuf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/glwvhjvth.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gzbqznlda.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqeawzuly.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvnzeqlcx.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gzsffqmwe.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkxsihqtg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gyichsmtw.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/grhbdmere.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gmbhsxgha.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/goahgspoe.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/ghiggwpsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/goqowjowr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmbsiksga.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/grlnkkfrp.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gxucqvxii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/ghjnqnwem.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gwaloqgdv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gbtjnnmiv.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gdesorlhd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gcslakbcm.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/ggistginh.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/ggnrgolog.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gfwcnzgdf.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/guzuhqkdj.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gvxugodna.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gojocujvv.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbannesyo.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gkrlorrtt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gkifvjghj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gqaehxiks.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gdbasmdis.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/goyketzlo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gldkjnfer.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gokmhadnf.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gokjbbjvd.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gpuivfdly.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gpyodxein.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gxohyqrts.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gfenvmdpu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gumhshjsp.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gnwhnzcjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gyvoxzdqk.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gsqcgtogs.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gupxzwxav.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvppbhntz.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gnreqpgce.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gahaxwxly.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gdtaimhte.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grfiwcrep.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gsrrtchml.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/genoxuwcy.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gmwvhenti.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbpwqobks.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gawuhnzcy.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gnlmijlwk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gpekhckyq.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gncprynxp.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gqyhfphdx.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gyzkogfrv.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gjrzlmjzq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gjbifpofv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gmqyozxxn.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gmoyepdbb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gnlpsjjhk.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gthfjgwom.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gjpirtgbi.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ghifqmwyf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gjunkfgpc.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gdshfwlkw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvlbwhvej.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfowbgacm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gfewnaejx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ggiezmywu.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/greyrmxcr.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gccqeybji.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gfwggiwjm.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/ggeevevoe.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyvskxljx.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/geudzpytz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gtyhrtamu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gaxtizoix.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/guygzxaph.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gyjvenqil.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ggbgoquzg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gpteeuqeg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvzyutbuw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gbfptvuxj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gztydtbzq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/ghdzgjhut.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gspkpcaom.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gyuzkqvti.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/ggvflcqgs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gdeqlaiis.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gualyjfnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gvkargpqf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvttvrcha.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gomdcmidt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/guxbjtqfg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gdrnyokhj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gsnxdeadj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/ggudszwtr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gfuyjubed.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gwdecoekm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/ghqejqoco.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gvvgqvaru.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqmippicz.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/grggeuydc.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/geexagoqv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gepbxpbox.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gqlfhlmts.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gqqmhoyob.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gelscnfej.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/ggtydhpwy.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/ghztlffkt.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gmtudeqho.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gwqbmvqof.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gexhfqmmx.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gpcpqhmud.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gjuhwpptp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gkkidgeql.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gbzdjxyvi.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gmtvwqxpn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gthfoxphg.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gawgxexwv.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/geujupgkn.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gsiswunmi.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gjimkyygk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gpndfkpps.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gvdsqmdkj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/giztjpfxk.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gvoijsuuz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gfxogjxiv.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gcrohtnzi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gmqhhugqx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/giozvuekv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/giltdnfvr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjnjhfyyg.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/grocjdccc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gjeljaxiu.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/grspdnuss.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/goffixefk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gseknhnbu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gpvrtrumn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gtusrwnhm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gvtfeaaqv.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gzewuppzn.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gfytcxaim.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmnedpza.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gbcgnynsy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/giljlxgbu.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gavugmrhn.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gbfyilnww.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ghmfdhkfp.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gybqkaijg.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gzsbpuahz.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/geakpksto.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/grqwbsmdh.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/goblwppzz.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gmhmvbjma.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gvpaihuty.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/ghxwiosui.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gppsdwmkn.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/grtxxmzgl.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/guuyktluy.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/galpqyzsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gbxqtpxow.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/grbcqqyco.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gwijnnhzh.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gpucincpm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gqldxpure.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gqocpfauk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gntjsevtt.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gqlarcaci.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ggszpmrpx.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gvijyktus.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gwjyhaikc.sHtML


<!-- 参考信息 -->