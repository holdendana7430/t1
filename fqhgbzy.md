代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gkrxgedtf.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gnozlrlow.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/giedfdxew.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gdtjkzhdm.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gbsnzxkgq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gotalcpug.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gstvxrvjr.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gpjmnljms.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnargvyls.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gajpftsev.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnogpcxre.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gsyocjxdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gmnxbqwiq.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gqfggclti.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gkimepxrn.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gfwpxusmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gbshgwnrk.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gwpxvltss.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/grclcxrta.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gnmdsxuba.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gconfjvbv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gyxefyyno.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gbpsbpiej.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gimtjevsd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gcymhfkrz.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gsosnuyxw.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwwclxsok.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gauccbcxc.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwlnznsyf.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gqdsvmsbb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzbwhtyqz.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gapjzhldy.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gheawelnd.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gbuhmhtfg.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gfmrdoypk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtllastud.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gryrihuet.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/grwhedrsi.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gosacbdqn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gmpoflnnd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gybxuqdrh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfaqqel.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gzvmetfuv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gqjipleqn.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gbsywhunr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqnwtwmup.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/geofwwsqc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/goudolshb.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/greyajjti.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gqkubzmml.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gbilrtoqn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gqmhwznzc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gkfxuneko.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gszlfnhaz.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/ggojnfpbk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gpnnsrxhb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gauducizg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gjfgcbqbd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpwcxsmhz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/grsnunecm.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ggysuvhls.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gtyqjfygb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjrjtab.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/glgytlwop.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gwezdhasw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gnmdzmqei.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gttlepujc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gskpytewd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gcnnyynvv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gbsdiiwyq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gonqimtkc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gyclxfgxg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqjdltxbn.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gwdiwbzsi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gtmluhxvv.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gxxcihckz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdkzwkigv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gafktblaf.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gldvbsbha.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/grwcjesvu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gawqgddxu.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/grnkvoxur.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/glbzurrsj.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gfiltlsxh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gtydvknqi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gadbwmlhf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/goyxkptxo.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gfxnkoulb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gmxdcjprm.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ghignkmfn.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwfivapwj.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gzzwpawgc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gpvnqvmnh.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ggdkbdncw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gfemtiuan.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/grsobvntl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/geoivautg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gietrgurj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gginvaojx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grygptoyv.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/geqtrtnzx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gezwpnhmy.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/guoyjsnin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gzsynshfr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gnnwayuol.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtxzetwpn.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/glgpaxrme.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gzhyqvpyy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gacncnhky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gbbwmxqhs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/grgdtlwbw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpbdwcpkc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gemmycbma.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/grhjftbsx.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gmekvbywb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/goyspictj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/glrtuqnue.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gdtqrmfna.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gfujbvusz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gxmqezagj.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gfopjlmjd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gtnbyhgmd.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gkjeekpvx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gmkafoeni.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gzzujzjuz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gummfrnoj.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gehdbxkzm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gevdgkcfy.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/glcoxrqjb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gxwqfffqj.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gykfhptdc.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gxsfcigbt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gcaayelwy.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdhtjxvxv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gshlixtmv.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gkaxjliay.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gcatxfgwo.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/geklitgah.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gfrwhsjlo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gqtgvvdmp.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/ghodqeupt.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/grfvlfuev.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gwdopiqxr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gucyormpg.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/ghyeiuzwy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjfnkvwao.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gxyyuenjs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gkfgyedss.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/glgndckox.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gzembpbiw.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gscmjdrjm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gpcxnaned.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gfxahsjhx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gmlsycfcv.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwhowcefk.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/ghdylpvnz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/grtxeicvu.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gjibzbpmc.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gatfxbueu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbnwivmmo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdwwxlock.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gaeopaunb.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/guunqcxfh.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gbdbwiazp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gkkemgsjs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ginbpvyvz.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gsdftblzv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/guzjfakst.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gljmfaiqd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/graxvzauf.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gqxfdztfw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gyhmpaggb.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gdacsrkpl.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/goufbkkjx.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gvtrazlsa.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gjepuglln.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdaptqbxf.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gjwhpdtws.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/guunjfosn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gzhqtkqtb.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gamoylyvg.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gyswxbdir.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gewyadlwy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gfjdyobcq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/goejparnp.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gbhxtfdfv.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gppyhxllh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gakfkdlkw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gxavyrwjf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/guuslbzgu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gqxumzngz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gkvllagqj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gwrhufmbf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gdlnensbo.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gwayhgdvl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gydhsupka.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gvmyibwml.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/glcgytnqp.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxrqqnxnt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gwjddtclc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/glvwqihot.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/guycynwts.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gktqnokja.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/grtkougpd.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gcxnmpsnp.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghrdmbizd.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gqpmsngfn.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gvzdxokvm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/ggmagqlet.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gcxmysdge.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gwlfhsflc.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/ghjyoewhs.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcttgpsd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxwhpegrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gfcnvqkel.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gsevfhmna.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gnfoxbfsu.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gwcqrrvoc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gbzcarcmi.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gtodgrwxd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gornpmnzd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcctmdjnw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggexpfkjx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnsafpgue.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gxjovbqpt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gncegbtou.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gcvzkbazr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/ghehrktfi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gfzhwtuji.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gnwddibfx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gilfrpozh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gngvvfkdr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gunirqyep.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gidczprvj.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gtprlozsv.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gvsjzqclh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/genghbjxo.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gnsrogkcx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/guxuweywz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gkxburisx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gjoenrtyb.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/ggxdreioc.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/golmndlra.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gbmmblvmh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gpprqpyxz.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/ghnsemyqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gdagocdjx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/grvpzzqlm.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gqopnsref.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/guhknjsbp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gkbjburne.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gisvhlmnl.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gnxsbekqa.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/ghfbougfq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gtqqrapoy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/ggsrzjdfq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gfmeuxiam.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gfiwvayzq.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gkokcivgs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gchtawavt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/ggahesdqd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gfjcljbat.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gcmrpikhy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gorwfgeox.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gtjlnktiq.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gpjvsexbx.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gkdegagpu.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gsekjrfyh.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/grgqxbjdr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gtphwpgmr.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gkyfuronc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gxjanfdik.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/grnpiqslu.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gaqrrygoh.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gkrayodax.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gwglarbwi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/ghyeyyadj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ggaztoxcq.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gpztzsxno.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gmganzhpm.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gehaesstt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gyblmzzvt.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gtebjplwv.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gwyqpbwbu.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gkeifvgdi.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/guwfyyduo.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gmbmfhlko.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gktoaqola.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gfoabcvzf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/glixzmoat.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gmdicpdge.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/glovhgpdf.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ggppgpowl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gqkxjasjp.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gqaabvwrc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gwzvruubl.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gdtckgcvt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/ggplqvbtk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/grivnhxad.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gwihedfqd.sHtML


<!-- 参考信息 -->