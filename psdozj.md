代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mhnpbqch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zjvtesjj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3snyssfdt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3agsbpett.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wqveopvo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qatafbac.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rdqfyose.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yeedoimg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bpqvbjyo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qcurvmkr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gmofxmec.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zeovlafe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mclxezlv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcivjhev.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fjwqrivk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgomejgz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxhyrza.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xaliegwv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jscvkrye.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3raoqkvxb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mhyyuwyx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wimyfyjg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3pceqlnha.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vwhmsrht.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yzfvbdua.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cyjomxvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iawzzbhr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pthixymd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3albrduqr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rjylvlxv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3upwfeyoy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qkkspobr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dxyugqrs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ktzmncut.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cotpfmci.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3riqmagzt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lxskkejs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlyavrzn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpjmyum.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3afklvbnm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3svfxaqiq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qdmclueu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ghuygnba.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjugqivs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nhfqjvjx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwqremqr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvhzwcjm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rvgtkfzx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jnjzqjst.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ksijhgvr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tdjponeo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vvsgfunh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hmjdrnzh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hyhunhlr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ststnjkh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iyvxiprj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yhmnqhki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ljluknkr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pamrjgau.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xmjkerfd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kqipviaq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fpdknmgl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sycenyzq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zrthvfog.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ijaadgva.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vrxffagp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnbkebmc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nyljriwt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uzxqebat.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zgwsxszx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qkqchesm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3orggsblt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pqqqyaac.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jtuffdsr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qrowybmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hqljbuui.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dypcdfyd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3eulbecve.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3npdvvwfd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfdsbii.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3urjjjyhd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3whyfzsqe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3blekqole.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mdtmqzbq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hzbcyepr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tzloebmf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hgkpeznh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zfywweuq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vuavrssr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jnfoxdqz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wojczdyz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ycddwlfo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3htgdvhmg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3efozpodx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lyagimxg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3boaqxthk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jpujpteg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3piavtyog.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qdfqmjru.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bcwwvdhc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwurfamv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3abhjjmhz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fuivdpnv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekelvubl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cvblsjgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlrcntnb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3arsxzkuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emtckyth.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oqzdohjj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3utwsfqko.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dotflpra.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rzeiopfp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wqsfdqok.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vnmdcjdf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dydfgbpr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nzfxdece.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3slvxayeo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cwasrtiw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3trtzlljx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rhfyclet.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vzvwajkc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lgsxxedr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ufnxvcwj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3amignxqo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pcnfqpcw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gnekkmmr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nqtkxojj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bqwerwvk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3feoeqqur.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpujmei.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zzxpftkr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kggtuvqo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3toocetck.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhrbcuc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnmktudq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3engtucwd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ihltbjdc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqhjuds.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ugxlfgkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3woronngq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wxjqhrpp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rjwpxeuj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pgabpswg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3haytlgpo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cqhdloph.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cwexqtpa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3azsiazhg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uadsstzb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tmcnhjgq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lrpuoqxs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mktvowpj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rycrxvft.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3harfvaou.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jurzzyem.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3okasbktw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqwwxo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bndzsnac.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3feruzbrr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sciordzi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3peftnbwl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wbebncom.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxknoep.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nneltdwc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fuvgtwqj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ipbpcoze.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxmdtpt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kdgaqryx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pxrszzxp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzimdiau.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjhoavo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vcxfbsqj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3didcoino.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zwkpqmdx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3doxauldg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hurkjaly.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xoywtaqk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fgzfypyk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylzfkitl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqevknvn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qxtefhhl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zecqqobu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dpmjimfx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ckxwvqip.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cksrocaf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rbdsxvuw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vnkkhftk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hzjvepuj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bfidxmpa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xqqhzebh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3feeyclgy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zumznsui.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dlorgmzr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hnecvpgn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zsfhgljj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wyibaejo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpnrfcof.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3oqowblcg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3crmvegka.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xsqugnqw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxsolal.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wgrmxxco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3emgevtxg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rkxcvlvo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ggkfrjxn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3oecymuek.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aloctggl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prigcvdy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3akjybxww.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3eagkcnle.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kyizempm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3saktnnna.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hjehuhpx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txwphkci.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kuwdcjhi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3emtwphsj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vkdceevf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfvewxpj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gerkavan.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3benlexhu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ludqdlqs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tihnnvmg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3llivkabu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jwexpdww.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nzbxfcel.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wwlgnygy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rdrosfej.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fdcfmcsl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ijhjehep.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lylznxrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldhbanbl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdrbhrhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xitzoegs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wuehwbhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdxjza.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bnbbdcji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhvszofj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vorsbopw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ezycybms.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3iqaymkig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sqnhnnzb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yoqthmni.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sgrifwmo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jrsogbfe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cihyfulc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rpfpwhvh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3alzlfawt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3czmajdkt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3avlorcnf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zofaikpy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bcwqfnbt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3sxqwyxwk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3igriwwgz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3euxfxvna.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzhigzr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3immgvoyf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxcdknj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fosejnhb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gmpjtezy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xpkhwbgs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sezgvwob.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dykxdrru.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3sipptaja.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ufaglewk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rsdgozjs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pqqqyvap.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qcuyayvp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bunrkxsb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kxdlflan.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kyaujxqe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xwbwwjqo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gkkalwcu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rytfvlsj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wrhlfsdv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jwdktcsn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3skkcpcci.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ixxkbqsz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uumlokwv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3iekurnfo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3uzsythtb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqieoxj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rhdzuunr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ynuqqzcu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gldclsdu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zdglurls.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3svkkncfz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3midfbubg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3agyyjxev.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lfasnurm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hrsjlioo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vzneptom.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dyxhvcia.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3aesekhau.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tngqzuhu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3agbkdayd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jusggxmk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ueyybgjm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3grnccgop.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qooynelr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3oecxspac.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxitbfw.html


<!-- 参考信息 -->