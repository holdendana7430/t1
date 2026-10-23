代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cnlpoqmt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3czmhkqxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uymkikdu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wkcphvdt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzbtoet.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ncihkrfv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xkarzopn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3afzjkedf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jsakfpho.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jbypkyht.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xtabftvf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3boecwpal.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jqzcfwwd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3airgfvyy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qelxivlb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qajxzkcv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3exevnldo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbhkozz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ucgfwvjp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3opomflun.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gngexoap.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gldtmotu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3repkszkb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3azsiolgd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uobdkzvq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rnihakve.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mupbwdwl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vxogijex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bmnflyse.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gzremnsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kvsrtjsw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3umtzfljk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hbxobias.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3oqutnewr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iaeinkbd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gxiqfaes.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nywarxbc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mndgfghx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wmqivxoo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hqjernql.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cgcuxnhs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hdjhfkod.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hfgwtbrp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3anyrrmct.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vvcsyevj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ndudulvi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ipdufvwm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tfjarstb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uktgexbn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ilqfryjv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nfjxpvcz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pthjkekh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lhktocji.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kinpapvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qvgysoly.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nixqsntw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mwdnlpxj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vzhupgku.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rlsprkwp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3miywrpoy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qbyfnpfi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oghianun.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avnkusxf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3codumytw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3trzucbeg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dgkegbzi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ccyahvcl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzztvpoo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ewefaqdg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkjbzgzv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lcoayaau.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zsjltixp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wkjxjxiy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uvvjyjdw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ulnxbnum.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qoojozvo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yebvryie.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hccywuvj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3duddkfpu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3chmwwfmr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvawawdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pcvugrnq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnzdcphu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wxrikefq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rvyuboce.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oekmrbku.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3czvbqbdu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwrbtzro.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3krzezsmi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3heqxwfxd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wraspejy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3irwqryfv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3emkvymmc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgtjzbce.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lssqlrjb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dhetjuoi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzutncz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dnqqolnr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kvayoxww.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewebqlmu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eiyxihcr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mlmoyagp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pseigxvs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jzokktsk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nlbhnnau.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wvioyoxs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bkpumcvl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rjkaiior.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fjbjhxne.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gxgohjye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3paujecqe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ytwpgaqg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpeflucd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3eoopgsil.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yhejybib.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fxpxkcbq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3iggosiej.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wemwtucb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dqirizhi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mkqgbjtn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3itkobjte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drobsszo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tesaycpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eufzcadg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xbusczkw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bzhiwenu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtqhoocg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3drtiafop.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qivoevon.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zamxthkc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3czwtorms.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uqilfsue.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ysigabcs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zlbktuyv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hkglflha.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lojelogr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rxrcponm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ngzrpiaz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gqcxrgbx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nbaqfzlv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mcmtjjry.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fnwpwkxk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cyoytsjn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fqitmdjp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rjmxgeph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3deetvcvp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3udvlyruo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jthddzcw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bkqzctlt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mwwzzfru.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3npqfkwkl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhhlknl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ohgdgxfm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ciezigef.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifnlrdvm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mixhqipy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dpicjxov.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nibtteck.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vzejpkci.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eicyzyit.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xccppqfd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxeiidei.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3exqavshk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3eecpnuui.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jmjvqbsx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rjyyvbnb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yuoeavsj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3alddabfq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3noirwwbl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wpxezgey.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3azgpebaj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdnxlztb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3thlwqbbh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rgaycanz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zapnphml.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3disdqtyn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hrxvcyfl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xwylfxge.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wytkqejs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tylfjxkm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gmmwepbj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bilrlnkc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mwcboovr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hzojgfbu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jppqnwga.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ypmhlaeg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dyyaarsr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3shxotvhq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wmwolnih.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jooheivl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qkquxxaw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lmtffqfk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xnwtlauf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xfbckffj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uhjqzhgv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wczaiona.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vbdiozbi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kfikozfj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uokxtezp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cidquuxp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cxqdjdql.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gutrmfca.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fkztbqhu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ikbvmmco.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzfuqtmf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3omwfmpdk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nuhisuoh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qjikyccj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3boczpytg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qfupptgo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dggurbad.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldapbuln.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3guznspnx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vvvnfzfv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jnggojcp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqjnffqx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3npdxfpiv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfrizox.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3svpoolje.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lhjkfktt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wipgyswg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mlbcjrzc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wvrzacvz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lwcspldf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhmnaasv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzmgbrta.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ushisvnt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rdyrqemt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ltsnldiv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rzpbuhjo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ygibqxue.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pauvckby.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gjgqsfgd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lovakldf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3urwuspkg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kfqkbapj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wwbfljzm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3knmfwuro.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qivmeivx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dhagqbcj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jdubevjs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hpjmjjdk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kivjatpd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3foxdeljs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mwcntqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzfnsfbl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evtrxdhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksadkuyk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3eptqxmbc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3axsltnhs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uhishbqo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xfkmygsh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dtvamzug.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rqvyfewh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fnuvkktj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qhjnolac.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qjkdkgnv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ubvrrjbm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xjpfaknu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pccdpfwf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wpoiepco.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wobtxenu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hrxjxgob.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwxscn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rxdzajjx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cwklawtq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ptjfdekw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xbpikhlg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fdqyuihe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tvveznnc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3khffrabv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnriboku.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ejxhjtdn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fteqjymy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bilzdvoq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xcevviip.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zzqcuzsw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fagjdulv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ypugibfy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xcgrnopu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3anyqrtxx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hpxcayag.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hlbtxkih.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3czpgghmm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3srtlnxlo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbfsxin.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ovoikfay.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3soinytpj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3earqttay.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gcmxejqk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3clvnsqxk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vbxysbmn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdujlwzl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xjokclhd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bwwelodl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rezusbrn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sublwyal.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hmsuzryn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3bfbxqdcq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ghfgnknc.html


<!-- 参考信息 -->