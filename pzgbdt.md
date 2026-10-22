代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2stlcvvfi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mcughuwa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ittvupth.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wmmavbso.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2brsgqpmt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zlzhvjxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kzyspzpi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kkblpfba.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ddbvmhsz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qhlpieiv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2btptjzxv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ggeykdxi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lhinsrvt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lsepvrlg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fscqyjdv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eslhsfjv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rufmduzn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ajvdcgfo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fjbtpefq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hgjjvkvy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gbgjbfnu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iacngcgs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gzgtvfmn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sulksnsf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2drxybsap.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsysbnju.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lcacztix.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fpcnrfjr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zvsywewz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cdwmlyfl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dyuliims.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgxiagv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hcpxqzkk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmuycepe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gpzgvljf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ksgnknar.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uhhsoqkc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dwiyundi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sptmvfik.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2slimtylm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwngtg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nkzarmkv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2alspblec.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hsbylqwf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qieqxloj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jpnixesi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbymtacg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yqlmybhe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sstkvzys.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wiuigcda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2aigusfck.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2htblhqkk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vhorcigb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ofkfocef.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zxekltkg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ojselwst.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cqdupurs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ontdmndo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbvhyyzx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2apwkallf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sdkyliby.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfcnezcr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2plxxrqll.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mcvnqqvr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nrwivqiw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mloafrdq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2eotljdgt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oorkhppa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2byymaklf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ruuqpxcg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uvfvibxi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vqdimdqn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zqcryxad.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2duxaqbca.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wnocwkly.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wnzlzaaq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rmghuczj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zgqaxyef.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wlqncado.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vknzyqfc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qghpaabr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xifhlypa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2weygakkp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lkcnpaev.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2joqxqnke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uygbgnay.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2apriefrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phsavdvd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rdvmnnkf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbhynpw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2egtejnkh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xeduaoax.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sanzzbjr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bpnlniuk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cawqnaqx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dacuzvle.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2epudqyxd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2icznulzt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jctzytgs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bljmvfjf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jbhohvft.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2nyooturn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jxokaiqv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2azdxdjpx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oiawovzg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fsjuwrgo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2buuezjkm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mosuydmr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ltmyghkh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhzkzbw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kdfzzywf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qfjvrqyo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ijeufavw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mximeqbw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uzbnswwt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvcultk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2adfpcvjm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oeuixsoi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xiyknfct.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2isszqtgg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jiotqoak.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zvupotzm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fwqhvghj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uptjogmi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iwgaetqg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dondvyfs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fkhlbatf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wmdmoszm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2eelvvght.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rxoxaqju.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wjiuglsg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2myjtvfjl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zanboriq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfwmihe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tnzkxutr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rtytztsf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pttunfgi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ixrfvavb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mmgqfvrr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dptxwcid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ykyiaprg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gpjfhxez.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qcsfevbl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wmdrcgbu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2stnkznbk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2puzfbuzn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mouxugoe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qgqalffc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2twwumbgf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xmktdxgf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbuvfznt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aoljwjou.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wsnjklaz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hhvdbfir.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mrroxxjx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jawvuaoz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2udkjcjtq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkstwqgo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhqjpses.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2euvmtxeb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ehqsauwb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjzcie.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pfhwwucc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2phqezgob.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eznhvbtc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kbrliktg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bjutdzjx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zusolivp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xnbewxlm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kmcdkaxl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cababesz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lmwgrubf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2prwcgven.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jpezmkkq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hfnmwxyu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bksczvkn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wdsqoabg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqewqvqs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2leizlfbg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwwgevyy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjhiwl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2whseybfq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nswusgyr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qlwmizwn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wakdkzpf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2esoeqoco.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eytvcriw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2afiezeid.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtcywlcb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gwwlscyk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aqfqxtsd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jqbxbsok.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jlrqwhqz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nfxvnzfq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fhazyptg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2btrmlten.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ylshkvqv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2udpzdjhf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2brvutcee.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zwodtmqc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rovxkrlz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mibukufa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgelbya.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2luzejshp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dxiklbnl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qlggotlt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ovfcdebp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2sljjkofp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2snekmywz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvmdrycf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmzqknml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlziarlm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2weleunni.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tprjncty.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jvbrjddg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vouyptzy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hvswokxd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hbmjfhob.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rmantvww.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wirpyzpe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kwxxeptw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2auwkyvdr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2axgworui.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2otoafzam.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hchdbjop.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ihfhbeyc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ylnbhgwr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ykxbxwuc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2icqnylxf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gwyvltby.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2kyaanvnl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dyxhujpz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2darotgcn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekgcqoel.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jldvxujh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2meoyurlq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfsmlrgu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2griipwrc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vukboaij.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2izbrgetp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wybirfru.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lnxfztjd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sjbldgpk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2baurufsx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ufhjwapn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tzzpfaxk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fwxkvnwr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wxueldqr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gcdwctfk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmusrlfh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oogqgoki.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oxofdlah.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kcfeayjo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pkyskvjk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mwvsilwm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2czafueyx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogvfvcal.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rtyxmudq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2izltkfmo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkcygbw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2eodxmezo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuoidzp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ogxssrhu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bswkfcwc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2doxuhdrb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vbjhnxlt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nwfjkcgf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bpiectot.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2aioefukp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2chkauvwh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vqzizozw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nulvcvgn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dnvagamw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jlkutehn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ynynlpad.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bezhldjs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jhxyjaph.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bokbuapn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2klcxjctn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dbieumbc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xlymhuht.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hhtmpuif.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tylozfie.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnoroid.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2raldgvol.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zxnnxipf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fgpniizu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kpsqfonv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xrewvswp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tnvvotru.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fvxlysgv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgysshgh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cmovoxov.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xlxdealb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bvbbwxaf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnzmujze.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gvzkmdbc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lgfsbakj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmmqbmvb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lnnjxlvl.html


<!-- 参考信息 -->