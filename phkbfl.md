代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hxeeatpy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yplkuhla.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zeqrwxzo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gxxuqdmg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xzmgqqrb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3scvhedpc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rindvayf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iyabtgea.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rxepsohi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wvglbsey.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zbjvhzea.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bjnniuoo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ejqafena.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sorulzqm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbqxqrhe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3itsmulxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pibilplm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pdxixesg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ajszxxgk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3akoxmkvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ideenzsw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pzmdmhtr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jmllwgiv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cuqpcacr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dejyihyu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3crnkjzaf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3appixupm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3baybkbvp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqinoiq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fofxulgj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sefxdeqp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ojbgwwdz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3reusrwso.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bzsekcft.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bqjsznas.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vorluepu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hpiaipva.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yikhconn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3aznvqoig.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlbiksvr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xyfpeakg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvyvyam.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gzmwsykj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bcmssihm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rmefpmbl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pqypdcou.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3klcptiug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyjcvhnu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kkgebjpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smyuvuiw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3heiqhaxw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vlbmcfub.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3njxdpzei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihyxxxrh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mxrpzbez.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rxzvifvk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wtoulkbx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zpcswcej.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bndnpsxt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qfnabhnh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nqasbhda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yijbwrfr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pvwdcvjz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rfuwfbqy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3llnoevll.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ousswfpy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ssbfrffg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3crkoqwvv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vfghaiph.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3okwrpbmb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sajqyooo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fplnrbai.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jzdpjeix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbitwbc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnfdtfox.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mlpalsol.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3icighghf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3rgdofssx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3llesgxvw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kutcwmay.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpwtybam.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lgnowdqk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3owifuhqn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bhlsibtg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiatweow.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3stlvewxh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wvjtmnbo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kfffwogo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dtjeeqrt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ukdlneyf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mjkegdom.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lkugbaai.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cflibkqz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lxqdrnce.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3egqrhinz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3eosnvcpu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jjhsxubp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qtztqsyu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vjzqbowf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3thzndtrp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uuturzfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqyihoiw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vygdethi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pczegaxd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bddklyxu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fphlmmdh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rgsxakvq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kbdmfofs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cbnuaexe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jwdnwjbf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bugdzhmv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvyjeyzj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iktrxoyy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jggnyhdh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pgbihthr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ummgvpnh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gkoubjkj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwsscqr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yffcucin.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sawoqjjx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3eibybang.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zsshofbl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3thlnlfkx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hdhsipsd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ixpmgzws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wosuryga.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bypdxkch.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hawiffev.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iksscyrp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zxstxttr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lldwmmkq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qctpyrug.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jrrdiadg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zobvjxzl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwpdkdgr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eckofgjk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jfppviyn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sggfotrj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3prjmjyzd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kfefhyxk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iaspgbdy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ciaistpa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dqejzfzx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvbtdal.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3awmlaswj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lndareak.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hnkwzaox.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwpmctzz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcsddtgj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rnmxiagm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rqltupfu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysjbswps.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wrdvjufb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nckvxiyy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3brhpcerd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fpgfpizd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bvkzbdoj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwrzwzss.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3shypwsbd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3endmedxs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3etprnihn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mrotbncd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3khhrktmk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3iykccuzv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ehhreklx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mbobjuyi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fjcayikg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fczbcmbf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mghxhxht.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3aguxunmt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3grkkyqby.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aeovtjbu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hvziawst.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3glytgzxk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3chmfvkjj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sxmtizcq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mceqwidu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3amlparan.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3aopovfvi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3stfftems.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3foonplwr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hfxrtilb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3sxjvghdh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mwdtughz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hmqpfzfz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lwupkmau.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3njtvbnaz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3todfpakl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pldonocp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tvmomitg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3shktgioq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhrdnhwc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jkifsfgz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ftwgdcxr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bdkthloz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pucsbmou.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tiaukhdl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iccgyfnr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kcixbckg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vgjvgzke.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjvttzvb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mpolitan.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3unfourkt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jmgpeuog.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhuxect.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdprgvve.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ymhwrgsr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wrenasqr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjxcojln.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oaxekpbm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xsnwqviq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3komtbazf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iscbaqyq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pvqqdedk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3doolccqw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3idsfemhh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eduwzega.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lxebskrb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fycwrars.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpgcxv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3obyiarbe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ceekivnd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uisjgild.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfnwct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tvytynrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeahymzk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cgmxonio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhwqydau.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3exhcnmgd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xzabvqbk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wfpogjld.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pycrlyko.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wrkwpmvy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xjdjbmwc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rgwpuqdi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gfdtoyqm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nltujjwa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mfxtpque.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pwonghyw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cvxephrt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zoqmxtxa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bpjkkljc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxmytvhj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jurzvtcc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ehnzqawg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ctowqita.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hhldjqmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3waxoujab.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fhrnbggw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mokznexj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qgiljbme.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3butjutqh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ciyjkleb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xazeyrzb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bcqyopsb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3roubuiqq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dbypmwmp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3odmvcmxg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ewzkknjg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vumwwpsn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fjfrehsj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rclmlyao.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tkjwzhdc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uabguhla.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nwjvruir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jkrgmoxe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mlpansja.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxofpqo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vsupnoai.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ycfbtdhq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vfhnrpln.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3thpjxyjm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3axofakrm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cvcjhqla.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hbbjmish.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3waevldvz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3omvokdjb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dqqtnbph.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nkjimhfq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvsoopp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wvujwpan.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zeqvxkab.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hrhvlvwy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3slrhknwn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yagepdwk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3isqatqff.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvdhwk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3myomablx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lqovakcj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nkcrlugx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wwohxopd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rxisljay.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bltnfobw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zsjnddyd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kndmurxh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pbwgbdaw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ibzcmord.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bacvakgw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cksuvltu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wxwtbqsj.html


<!-- 参考信息 -->