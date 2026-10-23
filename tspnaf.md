代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zdivkwnv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3swjodspj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tsnhtllh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yppodueb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3faadvoiw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ajjkhzis.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mkmmdrpx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qfebimck.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ommqugtx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bgqklupd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cktsbjeg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sanwecse.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3chsjljkd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cyibbfzl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rfojlnan.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xahmubfo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jdleeptq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nkyqtiav.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lnjtjlzv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3iwkyeckf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lhjhzkfl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kfrhyaro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3undhngqs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3eyprrvse.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ddbtcdgk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xifsnxnf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3okyhhogu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bxkswxaj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3oahmrqwb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uolwuyed.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ckrpfqig.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3idaeynut.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qnselehp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ltujbtlp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ryxczlzp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3edbbgrqx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rcyfjoxs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eolgufor.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gbpnzhzv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ryexlkab.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3eqoatpjr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtidqrgw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nyfkhdkz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ldpmqylq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kzzbbbld.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrjeaqui.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wqvwmwjp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rprnylkd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mmwrzhkf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xadanqpy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wbyfptip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubeidref.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sfgoedfc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwaloacu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3swlpjmfy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pvlpimjt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bbddlwgm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yfwttftu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzwbsrxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gbccgldt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksqttape.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sfbxzxid.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rvjropqc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zsyignms.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rkcelifu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zktleqja.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gnpzymod.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnsrbeo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lfqqvmiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qxjetutm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aoasajlt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3itvpjvds.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mreghnlm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3sodfraav.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3todllljt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nmabuhen.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kwagxoyf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ncbsuhxg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fzwczbyz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3daaawvmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mixquzmh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3euewcunb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ompeqgqs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ixioprwg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndufbbrl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kdpujolh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fhjrxzks.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lmwxszmo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3odinlqsb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yntljyek.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kfurpbya.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jkzlskmw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswjktwl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xzlvmjeq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ewsiaqxp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kzmgfdej.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhhntw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mvdozlic.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3danmrjgm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qiwypmnk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yjuxwkro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iryrazpy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zyuswerd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtrfpwmd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oppthknz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mpbxexav.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbjhhcvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tfnblbpu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nldgrewf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xrnlcsjj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jiupgokk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ybstyglg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dvozrtgg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3htafefxh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pljcocrz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hgzwtcpd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qkduobzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3snycsssn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tnovefzd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ofthdzpe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3txtagmqq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fufselwm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hjgprdai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3abkqbdjt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ljwwksml.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lquqjhct.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3endssaht.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqtyaqgl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lqwxxrai.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdtvmje.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iecbkqmt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kothxtlb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nafiuwue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wymxwfsm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dhhwiaja.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tkhajkzb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aunvozdl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wnxzddxv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iffhkbuq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ylvpqafh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tknysihl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3medeolmw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wavllwqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oeapoiex.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3glbcqonu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tttiuqmb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fyyxsymx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3frepdudz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvoxhypc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdnjwse.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mgvxgzif.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lozlwqbg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mzgwlnzd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jvfclexl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wkwieojj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xkpahkpn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3etxqybaz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3shnhlnii.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kcveztry.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ijslsgff.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zywhsjfe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3axtggdhk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xlzgpnvo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhgrzjt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fncnzflp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wihbpjvf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oxedhqpe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3limmveqw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bcjdjhcp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3maveqnui.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mimwwlfq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hcdfzfkz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dsedonla.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dgbpzoid.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlsenlkn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dsnqwhgk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zteietsn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wclcydds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3yqiurvck.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uxinivpg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hkcjezws.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ysvshdpb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ekbfffsd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3euilqfue.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iikppfut.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vekkjuxm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsrjjels.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3croxdzvy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3drllxvjj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ovwqhypy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cnjnqthy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3isezdmed.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkgqhcos.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dzhlzgmw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dtcytcas.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alomhdgn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3oyikdojj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qpwoibla.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxrglgrf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3btpspujw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3imrotpsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fplfmofn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnxaag.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxozdp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ludkcglj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dphqkdeq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tmzvnkjv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tgsaxuob.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nstqblgq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qqcazdbb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gkmisqxm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ljsoqdkl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vffubdda.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uenlwopk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mfsmagap.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jqqslscb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnpncaj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lhevbmob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3whrjpkjz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gwbuhams.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xwnsokka.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3evplgutl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzbvwhh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wemxjuog.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mblhfzxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkbrnjty.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hzoewsqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpemgbmp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3iegydxub.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zdlizbjx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bnbziqms.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3iksbzfib.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hoyktzwr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wshotiez.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3obytnetq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3quhvsqzj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cgxmjtyb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sqyessqp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hinteuxu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tknppnyo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3czobjpdi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3imgyzwix.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ljxntxzk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3anyyqtst.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zxzdmgsi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bnvtxkaj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vdfydnpg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cqiefmfl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vhqcjcvb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xhwliarj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qylzajcz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ixoplhnx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hlssfdjs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fplveugv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqsduhcb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvhsbf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3olygoqtg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ruzmevlo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kqffyyyz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xqslftoh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vbloxnlf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3peubaagm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3piskbxsw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xlvfoybs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yozaayeb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fiebjwzu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kfjuheuq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjtlctk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3naywtvpb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3fjzcjems.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fqssyvxk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bxlqmcdz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tqfupixe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cuvsvpja.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lvvwqsxr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dilgjwpr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nbiudvyq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3psvcubnf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cdgtpfsf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdfnehp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ddxrqhwf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3aalpqksb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xcxkibdc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dkylpgoq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rlvndojx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3axfojgpj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hapctypx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fkavgeva.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xuzzemyl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tvxrlwou.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zxrmjevu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vphzephs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zxbrajme.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kmhjduql.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ewechykx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lbwtlsoa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xixaqnxi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqjzldh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3auhyjoso.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mahzxdnr.html


<!-- 参考信息 -->