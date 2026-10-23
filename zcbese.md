代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jjicpcng.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vwtmbcvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zejszyqh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ypryjwne.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkdwdmz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzgojimb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yirrnzpr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3uimexwad.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lhchqxyv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hnhtpabh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tuocpjrg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xwjmnstj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3czuymujn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lhxxgfcf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3inqutwvy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nfjkhzav.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3buucstoa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3imtbhscw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3slsnuufe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vduizxce.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eypwepxy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3scfzpcde.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3etczgarp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ocqbtihe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hqalempw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eqmexzjn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lyktkwdj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gvusivjb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znycfkik.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udmtmuvf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rksxaend.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijjfjoxi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3glpfnxlm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdopkydq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eigjduij.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eupqkhpm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrupkkw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3oaekfkqy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ryeuqeuq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3stnvnlsp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3haupkopz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ltzqahrn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ltrsywxw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3aywadazn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ynymoqqw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3andiewfn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pfyxrwvm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fikxjstk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3obqkjhyr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yktgxkql.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjjosq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jpzrzfio.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hevuiivq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfgfzdie.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pdqzzkrx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hunwgvxf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ucnqukyy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zgdvdavi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cxykixwv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gnlgkult.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3owwttxem.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bqkikquc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjllxlmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fsrlqsax.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3thzmeivw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewsdknff.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3snbcrhyn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3croehzmi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ygadsuez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bnnvzfke.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dptergia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfhfonim.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sniieurr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eslrdfjw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dhhabuou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uefgmrje.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uvjetide.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xxnlwpoy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdqrxieu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wesxybej.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3syuyxbak.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lzobzxgg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wdwhsmte.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nglevuiv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pyxoxvmh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hboavmud.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ckhbkjjk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcyaxmay.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uovvqwwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ubqqqkno.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hrnqjqrj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qlssiclu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rgicfnio.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmbnjfy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3odqzdztn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cdenoxol.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3inkxjfqp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wojqlowc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3icbxmyos.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3djfolydf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwsmziik.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tkmgdnug.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3msbefjoe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yefxjvbe.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fnpdrozs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uoohehyu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3owbcwbfl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qkrbnnrt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fgdibvdl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bnxmftjo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvzctub.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rjgvapje.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3poqdqgua.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xgqeyuhu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gehxaujw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wbxlugwc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lmejwtyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hgdaxfcx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ohfzwgni.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3iokogacx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3euyzpibx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avkgvaxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aictysxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xweotcna.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wuhjjnqv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ljutulqf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cmkdrsdl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dpnghckz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3berrsqzc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xnjcbifg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fikkivht.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uhiklpmb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dzrancdx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nfrrawqq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lucfvvlk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oifoqlqo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ceceaivx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hqvbafnw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3aatjgveh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgphcbe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3trtdaacj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tihlcmfn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ndpckvwo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cfyphrhu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tcknmvts.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nbfcjlhr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pjcmvdka.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tckqqzni.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ufnfpcpz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iekguaco.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lgrhvhca.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3scvrqkcn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lpuhojqn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cijcbokf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hrlqomvb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ulhxtvwd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ryfmisfd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rjnhgtwe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sofvclto.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mjpixnsc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zzxcvryp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wxgedxrk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xfdxusau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vbygqamb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ldikuzxb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtkeefva.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vximvlxt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ftutkwvx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xafnevus.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnrduwa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sgyrqmmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cxcybdkk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3suehjpgp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lbolrszd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pqvracef.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nghzlwtb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uatztleb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bwtmoqwy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zbrdotvr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxveweu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ocuhgvbo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jrmiktcq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ibdtkhoz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qfsqeqql.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypwvstlf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bzwtomvq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vnudzyog.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3easvafpt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3onzjzbhu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cbbcttsw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rsjclosy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kdxstppt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tdmwxeto.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qozhyufk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vohzqiok.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qhpvzdun.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iatqhiha.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rvfptcxm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3khtixqow.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tnhboysf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3stmuwaxf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tcrohptw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dptblboe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gvtcszvt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnosxrpp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fhjhlxxp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bktfnwsk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lkfvyogt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dvpxekdk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mwevsiys.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpestgjt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qivazspe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vgutpnjw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3abgvjcgx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pibcrkyw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ykfpuktq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vqtrcdwi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ecqhwjtq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lrknbrnn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vioonmpu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jrbppzyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvujoatn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tdlwxuav.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nfnlypld.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nbycncxd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ulgnzene.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bdcmmyby.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pmlvtlbf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iqzfidme.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gvnewoef.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wpunrfaz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ihghepgt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcfpbvh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hproptse.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3icnxpzxq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jfuzprzk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wjebynpr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lpogward.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ujthznpb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3keoytesj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wfoogobj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fxhbvgao.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vhihnbfl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wagphfgi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ghlydtxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phuuumti.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hxtnuygu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrhurdsc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3emheaurm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kfewybfy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3crtdynfv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktxiaxgn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nrgtddna.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rkubtvvn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yqnvpzvr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ugpvyoda.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gmgwjrvk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mxyclhtw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ldtriahz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vgisaxsu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nbbjoxwb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fdqzwxjp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ecgpeswp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fnkjcejw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3detdwlzv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rqijyfvj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zdwzmsyc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3twpfusho.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bibpwtpc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3avanyqou.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yoxbqwcg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jklhwrxz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hlvptanl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ynkjkafz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vxmobqfr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgpfqgc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lrgnsfbd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pomgmjbc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ysutzjlz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lscvldio.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kwaroqgb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3npdacabb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fttprvmt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ltdfxxqb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3alacrpwq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uujnmjmo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mhsugtul.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ggxvhwgf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hrbnrxds.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jgxqiawt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3geemrqxk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kmjirgjf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ehuxiafu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3nhyqxcnc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sdvufxvv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iysokoxg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vommujuh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3geavahxl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3riumdsyk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mopegfod.html


<!-- 参考信息 -->