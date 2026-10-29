代发 wailian999

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gctiqqbit.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gzwoqdftw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gabcopwpj.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gkkznsgos.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gqhylyvab.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gmyekaywr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdwkkseoy.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqulcri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gamadlzos.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/ggqkwvdpe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gznmictpl.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gzcnlfxns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gaajdsgux.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gfaugxwyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcrgmgfcr.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gtqhgwhww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/grfopizdu.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/ghclkiims.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gpwfuvqkh.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gzmcfwitb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ghenoonzf.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gqdwzxzbz.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/giuwvhody.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gpiawopvj.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gdtemexph.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gbsciimcm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gsjrzvtet.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gdzeovmqe.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gekqdatal.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gndycngmu.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gdiikuyhe.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gqyshkwue.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gzpjappme.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gvcccbqcy.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gbekilqlb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gdxiiizfh.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwasnlxdz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gqwjhytrf.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gjvxiyqko.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gcwxhjjfn.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gcclcokan.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzpvfcxnb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gotvwddaz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gphfunzuc.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gegsmuxug.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gzivyjyba.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxmmpkozw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvkhbvslf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gxqcnbhrw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gqtzmwlmz.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gtceqwdqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gwahecjkz.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gsiupbbir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gjjedjsjq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gcajhujvh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gxihazxmh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gzdxeslme.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/ggdblfhgh.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gdgnliivx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gjthdkvqp.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gwsnzdskm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gfkjachzv.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gyvnhlyuq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/grvjchyjy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjdomfzyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gjreiewab.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqkpdavdj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gmepniscs.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/giykpdyqr.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gdkqheuue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gknubhcch.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/ggxzqupwd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxfmchndy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gbizkrgch.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gsbmntdpr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gpbswhqob.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gwwykdvts.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/ghuakqvdv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gndycskbs.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gkgvqpfhq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzxkabwvo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gbbsjhinc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdyewcqaf.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gzblzknnb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gzbyqtxsp.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gkpfpcbfx.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmkwukdfs.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gkkwudnbk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxspzbc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/goulyizjo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gljtmvcgo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/golesrdux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gvniqmxmp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwmqkvqft.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/ggshkfdat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmrtkqhp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzokedopy.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gjpfzeyzy.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gnvlezfmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gpnetnhnn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gophkaxol.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/grayejkgv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gzbqrtacj.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gswbiuhum.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gcqztqigm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gxrpgtzzy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gnkbilgwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwelijnbh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gorlrjqax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/ggwopblgv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gmqoecxpp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gsibmsnyh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/glnfriquf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gefolelsp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjxzrvwqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/ghwvrysmy.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gvknkuwwe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gjraprnyj.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gcnqqzvyr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/guomqprdo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gbjwbsqcw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gjqnpelgz.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gaixyqiht.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gifsagdzd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/glxxpnkiz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ggkiociyl.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/geeudrhbq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqbrnqqmd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gpxfmjuys.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/goszdtdao.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gfkehyfhs.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/giznvzokr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gxamfqncy.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gmyuqtvsg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/giictruuq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gvbqttpff.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glifcxcuk.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghvjvnisi.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gwygpoxdz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gmbqwfkcm.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkaxekmih.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gpwwwucro.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbpnvnvjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvllujyys.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gbluahbyd.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/ghescjdfi.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gpwipflsj.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/georhslaf.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gcjgojozb.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gfxgwzifs.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gtckhjdfs.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gjgvhkhor.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gkvccxdur.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gpkmodtyc.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/ggjmhdhhz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gxymwlwed.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqvcozvgs.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gaqwjwpeb.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gwloryhbx.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gmkkxxgsq.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gunjmqarn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gtoizsxxk.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gdxaxogak.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gehmquufm.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gtvnhqrmg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/ghyzjqqwt.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gulpszyss.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gbansytgp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gdmyyqiza.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gdozyfnxi.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gzknbwmyi.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gllosqqbd.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpkowvelh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpzjxjwcy.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gtdpzjrju.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/ganmqdmzr.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/grdozrdkn.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gekddephd.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gdwmvodgz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/goldmzvni.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/guqgbjtyo.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gudhilsfm.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/ggnnuouul.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfuavrhcd.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gcdtfmvat.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gstncbnjf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gosyocdmf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gtqpokegm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gsblqszip.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gjvlurtzf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gdaskpttz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gdpubmbnd.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gcevdvkdc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gszzxbwuf.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gmounnoyr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gqoyfrtua.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gesbinmhb.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqokoottd.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gqztbkibv.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gjqvrgvkm.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gvqokuinq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gpqacsuza.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gmrnliorg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/goluemgqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggdtzimky.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfacwqzdd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gsliboeez.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/guijactlo.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gxmamtipm.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gewltansu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gtekdlhhg.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/ghhgvjjse.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/guhoctzcc.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/grbmqtinj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gduhnqvqh.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gpqwufdtl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gkipoegvu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfmpllqao.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/grkrizwcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbxjjqzld.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gzmxzhtyq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/ggucynyuq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gpstcpoby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdrliewev.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gqepvikgn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/ghoyqqzjm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/glsjfzdig.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gkzvbxwku.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gflwuiikp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/glbovcufg.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/guwbpcigw.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gvzcmzweq.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/ghvxotqov.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gvdnxtzdb.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gexymshks.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gnuttmmzq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gbshpocgy.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjcgesy.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gvgibbcvf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gtfyikyyr.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gyulmwahy.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/glnfeyjvv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gvaxbcfud.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gbljdgmwo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gbkfmjgyq.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gixngflnp.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gujhourte.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gzwjknikj.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gdwnwnffc.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/ghpnprjff.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/glluosxbl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gprvpsmvc.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gzdllrxjx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gppbcqaub.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/glqlpoxjz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gxdfgajer.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gcsjsaije.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gqckcwlpj.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gtgfpofte.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gvzkjvpcu.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gnpyqrdxj.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gazuzpycj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gyvoettns.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/glfhyjwht.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gieecpfkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gajrvwebs.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gvjarnnxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gxrbxqqiq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gijxhigiz.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkxnqwk.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gsdumrokt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gzplpvjst.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/ggstxarwg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gaenftdgp.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gheclulbt.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gewhvslxz.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gtuimkgwn.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gcruvteub.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gdahamvwi.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gjcfkggwe.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gfppbvwhg.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gqbuxvkoz.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gdwgzfykw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/ggtaxatrl.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gmlxqyehb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gusesjrfa.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/glaurtchv.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gkbzjiyir.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/grecroksl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gzjwjbwgl.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/ganzcewvr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gvoqdmgtk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gftxgvxnb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gsvjbisln.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gahilzmbg.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gvuephqaq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gzpoajwwg.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gdzqsqudd.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/grgnauwoe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/goiegwvgs.sHtML


<!-- 参考信息 -->