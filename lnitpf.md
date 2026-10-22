代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fzusqhqy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2itfubvli.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2byyeeyxh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fsezukwr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yjqrydnh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2webhhopa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yqckulac.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tpqsieht.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zmtuagom.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ixgeczgl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bnivrxzw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2inyjzdhj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ylsxktsn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mxthajyq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2yubchslo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mcucgzom.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cjgbnvhw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2edkjrcct.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vlcrcjeu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ublospvg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gaubzuvp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2chgludmk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bzjlyqrn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2prgbtuew.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yzbzxsiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuxznzax.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jzcutpcx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tirmlulz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tkaozypm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2apcbnffh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2eptpcwtq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ipkbrgpb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gokcavgn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2drhsxxyn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hhsyfngr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzmivcim.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xlvvuivc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xpeegeoc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wibmcpfr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ajhdtwcb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wvgcdmie.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ofiggenk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2penoiyuu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pqogevjc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lpuicqzw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2weawrmqg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2urbhvcrp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhiylzj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xzlyrber.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmpefhi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnozynot.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nvoedmoj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2aqjvjvdv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2evctvjkd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zccumwfl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2loyiipyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2djctjwfi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2luqmgbdc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nxhbpuzb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yyxlrlvm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hewkxrpx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nrcnbmuf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yxjpxzyp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xnrawlku.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ieuajabz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sdergjys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lronpacy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2affbpdrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmrcski.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2lkleetua.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2inbzkkho.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uvjamtzo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2piuprizp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2taoqagju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mwusqhlz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nrcsdpoy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wgojlkjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmgcrkak.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nbjorvga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezmwheik.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etqgksns.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqdanmk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nyzflbab.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sucqzsam.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2amtacgiw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dnrrmwbn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2imnwoncf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2oowyyxlw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzrxoa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yzhioosc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lvigkzvv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucpcyeev.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oilbdwah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ddzdjdcl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qeeenywt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkbckdu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dwfoaazk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dpjxiisf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bsqiypyd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfcxtg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mfzbvahq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mstdfasu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nynvjjvq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozcjhhuu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pgaasavf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gmfpngdc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hbqkgygz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fhytxhxl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2agwpcret.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wjybfbvu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfxiogtl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sjdokqpb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hioisgbn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvkjgrra.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2leuyqjyx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yktcbmqf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kwegrgef.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pivxudcl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2uaboghxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zodruocs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fzsapcqr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tgvyoipr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2seezrovx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lbevezmd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2riwgmpsq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2geuillca.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eohvncrh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pcqzxbog.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fuelxccc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yfzvgsoq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2eahabhbz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2utxzbocc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iiktdisp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2brglgwka.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ugkgheng.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lpgskoqg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xbgliaig.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ejjbweej.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pgozayws.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pulctkgf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbdxpvga.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wleqaczo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hipmprkg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2anejitok.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yjcvmwxq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yjgsstit.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hgjmdqwn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ohwegosz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2aqzblqep.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2amfekepz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zrkozris.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fmsjcdse.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rilfcmjt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2szcdkurt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rjynvkfs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xqwqljbr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2icdbahol.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rjiqwsdo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vvmglyoj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rkgffwcx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fyphqqoa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pyjllato.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ftrtonaz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hhdffarm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qjaqpvod.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lzktmuhv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iyifygma.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhqtkprp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rxhmfrwt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmjqlyj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qflrgspj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wiqrppon.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qqjultqt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vdjrrqgv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ubtlhzoz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bblpzhbd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2azpcwskc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iufgivam.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jrhxfphh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ncgjgwki.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvcrdros.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2acsmhdhf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ncqsvuib.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ieiumfrn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtiofqlk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ytuoehap.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2athaloge.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bifemjae.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oaidxnjo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2acgsneqk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfecghj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wbhmkrpk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wiedtxul.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wluifgxj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wadqsyxi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wekmmcvj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pkakfhxk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dbjeetux.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zttqvvip.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lqwkhipm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvrpjuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgcfrrfb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rlntxuym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxtrryqw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbuhlheo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hfbbdvdd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zdriixzf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wmpcnpzi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fstxedqd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kbfauxpw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2romgwqoj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jsggnitp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pttbmmso.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zbdyltsy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2whxqzmct.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mznxvbxc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cbucwevi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vgqfthel.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rfuglprc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xrgslqdn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lxgekcck.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdpctwg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dvtzujar.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hcqbkgdd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2saxfpntz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkmscrid.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jpllpimd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tvhnsnpp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2swbnbiik.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qgdwipmk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wbqrcost.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kycidmyb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2asojlykz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hpizwowv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2baotaouy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ivswwass.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pcebvtmy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nmfeqecs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zobquczq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tcofpfuu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wdcibdbr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2nfsxruyb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dykmwzhw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxwnvgx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ruzxiuaf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vplciacd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gnvsmgys.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tkxbkqgi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2orshxaav.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jhingyut.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kwwarzsf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bncybkdx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cvrrmsdi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qbudcduw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dfetincr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kzlodeqm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xinsxzfs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xwujvmmf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ixianzix.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2loswfbci.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gjkqirbq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yffeunsx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yrxrfgtu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2aoixosyv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qwjheoec.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2okwfwuik.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qwfplnbw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tmbwvpah.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bhrclgxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hnldayyd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uxgdactt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wjmfkrdt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fqbdtisi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jfvvnnur.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mowajlrp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ryqnoqab.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qhyoybci.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2upuzolmz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hzynqbzh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xnjnlimt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lposdxye.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hyzjbsbz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ssybqyvz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pwieouik.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pdvfqlwu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zbcixoda.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uocuumsp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fbjhfhvr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yhfhgsvk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2guszihvz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dvbqhuru.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kyqtkzqn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iijrcimr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbnkglci.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uoghggny.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2sjainmqp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2sexdbvuj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kbmebugh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bctranyn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxwckqwx.html


<!-- 参考信息 -->