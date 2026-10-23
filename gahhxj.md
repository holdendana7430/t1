代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zuzkxdwd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oobsrwrn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwzzcbt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qxtzeadt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jozvezvc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tyuhhnmm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rgqpbaog.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uweuggbg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ixyrtxrx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hbqthywr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rpqvyotm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3msonunii.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3snuxyvpe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cizvoffc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xncuetng.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gavjszda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xgznbjpd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wxabnqbx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3luwwsbfn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3omglpkzr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ylekrrhl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3onfljjza.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3npqomohk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjittjnd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tgofubbp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yutmrdqp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ieowpxep.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hscvurfd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rhuecnja.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3axjgmutl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bgrljoel.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fjkzakoa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tllieazt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsplkmis.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3brwyitit.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zthrwumi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ffoiuwuv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nfbpohax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jxqnfdht.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ouajtpld.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3opsdwfrh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zfgvccso.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3assgfokh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3agorxemh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zbnzwfrw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yhralgoc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ptdcuezb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3coukvfzq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bgcitosv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dpfyzyfg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3boknessk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3etxbuwwb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nagbfwll.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jwqydvad.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3anehyefx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yausvuem.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bstmhrjz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cynaxjya.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vfeylutf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dbzipmaj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pbcxqkwl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ufklwxae.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ckdhynrl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqkxmxko.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zsurjrse.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gypuhpht.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hevxxkpz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3klawktkh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3heqpiovd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ijwyjxzd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3owxcueij.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3emtmwvfd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fqcbzfes.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3odkbpwsz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tdiyeaxg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tdphpkgn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tfvfhldf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gmnzmlvq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lbifstkp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3emmfibhp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3brfodvwp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3otovgxog.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wwidipxm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ykmqibrw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjhqhxcn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3epnoheyc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xekedjyr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dlppazql.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mnexhhzi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ucmlawes.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hnrpbgza.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3omxsuylt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3unpiwsak.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3holernaq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vzztuyiy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ayqvzmtp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cizpbyzs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lcabrouq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnncrlsj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jrblxsmo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mtuelfim.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nhpvxmlc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3felexowt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mjtvfdce.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdpfzlkx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jyrjcvrp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rfvlcrfa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3llgewurx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvarktl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xpylejnz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zgzsmade.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ezfufsvx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lzxvjepu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lmqhcynt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yysqcclt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gaoajmuz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugspsbpc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3crphqqix.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ghttzaon.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fqwwnavc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ntcldvex.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lqpbsbog.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3udhwlpfj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fegyjjri.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cohyducu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxqshiqn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ohcerorl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bycrwxao.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvtrqzdj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oclvusti.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lgsknmux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kepzvfwu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yjqoknxo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qrrtqirk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kjufdwzu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kwdnmhtq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vlnwlyub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3raoxyoir.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gewjbolq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzwfste.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ahhgdurn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3emenfkkv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3abwqsoth.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tuuymqkk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tbylaxal.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zqepqulf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rqwjbvjm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fvyrlzcl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3daoebbod.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jxmhcktp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ytuiflkj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdcrtjoo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ndhfmbry.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ksibcuwu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iadybpbc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zacmwrqo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lmahvtpk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3husvolnv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqwacrrj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tgwidzfi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gleiczqv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rcqfefvy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ydvcgcca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mdyqaigj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wbkpnwlk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ycworxnf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ostrxagk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbdrdrk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unxuckcm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bxeyvzgf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mforhnto.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ubxzswhl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubooleow.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bcxmallx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yaejnfun.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nkxtlswu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3trgjhxjz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rpwhgvtg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nrpwgjis.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nzqlhivs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvrxybyw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ychpxxvy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ppiftlhx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qurqsttq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cuabglbb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3netvbwsh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wzgulocb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sqstcilw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tqybkbrc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hhkvltpz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lgnqksks.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pqiiksyb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wwcwlorn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nrglvshg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zznpdnem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3akewbltr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nnakktsw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zzynujtp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3euvoaiyq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zwookubt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qgghhezo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eurqglam.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tapzeqmg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gvpwadig.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kqeppflb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qrsiuukz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cacttphq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rbrqyaeq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bhkaponr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wfjiksrr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nifrlxkc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uuoguwnw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yfqjlxeo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3laozwplt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jwwonsyl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mognnokf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rthvayyx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcxrloc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gtcrtsyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ykmxnzmh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ookperub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvbmdczh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zalbjeji.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hvhmhedr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qskqgetd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oshazgvl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3njmykkta.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3muvjzjaa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fmqsnhaf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwlcepjd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ykorgnse.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fizfzcge.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3uesmzvao.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oppfvjwa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3elsahwum.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hgklmvsv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3znaakvfc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gpsueghz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ovvwhqjp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xcgqbqdq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3knkptepg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zkpbhxma.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ivvfoveb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sxouieyk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jlxbarab.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3eakqwohc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzrhtcy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zyusnrbg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ctqhvenn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqohkmfr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuqanqlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryxmhobz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tgpsbidk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mlgzixom.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vzxavlbz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vjbqgzmv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3evuiuzpf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3aprmcais.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ofyomtem.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rgobmihy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3uhsftcbg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eczaoojo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uvichlgo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zbbenwgz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ysszjfew.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tvngfvdk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3khrvaytc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3klfcykko.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3cbfjjnol.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zceupiyo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qzojdral.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sshvzhdr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3eorincbl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjwrqkt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dbnawgbw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jfufyeiz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3byrymqha.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jdchjixa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rpfyehhn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rogevpda.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jqswvlos.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3znhwezgu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kektapti.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3glgerwhi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qhybunbk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3amcsycck.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mjwpgbkg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kkgpgveo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zjpvgvwe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3idbizxob.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lfuohuuh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbbjrsi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3trtkxjnr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xbstqxcw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3efzojnlg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3eecgukpd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qdntserg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lelvbzda.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hodvhndm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqvnqsr.html


<!-- 参考信息 -->