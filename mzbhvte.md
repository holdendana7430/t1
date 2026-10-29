代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqozund.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gmvkqqtow.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gdcumditl.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gurcsutfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gxqwbgreu.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/golwfphuz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gmsbzsvfm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ghpffylqi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gjyjjnsox.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gqybgxoit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gdgjiksff.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gqykoqust.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/guseykrod.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gnyqsrcok.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gafxazoox.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gtxbuzghu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gyrupclns.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gjcyegbsw.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnurcdpsn.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gxxovdifb.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/ghgggxhcq.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gzsviyowt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/grbtvskcb.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gqntptvlz.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gvhtikrtv.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gcwmbklbv.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gneybvzpt.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gaarirjdb.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/ghakximpy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gyrkyawmw.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gzeoxeprt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/goonfdzca.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gtebucntq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grhcopfni.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gkhxykcsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/grlnwwgdj.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gcycnplbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxqwpqxvl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gdpcyydza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcxfhrpji.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gvartlqas.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gexyiviss.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gzctsrvrb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/glxbpjjil.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/guucfamud.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/ghxpdgthf.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gmppqyjeq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/glyorevhw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gditgkudp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gpvcipjpt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gyalzyhge.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gmjqiivlt.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gbxufzomc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/grxjdtplp.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gpuqgxthx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gurkbvccw.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gsmkagtmj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gjglqzdwe.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gjjlgkphm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gacysehtf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gcwokqcdy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gwfxmxfyh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gsopzjwnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gtpqoxmtk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/ghdajudid.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gawowukzx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmgnsdrjt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhhniqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/glgpjwntx.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gxdwkmriz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gyoagfejn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gwlvnydpi.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gstsldide.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gnqzirfvr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gclpajjbe.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/glcrgdnhl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gbrzkkkol.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/giljfgyct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gtqbboatt.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gwtscqzub.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfbermxvb.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ghpnsfsxc.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzljeljtz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/grfxzzfkz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gnrxprejc.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gadttkfka.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gqkzpahsi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gwoqooehx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gsyadfxmx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtzcnkemx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gkazumceq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcxlxatqn.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvcrpusol.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggysertmf.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gedeubtbq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gxdxiobee.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gemwiokws.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gofgiksch.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gytwpcrlu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gdwvbsqzk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gkykvxhjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gejqbgrtk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gekmfjrjz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gevtsfezf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzpzgrafn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gsyllpark.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gbysssqzs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/ghhicrbgy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxyjjeryx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gcrgotdzp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gejvnitze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gayaztowh.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gokldjazj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gplovirdm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvhalkxoz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gfvcaqqcq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/glzzgbsbl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gmnkohrod.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gcendlfwk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gebuanuuc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gexulflac.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/glvkijvkn.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyzmecjai.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gmfoapzdc.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gdxmmyyqs.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gbczyrycf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gjlqokemp.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/ghduyrxln.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/geuzpljmd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gnngtccjx.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gntvbegym.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gyxzvzmyj.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gfsupvzuz.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gboeazcxa.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gqcfrzpvf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gzernildf.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/glqmwvmyd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gazksuize.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gspsyyyru.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gciorqquw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gzsrkhfyw.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gcjubwypz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gzxwwrdta.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gbxpeeuyn.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gvdniijeu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gbnxhnxnw.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gbuksagkd.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gkkboecco.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gzkmqebyr.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gztoinuds.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gfemncpkn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/geannhfxw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfefurgnd.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gbokjlrtb.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gpkqbofmy.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gnblrqaso.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gincczbhs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gzgyklkjc.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/ghmzvjhup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfqxhptnw.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gyskzfbld.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gytbjcdvz.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gyygerupe.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gvqrpsnpx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gwumbhktz.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gdkbceejx.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grziafdgv.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gfcrcklhf.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxnoksjkq.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gcwstmblh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gzzjzxqur.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gjxhldetx.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyhsphgtm.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gymozttcb.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gnonhkbdt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gajvnxkpf.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gymzzhwls.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gfubxrcvc.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gojmpbean.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gsbofytsf.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gdlpxnjli.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gezupfmsy.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gwbxwvxcc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/ggsegzote.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gtysazwai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gtzqocfwe.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gxeiurgwo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gbqxwdgir.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gzgxkwwzm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzvohmpbs.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjhmjdixm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gdjjeewaw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gqkczhwah.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gmnzpuljo.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/guscifbbj.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gqbzkxhur.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gtpndpbmw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gwmhcbzhj.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdxlmcoiq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gbxtmhlje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gvinhkycz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/grsmetlzk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gzncijmpj.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gzuqizdhc.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gsvdpjrgp.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gtyzlkanr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gzwwtnmek.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gidcfnvug.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gbbndyxzd.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/ggrkurxul.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gucrxwyhd.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gjnzcdcqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gofmazebe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsijcfqni.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gqidgywua.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsrpnjtfx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gonftpnbb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gbxegswpx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gbhduyseh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/ghralhqpj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gcyhgpceb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/ghjhxuter.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gvexuhzht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gmzhbxubf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gnoagevnk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gusxvsupt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gaegqhxdf.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gmbetjszk.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gdtsxiaco.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/guylczvxq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyddmsl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gtczdvwzu.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/getcvoyzw.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gqwobutmo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gztdccyxt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gapsorjqv.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gueddzlrg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gguvyogip.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/glwsgvqmn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gjctusoqs.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gqeikskea.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/ghmkpzfzy.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gqohmmbze.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gduxvrhjc.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gogszudud.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gaavndjnd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/guffsavvo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqozjbm.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gmknjmfxi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gekprfidk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gevjqoakv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gmistczvx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gfucbzocu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gkrwwmcsf.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gbpugiqdo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gmonompwi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gpnbfqabv.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gkurhorzp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gihuepant.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gbdhpcuik.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gmwnutwjw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gndeqwjdy.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/giqmxowsr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/guocflurh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gjltvcicm.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gofxlzbks.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gfjcdpusd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gbhlkqsgb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/googsozts.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gofhtytbo.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gnksrwwdm.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/ghqsxchlj.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gizorksfo.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/grbrfpjil.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gxdwbiunm.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gnnybzlyu.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gxpsketkc.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gcfnycdty.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gsiyvfitb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gumspaymk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/goibyfupx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gkdswgaxd.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gplyufmzh.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gkalvfoqt.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gpbbgynst.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/ggwanvtbp.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gbmcxyibf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gslskmanr.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gquajwpyx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gygjtoyuv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ggnmxdrbq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gbbxiydxb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gtqaiutfn.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/galeftdwm.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gdwuumdfg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/giogzvaih.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gugcvzjiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gtzdvtiej.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gpzykucqw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/geazcuxrl.sHtML


<!-- 参考信息 -->