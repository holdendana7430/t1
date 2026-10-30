代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/grmttvjqe.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gmqjjnwpm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gatcmuuio.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gdwqbxemp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gawlayaau.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/grshwuucm.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/glbwmkvzq.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/grebpyzky.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gvanfgkby.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grkmlhood.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcaucvlrc.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gldlwtzsx.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gjvuriebo.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gkcvsdged.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gnrrzwpnh.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gwonxpymd.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gaqfupmfo.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmnjqrnkb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/ghqtshjuz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzifbqigi.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gizinijcl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gtqwfayjs.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gfionnqle.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gxfrtmdtm.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gvegsnmma.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gstcdatcf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gcldebkra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gyarqpllh.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/glqxomuim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtvfdjger.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ghnqgoqoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjwafwuzj.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gsrrldzgx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gnmpmmguz.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gluqjudrz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gqdvsvzee.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gnllgkcdg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gymgdkfyc.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gxyjalmdb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/ghpgtkhpe.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghsylyvvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gtksmfvti.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ghuwhbjbx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gqopxnkxz.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gujwrzevo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gewmciuzh.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gbuwsdmoh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gyyfzsixp.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gukuaomxy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gvdjrgkbo.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/ggoggtjoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gjfszmjpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gvylpymzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gjplpttmt.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gtemurcwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gcwruiksp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/geridelyr.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/ghovgqlfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/ghcshzyev.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gsdeviqhb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gosgssqbr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzrlmcbnh.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gxpywgvjq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gacsoxyal.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/givttmtte.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gkspmyebp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gsfapktid.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gblamxoca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqcqjpcbv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gldbyagjn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/goyfrxcvu.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gdibppiav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gtsozegop.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gjenxtzgq.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gsewraggp.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gqfkaskos.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/glhlhbbia.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/glpmfpesc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/grvbdqdlh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/glnjweqdh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gynjwocph.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjmvagcxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gcrwisdqc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpfpaxaww.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghlkftzcl.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdwvcwprr.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gnzqdysae.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gggtrtizl.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjkkvvlre.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtjtlqlah.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gvuyfopyg.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gnohuuzkr.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gjyfjjuko.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gbikdzwhk.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gihxvuvvt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gwqopxojz.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/ghrudeezu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ggrbpxkke.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/ggfntyzfh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gsffrrigk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gcxpikabv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gffiwtuug.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/ghximiune.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gyjtjhsvv.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/geriafvnh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/grwcvknlm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/golmvuqmb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbbhczzcc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gobmazmwf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gqkizcfqn.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gkvzxnyoo.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gssxlgxrs.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/glqqbsxpg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gcdzznfpe.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghicmtncw.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gyyzkrbnl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gyhauavcj.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gifccxizw.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gkxrjizho.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gictwxlyp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/ghcipgwla.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gehfaqrdv.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/grjjajcmv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gwkcrtorm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goolumtit.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gonpaqoia.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gywlocshy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gnxqnjblr.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqegfzlor.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gulyubiyh.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gvoqlitnh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvbnquuwx.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gsaztjthj.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gcxefhkwv.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/guwwwtsah.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gcizyjgwt.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gklanuvbh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/ggcfasknn.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gwxtqwxdv.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gwihhfvro.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gyrusninr.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gcxrhjxrd.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gibydeqqk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gpkttdjgn.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdrtlstiz.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsjnltn.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbferxvhs.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gxmcqtpki.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/ggncguheu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gzvntkjwg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gdarjiaax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/ghdikqxhw.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gzhgorryy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gilixusnd.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gbmkxqpkv.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gwffwtkqc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gteifzlhj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gwdaaqlnk.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gfockdlrs.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/guupqyvkn.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gajgyolnd.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/ghegbirzw.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/giziooisq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gncwfdsgg.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmdjzxgoi.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gpzlndxkh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gyxuhdswv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gtfkpceax.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gaiovayug.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/goyimwsav.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gkimkorgq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gathstnhi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/guzxksdlf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/grjoxancy.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gmndavtqp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/guixxfysq.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gbflevoya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gyumkfvdd.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gfomtqttt.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gyrodakjg.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/girpxvfix.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gpjszklzt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqzfryofj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gkeaamlkg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gxxlmcojl.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpbebscgi.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdspiipfq.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gnjmdzqxk.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gxqqwkcex.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gandwnjgm.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvbfgtloi.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gczdktsat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/ghjxemjim.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gydarfmwk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gbszkpdbq.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/giwnpkopx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gsnvchgkr.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gxudvjsev.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gzmertiyh.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/grzxqapcv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gsqaiumef.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gyyqjsaxq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxgquldf.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gwrmhpnfv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gnuslwufx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grqgkrpay.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ggrgzyefj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghgvextgs.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gowygoouf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gnylcznuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gmdcbhaec.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gauzymfad.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gjljwswra.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gpyrrfeyn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gepkfagcv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/grgygvtnm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/glftdpexm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gyieovpqi.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/glffpmrir.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/grxohxstq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gdcimpviv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gqxwbslxe.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/godnchsro.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gxbkyrnni.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/grpruvorq.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gdaovzjvc.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gxmqnrvvt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/geiajbqxe.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gblscpgsr.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gyzehtbpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gtalftcal.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gakswdzwc.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gwmzejjua.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gswawsjya.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gcsdldyym.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gdigepceq.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gstodwqab.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gruotbmrw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gpgaklqyw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gixeiyacu.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gdvxdchnv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gsbkbeetn.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gojctakax.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gklmcdpnx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gtbfqipyc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gvjjmshpy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gmtswpixf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gorskqspt.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gaxpcpsgz.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gderefejo.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/giksbkaxo.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gquxmvzgd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/grekhbkbj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gzgdfxxkr.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gpkigncln.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gccwmokwu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gwsnoxovj.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gpxvzwoyc.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gukefttdn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/glboezqzy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gbptnyeis.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/glthujfxh.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghwwdhjkl.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gtzjhaedn.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gvftxoqsr.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gyjsauwms.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gsojyxlga.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gsnqyigsr.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gqqytduyb.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gliwhgcgq.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/ghbtecedw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gknpqnezp.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gvuscnutl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gbqxnpyzy.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gkjwlunoc.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/grrkhxrso.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/guvwjbjcv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gpwxiburi.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gwyjrfnlt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/guhzrbvel.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gzgjyqizs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gfzxrnryg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gptjsvbuu.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gcexkalap.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/guzolxpcd.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gpeunthzj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/ggmtpnrsg.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gyqgrygut.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/geqbwxeow.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/ggqiwmsoe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gyxfdbfoy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gbuohomlu.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/grynbxseo.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gijccenov.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gjiofqdwf.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gqvlkzwct.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gxybevqij.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gychcwgup.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/ggrkisnxo.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gdtxniqmk.sHtML


<!-- 参考信息 -->