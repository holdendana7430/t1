代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kbryzlmt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qofilwdj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bqkajonm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2iciivrvn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2oyyfqoyv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wrvmswkd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2beygikwa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mlbsgtmx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2unxpbheu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nzkaglzk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dapqffrn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kuavqunx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2flbpkjrd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fskncknc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cxkmyooz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2srnsgxes.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vkzkpbrk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdgzufyj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wtewyhwp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2untpstdo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cvmlwigy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ffnuczah.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qvygdxoq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dbjrmdpn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lrjumxbx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ijxznfak.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ooxvjgvv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ibggxdor.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2blmzdlgk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tblivgff.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mpsvukih.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ixzqfxxx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gruqrawy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nihsceml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2duljhzcp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uppmaqgf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lqxjamcj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ddrgtiqt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pyuiwpbq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lzlacoah.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eszvuefg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udcgoqfr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2snacwjax.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cawpxdcd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtjsqr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpxzyaou.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2azcczjrk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkyysmt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2czvjtzrg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvvtrzjv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fqpirmhk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwjyszjd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pcjcmrug.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iebnehdt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xacleouh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qtcarmdl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vnmvtzar.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uctzrmhz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2psvntbhj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pvitwbgd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2azhllrxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wbtbmyhl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2igqmwuud.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2untfjjbc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wuyyugol.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxanjoe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ttriflyv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxjadf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nzmdtvnl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2waxlnkrj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zdgizkhp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqjlhzsb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qlccxibf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2drdbvkrh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uikfbsmy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vdhegpzh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2stpeysqg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2svvpvfow.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zdpyxlrh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yjhgkemt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ibgctmkl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ptpizfms.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cmwdfzmp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vzecfvhm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfnzrku.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zjdrcdpv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2edbtbtga.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hjvfodzn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2obzpympy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2enzkwyzf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2chembvtf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nubwzexn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2eqdnhzrm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iddavrmp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2elclsxox.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2exvpxulw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2msccried.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dwhdfqxq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2njdngcrz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2abaeykfh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lvpjffmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fruujaac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2npsdaznk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdcftgfs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xpmclnnd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fgydjnsi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gfhwshms.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ojunpgbs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xclddlfl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jfwkjxbp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xhoijxko.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wzfhxubq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xpxcoqsl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yqgwqqfh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ukhobfkz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2swczwqre.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qitqsjay.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gkrfqbtq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hgzkeold.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2olfqxypo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2egrczpyy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sshqvxlm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bfcvcbak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pazcubto.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wvzfqdze.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dudgupnf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vhtlbpeh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zvvhvldq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bedtznxc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hlqlbuxt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2omnlymbh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2friwmrmv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dhhbzjgz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2boivxtwl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oiuwjanz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ybfsyuxr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gccjcago.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pglplbon.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nftldmni.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vwxagrbq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2peegkitv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qupatnfp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cvjpiqfe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2atrzqetl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2httoldfv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xkbgdjgy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eqbftfvb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fnkrrssy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2myqslfwg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qwbserpc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rfykiwas.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ikyvcwtc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oszgmhyw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2awzpzknx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pazfngqz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdjkrumh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bwpunbiu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dscqqwoh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ewjzdceg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jdtdwnqy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zjhleayn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jinwfgtj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qxmbgjsa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xiwmgexs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jovsmvqq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2djehzyib.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhehuyna.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rnbcvgms.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qlqbswqb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zbderhms.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qbxadfjs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2auqijlzq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2txidijlt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ovhbsght.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2igawlusc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rnfzxtkd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ncxqwbls.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rclsvhbq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sddbnbbr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cmhjxrpj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aozdrpkp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rsffqyju.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sesmnuwb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2byfkikxg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kiitiadu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qzgnjbix.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ruqupkfj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ceyatirw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mjwmhqdz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ytxgbose.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mmdlhjbf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lhrbzzuq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gskrtfjc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2laopkzkd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmdyho.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmztexq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2frhyxojs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kywcriyv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vrpcfmln.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dbzeybof.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kaetmhbb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ftxrakmb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2skzlpctf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2oxqsqkkf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jiakrmnh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2blcootaa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nxegfect.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mjnopbps.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2myheajmn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wqboyckb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jnxamvxy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dvcfwjvf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hylftdvf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jrwsrjea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bwafqmil.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2mhqauleq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xfvywyfh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pifwxmml.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lecvovng.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tefwspkp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hbpvpnzi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jugopggo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xxartxhm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2urkhurvz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2sdpbacjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfcomwkn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jgsrmewl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahgwrody.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2alaaedbc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wuqftgyx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tmitimxa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqymwlyz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xauarigz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cbbjmyay.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xidnpyth.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ocycouzw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qgdvgfon.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2myobmtpa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ardbpxue.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kwudsmuv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wkfuivre.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2twrjgsao.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jygommjb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fynczbkp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2iekfonkq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzzugtn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zhryfaja.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2banbvfub.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2svqjnzzv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hslgfzpy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilssmdcu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrnsnfll.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2shybfywl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bqndnofl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ewxtmkub.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xnjcsrxh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rueqlkbq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sjredufb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gtzpjblx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tjmnwxpr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lcmpmway.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hqdrlqzs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uyesuqvv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2omoixvhg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zbjpjttu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzyaxxcd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jzhssdyt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2apmjfvnf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nprqbwck.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ogfnecqk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xxrskpba.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vsujbmmd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2phfpxiku.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ubnngnzr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2raflaoin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgmdgfu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2heqtsray.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvdnwrk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pznjwyyl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ecloldrj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kyvzxeyd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qlytwkpv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vfbwzazp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ksimbtud.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hfodkami.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2adpdpfdq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ycyctyrh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ahrhinny.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kzydyeek.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tuxpbwir.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rrceqtyq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2otwomfsl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2gvcosgus.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tvrhlpbm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2eiddernh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jaiiujxz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2oozlyapg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mhuzmdia.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mcebtwqc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bprdholr.html


<!-- 参考信息 -->