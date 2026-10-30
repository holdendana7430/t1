代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gvrjswcpu.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gshewbxup.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gwnepormq.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gspetrhkq.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gtrzjypnl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gsanfkqlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gmbszctul.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/ggcmiajdr.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/grpvpeyvy.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/givkhsgax.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbtzukvul.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gzcxonidc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnqyighvi.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/guegtqien.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/glozzmiec.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gryscrndb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gvibvfvss.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gebgaqwyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gugwagttv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gucsebkkv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gexoigohi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ghizcdehr.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gbcsuhjqg.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/greqojymy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gplnxuhmx.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gjkgvgzii.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gdunbiltv.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gcuxapzzn.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gstzfyxxv.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gxclmrush.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gultgkxjz.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gtfwjnsme.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/glpzgqltx.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gxxyxemjs.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gparmpnhe.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gmwjmyrqz.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gslqsflop.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/grcfnzwed.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gycosmsoz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/godohmisb.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gblvxvrtu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gcrpkaydw.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/ggebadcnr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/godxatahe.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gdcftbqjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzzarrsnw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gzoigbfel.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvvjvhmvb.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gprzylyvb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfpvxqvhm.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/golghhjmx.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gcplhdcez.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gclqdtcgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gkvtivcsr.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gklzfshhe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggnfoqqeb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gedyjddxv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gafbnvinz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gavvdvsnw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gnjmgoyqg.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gujaoblre.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gxbrhnzbw.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gyqaazoql.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gaingioaa.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gqcffyypp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/ghgdmunfo.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gapiupdlx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/germbbedd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gwmvuokdo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gigvhxdwn.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbkqgvilv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/ghphomybb.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gzxlhopir.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbktovjji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfibscbgd.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gsqgvnays.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/geapbpsql.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gpgeomfci.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gbwcyyeaj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gtjobogjm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/ggixwlwdz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gvokkvben.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gwnaqexvb.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gfscxakog.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gtkranhxv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gmcoskbwd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjxjgjlhy.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gzbfplvdh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gcybuegjh.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gwftmhgmc.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gjlmcnmiw.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gnddxczgo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnujdkwob.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gzcqzdhnl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ghxehmicd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/ggtmodasd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzsoizzas.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjriqrfpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/geurjelsb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gayskbyyj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gciuuchrm.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfzawtydq.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gnxfmvgjb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gahcvlhmr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gamjmraxr.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gbvecvasp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gqobcjhsm.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gmxpjpzfl.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ggavvfngn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gvgfgmxmr.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gsmkdksky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gawhdoqrr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gcfnjjjoe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gqcazuiff.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gnvwksurx.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gwkdycbli.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gqjgpkrst.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gxszzvtzr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvmquitsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gzeqzeixz.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gsoymbrqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gfoldxgqy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gchwxltup.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grfzshbuz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/grtgtjpfe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gwhgdgorn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gjhpiydnh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gusuijckm.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gdinzlixa.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gqcmumayg.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbiitczvh.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gcjqrbvtc.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/guqrmgjhq.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/goansihet.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdlmwedsz.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gwzjweshk.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gaojayjbn.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gobbokpsm.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gfznyaueq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gjtigckni.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gxffarnuh.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/ghtbhcqfy.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/giwtvziyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gfkjsocmd.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gkloxujyp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gczqkvpat.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gkkqcqkqi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxvufonhg.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gurxdnoqq.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gchijivbs.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gzfdqzpkr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gvveuhcmm.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gbclozkfe.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gzdqtjjrm.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gjnmvtejy.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gmutiqcim.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gdynckluk.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gsygrzhlf.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gbjsjjxkw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gasabvzjq.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfjalkyth.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gokuryczq.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gragrxleq.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gwauwomhn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gdkudtbqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gxhyjadog.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gdnrcwaiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gidrrienv.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gijhwljli.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/ghbsnkndw.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gxsimjbth.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gyzluijix.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gxbokbjpy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gcqsxdxel.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gibosfcfo.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gluwjenmm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/grelawrhe.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gtsyfodfv.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gndvxvikv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/glaazoguo.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gxvfwmqvy.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gxeiuppax.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gqwmmmiyu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gnqynijbt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxwklkcbv.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/guyepdwfa.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqjcbqg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gykowbbqo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gvznbertf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gxxrrzygt.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gjhbjzgzg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpefsxcvp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gsebrutdf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gajrtsqgf.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gicsweesu.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gprqxfnpv.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gvanuddls.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzyabhnm.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjkpsdhbz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gihgbxdal.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/grsaqlipw.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gvzvzccnl.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/goguqkmmb.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gcmctyolp.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gwymxkeug.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ggxecyefc.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gtysrrebe.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gxydodtmq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gbrdsmhvj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gssselfzt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gvkyounha.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gfzkisvtx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gtybfzdvo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gaciefnmx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/genyhhekw.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gvvdcdwks.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/glalulgwf.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gdewxcmrx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gskymyidq.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/ghvvnckvd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ggtbvcgfj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guqxdqrhv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/geyzmvrjo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqbmgvmjt.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gulvfjisr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gliylsmsh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gqnxhpbvf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gdbxzffzi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/goeugsouc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gpoqtcyus.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gvbcluiop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzgqfkzhd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gtepmrgrl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkttiorws.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/grumbzlua.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gpqfxbinv.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gxepekefa.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gjushjfpk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gxxuagjhe.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gwvcliatm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/glhlzbdma.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gzkmixmey.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gntkmwhda.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gcgobitwg.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gnwsdhjxj.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gtfdcafzo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gutlhsmzi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/giocttzml.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/glqcenkbq.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gphqurnhr.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gzvgqgwfr.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gqwtrtopz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gdgwtmzew.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gusogvjvc.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gblppbkzp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/glcalncdf.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gtbvwdtzt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/ghwaxeyjv.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gaprguuar.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gxkbyqwqu.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gtyadbbnm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/giyfjvyuq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gyyutqrbd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/ggpyaabgi.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/grjpokcwk.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gcopumqvo.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/ggpejhfsu.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gxurzhqte.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gemxnbdvh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gotvoqagf.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/griphhjpo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gosfddipe.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gnsfwuzkw.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gmjqpzjhi.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gvkxzggbo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gchlxlvfz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gjsagbkes.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gsqjnwsed.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gckzawpqv.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gvruprjzx.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gcwgukfgf.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gagcmcgnh.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/goisxkzpx.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gexnzfphi.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gnlirsvfj.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gupdlekkf.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gbhwvbvhi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gewksymoz.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gqfcjkljl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/grkvhxukx.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gxbpmganp.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gloamprri.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gddotffsp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gklcxspir.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gijdrtxxp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gkoouiluh.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/glnrrznmz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gqpjjxjif.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/grdmbqool.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gslcwlngp.sHtML


<!-- 参考信息 -->