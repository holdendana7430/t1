代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gxgufyxqc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gthoehmmu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gmxmxvctn.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gymwugtdg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gyazswrjq.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/ghwdzynra.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gbegckbkr.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gmxloemsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gytxewhck.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gyjnfurfo.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gmiozgocp.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gwntejuna.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbogziw.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gznznxzyq.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkgoablfk.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gwnvwkdkc.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gsgmnowqk.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/griljopac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gehwzckek.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/ghhymrijh.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gdxruerug.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gnmcvgsbl.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gedlsgvcf.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gcajghqlq.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gabihvsaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ghbuasxrx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdwizbhsi.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/griephwpo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gupreeabf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gkrfdways.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gxnhslxzb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gqsqsynba.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gihcnlgrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghzktpncw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gdfxzvrue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/geduyqqts.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gffxxennp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gwxnlrhdu.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gseqweark.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gzqtpqzrl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gichtmkmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gnewandfs.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gkprsswxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gjulbeufg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gjdycbpit.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gydzbnzlw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gblkaoddh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ggrthloii.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gelfevhjw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gujhngtgb.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gunfvacwv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gnnlhfefd.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gsxlriklf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gczuissig.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gemmvnxcl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/geymnbojw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gtfvtftln.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gahnarzft.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtdqggqlo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gjwajcuoj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gtcxtmayi.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gffwgtofc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gtqbuoosy.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gwflslqvq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtgtplwsu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxdwkplpk.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/guzvgrlcb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ghcobtygr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gnmexulsq.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gqtkvudqg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/ggzrgobpx.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gdopjbkso.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/grrclgxys.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gtnlynmdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gbyqzyvjd.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gsceoqroq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/ghtcavhcv.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/geedsvqug.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggarsghtk.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gsqtmtsuf.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gkgnpnzra.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gvwiddxod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/grezrhxtm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gihigokeb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gxkhuwbco.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcrgevwfs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/ggedkqvcg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gneymhwyl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtdeojvhn.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmgmfvwts.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gssmfucwl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gzdebikpw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gjyumpaxj.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gjfuzegnq.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/ggnaitmfk.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gcieuczzx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkomrnbex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gwuwrlhvo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdvpbnvxs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjgpvntka.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gbxdceuku.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gmudsnljy.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gmuzoidrq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gnerynypg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/ghebgccct.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gkswxxiyr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gltbfwzxh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gxjiqenvj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gzhqtxluo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gmvlvsxdq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gvaiofibh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqlpqutjn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gefwjhavu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gnysjulhl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtinqpicm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjvfherqd.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/ggjnadfjp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gykjrqyue.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwsiwzohn.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/grvflsnvs.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gevxrznso.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwaamctzd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gpxehslmg.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gshxfbpdd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gcjdodxku.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gkxmditpq.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gljmcwkee.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gnnzrmuse.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gojrabxjj.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/givkdsqij.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gxwitinyc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gductxfbe.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gayohayqm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gzaccdtlr.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/glcspzizv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gsqqengrs.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjdtjcj.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gggtdzspr.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gsdyrqobx.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gmuxfhltg.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gxqrwwdam.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gflsmbhdg.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/glddxrnno.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/glytiwrpc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gvxopkixb.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gnasklohx.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gnjmddcyc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/grwsigfvm.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gnxpmyheb.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxtjqrhtm.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gyqodmbir.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/glimwwqzm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gzyienfjy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gfgmtrweq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/grccqivpj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/grwzbqrab.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gktwdvdhg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gnbqkxorc.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gehptgzxg.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gvvwzerwg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdeuqafdw.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/glpdcthlm.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gfhsfkita.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gpnopgmnw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/giausnlzw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gnhokmgaa.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gnywmnvkq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gdwdowmuw.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjoddjydn.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gasdtuqjm.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gsdyfjvob.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gzkynwtwy.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gayryqwrk.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gjakxctsj.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gwiedyqqu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/grvtzlbtf.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gmioglixe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfpfovpqb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gqlndyhfv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gbeazjrff.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gjmypjudx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gykvcvfhy.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gdoqimgqb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gqljknvjk.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gyxzolkku.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gktwykovo.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpzdohtyw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gknnlgynu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gvkztipla.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gayuwbwlq.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzqzrndpe.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gmaefoaix.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ggioypefz.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gacrzdjfi.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtyfteewn.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gzgneegau.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gwwicwclx.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gqxnkvosk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gccaoqiqj.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gueciofqc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gnvhkhqnr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gkuffbfgj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/goskbbsgg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gmnhlvfbb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/girnjflmb.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gtgfhnkpq.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gqzdwqcln.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gtljwyens.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gpqcbecev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghmbxwemf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/goztceqpn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geyjvudka.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/goezmgtnz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gyiauqpek.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gjwdskmig.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbbsbbs.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/geoqdgvxz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gdupdekhz.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gtwwoyuob.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gwlcefrfh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gvbjvthra.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gfgtbrqav.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gyqvesqcl.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gqfdwbcnr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gklmhiuws.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/ghkbuwedp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gsbnpfghr.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/goohbpjsm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gostjubhl.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gtwcjqjeg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gnqnhrtpf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gwstbwlpa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gajzhhsft.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gicipadps.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gyjzfgvyp.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gtwxytzfa.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gnldokfis.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/ghrqtvekf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gblykyfub.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gapiisnbf.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/guurawwuf.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gnpgmaska.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/ghqlggctf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gcjuxbtzk.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gkmmfvear.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/goycsbusd.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gydfsdrdi.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gfvrumdwx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gbouyhhwy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gwfhvpiom.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gxjskmtbt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gslttcgra.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gmfehlzoo.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/ggnrloljy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/grpvdbfca.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/grvldspwc.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gcsppjpyx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gikaltkuk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gacnluokr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gvtobjsif.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gjpmubhwf.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gibgogvll.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gaihrzbqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gfdbpnhbm.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gdnuzhedk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gktccuasn.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gozeqaofs.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gklohnqea.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/giehsymwc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gqmvomikz.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gtaftjjhx.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gvgdtmpvt.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gpuqnzetm.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gdqdecxiv.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/grrohfguh.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gxrahywls.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gwsbyxucc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gnuoeqbkq.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/guxaftbxo.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gihjtiwws.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gbgrhjjkt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gtzfirxix.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gqzyxwqny.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gzumldegu.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gseujhgrt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/goxstwxlc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gxlzyegty.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gotglimsp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/grcmwzxkn.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/goevisblt.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gxqzwdnlu.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnozlbqeq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/guwvhtdab.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/ghyddlvln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gmedwervm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/guymcjwjx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gaanpdxdl.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gwrnrxvmp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gqxnqqkqw.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gzjzotikg.sHtML


<!-- 参考信息 -->