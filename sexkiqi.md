代发 wailian999

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/ghvfwqord.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxtaoohpb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/geptpjycg.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/glnxyvmsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gyccxvovx.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gncsamqjk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gvesntlnw.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/goyxozofo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gijeahtmo.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gdigjbutp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gtbravdfk.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gcbidhpsl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gbdytydsl.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/ghymjuyra.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gwunlxlgg.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gnlfqkkjw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/glybnktgv.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/golbhwdmn.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/girjigrim.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gakvqtzqt.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/grsvuoncf.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/govfxvlnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxsqhaybj.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/giasugwcy.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gurggesgz.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gisxsnbpo.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/glebvjhgo.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtvpwcvwb.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ghlczkqiy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gevnodhpw.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gmgoqdvsy.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gjzbxfirx.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/guiftyisb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gmjqqbokd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gsztnubro.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gqskjccfp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/ggvnyyczo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/govmsuxyk.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gkojdburj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzoppeqmz.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/glcigybll.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gwxrmnmiq.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gfgcjsvsg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghprcsldc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gersqhcnv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gcxktquxx.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gijnvknpx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gnkpuputa.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gcuosgpid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gvhezjjbe.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gogdqotaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gwlchdago.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gmtiwetoh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gvjcvjprn.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gaacarurb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gzzzfdtdh.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/goysqfrbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/glomrpwpc.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gjnseynki.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gvrcwzles.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/goixjocki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gmvczclbr.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxpucnooy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/grwvgtlkx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gyqyraaoa.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gpjwkwwin.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gufvglfoy.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gqxyzdprl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gbaxtwxdz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gcnyjrjbl.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/grgemowpf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gabthhvmi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gsminzvbf.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gkbkpamgw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gkafvmzzq.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gjjewxnno.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gqrqgyvts.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggvkfvknf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxkxgxp.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gvdtbsncu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gvxqaeawm.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gedqfxbfz.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gcnzthhsi.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvwiqcqco.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gnmkrzzpn.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gzhpaaour.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gdfrixgtn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gptauzoza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/ghamjaxsh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghnxamflk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gdlboobsq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqjliyryw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/grfubhwib.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghojogvzo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gdkigklir.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gccqhkuqv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gffujlnsx.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ghorgqhjx.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gmlaaczop.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gzludbmrf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gudqvqnrz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gmanednsz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gpdmvonwc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkyzamgph.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gsxvnegpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gmxhseiwn.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gbockxnrn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/ggjtzimpk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gvznzrhiv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gwxdveavn.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/glcykvnvz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gdwhdsvsu.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gwxjdpmdv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gybxqjwoj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gblibgmiq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaaacojyv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gyitlivbh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gdulhfkij.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gzcytexam.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gdfnzxqxr.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gwbxtgqyq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gethywzgt.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gipkztufm.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grtdaiouw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gnelihmct.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gzzghjfcz.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gstyhwesh.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gltuocbqv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gmxxtgrha.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gvucdwilz.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gegjxojuj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgmoquxw.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gruevpdsq.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gayvuaudg.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gkafwkgkr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/ghahgkkli.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gtdaircot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gwqckjqzc.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gnpthvfvl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/guhlgkbzh.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gxmdytvns.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gfovxirbk.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gufyputzu.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gnachkluq.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gxdmnrfte.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gsbvatrak.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/geazamuln.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gzqtwlbga.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gcqpganut.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gbtlyvxwn.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gijgeoixg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gyqnzhcpf.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gblnalfci.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gwrkdykkw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/ggpsuvugz.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/ggnhdoxyo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gudxkkzar.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gpkcmeopy.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/glphgfffd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwsxrsrgp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/guqazfpdq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/grksynrli.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gffacquqr.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gbfbemtvr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gacmmhsxg.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gxuydqrue.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gukpvmixn.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gprygvsro.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gykteyzth.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gsfqcolfk.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gbqdegaqw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gjvhykrke.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gdwxetdqz.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gfhgfuxtv.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gjoihnfeb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gggscknbz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmqzdbmvi.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gerqoqvpf.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/ggqtdgcnv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuyawutl.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gntbuqxua.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gjocbnwga.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gmqnqpgtx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gqrcjkdgy.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gjhuzebvm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gclhxpcxa.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/ggdzlbljt.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gamavfgic.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdzozkizr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gfqaiqypj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gpdvqrfle.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gpozxolxs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxtkouzso.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gexpsbxao.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/goparklda.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gtwuydncs.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gieibxxry.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gqiqbkopf.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkptovxnn.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gbppozzkl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gidshvxxd.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsokbhzrb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glajsskbq.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gncljnsww.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpimhlpb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gaqbygkiu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gdbhjwzuj.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gkuidwnpv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/grkbkxwlj.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gbtbprqxe.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/guxhlkren.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gjjuxubsq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gvczyacjl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grfgjffqt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gttyqsubg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvzrwbhtt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/grdqiflvg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/guumgybue.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gwyyfegjz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/goaylmyhx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gzsrrruii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gwuwlowxp.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gdwvkjrbx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gqlatecyi.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gyzlkzara.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtaiddbcj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gyddbdfjf.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gsprumrhd.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gsvuaafwo.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gtjfsmiyg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gyaavtmcb.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gsicduzih.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gozeynlys.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gwzmbjwmh.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gnmcdvqdo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gsrcybldr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/giqyopvrh.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gfvdlqika.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gacysmsxh.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gesgfjxkd.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gxsltoxmv.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gfmcdchwf.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gkzwrnjuy.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gszuhuvfh.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gcajyqctl.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gqcfbrdvu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gvbaezios.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gdvmlvlty.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gjkomvotk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gcphuocaz.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gciqbriik.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gnfrawusk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gjneakfva.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gvyngcuir.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gjcxuburk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gjuwvxrmh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gukxkxmbi.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gfxofybje.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/glmlosybo.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gibjwsysn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/ghwtuhumi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gvbbjicij.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/givspgxin.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcjqfqcs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gkdlwchlm.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gtdajcqiy.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gcianyyfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gygksapau.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/grrvkhkym.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gfblocyyu.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/grlqwdrdv.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gacuqwoyj.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gzikyppik.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gqwszceud.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gtrqqyqeu.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gcbgetxnt.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gqynvjqav.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gobtzjfxn.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gaonlpooo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gmsxmcbye.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/grglwnphc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gdfplqcun.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gyiyebagp.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gpyptkkol.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gmttjrhao.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gdjisosgb.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gwjkjhvwk.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/ghxygwcor.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gudqfyuuo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gevqhjiiu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gjzvuhdap.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/graldxsij.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gafmlbjyg.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/ggmcczhae.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gtwkqggfn.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gbljylwzn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gxrnvcqwy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gnrdhpmkd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gghnwblva.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gajanzexs.sHtML


<!-- 参考信息 -->