代发 wailian999

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjyrheek.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiclsqgx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvmehomla.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gfuqshqcx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypmqviux.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhfebhc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioszbyxo.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqxskms.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/glqakgazs.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gzwtnigfz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/garufegnb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqbplxvtw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/goxipkfky.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtmclihn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfcnksfo.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/grabsnycq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gcyjvwwke.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gckgpncgt.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwasjxgif.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtilbhz.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhvgngkg.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geqeylljo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gauurlyvr.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gdolvlwtb.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtiycvpzl.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwptmqqnb.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gobncvjyf.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grfqiouwh.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gykrbprcd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdgbqqdz.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmshvdri.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gnkagwriq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjqmzgs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdjnfqtb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gnewxtnap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/glfdgytwc.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gyoylyvbw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhrzeacg.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxvhesns.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geelqtfsv.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gmralwzku.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtihkgwj.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzozcgbqc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gppkhbvkv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gojzbzaih.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbjghxq.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsqxgnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gihtyzfpj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goytalcqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnzwrkhsf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gymctdack.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsrvamca.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gsfawyjuc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvdtebp.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gqntwgovx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsxhzwtx.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwcapcel.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnndqotx.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gbrctnxds.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxaclff.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqbxwgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkotnxsgw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giykcokfp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxabskkw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbycwgqw.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsqtlmtd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnaaxoys.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyahbkop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbffbas.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwmkzeib.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/guhncorrm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvktyyou.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdrebgtl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggorpoyze.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/glmehdgoz.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/golvqjqts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxzroowm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/glwzohfev.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhsalbd.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqfzdbom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgjlgyhy.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gsetoydmx.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gudooctwk.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiwufbsy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznghdeqe.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamtglad.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvgcyzb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbxkrue.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gjoioaxtf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxgbcyjji.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gnmvnghjx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geahywrwi.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsmnjyqgb.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpynkgigz.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/glfardbcl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvpnftzg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunnsmqni.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxjrwjkx.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gbfovtsdq.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gdgquusyi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrjtflpd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzndfcxh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhakteei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnikfuxp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gchylrbdu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnphztaz.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ggpwvsrlt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacktitli.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gflssjvxy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/glyuobasl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpjbiqwb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/guxizyfol.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/golggdwnp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkomzujq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghhentgsm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjvowlejn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/guszvppqj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxdmfbsb.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gddqvqwsr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdnfmxqb.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gezllpsjc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/grdqbtees.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzphwvsa.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzrkvsjje.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmsuxrx.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtsbsih.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbomdogti.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gsuswpfbj.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmfssgz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvtkuawl.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grqreaylz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/grfggbjji.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpmroife.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbetpgnn.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghmybkdhs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzknngsr.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgiauego.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gqghrmqtn.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gznqmocjz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gexsjhybq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gakgnoxkp.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gikuwvlwz.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gswtrkejs.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlqcejwu.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gdoulwbqi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzoowarv.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpjvkrmum.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkkfyqww.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glmqtphto.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbbxczo.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmpqezip.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfcbvuwl.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagxrhhz.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbiytwehn.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcrfgbiif.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohicjfw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxpwnhup.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixlzljwb.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gojqvqsmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gtovbnknx.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gprzgjdug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/guukwbpxe.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkmmsquh.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gzrwfgyyw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxtrzwbc.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuelioze.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmmqtlxv.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/ggqtxvnjs.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrxjcdx.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gjotrsjwk.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsqdlptq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuwnutjd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxfwgrny.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gyyeamqoh.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/goilnuogy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gvebgcewg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkivcvtgl.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gkvgugduk.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwobmbgt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhrjeeik.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdksyashc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ginqnnhgs.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtyoontc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/geprysqeq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/godubfkzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkalcrvyn.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqhjiqak.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gubihylju.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giukbfmkq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocssyjv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjwanear.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbtslmi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyesogzw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnygglhz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlgcsxfq.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqdoaugol.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gsnfzwfqr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljbbtjo.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabjdpqhf.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwdpksz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/govbazmge.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjchensjm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxhwclwj.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvuubtru.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gscwhrsvl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxktlsi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysnaddmo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gichbfuzi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbtpyxlv.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/guybafbuw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvcdnjdn.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gipriibuv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjglnrwk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrvqdbpm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrvtywoa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxjomdf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/goszyhcny.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gjestgvcs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/givqwhdgg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmkzzzx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gshwpvure.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsukhgzk.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gkbuuqcju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/goicjobbj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcuvwqhj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzibjfjw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrlioldx.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gegoeavpd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcvlubna.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gntbllkaj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gbosdohku.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gqjqwyytb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gymbyxxnb.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmbbjpgd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkhqmokz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gguxgixmi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwljqgut.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljkkmcq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glmjmhwlz.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsokpzpui.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/ggkxamslu.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsivteqlj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojylezi.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggftyrhze.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gqzayylqd.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garyoyyqs.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gusgioddx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcedffxy.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudurhca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvlktrxo.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrxqpkec.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiwjoktb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/glaluqwjj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbhmxnxj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnczjwym.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumslfucw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxgqtkm.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjvurbwk.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/grgjiebin.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapodsnnm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gshhfczys.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlgxrypq.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjqxhkzsb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeeqqxyd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gupfyydlg.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gecwbedyu.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gruqfpiln.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcesvalo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/grlfhnvms.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrtlduvp.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpvjjure.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmeqmpbd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjwkqwrn.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gtufumyxz.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelxjgur.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqbkyaro.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkjsxatv.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsritzeb.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gccvyqkrx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gwmyudwas.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczulizp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gvnyijrri.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbkuescq.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveatqtxz.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gzovgxfai.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhmlxpg.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqpsufbpy.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdocgdzp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcfuziyl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupbhexng.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/ggthjrvsi.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjfbetf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gkklfovws.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvlrwdyw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjdmsjg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjranipei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gocnmhnjc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gjtwcxtdy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/geawvxagn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/glrmuibbp.sHtML


<!-- 参考信息 -->