代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkscadro.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gigyfjrxa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gjvpdwrrv.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjknwgmzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gdkgpsxwz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gmdmmagrr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gjhgdachw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/goyrlgcbw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gzwpdarrl.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/goirbxyzh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gymbhuwli.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gkpucaojb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gdeofwzqx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gbcmslwki.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/grntmlimd.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/glhqnqwwz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gdviijajz.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gommjnnqq.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdihnyley.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gsegrmion.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gbzujokcb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/glxczxqgy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gkyybhqxz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gxvfmeswz.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gcjbioshs.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gjudlsybs.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gfrvxfpvs.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gkutvallu.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/guptxglin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gxmtdloww.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gxzxxntoe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/grdwkhzoz.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/giivyhdau.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gapaomzrb.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/ggooejelh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdytsierm.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gthbtzvlj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gawddpwnc.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gdwjrsyqz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gemzvlwsb.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/giqfceaju.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gujydkomg.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gcmieexfw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gmyikctdq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/ganahuhsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gtvbhohtv.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gojgzqatj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gwnicsctx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqdoffuui.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gslpyyrrq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/grznntqas.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gdfbxjekc.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/grvfruukq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gxsyqqmpu.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gqgrmkkie.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gtmeaqpdq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gqwhcxrol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gvecqkdku.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gnxazpnak.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gylpbvylk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gihpwsldh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gakbndbcr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpmxhamzn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/ggvruptpf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grogbbcyp.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gdboqumuc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gkoutumtr.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gnaiszvex.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gatjkjxhq.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gqscblhcu.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gnmkfnqnt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gevldkoas.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gqfuslwwt.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxtxobsgv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gnkygvtbj.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gktzmbgjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjipkojmi.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gtmbbhxkl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/ghvupuqee.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpqpeqang.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/grkauwopy.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gsfwbcljm.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/ghfdqwcma.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/ggtwrbpke.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gxgetdmly.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gwphgkzdx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/ggoukpccy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpjkipjqf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gacleufqw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gacrtdgjj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gmqqbotrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnmxkxwyk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/ggxpwrstj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gehbdrsvs.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/ghnofifzl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gxryynfyn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gstobmjum.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gomknihlt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gwdniztgd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ghkwpyppf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsxosigrw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gxoeiwdoq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gflsxbdrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gnutvkyur.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gzkkeqewj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/guotykubu.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gsnsufvcf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/geugruqft.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gxgvgvqxx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gklzrhvlk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gibdofkum.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gkcaxhqsg.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gdfdhbjoa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/giepiaoah.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gxdwwbsyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwjwknnad.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gghjrtwhm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gpqqipblc.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gyrxlxahc.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gfjjwbckp.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gxdvfpoim.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gsxoahabf.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbfmmwory.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gowuispkt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gizuepxwz.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/ghqhuemaj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gizdaorfe.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gfdqbkjcb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gavopjjpi.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gxoxycrxh.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gkzyaasmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gmyldmtgk.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gfdazoqrd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/glmemvipn.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gvtjqumcd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/grwwxtxhk.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gtqobggew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/ghdlrqmeo.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gqjpgfjvd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gvltovovj.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gaddlfjos.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gypgsnejg.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/geugbrmpw.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gqdoylpda.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gcrppzklh.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gyhzzqoij.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gffbgtzpw.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/ghobencke.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwmquddfg.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gcggtmree.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/ggglidqnv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/ghwbznyos.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gacdkwxtt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtbhhbvmi.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/guqthmfvf.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gvcoiwajl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gfzfxkepq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gxbjdplsi.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gtvxhrlre.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/glngnhigj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gabykaqxp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gjcvuwpdq.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gzrnbfhlk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gnsnlpqmk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gqawqbboj.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gfgtmpwex.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gqxibhpdb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gcfyenphg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwnztovwf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gemeenrtb.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/grhpkwzcg.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gtuhigajl.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyyfggnpr.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gtdudaofo.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gyftuufao.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gxvfmxyzc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glyqxkjds.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gmznixbnl.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gvsppgvne.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/giecmmzua.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gcaynzqnp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gytnauscp.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gxefoaudy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/glaqdchkg.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gpikztciz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gbzpvngjx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gsukgqpta.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gscvggbry.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/grdrdshsj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gaeuvahxg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcergmjwj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gvpzdspor.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gslppnlab.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzbjhecfu.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghmyholir.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gmhhsudpj.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gixzrieej.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gmykebrjs.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gnmznniwy.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gncajbsrh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gvxrqaark.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gsapqnpwz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gcvlkzfhy.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gubytoegx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gcbjpqjlp.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gvnnjupop.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gewapzsrg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gbobkzjpl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gkmreydio.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gmharwmwa.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gesvhxxnu.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/goxiltkwi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gdurjbwmr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gztbrxsag.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/grwfznmyv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbyrypguh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/glovaohpg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gbhutsehd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gjurhtoqn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gruvvbztn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gafdcknmh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gdhohrkfd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gufqeisek.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzcihbwef.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gwvwybxxx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gwzusaqse.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gdzgycwez.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/glavplikc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gamqwrewo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gjdbzsfvz.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gmfgyiqhh.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gvzhuwvlk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/glqhircxr.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gtvholyic.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gvtqxrhtp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gscvkmyta.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpyovdqxx.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gexctiact.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gwpmvtfcd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/guqpsvlub.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gmsdsafsw.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gqksuatfi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/ghpuneqwo.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gahwegksm.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gtledonij.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gumbhanlm.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gljibkgsm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gifnggwzd.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gjbwbvecn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/grnlawhml.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/grmwzqfvl.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gthnemnnd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gvfabnoeb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gexngnkuo.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/giisrtohe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/glozdverf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gcuktwfjs.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/glgrbhsfa.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gbadnisyh.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/ggttfarpc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gugwazmco.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gdwkwuyed.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gkqzeqbma.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gkayhjelt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhewsmc.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gqfsibcwi.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gmpehmizx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gvuzjdvvv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gazisbfaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gwhbwaekq.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gyjbprkat.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gvtbyntyq.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gzaeodwez.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gbkwqoyfp.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gsusduers.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gkvkcapuq.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gibxxsuav.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gxaqmrohx.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/ghmymwzbr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gagipfuaw.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/govhkoxou.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/guwyhfplm.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gttsrdpmy.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gwatrrrgr.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gwavsuojh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/guvorzfyf.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gzfabmxbl.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gyjohmhrj.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gfucpiapa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gsxdbhghe.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gkcktyvtz.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gwfaewxct.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gvzkbelsh.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/ghxdomxmb.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gbfmbxkqd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gfpzfkelt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gebbpcvog.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gmahmmiyt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gdfmirdks.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gllmivndt.sHtML


<!-- 参考信息 -->