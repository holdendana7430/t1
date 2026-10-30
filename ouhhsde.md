代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gzzunxscr.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gdjgtityy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gijcvgmzh.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gkbzgzxkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gcwzbrswv.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gliostdcc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gonvgxkws.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gjqghbzks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/glxragyru.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/giknemazu.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gzcxzmcpl.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/glriqiqko.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/giopjovky.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gciticikc.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gthhlgbgk.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gbiyynovo.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gdncabnri.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gfpxrsigo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gywcphpyf.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gzzaffxgi.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gqlqzdoua.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxbwftiic.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gkxqwscbl.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbwubljiw.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gcllmunce.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gfwgogleh.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmmjwvvim.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gsqrnizis.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gnqqnwxmj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gxadygjua.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gokswjhgk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gibrasxyz.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/geyacnxyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvasbysnl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/glutyggtf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghljzztku.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gqryrfwuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gxvowrtug.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gluyyihgy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/goisbejom.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gdrtpuzyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gunrluwmq.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gxoumyahu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gwojhirbo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/ggeqnheja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gtllbrmyj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gegauawnq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/goxyujrpf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gzvnxhxft.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gpgcjatfy.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gjeroemqp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/glqwcrgnl.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gcuyszboj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjduwywsc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gvrhruomd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gzgkmatqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gertqmluy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gcdgcnnsn.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gizqtvssu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/ghkuiagzp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmfmdfb.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gqdbmoypb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gdvwghnaw.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gbauympvq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gapbuzrrc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzkknawer.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gyklqwvon.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/ggbvwbdsh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/glsbwuonn.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/glzkrabye.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gfkeopbco.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gxhpqtxmg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gwbobrhzv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gqltdhvzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gnxhxrfah.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/givlqnzfq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gbswlfgre.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/ghowuqgbn.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gnkfxehps.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ggdbiaoxy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/grlmsupfy.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gcgzdruow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ggnvmpkwv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gxzaxwuuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/geocunxai.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzzaeckfo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gnvtiztbv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghrwgmcye.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gojgtqpqm.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwepeeane.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/guhnqfoif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gxrgjeqhz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/geayaosoh.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gjxytpopv.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gmhmzxavf.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gnyswobfg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gvtuqozqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gdfjfjhpg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gozpdlztl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmiwnmbhj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzgswjvpa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/glurphfhy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gxgrhddmw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtyzyebll.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxnzwbztz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gkqegcqfx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/ghinryirx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/ghxdirstj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gwtquzruk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gfwdwlxmq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gjfvmkwck.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbtrshezd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gwuyghhnw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gztrecozx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkaltzxcu.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gkfnpdvvf.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gpkxjrgdh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gvwonbgpb.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gcrjauxfu.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/galbpxoaz.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gpqdyfyvg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggvlfybur.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkxshzgst.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gawpppveq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gfxxwvvtx.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gwjwchkxz.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gtbuggxku.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpxjnsfuv.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gvnczgobq.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gndiygcqg.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gohtsnzod.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gzrmumxcr.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gsezthjym.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ggdoblktl.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbghlyfdr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcsbyupkh.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/grflcajlm.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ggmvjzlqt.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gcrnmkmyw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/ggxqqabgr.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gwgrrxjdx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/guhdaxdct.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/grosbagef.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/grrabazfr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gzxufukvq.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gohobrqnz.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gzzflrpuh.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gifehxgsc.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gptqpihrb.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ghsuifhio.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gsmbopkub.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gkiiknujh.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gjoekcswg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gxdvpibbg.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gpijbcaby.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gghyxkzxe.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gqaxjckos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpmoxlkpn.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gnqixdelj.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gxevnjlfu.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghjrjljph.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/ghbdpuyxj.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gwqpiookd.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gbiiygamj.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gsxvkiczu.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gjxhmsxbq.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gqehvgfet.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gpqpssnvg.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmzqewubc.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gdtxmmvwl.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/grwpsndsa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gjbnhahbc.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gnqkkbmgo.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gxyasndrc.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gyhnjodyt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gjykejvef.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gxwirprkf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gykudollr.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gmwhvorhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/giqonccgn.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gitobhktx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gpedigrkz.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxetqzgug.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/giemmzhwr.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gvywzoifm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gabvctfju.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvoyduwhm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gjaqqxbkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/golbiacik.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gsbnvwdpo.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjinqoqwv.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gsjducumq.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gzvlqfqqi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzelofetm.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gvqmnqkag.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzfeyccua.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gmfatajrs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/grvunxbkb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gpmbhxlqq.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gtejdflen.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvncwmjox.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwungfmra.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gqlofirez.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gllnwdrvy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gcggeskri.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/ghsngyojw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbfgbbnar.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gxphvxoki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gprvsqvtw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebwmxzjx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gwqccrmhu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdzberwak.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gqlgvjhzk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gbbflabba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gtpyrybbb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gogolxcwy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gsgjthshc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gdhsuzhqq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gjoprdaqb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gxkzjsbyo.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gvfyrbbgy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gkigfxsiz.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gwtpukhkd.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gduaqbnfh.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gqtgglljh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gyqervnaw.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/grxxlzvsz.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/glowfzkrh.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gnfdwhmne.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/giiuenuui.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gsksvynvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/grlaeikbk.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gmyqrqumq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gahcavsmj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gpyapuaht.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gucrjnhcv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gydgohvza.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gsjavlmvw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqnreyfjr.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gifunrnyw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gqkbqyaqh.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gqpwwenpa.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gxszghidh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gwkumxuhv.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/grerdkbfq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gwskamcxd.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gvnnigoct.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gtxylcurb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gfodvcqbt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gesjyusya.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gohvcomzt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gzrfbnjjp.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/ggvenpazd.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gtsksbzry.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gptyorfte.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/ghnbvgber.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gedoudyda.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gxhlrzglu.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gsmhcryvk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gqqzaprnz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gqwzxnfxj.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gjmilxiwm.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/ggseftxhh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gwbtpybni.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/guzrjdphk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gmkyyogwn.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gnivimqnr.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gilbghcdm.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gnioujxiq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gfhtcvppe.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gcrkqwwmv.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gydubbjll.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/ggyssmnnp.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gqwuufplh.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gkllvrrjp.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gvurteztl.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gbcatyxfb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gjsmsypta.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gbrribyzv.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gghotlkfj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gnpxhtcxh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gcvmfoesy.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/grvhujhpg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gwbkvdoox.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzgkdix.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gbjvfwgrq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gkueyrhmn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbxcpgh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gdnjgdpez.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gskodacnj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gzxltagfc.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/golmzkjsx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gvvqrmhdu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/ggerlxrxz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gxqrlbmny.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gkwygarcf.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gmwsvknny.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gpbklegrs.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gfagkiqsi.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/grbptdhqy.sHtML


<!-- 参考信息 -->