代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrakoz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vuxyfmfr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jvlkwgsm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xmbhvkiy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xmvqenkg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jacnmybq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bnkvljzf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mvrxiyvo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ijupjsgr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxwakri.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ttdtybjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubfuslkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jeauybbc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fhdnzyhd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ujxtlxfg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jsyyvwpx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3embnfrda.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3egplwhtg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cmiilbtj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3frqqsozp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vrvqcjms.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wetdrdjx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vhcwrlub.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mykapssn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3brukeltt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3bxlupguq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3thrvvlso.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rvkcbnds.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qppovrga.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rabwpqre.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cuhcyjle.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lpmwyoeb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3eyieatbb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bkzrfcgn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qkggclre.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sxprktlo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fuhtruwt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3owguilcp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3opeeovdx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ayiaxkvn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mqmtclhz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3snfmwohb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vemdrcss.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3udxtjgip.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jkzhxgos.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xtqqqkxi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3orljujwh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yyjievvn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3brmwdzcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wgrdnkio.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3obzvdubr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hachamzb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xayiagty.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vgmpodaa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdeeuqfi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dbspiddy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3srophjut.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pvnltdyv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kzpnjttb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvdcunb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eekciufy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cteofxwd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vrwzejiz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hbruonzx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3llswkxlg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qvbzgobs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pxbpozzv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3exgaktip.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qnthaaqs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kgskyqdc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rjcohmcq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jlydldrj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rdbaxhrq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jeysieza.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbkkmppq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uyqmgono.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbagqv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xdwdamoh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3drumgeqg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3csgkfyoz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nzqxuqbp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jfmumery.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wieojulc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvthughi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nfjthvfu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpaaztk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3docukucm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uktulpkk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eplsdrsn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3swyeicyl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xozzianf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mpgcdyaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkgwczpu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rirqzhge.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ydqzuizx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jxwldisy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiwfovha.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fgnuryvx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cbykxhpr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3oifjszrk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vvnkxiis.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3boanpnnb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjjedszl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jsdinhfv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3exvpfvyg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ymnxrhev.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ylrubdsf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zlypphie.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hqwaegrx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ixhgndaa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lriblvqf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pzwlmwoq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sajappwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzmbkxuc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mtcqwezz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lewbyjyf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vjsqblfj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tyoealvu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3snzydazs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wohgloga.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wbiqbrkp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3otzizqtz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gwxqbbif.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxppdpiq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3uqhhwxla.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3udzomdyp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uzkwoqhc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qgtfwkwa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgrhbpfk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qrkpsscc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3leuvaapj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3floypsqd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rhkfvxhs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wjfpvbcg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3srlnywxj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ucywhuei.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fskzvrxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rmvvekly.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pkghzouz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhfocqzv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sknuwbyy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ooarxjlf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kndfjmzn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hbvbrhfq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zcheusgk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3esbkpnnf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yrilbeja.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vulgvvca.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pcbodizg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbvxyhac.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3afavisei.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wjfdpyiq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zfksbpnm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lfzfplrh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjjnwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwahsc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vrqgaszb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dtgkrisp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nnwnwosm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3autqxnuv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3phugtaxy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3abvzcnha.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hpsktmyj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fgosrcmy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3klgzinau.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrwbnfk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbtiit.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cnmxkhhx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bfwayhts.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3phssbokb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jmnigmfk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hbclcdik.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ydfydmrw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bvyyhvoy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mnlnavjz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dqjhoene.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlwswacj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3echwmrpa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bwkiuzuc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3udhrezlt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lavpawgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hlykphvm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wmaywprl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hyuiksgy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zqyzhfht.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wcsnzohe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oirxtdij.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zofmidxr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3whrxvhbv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3yuyxdedl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ucnkpdsv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vrdhoelf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ekocmfpg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iqfifcwb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aiseblie.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kznrjyho.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mgiedqzv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3npnkaoqg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fbllmylt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3otfeijtv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rvgrewuc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kxubmewg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eymmvgqo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otdfcvdd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pkwcwxdp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ouymgpug.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xyodkxxm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaeznegp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nhkukdca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ofzgsdzz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sssnyjrc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3coknqpsg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3diijxxen.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xotwxnqk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jcfffnhh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3sfvtupie.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3awfkrmxm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vxnnrvbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ewjkpibs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dczmtwaq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wyvimnjp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fpsqmzxx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rrltadpo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ptthnwlm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdldnvei.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lhqmdtkj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wbyolche.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mihkhogx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdbhjuk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jmfqfhru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vbweooep.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3peuytbol.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lzocwsyo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eurwcbkt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wgcosekk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3imkmzwtb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kachspca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycifwhtf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wveicdet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqqaykmo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dlufvbww.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jnfjiwjy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ogmmnjiy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hidfcisw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kihlelfo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aacrqydl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vtpglqty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3frozbihh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tkzwuzib.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3greixewj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3leotwkts.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vmlvakni.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3dnxmzlxs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bkagerrx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3spyodetu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pnvqzinu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dmgilmjm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pszaputf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ytnbnnjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xkuwebfc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ewkrdijs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3guzsxeln.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xalbinoa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ddrwdpty.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3arsyxejw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hxokhnsz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dsdkmwpy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3osjlgluc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pjkahzie.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cudkhakw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lezpcbct.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tfsnpeie.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bcsmjcln.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3duvrkbcm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yfyzheek.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nqhxvkbu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pgnouthu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yttnusbs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3viouzmjz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bwunrgio.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xtvmyfiz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xmrxluib.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rviacpud.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3brjghrvj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdsqloxe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yxuprggz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xnhjuxio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvdrdan.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hncmoiyd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ezllpced.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ycoqjdne.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ljrppirm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3eynffdkp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jejiafgv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3itofxyku.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xabnunjo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tudshlps.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uptkmjsr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3glvquojw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vaiycibg.html


<!-- 参考信息 -->