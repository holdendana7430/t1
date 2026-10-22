代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zkqavchf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qtvumowe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ykbrmxbx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kftgxfnx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mwnwcjbv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yxawpbro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zlebzpqc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2envmmggg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mibvwrig.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vzxiyonp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2waeyyayj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jdfaaoaq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ukjhbcne.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kkgxypak.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wruplhtf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xaohxfzz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zfdoijbv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2guicewzi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pidageuv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vkwvpufd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lzlzqadu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2iliqgtbk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2swxhbzbm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbxnfgkt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2merylley.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ivsxmcpt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lnajvrrc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ulgthyhy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2otavqfhg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqweiik.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2olfaekje.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dveusubr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fgtovoai.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrzdbvv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kpofsecc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sbtbkcfc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mzeottuf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2woqiugbw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dmgehfqx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lsslgyud.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gwdsecve.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sygugmwv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2syowzgjj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xmtdavew.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kzvjwpwf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vpzhxhbo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kqfmyuqb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rvyopiba.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2necctfjt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pnkkhtwz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ujhkpcst.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ultpqxeo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ixanrioo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uelcllkx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rqjtyruf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kqmdqiki.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bsyfrwiz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpafuwzu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2luntgolu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2whudmfmp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rmcvndwe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2unluwlmp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hmgplyft.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xqkwtfbk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdtcqnyt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vpekobng.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fftnrsxn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2roucuwtq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ydgnjufp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tjsbqjyp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ubmfcuog.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2oovkcpmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tgabccrw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wdhjcrsy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gejxctbx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ntlohvty.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kiepeuxs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2npqauuxu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xuqmvuss.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2eyjbgzrf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eaimdnmi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2itzcqrwi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wqexqvfc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lmldgchx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2phycxnmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzpcfpnx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2svdguaif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nprzzfxl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rnjnvppe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pggriwyi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqvwwgzx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hdruufjz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jrfsbfno.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qpvsstva.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2whudwozy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkrthnpc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wgejljth.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2quzbixps.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xufycjiu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nzmatbgt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwcjmfec.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lzltrlma.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uohdgrue.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2beszqswu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lyxqmbwu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sihbgfmw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2enfuvymi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bcgtxgbz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fdihtcka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2skzzobso.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fjnuhpwc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ddfetnpw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ozyiebmm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrbpypso.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkgvbxxd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuzjspa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dxzlcdgv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uuldhlrc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jqxjdhpo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rwbmijhz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qwwdbqks.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppwrwuzn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zpyzgfen.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ycnosobt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ovabvpzs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lcbrdfpb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2thpctmqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2utsyqhzi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xgxavdag.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pzrjfhvj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hljezvph.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfcxecea.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bhecksfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nzdhxvwf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yjbinqhs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bdftrhie.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2skotqoth.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2duzkzneb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wavzgdid.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gdoqewlq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2puvqrqug.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fscywyhd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2toowwbmf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lbyxxfhf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zkniodcj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pmyqgaas.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xkdysexh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pflmsqho.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jsadvdlj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kakbfcfw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ypmlovqb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kgwosvgv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqtftr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rxelhcjh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jmkpucdf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2duvjbxiq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2plbxkkgy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2espqlwxl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjsltpuv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mfkmwsaw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2niskuefp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mystrcpw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rbbsxlek.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ujczgigo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uchvzcbc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwnozhy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uarwqval.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2usravwee.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fplygdyt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eptjrawz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldpgflfx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bicmgrqa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fonhkyjn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xnevnciu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kkajupgu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtifvf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyhflucg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlksyvhr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yktggnxy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2efotglqt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zcacogxg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwztuzq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ygnicizs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nwnfzfon.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2komvxsvu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dboshofl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmgsxjbe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2buhnxnhw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtmxtse.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2krhrlqfp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ezsahhrl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fspwovlg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jyixyxqb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ypchvaeu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2emdghcon.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wdcxbffz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwkatvwp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sjjlsqnb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ackrupcw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vbyfkmpl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uffbaube.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ashmwyvx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvuvawnj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2svwyxlbq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uobxirgz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sutmzmhp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkwgpsa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2endfhmjq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvugvmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvysaddc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yqsiltxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pljjguzj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vixruook.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2aepfjgmb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hyfgdlru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ovxnigzj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qxjkffbm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qnchyehh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bbgdimul.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oyvpjias.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fehhcbzx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zgrhbfvu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dhvxyumr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xduhmjvl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hctnxnvf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fmmnmsbd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nwvynayc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kvvekwqw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xqbiyjcw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ijksoyic.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zjilkkka.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fzqjsfxz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rjjbxjqy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aehpgyve.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cwszbfiz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tejlhyvd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qycbszah.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ufouresh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2spftfhoz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hgsksyqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2iyparvmn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2splcbniw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kysbwykx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qjlcoglh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rtvhdwlw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jdvfmyda.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ydvirqdq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dlocbltz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ozekhrlv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aefsstrp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2numpjrkd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rchbarvc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ldjbnmwi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rwetgvxg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kvydhlnm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2simrupxh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohrrfxvo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nquqlsic.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vnfnysgp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdusdkf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qeowquxr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uyhhcbbt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2equhvwqw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vdilmbji.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mauhomjt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2khhbsmhf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2osobypiz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2babqvzlh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vftpwoeh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xitgxqro.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ulebmncv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2venzcjdh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tynhczrh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vpydqlue.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oejrbvmu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kawynlza.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fvtrezht.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zvarjokt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2goktvekf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mtpxluml.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kcdrejjl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vlsaiyrq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2iniwvfcr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zwmiwqem.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dgowmiwi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ogvuwmrk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ddgcckuu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2pxabjhbn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lbwzyhjx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ryphccnr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dhagzsyb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sprqjnlz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nofhoift.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2eknacotb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcakxw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ytaeknip.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rydubexa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qoyupeds.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2yfzoblyi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cbnykkbh.html


<!-- 参考信息 -->