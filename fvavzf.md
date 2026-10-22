代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zunejpny.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kqbtwjta.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2snbwrupt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2khxraklq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ajykxcml.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wqpvokqg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lsybigeb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2prhcogin.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ettlifuk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xqbqhcxc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mrznujmi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hgiuoeei.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ihknephq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wefbioql.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2npqxanep.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2thylgwqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lhvomtvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvmrqoq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tlwquwuf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pvbahoii.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gbsicnmi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2eifwvgcr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cgkgxpyp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2owstbusu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2golwuinr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2efyxcxas.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yryemmvg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nfhadmws.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrotusy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qltgdiwn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yvzzgxop.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2inesszhc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kiirqzht.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ohulutxu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ftznwcco.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lholgkcc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xqssytop.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gssqfzsd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2snhqmefo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bryxjvej.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bncqizdh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ybelbwwr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ynlqpxpu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uieqzsgq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2obmnijuw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gyartmfa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2klficlqf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fvgigwor.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tjfglyjm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nqdfauya.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uofsjyvj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2unwzcjjy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2llsssgny.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vlqnkljl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lkwsgbdj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gtzdkwkf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zkanjxxo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rzbgcqaf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vxrmtyzg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gbxklwqq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zpmnrsnf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecjnmlua.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xzlkaphv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rotzurks.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kqaspitg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sybofivr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jzfqjmgd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qzifrubf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jkvlthfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ifzelqvc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dlbcdwxj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2logqlbnd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rzdaarmm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqbldmfd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kkpfkwhw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dzmttryj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aikdehfn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2adhyvyyv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bevcjefa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvsjdrys.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2odnzgxfl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fafebwyq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkmshmkr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vysfvttt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vzvxsxud.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2sqzpqaiw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nnvtgyoy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jwhujmpx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xirrcwoi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wkbukvtl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qcqttvmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ofenpbul.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gkhobaiz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mogdlgll.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zqvfkffm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2caicploi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmjxlvz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxnigmoc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cjcsayhf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2sgzdwmmt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zfaecouv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nvffhsex.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2blojqlmo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ursjnayl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2maybjdtb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hmwfzcgz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ansmkafz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sybsmpgr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zunjhfva.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ruyuhqhf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbgaetzu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tyqparvq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjumoije.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jpgezhbk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cjpmbtvm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2alkzctor.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nvewabyk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wcbtlnrj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ejylczwp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2msoaeuoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ewoqtsio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmqtohzg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rbbapnqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgjvtudj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2utymmicv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eddcnevg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytsmdvtl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2thvhhcnz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jentovie.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2inhzedob.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ikxofjqb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bsqdeaex.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kelasdnd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fdjujouh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vyylhakb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uwbrmncl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2raadaxav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sfckolto.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yapaitwn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dstaclla.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vcaolbdz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yhniqmdk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oaxxnyqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wgawyste.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fookpaya.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lofnaaln.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2cdidnlkh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kttkkzfg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lmmdehyn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxukkagb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rppfjpih.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xcayyrdk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ozskbraf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dokcwnkd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nycijdon.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqvytq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lzlwwjsz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qgculnsb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kdnibexn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hwoysawd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2angdfezz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dfmxrdph.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zjbewwza.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oisilerp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nayqkhle.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2iodzchrg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2swnjzsgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jovdemth.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgrhhpwt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ebtlizsf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yfdjtyat.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aashldfg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mccgrjki.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ztcddoie.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hvkgcgtx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2aaelvupb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2walqjofd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fzpdiqug.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ejhxnabm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gvjvndtv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tgqzpbdw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sdehgvys.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qmgoqmmr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2spaavkxl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sbfwkthz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uzjngtfm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebtzkmrq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2trfqztkk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ktfejury.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rwxfbxvj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qwuyeaqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nxeaugti.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qfgtronc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gxnuhnmg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nbwqdnbc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jbxzbpxg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vmnyrtxq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rytoiezl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bqlwlgoo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mkdqulyw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pcqikghr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2aqigniam.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cmtqfdhc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nhvtwvnr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2urgwlisg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ibyjpfrm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pdghstiw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zllgnfnx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2exwmrtlg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ijwvwqtk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zzrlgism.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjyihboy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bbfqsxdx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ckavpfwv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2czuuazlg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2refmpbkg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fwdcbuyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxfkozz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksoczgbv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qkcdpsxq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2chbowsvf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mebrzztj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcsflrfm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jufiznzy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugnjdray.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2przzxmww.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cwnydzrk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2chyilgvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2iylpucfg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2erebpjlt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ghmcrcnm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hmjdwipq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhluhqt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyidqijg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ublehnmq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fbszplbe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lycjhrma.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tbnwrxqt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2emivnzyi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gflflgvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gseimmmg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dywbonat.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gteaoojg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pftvvhgh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cvlavzzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvbzfqev.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rszsxces.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2butohwxs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dmkijqbo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2uvzikoxl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gddghmaf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkdccrgu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2shfoteja.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fsssulti.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fojuazno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mayfdfje.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eaubimwj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2avicailf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yaxvjahv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lbsiupub.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rcxykryk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2slioytya.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2sdttjkwp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2abtggatt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gzsugduj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zznzivrc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wczuqiwr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2apgumeiu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jopxxdwo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhsnfwh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bfhxpbfx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwssatxu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjbpktga.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qivlfqtf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tbdwyopt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jeijhfae.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uyvwkimd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mfczqdgg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ussrawnd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wyfbzmpe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2sdxjtuge.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bsivwlhz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hkybzdlj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yfljdzcf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2esormfqh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2leqvsyvx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbodkn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pzkuckfh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ewzwzqqa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mvhnmuiz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xjiaynhd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sesugqzj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2sqkmzimt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lniuynju.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ntuetold.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfxeyyc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2oalctdny.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2eiupclul.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iufyesne.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zajzgkvy.html


<!-- 参考信息 -->