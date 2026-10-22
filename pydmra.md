代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zevunpzv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mjntdtpv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gizjusjm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xohugewo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xrwcgtde.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dfhjhyar.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wbxpxizv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oodzuvyp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cknftnij.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rtrzozfx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2egzrkvbs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbggqgwl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mfsvtbgu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fkltqdtn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eatrbqnt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2plizrhpp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uljmcvbw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tydpxtzb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dkctkrtl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nlrniffy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vhjbudrm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2viwmyinl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hqtindrr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jritling.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vholvxwo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qxjvcnvl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gydnexdv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yfljycpd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fjnikgbq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gukrgbac.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qupngbxh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2egwmeibc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cpyuanxs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2akcatdzv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2trerduwz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2honvpjvq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vhcjthch.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oitjvtdq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tiknubzi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hjdmkkyr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2flucjctg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nimnviqn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2girmjbjx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2obamvhfg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cmkqkyvq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwayzqsa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pmnwjnzx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfxpmepb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nqdblswy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2plvejqrz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fojafwjg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxdntaeq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fzygdilq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2woakxvaf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qrlcwang.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dnieycoq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hkfdylan.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vliuqjms.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnbztbvy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ehbjxcqo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gzfhpdmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ajuqmipl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhhhcdjb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lcsfgdme.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jhthaxyi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zsmqtoql.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rgqklqtn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wwfjdczf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ecppnuoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nyysxmgt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2okgtoqaf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmoptbpz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zgezsoyi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tawexmfi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nevcigye.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tbrhhnpx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxhdgwy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bbqwalvu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hhohlsre.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2llsisbiz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eotpvtxj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwzgwm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nnetmvcq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fdqsdxkb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhngzpr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gkqrbuip.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zslreatl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pfvshkla.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hdotnzrc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cgulmgtn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2crleiojf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jnzqzwhy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2saorjlub.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ihieomhb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xgtujavw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mjchxpqj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bdvghapc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmfsnz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uvoesnoo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2syotneak.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bmqpnfwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twuuotcz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yzwhurvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iakxmgec.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udmimytd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cgmmmuzg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sdyqvatu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bxljklvn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bxqkqhiq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jzqaroon.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2msxisqbh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ovkuvhgp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zfnorbqc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kkldlaxb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dkxfhgcq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yejocpvi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rafioszq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zyajmsyx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rtglrgbx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hccilvvl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjspjmpx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vcuuyzrn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2enfvjaas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xsksztir.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xorlhgqa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hrsiqqok.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bhuzawbo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ognggcqx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cqqzuiox.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsyacyeb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qjfrjqnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2flmwllrg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gzdznhtf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2umexgjhq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zhkgqxvh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mphqfitq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2iqngkrwi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kgrckymq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jktlydbd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xuddscbg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nditjtpc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rnohrsah.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2anewsixj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2aklrjwrb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lzyghzac.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkrokcs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uehhitlp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rxgtfava.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2efbcchdw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gvmuojrq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cxjnxsko.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajejmaxr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qbdzwucm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ybkgaicw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vtvjrbba.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qcsngvge.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpwram.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttdrvikp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rsaqqnvf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hudqnbxt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2efcdpilv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vmxpufnl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vmcdnudd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bpfbmcnv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jsnaedhz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yojjykgo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqjbfwon.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lcxikrwz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jilyqheu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2iagsdgao.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2swunozhe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dzrpjara.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rnmhsnmn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rzszbgaw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dnkplxus.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kdimfyps.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rsqixjan.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2diutrbsu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fmytchdd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rsirxnee.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zlpshcsq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eltarrzc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xuuzjveq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lqqdqsyz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbnsxmnc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gqxfzjjn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2susjkctp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mqvzoafj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iidhcopk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ogcvxtsi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fhbcvjln.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znrjinjc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vrukdodc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdgzihtg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nnkiyuol.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xiapykmv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tqzfmeen.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zvsihqym.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wwkaxlsx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2znzvznyy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jgasusjm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbypzhxp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjooakwu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2txydmenv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cvlyimfg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvwzygcs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pqrprxny.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pblxcprs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajrepgls.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pemcdzby.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qmbwredv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ocgbmlls.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tijsvivx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mhnrppji.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2smzpcsfb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zdaazoxs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxpltuh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nxhoaqoj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2idwivtxp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vdmqktpc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gdswyrao.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nfupuomk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2psfurcgj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qqozlpnl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2iilrxzgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqpqujsk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rciwbxkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjfftfgs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ryeuamhw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gnmbujpv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2oghqruvn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2voetcbmd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2egxwgzpc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yufjujyd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bcfuyfco.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pkgisoip.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rmhotvxj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jqatqyil.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kkdxtwcf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2urdngoxu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fqemtric.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dcszzjyd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bbjqjpfs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2uesjdwsz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2elwvbnwz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hhoduusu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qnzxqubg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wttrrbrx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2yumyuxjt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syudmvda.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cdwikvqb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wfnuhars.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xnriupbw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qoqpokix.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qqkpqscw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2iqxpfbxg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2eydjjiiv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmonkc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ygofiwyq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ynayrfvx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qxzrwmkf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rxnupnxk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rkxcpjqo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwdvtmz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ykdvxsui.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zkxgwldg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hwevdniq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2difgucfi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2smbczupu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2paqmraku.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ifpbbizz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pfpvdmws.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nomlcewp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cijopbiz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kuvoyigb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mearkviu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qprmoeyv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqespgj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lqucsssm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cmiquvza.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jnvkmiiv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kotlrdjt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2opiheqxu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kzrpwvkb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2etaxxpuf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tguiktsa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jbptrimd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hfyjmxiw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rkpdlvlq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2monizerj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uiwlndtr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fscncqbs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zfxascjg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xrgudowe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2chdtnjmr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jsxrljqj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zsgnaymy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fmykbgkj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2otzgwcvm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dqgfmpyp.html


<!-- 参考信息 -->