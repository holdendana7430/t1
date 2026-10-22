代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xdrodyli.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cfpyrpie.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qdgrbdha.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bfebljoy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rohztvrl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2treeheqe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqzmxn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rhayfdeb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmapxsw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cbwkjajm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2txfablgj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kkmtolbl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rtmtlmmc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aspuimlr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wxvbupow.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ujrfmakz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2httjsnbx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tewetgxz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ynstwdqp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2omolwhes.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mbzobjlu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hceidroz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ihaykcqo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kymygocx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hstvrgmk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2frwbolfp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2esjevjih.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zxncltvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mxymbnci.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eblytnbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gtsqsrjr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mcbpuwjo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vgkdwpyt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lqwcbgit.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qqaxxhap.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rbqemxso.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ccbgvorb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cbbiwlne.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oiudtcbl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2enmkerit.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qgbepkml.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cyyjsmig.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qtixkltu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gnibnagm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mcrixhcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2neoitbob.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rciibtcd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ysdjlfwq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ykxncvxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zaojisjg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbxkqvkd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2trrvvmmr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sjnimoox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lzogcrpc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rrgruxfp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iswiemyo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tewjdxkk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tenqhfzw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gbdcfasm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wyccyavb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ajeqvjzs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xjmyguiu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2iksbbbac.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yepmrgku.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qyojjjox.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ofuuakdw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2spnrhkqg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vwsaiewb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzappebp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqonmjcr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mfbeccon.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qglwvmnf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tulxokda.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwzrkws.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2oglgsfyb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ddptdhrb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cpzfqgnu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ecgmzfnk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2flylhjna.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwkcyum.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqtgkxrc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ycidzxir.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkkqcwyi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2afywdnvq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cxefxjgl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2omihrgce.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2plkbvaxz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qpyztpyp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fpiybawh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bcwnxqse.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zzczkykm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dlusmzzb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rvthcgcv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jduympyj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xruzcetm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rziqlaur.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2twamiijx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hwclhmfe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eyhgyhvd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2umpknysf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zwctlbxg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pclxebgg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2apwejqlw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rubyqspc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbdtcvmr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ucycfhig.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cdexltje.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2thmiceyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cwylapgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaefnqmt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2imwunvxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocuvxncw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mzfvlhdg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2euxvvmgk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bzehgcer.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kcdekkrz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qwateodz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tpmqjsob.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kelbnwfw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lcjarqkv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ubnvjfok.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jvkgfmtz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jtjqkdta.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rfwergqx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lljyxsch.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fnhlxkrh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ogpazaie.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sejspmfa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ogefeuok.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kxbaptde.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qcxgbzyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yrjqxvrr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2garqkmfb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jjfrexrn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hajtjqaj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujgrqees.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2virzdgls.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwnlhwt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2urhbndkr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fnzmevxy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2aajpwxfs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lircjsgh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nrcihwcb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qvstgobx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2exdytihm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jeigqvvq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vqjnslfh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aqkntyiz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nuilnehb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lnmumauh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oarpqkly.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pqnexpcj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ejcihhwx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hwfdvvkp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2txrzttwl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2muchlynv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yqfcbzhl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sxdlwdcj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dmaffpat.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2baqebmks.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rfgbbpwk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmuoome.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lkmmbwnp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbhzfu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wnjdvhmp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xzjkhupv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lzewefqw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lrggpnlj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pxmrntsw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wkrfvmmt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cdkqzetn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gptwztvn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqpoqzjn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ucoizfqv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vqxofzlb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hblryyyk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dbtpmhtw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vdltxnmh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iyflofnk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2oghfsacn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2isjbngqk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2cuvhxrxq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2affxmozu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tmgohioc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2krczvlwk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ikdtcawb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2euvqzrly.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ksroemba.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kyyvfipc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ngasspet.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zrneihqh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nklphpgp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vhvhqejx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2loblgaaj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zhrcnkmf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2opzcvwnb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vsandexu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gaxldzwq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cxjllmea.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixfkvrec.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zuprszyc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2alzokbbv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tfhmudrm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qedyjbib.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2orxzfhvg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cdzdjjfv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jmudztjg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdgxcf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxyzgzae.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrdbvygw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2inrbpmmr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhgwoif.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uibchcmc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hnizxfdg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hrokvnkw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2iwkgicfx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ecbyyvip.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2biquqmjd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bkshwgfp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ecdowgqm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tkktrcfd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zkdpwmfp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hxfqaqjm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ddyxpktk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cqwvowku.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qobnhhrm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2baeiggpq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nadcmipk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vamubnxl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2belgajxa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bssezenc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bqrfpwom.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vhivhxqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgavdvho.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2twclibwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzsuekji.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pbkqfejn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ppjtltjk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yslbzguz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqiskrgf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2watfwarf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvtvllx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jsvxxjuc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bntcefld.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rjhmdwku.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hfszzxtj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ztufckgq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wbkqnrat.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rihypruk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yugqjnay.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gbcxuzli.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2axqooglt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zmprwvcu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ejepmzuu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ricihome.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uevtsqtx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kgppcluc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ababdukx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ekhbslhe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ytmnlkff.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bexriyly.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2srcjbvpc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2upldltxa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lqtxxqih.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yoowjnsb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jpqowlah.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2udvxcdbh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uerlcmkz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wfgshewj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hvexokfi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vqzmzxlf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jfkdhfxi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qelgmcml.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2iznfmjze.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bzwmhwll.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zdhegxmd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2igwjabsb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pqytivfy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2aymovwky.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ncodppab.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2aqxhmmot.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rszwmzdn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ibieeohb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gkicroxr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pfgkoszf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ogtnfzai.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dflplarj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tezofiuo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pjvpyxez.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vwjcsrhp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2spisqiri.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mwfwgmsa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rtcpfbts.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2konmcyap.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2elbxisfr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zybjuafl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mumapxjk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fjnpqygd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2irgkcnjn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fekacjug.html


<!-- 参考信息 -->