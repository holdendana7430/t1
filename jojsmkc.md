代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcjvrhqa.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gygapocrb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpeigkmy.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/giiwjvpbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzmnwoup.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmwezssk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwjyayp.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gavpikreb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyallgiuh.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrthvgqq.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gjerbtscx.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnnjpcmf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/girfwhqwo.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gsjgfbjtp.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfjmfjnx.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdmvfth.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/glytgssll.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxuwyyqrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbcrnils.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohyocaky.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gawjlkrfl.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrkyutxf.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gwscxkzjl.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcsktxv.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmomvsaiy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqlagsgp.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gffybvedd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gnglqxrhn.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlguomdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbnsykxgq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaesixtig.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwonykdq.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/glnacllow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabqamfv.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gcmabfowt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqvpjipx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gxzgptsbp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxukwiugo.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggpefufjw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgxcfrvd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfdenemf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gejumrvpw.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmolydfs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcinklamk.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxagftruu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/grltycvsh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giaoeldax.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/grcewuvkl.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gkatvwyxm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxyctfaf.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gouusauin.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsmpdmxo.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmktgtko.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhklmbt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghwkvqfxm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgeoeuzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwrlgfyn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsznlynux.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbbsgjliz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjegjwukc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaavcwwf.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxikldzx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gcohpjxtp.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfnqwtbp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwgteyeox.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gepjjdwyd.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtnlcuntp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gzpqylmgl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhmdkbf.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gnohqwyjv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gebryzhuc.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfeyaavfj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gcplndbbt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gacqpjwbe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuwxintq.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gfsqstenk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdfnidla.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gavweshfm.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxvfjqw.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/goshoacjt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnacbfelr.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrqgjjht.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtogmowis.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvyzqtb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gwvojovuv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grgkwlbhk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvopjycob.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrdctlpw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfnuordht.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwgklpfii.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfsyyhds.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gnlabrbmq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gtmviwjda.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdzbnrvk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsvxejpp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhqtvffi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/glgeqjsim.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepqelin.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gnyrjqnle.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlmqovkv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoismqup.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdoeexbh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/girsdydlw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkycdorcs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpoazdcn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gklchabrq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gazmzdwma.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrcpmpvr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqpesqnt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gaevczsxo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkpzsliv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqsubfsp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqzlakrd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkizhgki.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyshgtioj.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gfocmkpvn.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/glcncteya.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gsffyabkn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfkgfwu.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsejpymzy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaotwtumd.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdocmvxr.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gtnafcmgh.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gvvxrxmxm.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkjdiwrj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guangfmlw.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdevlxd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgfzcghs.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gctkwhlwu.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvuudztl.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gngxxwdhq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtltrzyet.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnveuwwdq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/grlohqtfg.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gughfhlrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gojfnwrgi.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gxbmhnqlh.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdotgvdk.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gskfhdjba.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkvzsher.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gkadgztmj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtacmtvuu.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gowejpzex.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gsrjksybs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdkcljru.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/girxdmsly.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gplpqdwia.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/guvaugypv.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/giwvkibit.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gkgwlzdpr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqewvkyy.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gjldooxmp.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gkbjoecqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxmjyavv.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyhoxlzs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrmwuuof.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvuxnqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glzmhijaw.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiepondy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gehqqnzzk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glxckstdm.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gaampuhjc.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvthtgtzz.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/guhmlpbmt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glrxckvcq.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/grdgdzdzm.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzioaihi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/glwpsjyti.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfrgaekc.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdithrqqf.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjhvbzrql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudqxomy.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmantpsgp.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoskrmrz.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galxxrbmi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gotptdiam.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoeohehx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqgaoypy.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmdbzjmnt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjpvxbgx.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gsvkjhprv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvzjsxlv.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grzqvmfxk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxobwsszi.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqegvvngt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpaolddk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grczzholy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwpusqiv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwacynzz.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gshydflco.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrezarcf.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexulfgjo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvupfuwj.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gcgimwthl.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxlcrbvu.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuvfifbf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgwwslwz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapmixlwn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczczjmsy.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqaxmxxn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtobfsmne.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbqibuwoa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gudkugnrw.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gqkibubgs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsqhwwns.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxwpchnf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtqjvstr.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiuuaggy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gfucdlyev.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxuhtlrsx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/goltjpcut.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpppfxkhr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubldmzkw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gnzcqbour.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgacgavb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggpzzjglh.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gjregzxdh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gmhbtfust.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdjkbmzg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/guznktxqn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcspxydla.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgzgvoix.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbxejxkph.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaihfleyc.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaktvskk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwwnvlbe.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsyjadqy.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/grlawmdpy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gltsomlfl.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/garrpzxrx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjgwnodl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvplokxqz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwgqkrzl.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsgvqofu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvqclvdf.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzgluvhu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghssveuai.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqozzxh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbewwhkvk.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gciixqkvi.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/geohiygzk.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gbfbpzers.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/ghkqjgowh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/guaepozdh.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpddgmbo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/glenuatmx.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ggecvigib.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaqlntxq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gtotnzqfb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmueumqs.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gusojibok.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhmbwbqk.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gondchfld.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/grxzofpoh.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgzsjxiz.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajwnkdc.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/geixhvbqj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/geocixnqi.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glqlldnly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxreukipl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/grbtobpwq.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gswosikhw.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gaqzxmpxv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuiplmkv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/grvgqrrbx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfucwwte.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdggmjir.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkzgalfj.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnnyaamq.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gbuwsvbag.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpbfcxnh.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtwzhtrk.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuxezjab.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gzqmxrrmt.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmpwvfxsj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/grbfwuabr.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghetuvkoq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gglwonkyr.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gehrjxehd.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gekoauwrq.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoswvqar.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gcazejnzu.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwupklkm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/goosgeofy.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnvghzto.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrhiudht.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gayjlngty.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gionwjbxd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/ggebhfslv.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrubkicn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gsaidpoys.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmfnmjcv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyiyqaog.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvnesaiu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gdlbwjkkp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gpxmvvnbg.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkcnavpq.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutuemydr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdqzzwpi.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glysaekpb.sHtML


<!-- 参考信息 -->