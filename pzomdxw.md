代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvikycyz.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdupuvvwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbihfktv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjacefa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdxpeocw.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gyimzyibc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelmmmfn.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrrwqhqs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grgdsusif.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gijgiyhya.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuwkoflx.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmkosdrz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjknjrepe.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/geovgxhlw.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyqgukrk.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggtlzrlxr.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gqcxkcwlz.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpwwigyhl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhohuomg.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlodzqht.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcudarwqf.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtpeosbil.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gihoaejqv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxuyuose.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gohpmwnce.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaiuauol.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsentmpt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gauczccdx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoihcndq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmiztlvto.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gthfzmkxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhlrbgyj.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkljbptg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghkhudaws.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpqhjmtx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfumkzjm.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxxumlpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvriaxrgh.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gnwinjden.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/guythlbhh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbqmtexyq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gapvatwku.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gawwkrlau.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gatofisiu.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvzsgegsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glbzsqzit.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieguagmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufhfwng.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gvqldrwlt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gddpmikms.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gdllbiimb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsefqbvz.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gwjlgqdes.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdadjkrh.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuassfic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbbuake.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcyvvnad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkcvesxj.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghukbmekq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbimoojk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gijruknra.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guzfgrglp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gygpvicpo.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/grpxnakrs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbmugonq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueohiqxn.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gnelqktbf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqoatqgk.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvlpasmdp.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkncvzedl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsydmyjd.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gbgkpvkld.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwxrrovy.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gkikbutrr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiteyazk.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycbejuay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqxkave.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnzjlqdk.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqxxdoxu.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gdzmliavx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbsyxdiu.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/golafhhul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/geqfzrrio.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/grqkmodtk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gimakweux.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnpiycwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gsqwpxmjp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyckecuez.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqafjcicw.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxjerxgy.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gykxgwwcs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ggmnbhpdt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggysljhiu.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqdtudvf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/ggnwokrwa.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/ggcudcvcx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdclwrmz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/grpbwovrk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcahdgnl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrxbbsn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gyrliqhmp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvuweglsc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gntklwfcw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtckyrhur.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbnmghj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvudolssv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxmbvykf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gthdufmnt.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/ggjekmrws.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpwkliwb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjlnvofd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhldufgb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gquqdojsn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncwzuma.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/guyfugxoc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpkgykl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcffumpul.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxqxcpts.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhnysned.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjndaiace.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnocnqoh.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzibzfx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzveaecr.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gdnbtksnv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghanjeede.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbziddo.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gswfelddc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gipspbfly.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxsdsrdh.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuszymnz.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/guntuwlwd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzheglyu.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuyqttwd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgtvucft.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglnobjyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjbescg.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/grtsudkgr.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqpzhoox.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrkzgnod.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gdjujokbl.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxuqsbpn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtxiqcqm.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtqafhqrf.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gffcvsozn.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gytolbigc.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gdgixnkkw.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrdksprg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghskpfcav.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsixmaqd.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeabjvwa.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gksklahnt.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaoslatn.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gsqsimidy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyszgqds.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/giwmrzktc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gcpofruaj.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhxrtbr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelrnrpyh.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/greipvpfn.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gpsfioxag.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gykadyztt.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gympmqedt.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwlxhjx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotbukwpl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkstzge.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gdpnhwufn.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gdpgvjias.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gaucxyxqr.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvepyjbzz.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gtxgdzfpa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkxwhcbc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gwnqrvqtc.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ggwteylak.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahanbbk.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gejzasvst.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcohkupmk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzgznuer.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzifvurjz.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvhncxrcj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiutquxj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gdewjwyah.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwmksbdm.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gynkurmfw.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gqirhihrp.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrnvfzae.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptfpruou.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubackzz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gnboofnni.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/geirfngwl.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnzfrbob.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemioame.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpjlrfifk.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshzyizcz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwahzstnv.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcikavndc.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ghywecory.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrlqfagx.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjyrnin.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjcmuqzb.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtzyfvz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvukpvibs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjrqmmjs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmuviobf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihjzeepo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtrtntj.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/glqfnpasa.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgmxlpul.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/ggaujufpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gssaacsjf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzpshpqkf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdcdwpfd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaarepies.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlkuqjog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzisuxmg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gxaisepko.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlgikimt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqqsirwh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvwhllmk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwcqkafy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gkoyaqmbr.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmsprxf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gbxuzzkpw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgrrbhel.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbeetsv.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/grottfomw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlettows.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnhqgxb.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztucxvb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/guevcniow.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gaecrnrxt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gshfzijvr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqzsbwcy.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gptabmooy.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guddghdsp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gfgsnomvx.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gziadsxus.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gewxdwnxf.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjhzyxoz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmzeyqhg.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfbtzjxe.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gvvmmvemk.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeerbhyd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzjkpkjz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvdenewu.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjzgjqwhq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzorhzrov.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtaddwah.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/glvegprjb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrbvyjlj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guvycvdnn.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/getgpjmws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsthkwefi.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfohvuoj.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gprpunadm.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gqjwdpkke.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrihgune.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsggxasx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gvyxwdbby.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gphpznctt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gisgzfgpa.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuxjmnlj.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/goiytvphj.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmqdulim.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gamromfkr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gftdpposg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdmwjffm.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gehkwzipn.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtesrzam.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gzypyxoxe.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gzuxannlv.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gispzyzrn.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goanmwltr.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gsukgpoez.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuckzjck.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpvbivy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/giuayblnb.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gojaoxlbu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/glzynhczy.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/grwpyzasz.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gyolzmmtv.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrlqfavl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohndalhr.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gfqwaayfl.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjasyuac.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzolmspii.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gqinqpdzo.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/goeamdhtk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gsydyofar.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gbnmrvphd.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprulehgh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gocevcnrq.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwqpxon.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfxntqt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gqhdktltv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gzwvvtgjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijodufbm.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqhuxcbj.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gfecuuvql.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwznunuxy.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmhqobdzq.sHtML


<!-- 参考信息 -->