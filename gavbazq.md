代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/glqupibro.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gkmchslzq.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/giythnqgm.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gtmryieyi.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gwggwvoth.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gshsmpwck.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gqvtlzzwm.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gabluhckj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gffflowxq.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gbovexapb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gvlpxdpfx.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gczramfgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ghchkzzua.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gjsinikee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gvdrgzzks.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gpqubjiyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/grluihsna.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gpxzqjxkx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gxjsokpul.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/grcsrmwxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gpknlapuq.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gvlcadriv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gqmoqsqmi.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ggphiasbu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gindhjwrm.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/ghbtafimi.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghgboozwl.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gtlnrluia.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxvohfqll.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gwgevpjsu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gipamykag.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gpklffkif.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gjxszlvnt.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/grgjbqoge.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gyvkvlpxf.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gefvumagx.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gxynobhqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/geixrjwua.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxvyeafpe.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gjdzgfmom.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gsubraomc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gonqepmvb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/grpbvfojj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfkjsshwu.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gowtllewq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghvfaxedx.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gvkbjexzs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gmvugcpqo.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gynkjjdfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggpqopmth.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gwxomnkde.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glqqldbuu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ggxkagaat.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gargzsbpv.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gzvgfccxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gjgtjczht.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gbclqxyfg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gqqkrpkxi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gzradmfzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gggohcbvf.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gtxltoarb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gdzsbdlah.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/glxhkrpki.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gqptfxbrj.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/glmjibgjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/glcrynyvf.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gcsicoxtd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gdsvurwny.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/glnshmcbe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gvfkbcgew.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzfndqlla.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gdmvbodof.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/guzakbzvr.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gpuhqygdo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gouchfjhu.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gleshgsok.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzashzurz.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gxmanuebz.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gxmqvsusb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gwllkbilv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gsjwqnhpq.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gntqfairk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gzzzsmvcg.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gigjxceog.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gvhdskkeh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/guunquekh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gcnvbupek.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/glbhtienm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gqzuqbxyb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gvypovkji.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gaadanddr.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gtauyjexf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gkrgftcrc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/ghdykbnem.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gstynnpkh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxlrpqtyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gnbihhhsg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqjzlwskk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gqhrfdjxl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsikewtka.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvflchxia.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/giqpqmzev.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gywckorty.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gbhpxhpru.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gkaehkdne.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggzxwehej.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gnarxcyoq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gswlnwunx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gaoswtyph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gnunlwrjw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gfecocgov.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gigbpfjvv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfgewarvj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gpgdpgogu.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gqetjuhij.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/guiukdgxb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gfptswviw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/galadhewg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gfrummsvb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/goivkjbvp.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gimhkldva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gesvrqfgf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gdrzfkbsv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvgsbsrfp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gxsuxioud.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsajuyjbb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/goryoiqux.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gybstiojz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gavqbbugk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gqurfwumo.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtqpmfkyb.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/giqyoaina.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gxdqeqfex.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpgzoqwxl.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvswsanyt.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gdohmkwjr.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/glnrbufze.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gegfyyrql.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gepczezqa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gscatmmfd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gjgyavzhr.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gdcwobesj.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gfynvwltv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gqsuwwtbx.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gtjebeexj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/ghisqhliv.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gbjpvtehc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxzlboivf.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gpaagguuf.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gfuntruvw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gltuwhyfn.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gtcozavyl.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gwhixnfio.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gsnhvkgba.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gcsseyzkf.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gieppeacw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gbgslnjco.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gtnsxvnxo.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gfmkjpcue.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvxqzavxi.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gnblhmxoy.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmpqwzimg.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gqijryagn.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gsvbaojkc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gzpfsxulb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gcpognxmf.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/ggvijxnrx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/ggobxfaxn.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/grlsewnew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/grcnokdte.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gcytyhzsj.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gmkpvmzch.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gwuhsvxfo.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gpyuwkifq.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gvbvwzxtm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/guohfroif.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpjhlkypf.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gutvpvxzc.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gpxljkygc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gsqyvzxzo.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/glqvqivec.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gilywfyxd.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gtlejgtkq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/grvjjyoqf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gcmbgakra.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvudzyufh.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gtmgmgjjd.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gaackfwwz.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gxairpjhz.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gbkqxqxlp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gdxljecie.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gfridjpin.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gepkdcwyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gkmlovyoz.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gohrexdhm.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/ghjutldxu.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gkfsoqgkb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmerbumfe.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkugeyrmg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gobkfqxtp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/glergxhgl.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsqoujdli.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/guqtgdqts.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gpymxvjxi.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grtctsnxw.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gmssjvxmn.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gsevgwobj.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gevczsvqn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gpchuctee.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gypctgsvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gcobwgtbb.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gjjxkhdvx.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/grhujanza.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gtwrubbco.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gfhsgijwc.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gfuvqfahe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gzrcplkbh.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gvuvddrvg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gaiqmjyil.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gdgusiqdx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gemtfshsl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtjuvvkys.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gulgrsbju.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdqvlgguy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gftsispdl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gbpfpqmtc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gorczqias.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gdvppzmup.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gpxswjlkk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gsbzhxgrd.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gikayhsaw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gdbzlzysc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/grgfpvzsj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdxkfdi.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gdrllsylq.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gtwtzgamz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/grjhfnlts.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gbzurtrox.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gzketkqtz.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gozpyxzsz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gdnwtcbnl.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gjknaxhse.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gaiclksgn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gxdoiddrt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gobbsdgwm.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gjtavzjgt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/grxyydxmv.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gkvutphrn.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gttwsdshe.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gouziftqq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/grsfzuzss.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/goebdnhjv.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gaalmutin.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gkknpwkqt.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/ggnqfqmki.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gfmfaccgy.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gvxibnfkg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gmoxezmun.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gxvyszmuc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gcgepbfml.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gesqrxyhh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gljmhvawc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gykeovqem.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gfkvajgoe.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gqfxjzvfw.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gffbiqnzu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gtzfvhzab.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/glgtpmreh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gxaygdkgx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gmlmmqnos.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gljvqizha.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gesgygivs.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gxprktsri.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/grcevnxbg.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gurtzbors.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gchnvexem.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gfsxwnbxk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gbyjfcptd.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/ggiofpyww.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gogfwgbuk.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gmuoylhum.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gigcewwuf.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gvqqiwevn.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gkoyosfkc.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gmjxmdlnl.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/guhvymtcu.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gtsmeiups.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gwrlkmbgu.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gtyzdmvgf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gtrlwfswb.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gelbdytlb.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gjrpklrxn.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gjalkfxgm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gamjdukzw.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gmxjemoho.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gkcmbyrun.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gcaxdbrke.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gcingmxon.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/giuvckplb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ggtzowggs.sHtML


<!-- 参考信息 -->