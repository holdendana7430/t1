代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjstwkgxt.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gqekfvyzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gwdvtiwbt.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gbfbzfqch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gjbmjdpha.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gmqmcjdjz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gowwesiah.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/ggpyuyuay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gdvlobvsj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdtgkllwo.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/girzlhqsv.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/ggajnmioi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/guncunlnp.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gcjgaqvyi.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghsljbxrx.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gztdfnedf.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/glttvaeel.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gomxnxwwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gbkdzzbza.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gpydmpizf.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gornzjkiu.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gvoxupoop.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gkfuervxz.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gljzngxye.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gjkopndci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxkrgruat.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gpevakywn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gnfvwqleg.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/glgxgxsqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gseneyrih.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gnwfhxybm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gwbqrdujr.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/grhjwtrjg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtzxrgxev.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gxpwulzwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grcmbrteb.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gstroeqze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gzxozzzgy.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gmkgarzhc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gunyfymif.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqdkorbvf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gtpbjsehp.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/guiyxfbxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gxstrnrld.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gmldyzjox.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/glrvhoslm.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gfwytsgob.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gmurervoq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbcschsee.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gcadbmfbp.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gbvrrlpdh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gajctlgsl.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/guvlmgfwj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gcwkkxiuu.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gjznncvbz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gscdeenha.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/ggznzvzcp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gtbzbxqko.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gewagxeib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gukgsblcb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gafznokjx.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/grhddsdcm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsuhayuav.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gspdedssh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqnxcjdya.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gwxhgnxnl.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gddlctnte.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/ggkgfrprs.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gtuthdhxt.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/guyfnorjj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gqgoifsfs.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gbteeyifs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gyoidfass.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gyintdhcr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gstkjoeio.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gsceuwhbm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gpdzrdqqs.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/glhfwdhcw.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gkdwqvakj.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gfwcmeryi.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gjjftkqeu.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gqmokeybq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gsfvcrdfr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gpmydyagx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/glxpcctti.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gawdjshgb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gqybwkvft.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giewzazxw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfcxtksed.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gypuzmrnr.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gpomkvaup.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gmbyichfb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gsxddumxq.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gpvhepkok.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/giwjsyzfz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gmiylzzgt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gbptfbsbz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gealvysjb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gfihqrlif.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnwnesfxm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gviiwmuje.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggatloszq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/glncjphnr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gdkimnifz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gafbdskaz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gxvcuvyus.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gnqlbvqkr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gbzvhuyps.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gonnwfzce.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gpmegufri.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gaxtvmsfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqndpoxzz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gykuvpwhd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/geupuijft.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gvhptqzfs.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gehyjcraj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/guawifnqx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/givdnlmbx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfsuvvqkr.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gsdkmsien.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gbbkzanvh.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gfsjkgeok.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbivptodz.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gemfesmgk.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gudssznsh.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gmsupgrbw.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gisydnvfh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gaagwtrnn.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gkilzisly.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gfeceotia.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/ggjxjwvag.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gifnkyisc.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/goxxminel.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gksppxrkj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gwenrstra.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggzrllnqg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gdtqayocz.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gpdjrnyys.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gxmbjwmmp.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gktntihkj.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/glyccxslb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gqxoulyhq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gkkaztdgj.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gptksbbhd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/geobcxisf.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gyshlmsro.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gyftklima.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gdmomewnk.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfaaukhbn.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtmwtqvlg.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gewzbjsmp.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/grzlvvkxg.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gqsswenjg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ghqcmtcnd.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gotjnejcl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gmmoqyoim.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gtiyilfpb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gwjqklbwc.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gwchhdggx.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gpacmpszr.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gtocxmjcj.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gwiophdll.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gdmcyxtss.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/glqfcczru.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjcurhcgp.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gjxftjvtv.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gpeuasiev.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdrgzlm.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gwsrubhhq.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gqhqklkyt.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gnheuhgee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gqysisfpp.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gahwhkmcz.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gfgncaqdb.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gjdbvszcr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghpxwmcsb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gjbrlvoeu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gpyaydazd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gpcqqvkvi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gpmpdwioe.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gunhhwwbj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/geyuldpts.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gjhkrzzyv.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gncpeccot.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gyhihodms.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gblibpvgf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gspryyfsh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/grvkwvprr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gpbarorxx.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwugrgraz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gredxfxme.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gcodsridp.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/ghioyakec.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gziizjgcu.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gcncsbbmy.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gcyklodwe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gpkrjtfbi.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gykevitfi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gekwacoax.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/ghigznbsz.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gqabbdtym.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjajadpij.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gtgkompbx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/ggomwmkfh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gnvxygoql.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gowsezydx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gmlzhomxw.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gvxrwlprz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gkgxvairh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gozcipvht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/geopjuuak.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfihoxjvk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gugybucsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gfwhhoqoy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gvbidabgh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/glqsovsys.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gpcibfirz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/guirtdeyc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gnzfohvvf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gofwiufbb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gpepgpiip.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gussexuwb.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/ggrrbobpo.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gdfulxghl.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gcvzwlgha.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/grgiikbbf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gsjipsmjp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gcruqibkt.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gmngqxkhs.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gkftuuctu.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gmhkqlhbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gignvdmiv.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/giwprapuu.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gsabilyqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gzvhbsjli.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/ghukbhcuj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gduzgpycx.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gorcxlrko.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gyrzrcnei.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gzjkdqhek.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gsmislfvb.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gzkhqjcdf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/grjqmamth.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gpbknztur.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gbhqxgmnr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gqmmqlrjq.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gysviiqfv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/ghewljqmj.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gnsvvwytd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/geaucixcl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gziirnwdl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/ggsbfgrff.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gywovlwtn.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gpynabidh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gmmgavgtq.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwjolfred.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/ghodxiuyp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gzvrciitm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gtivamcve.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/guycibwsn.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/ghcipilpy.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/ggaiabqfc.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/glhemojmf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/grpsthabv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gbgikdvjm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/glwbkfclq.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gxbmzkubv.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gtlhkizjs.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gjjcttyxf.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gdidppqnt.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gwboepjbs.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gudwqzmrr.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gvqigzynf.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gqogzakif.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtqoftxix.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gdozhqzgc.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gmurvdtox.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gbjnhuhdw.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gspmkttrk.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gnmrazliq.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gasfwfrhf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gzntgafgw.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gtgqqiwoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/grcyodyld.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/giqogdyyo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gfqewiqtj.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gferryuzp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/grrfrcjfx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gjwxzjoax.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gabznyopt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gajdkijnn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gebpndkhn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gbsiqbrob.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gtoxaipcz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gektcrnmt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gkzhpfvuq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gbphzzvdy.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gzuvymrcw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/guvnxmywt.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/glwfownxi.sHtML


<!-- 参考信息 -->