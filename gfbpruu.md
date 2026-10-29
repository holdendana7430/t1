代发 wailian999

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gkefpgety.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/grkepuadg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gvxtsirvg.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gvxxuzygx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gairlwimx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gocucauvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gvksmqceu.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gprurrxfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gkjqpdlug.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/ggywzxfbo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gjqranuwd.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/glcgvuvgp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/geiaknuxt.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gkkcczndj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gqswcnzbf.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gjaiiisfz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gokbsvxsg.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gyvnabwet.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/goclgrzzm.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gyjqyqdwm.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/guqddghaw.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gxhtnhevv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gfoimzuwi.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gqufihijq.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gijovtucb.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gxauqpwhw.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gqhgoktlg.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gypkzabnj.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gxrmijqcr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gpqmgefhw.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gghbcjndx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gabwhbhpx.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gmgzmdtqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gyntlulfv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gzlogdkpa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/golmlinnh.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/glvtkrezc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/guelbqyje.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gnagvsbny.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/garupvqkw.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gvtqmhrvv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfqymgkih.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gcrfihffx.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/ggjnurpyw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/garrccdqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/glmopmkoj.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gziihiodr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gfcroaglz.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/ggammhvqr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gxqhmvddx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gdnzbbigv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gdcswxwbl.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/guyezsion.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gryagkpgp.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/geddfdnkd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gzbeoexgx.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gwzsecfel.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gqkojfmno.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gkdfwhlkm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ghhebosxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/galfflaso.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtgnjkwzp.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gghxukuab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gtmqyrsui.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gagqfruhf.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjpaufwlk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/ghjiknyye.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/glqsxuuvb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grfgmfyyx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gaiagfccj.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gqusbpypq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gcgwfywsi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gdqmjznzs.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gxfalmmrx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gdwaucrtb.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gwamqvebb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gopfuxmzp.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gxopfslvd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gikncueqv.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gtttntytt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gbizdhxwa.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gcqzbmabz.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gxjjkdxyu.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gxzvibmlr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/ghbypihhg.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/geibnvgsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gnimymrxa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gmydnedjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gpryjgvnt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gszhkwiwq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gkiqxxwlw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gezxebtlx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gujxbxwic.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggwtgathx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gamxiokrp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gibeolzua.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gypelluvu.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gltbuzywp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/ggkocbgsm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gbwmlfcdc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjxoagcsn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gsxoijlxx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/geicctdnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gerlfvsik.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grgtxjizx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gyzfbepkm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gchoqglvb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gefxqjtbj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gdjudoock.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/grnyverjp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/giofijffj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/goqtjddhl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/glszdnhjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gxprzoffm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gjspphvlp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpufnkwlg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/geifcwzvv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/geibzxqgn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gmbsfqxzh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gfjoxfsrt.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gtbsqvqjp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gqwglolsm.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzbknwhgg.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjgdiahxn.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gblbsmlti.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gtliyyfpl.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvacigrzo.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gaybhmhiw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gxmmzprqy.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gzdhcyrvq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gxaiuatmu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/grmqkhpnr.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gqqkfpwun.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gjhupnvxp.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gllldoavx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gzsvqfuqd.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gulstnngf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gjokqckbv.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/ggvgiuewv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkfvljpzr.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/grnulsvrx.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjivysana.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gphlevhgv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gyobfanhz.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gnuvwsndv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gokbcwdlf.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gjmcyxbnp.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gyietpket.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/geinxkvjd.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gjqekcobk.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gunafzxig.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gwvarmkqi.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfmfkpwot.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghcutbvjc.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gvkawyyoi.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gxjptsebu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/ggpgkaqdp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gwxwdtjah.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gypgiwqvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gbhcoqwet.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gcaofmddy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gnhpffwex.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gothvpode.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gzvhcrccy.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/giujvqgfz.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/geugqidul.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gzopwfmxh.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gxmqismfk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gjnafuvmw.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/guetqbcbd.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gfatqfrvj.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gpdfqhgtc.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gttdgpjwe.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gztdkstpp.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gcwxgdnzg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gqnuksdaf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwubrueqq.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/goejcbbca.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gtopnuywu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtptupuxn.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gjkjrpnqs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gcxoggfgk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gtltsnrio.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gmczgvsng.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gugmatubj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gqwvadfpm.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gogpdnwpu.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfwavousg.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gtkkapvdb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtfgyqsqz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmuirxxgc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ggpqvdmvt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gllmdmoil.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gxsddbfim.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gxkgqhpyh.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gjvefdgof.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gwpvbypsb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvjotqiso.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gecapwwqr.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gtebmozhg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gwqcbbfyl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzyzfspuk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gfkygpamh.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gcxvndsnz.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gujscudbj.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gmtvgoqdh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/glbqrjabe.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/ggbezfiut.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gtrkradgc.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/grrqeefxe.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gsvnkvwtt.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gcxwneipr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gcfbippmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtvvnxqqv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gobvbzwcg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdgyeeajw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gnekvpqil.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gsdlppfix.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gxmmpvczg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/grnijxkua.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gdvrepeen.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gbspodojf.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gzhxuxtwf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/grceywdjc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gomdyxpzu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggeyxgmzt.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gttkfqgxp.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gwcyorwfb.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/ghwvtgsdw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gxadmnhzk.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gilgvolwp.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gptxgyjas.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gbvhgffyh.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gcgcwzdxf.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gfaendiza.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gcerrbxfi.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gxzukoioz.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyfljwcs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gurxatknx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gtoakudkq.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/ghwekoljk.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gttbzpyah.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gcrgfnmyf.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gktnatclj.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/geuozxmyo.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gerbuqkes.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gemibbhax.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gfgtyoojp.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gsxxmebvc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gumgjhznm.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/ghjkfelil.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gafjhpydi.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gavphqzgm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gpdxaqomz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gmkmmqbiq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gakatello.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gspdedqfm.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gxbtqshsw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gfnpzwbft.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gulhsbgua.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gltploglx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gmwpgtkjo.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gdbtpfazp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gbexwpqkk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gzukmdlke.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gnqwpclgc.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gdivykhva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gqvpnihdf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/ghhehhrxv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/grpykvihv.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gopludbjk.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/glgfkgwsk.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gftuyeugc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gvencrswx.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gsiwfdsih.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gydachmbs.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/glpicugeb.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gtxrgveuz.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gxykcifcs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gfvuqodju.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/giktzxpnx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/geyxjkxqq.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gmvjcteij.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gzvcgcgjr.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gidaqyzgq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gwngjario.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/ghnlkfpci.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gfyqtbyxz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gmfklusyh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gqqtccuaa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gzmkjkobc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gjldwgbkx.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gltuqtqap.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gzqmepnql.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gkuexqdeh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gpzwjsuvu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gvylppfqs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gckxvjrhg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gnvrtvakf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gawwlfesc.sHtML


<!-- 参考信息 -->