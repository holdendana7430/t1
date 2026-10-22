代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2eqikmpxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yulyzkvi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2saxygxyi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2almpyyrh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ykbmixse.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lxafuvys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lbzeievo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rlkuyaic.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cohkzigm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbaysola.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qrlbhjxr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ukgcndjh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jtagrgjc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2apnjgall.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rjcgjsmm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecuupmvp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2olzyzkws.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nrkdqpyb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tucowljs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jioubeql.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjpatsrw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tsutejbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2totnctlu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mjdiikni.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pjxwncbv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bvvcksgd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tlmwzrdc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ypmfcfga.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lzbmqoyz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jiuetrti.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hswsbydv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2aocfzusi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lwhmtefp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hfddvnau.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2joxjbxju.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrucgyum.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kkdnnbbj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xthoduhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2olmcvjqi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tzqpqxtj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rainyjgt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2siieejek.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mmfezoae.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yujefkmp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qztuvwby.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mosyseuc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yeywvtqw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xkiyrych.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jwquiryd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rgakjnxg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gitegtut.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mgjbfjzx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uukadgmq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzqpokbo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xjldiezx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pguwkicw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wrlkxukl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhjapa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxasqzzc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yprbraom.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ontnwrdh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uhikbbjt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bstryflv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2suftukzb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvunjyyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gabxexcd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kegmzpxx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gmeudllt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2amflheha.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pwdpuyrw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2licaabku.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgoqgrhp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nhwxjeiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tqbhqgps.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gvkkeuxy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jygbgdcy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yhqojjtr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2frtkusfa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2afnukqag.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wxcrjjxx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2joomvwqz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zdnoqase.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2svqxfuwn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ozmqfstx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ttvshgbn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2poqyctwe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wyauewiq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kanlltsk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ttrykwrn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2omkdvawn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2eukgelyp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2owdautmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2pdyjqqaj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vaiwinkf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gigprkdx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zcbpcuyr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxecfzrb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ksorepgr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bpuwzhyb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kndjwnsm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qxtcpomy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qhjfenqh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qmuepidv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zcnjyemf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dhymrltq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qemdccnv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tlcmqtuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daesevtv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pgzccrlu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ahkwikud.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pygggsfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aqeftcap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jntohoex.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jgaycqhg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kevknjql.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vxoqegkd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2flpwwqas.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cghhkdvc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2goibikja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gsktelzs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xgkrvgdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2eiqojpea.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jxgrngbd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2osoduwxf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2trelerfd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dadppjsh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wdtxcdcz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2imdepmhc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qhdpabqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jllnzdlk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vkmwlfjb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pontqcuc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fmcujrdu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwzuxgkh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgytiqlm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfeeepk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ycsiguev.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jvjxhfka.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2szjfsjak.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hxxybhdi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uxesrwmp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2okvlpkxw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2licrviwl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xdfutdnp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vgxfncuj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qgpjrquz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kcjlpvjd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iirrmnlc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2harysbmw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvbldzq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iblqnlrj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mxlnjzuj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ivoittsq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tvjekoxh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2teklovxy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hgskugzz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bwnftqtc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bobwsomd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vuhkcflv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fjugxdxy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kumukujq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qyzwrlkw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cepsncbh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2iojhmrwo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ugfnfvyn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qbryqtea.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xdoydtww.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2khxzoiju.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxozch.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jvficgzg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hunjxhxp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2earrqypt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gknfulqt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nkyrlzxn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tuotucit.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2sxbzaoka.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gtwehouj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2khjfibct.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kwjhmauv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ownksaew.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mzewauka.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wfwwyidh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pqyrvdzg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2oyqumpah.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xhjszwzb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tzoobwzv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tvmdgazh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zijypyvf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2akujayee.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2owmbcfpd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eabbfofa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2boawlupa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxcawemp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2shovgfbl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fvthppmb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wshjyman.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gjmiknae.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tgatggaj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ecmrtehf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emaalvph.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xbmascyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2neuagjos.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mxjdizkp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sqkynowi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mthjfpmb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqotxvgh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sfrrjfpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qsohwikh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2eoaotiqx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnwgzadi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uykxlfzp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2crfafqsr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vggogcpq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vdjewyez.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wxmousim.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yjvergkj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmwvnb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dotknodf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2grouqdos.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2badwnxda.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jvbackag.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cgrhfwzh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hvrmcbpz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2sqxcdbdp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2onclwygq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oflzpwqu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dkigdjog.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bpglyzvv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjtyodg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqdzbsew.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2meqepsxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbdguuga.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhwjwq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bqggjusf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2drkbghzi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2llhqsxxy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wwiojlkr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2juinjvzr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uhnugziq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zwzulapv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dygcddqf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cwkjoqjk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fxyyzlkh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fhdeerhw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qeeajbkh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dkaoutow.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hrhkvwmx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2blazqros.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2adrnmivh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2timvdhaw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tpjxwzyn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jauhsglu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gmfpflsd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2iacmkupv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dplsgsvl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tqavolja.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bdzcljza.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hbiqtslc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xlwyisxm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2joetznmz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jqcmywud.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tosrmhyv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2phuegomk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2quppfxzp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cdcinxmt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sykqepvo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wghyznxd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2laxowbvj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qbfylopm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzkjloc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zrduodmx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rklsstps.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yxnkrfan.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ttxvszix.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wrgergsy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cagjpwyh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zkskrcyq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bxhgyqle.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qutsivlh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yphnpyxi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2efltvzai.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ayhrkvzs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zdavmtmt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zicmvubg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2etsmvwyk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jvvwlcdg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2frjuiafm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ppvpuyfn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xuqltmnm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hkfbxsto.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pmzgqhyf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cwiheqhm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ebzhnoay.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oozzsarh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tyrlzzpv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2frpwxwof.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2fbwgjuru.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hjrflope.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bwbmpnrw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2iukdifnu.html


<!-- 参考信息 -->