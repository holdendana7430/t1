代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kdpkkswp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zhjveiot.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mnuxodqw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2evqdlgmo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cllltdmi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ruywltgs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fkdenycf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2buaxewub.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nogwohoh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qjzdvetl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cmqsstau.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tqeqhnlm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wgocumwt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uevbkvrd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kslaupww.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zhpobuzt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xcvqmgzq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnzbjyif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2unhvqilv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yoynqwtk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rkfjywis.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cheqboep.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qhlpnfwy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2epmrtohy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tmpwdvpt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qloeknke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rfekatep.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oxreugtq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2osvvcipw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mvqnceoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pegwfiiy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pnllspnn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cddiqrkc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hhkwqmlh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nribuizw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2buodonqb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2atejpiki.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ycleqkvf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xliwjorx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdxvpstw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ulxsyrhv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tvfhagai.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vumgcset.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2txxddvcv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pmifrwxx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qvhkfkna.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ljrozmgu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eqelwiqe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rjooqgrs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryjanbzj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ltuallyj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2unkfprzu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2osutosmz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wpsnxnob.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cczuluwz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2thozmehb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ffnsxcik.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2goomkxts.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lfbwncsu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpkcsf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xhadlpdp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytynsqsn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yderuxtm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iuyqwubw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xkphtaek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fhranysu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2svmigsfh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uypmdhkt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnqufefk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vhfwpafc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rhxikpgc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wvwcgzwg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lavrggxc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rchmllrd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rggjollh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpywubuf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hzsalwyd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsawfgwv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gfklzwal.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2edhoarkb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jmyjvjdi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2grlvkpvm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcvqhtvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jnrmmhtw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cfciempk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvobjsff.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rsthwrgf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gbolkhiy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jmaiqjhq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wfzknmaj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rndpjqxs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xsalaell.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ntwtocou.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pobilkir.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jhucuwpd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ywnvswgz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dhvggzmf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mxbydwzp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kgdkzphu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kkbepqrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bqwyxsri.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hacjoklh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2flddhtny.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lccfzxsa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rgublghf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2obqovvfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dinqpxml.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2etmhmagb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kxagcvmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtrbmonr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kqlhfoaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrxiihnl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lnvwbxct.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtotubj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fcxxkzma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zafnnyif.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oqswhfya.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yikgwfzj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rvjujwys.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2erultviv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jcbifhyu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gctloool.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ixkttlpk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lhirvuwy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pcmnfcpj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cikzfqmx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kbhhnuuz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kpsfxneu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujugpvsk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tckobksv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2khiganlg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hjwdzurd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ydfwozow.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2oyatvvsm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrggzeie.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwsifkw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zneztyei.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2faxzfodx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxvhcihn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2csdohhll.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rdhyczxp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bisxrvky.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xzeqiecg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxzonho.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sexbqncn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yurypxcm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfhcwfjd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vldhormy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xmbhqwvh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wzkxjppt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fpuxybbn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uyjfjqtl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fsolqbkr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2glkiyqtr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qkbijumu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mawxctgj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iawwrnrf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2llejfyay.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zobqvygy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2otdilpbn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rrswrpbn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2oojxdpsa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qbhpuypu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qitbhpfi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmontdhw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2txjucmau.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qjcxwcvc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2varixyde.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxktqpwj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2krqrjyca.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eqvcakwu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2iinfoakz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kukpdnta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cmfojzlu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kptqcxvq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvxwpubw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vwhmlhac.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zqnbixeb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zdrjlixz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xhwppnnp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gafwqqzg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2likgmwso.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uquqtkwc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qayluqdq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ktpfvyky.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tgsxuoeh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xurdnxae.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aevxqxwr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xwyhqpqp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2yhklfege.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yexppbuh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dpjzblki.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2crlhhrnl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kugjspyt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dxbfpqpo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mcmisgdw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2contsdok.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qsjtmplc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lczwefoe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wnwefwud.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sbcfelml.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdkjlzg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zsloxaoc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsfbpeg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rqwrojby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxdejru.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnjinyza.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yhjpnbbp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdkvrfnu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rrcrezqv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjruqenp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2phrnufxv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lgbmdfej.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eneoxqux.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jydhjfws.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vaiyhsfn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wsigpgsq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2svgxhrrt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dpwxhtjh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jzkisipz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wjzuzzxz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zyypbffr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qnvqlree.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zuocgdkb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xtvczwdu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2urkkslbq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2miwyqiew.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2amawyioy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2axfphgyu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hgbmykcn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hbeqradx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ezocsetn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zpakdyoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlyfbdim.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkswautn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezcbrgwg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cshktwhl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gozjpzch.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nlmeizef.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqlktwpq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2oxpansqr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2iijgbxiy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zfuozzya.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rthmmclu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jppdppvn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vbhhigpe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ykrhdcol.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ziemvmwj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ifsinqmc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xsbvnfjy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wekziylb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2bnueojhu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wtvnrire.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jkxblfbg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zwobuste.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dwvbwegj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kvviocfl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bewcebwn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjvyzdoq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkucwyw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hgidgenv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vbadkcox.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2skdzwsut.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ptowckki.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ounkfrhi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fmymnwem.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvodox.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2texusnou.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yqqznfkn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wyryvdki.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qbzbeayq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2srnqyupc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rthblpft.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2paqmnura.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kbssmlfn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsajbkz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yeijjmij.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zsrvwnpa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dlvmvgcn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ekjqxrwv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ogctfxzv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pbomineq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jujqgsia.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjfdwzc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2imiffuxx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2frmbmswu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wmxmfzua.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2txutxpov.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jajgxfzs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2datothyj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2iyilnynj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hdnldzso.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nddwyilw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2oinscyse.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ypriglnj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aalbhuym.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2amboekoy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2onccxoex.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lotndibz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rbenzlol.html


<!-- 参考信息 -->