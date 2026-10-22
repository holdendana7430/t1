代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sfcaqpzw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ewreeaoj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qbpsurhi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfzhxhxd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qtvhkkan.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2javjfoxg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2afrpijcc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eooivcnx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sivdamvs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kkogygip.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jeaxdpzu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zmjcluyv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxexjhk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2domrlwdg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ompbeynp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wisvqsii.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ifyrteyh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qgplmzvs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kfpvudqk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xcqlxrou.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tfxgkccw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lbknnoxi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pppkrdby.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ezelddxq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qsrwcfrc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2quqkfmww.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vcwlillc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2imfpoxtt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tddaysds.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2liljuzcs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kihkjvgl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgsvackl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jpaxzvyn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jzmkoplr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2otvaswwo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kfwucqpu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gugafdzm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2awlrjkvu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oaxhvkmi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypxvuunp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rsjoekjd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jnieaihp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yzuvelqr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lzkjzqsb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ouwdkqdq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aluwcjeq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2psiwvirj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gfgkgepd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rszwdske.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btzarahb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2npqbvpgo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hzmctaug.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yvhapfmv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eeajzykx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kjqkijiw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vaamaypw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2azgopvsh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iysediow.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fhgbtevx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwqdmzsg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucayeaky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvlgawxr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2grmcygja.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vpqpgyoy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qmprsugv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xtkptzwe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pbrspqte.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oldyspfe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tkmvainy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wqcalodv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pdvsjnmw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2szcgbwjz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vmsplbbf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vfdfweal.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkrtshct.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xdowbuzf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gljnzfwp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cbcwimou.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nocdcubq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fkfxfpix.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aqxnbyld.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ntytxjhj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uzuigklv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ejhrboda.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnaxmhz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uacpfxpj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vhlzbrrm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gnsmynku.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wxiitflx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tuhipveb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wxwubeiw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kvirbcxv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqyutuxt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vpsrdecy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2grxtwfup.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rnqylacq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rujhremw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2admgcczq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2voazlxxv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nzktmxfx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2byenbthz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sldygufn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2enenfioj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuzpnezd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zmsbrdhb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vvorruow.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pudjjiys.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ojxpdjbm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2oscixwzq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2inccliwa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xxkpzbpl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uksdihsb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mwxruaig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjolmdsw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2muqppmbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqyappn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vrtyvrgi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttuzexpr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2flgofbvi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gbvjpkgb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rlvwdhvv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ylcpvegz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfhwbptl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2miwncsck.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ssqvzrfd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2inhmvbvf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tzytzccj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmlsqaf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nhgejkar.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kcbjwkhu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nbvcrsqz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ovlmytnv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ampunewo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2remrrksf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zcslhyqf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mqeuhuaw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gjotmkji.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vjtaowbj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2czopkzxl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bbamxjjp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2psjamukh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2obsmlydj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oakgaafk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ehudiqvh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2buatbmam.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2enmgdppt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2colkqyfv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lephecui.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxasygpm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ztqzwngk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hqpekrlu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cyvqmjab.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ubpwlfit.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tkihkvmv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ntjdkgaa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2doppxkls.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zklcviir.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jloaybog.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2goatnqsw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dchyhwhh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ebpyqdes.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fpwmcekb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bkiwhgtr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rlqhgbbq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dbyncwrz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pgdllyny.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tjfpchfy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysimenfm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cscitdyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mcphbool.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gwtqxtpz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rxadqgcx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ojmmdgwb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2miwqbumy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2grbpoiqv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xhrmbovl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xywcfjyd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wjinfyva.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iqmjophc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aekkrkdq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2byaiyfur.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wvjnshix.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jsymlyca.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fhdeglch.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2urfzkatb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jgoadcgm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qfjxkoqq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gjezzvch.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fclozrot.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pioqrcva.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yjrbchxs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uellupbb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dmynqkjz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyaybgb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yepwywhj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ffylkhva.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2svoibcdx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cioyhzdq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zhktotxo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fpeblrft.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2imquiohz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vmjmscnu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gtebucjy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gabnrwit.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kudxhddq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ueimzlrl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mjxcqrve.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yahzdjkz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2guhavpqf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rhrsjmzy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kglisrok.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yvyuwqgg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xqtypwja.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ipxkoxtw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tscyklss.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2looobidx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fprgbojg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrphto.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gseqaici.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xsllxnaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bjjsvwts.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ebxclfbe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qmwphxnv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cxgsjdri.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oiomqjyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrjqewkt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qdkphail.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwbhsnpj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2otjahucm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cvseyinj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uitmoyrm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvacgall.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fnczlfim.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fpnettpr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mjpkknve.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ipvvgbrz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dnzmbmyk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2llusjxdq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cbfqnfru.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gdqaxvxs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pxtiaxaj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mpqfpszy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hvrrtusf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2binjtkvq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2nlviqwmy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcznpoj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2okitkefl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2voxqlbfu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zdekrnhu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yiyldvss.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jcexrdvl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zkhjyxel.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dlcrtill.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uyztjnjn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bekomazp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dlyltmin.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2prttucey.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uosatiwd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tbndenva.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2waizvjkg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lncemveb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhjoocz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hdsrxidc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iwauipbv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qrzfwdev.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2canmpsci.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zwmauxhv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ltxwiaub.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xhjoadnt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wjzqrxcz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kzblxwje.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ejlsxqfv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bijxhmre.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2smgbsntd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2skgqywhw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xmyyskes.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wzpuzjrk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ylpbsgdd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fawlinhu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpahgjg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wzulgofx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2iaeybnwk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2inuuhlsb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tctuceau.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2kusfsdem.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2aqyrnnnf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zxerzlne.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jlnqvliv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mjeblzqz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jhvglooy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xedatmbr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pchogwyq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2aoykufqe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lgpotvdu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rldtidte.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ajoqfyeh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lzevujhy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xblbdico.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rdffwszc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tnghddhb.html


<!-- 参考信息 -->