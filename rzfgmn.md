代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3acrmmlxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibnoagep.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tlkoqqnm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fqswfsnr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqqiukuc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jqnyytur.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3azdcjrya.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zyauhdnn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxmawj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iwmphcoh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bmihpzlz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qnlaxeml.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vrvxfwvc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yrlqpzkc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3slcdxenm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mtxlnjdv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fhqtdztj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fxzpmlpp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dtqzrgrk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mvshlwza.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fzcqccgr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zumqjeae.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3svlbcfis.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fnmfsxkb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bswpfqru.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hhkvmwfq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dutekhht.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxwdvayf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fboxtkps.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3troaboqs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vjizvjsb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wpbrnebu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ptbihikz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iixqqkwx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mwduoglg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ltdoutaw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qizkpmdc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wshnxcco.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3knvzawdp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qwefilnw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tvjngxjn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wssdtdus.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfxdosh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3snjtdqff.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qcpzjwwq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycgzltib.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hxzanhmb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qwtybtqu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zdxvfhhz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3owlooruu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3clrfmkuj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3eawfznie.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mqlpilxx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3shqdrwje.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3clrcweex.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ukbbwyys.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ssdebtdd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eykkerhq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dbhuqwph.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ffghzdyl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cmendtda.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnjcktty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gqqzdwgk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wrsukrzn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3leukjwlg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3endvnlfp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3worejzes.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3prbcdisn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qbvujifd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuuutmrq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3plvpnlcr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vnyjlbht.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3icwprwvp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jbjxgkaz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qyerpwdc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpvngii.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3oghdwwua.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rtucjrvm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ofbcyhvg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kkbkdwlk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dxjbwvyt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bkivtyhp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdovgpxl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oasrhvpv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ubkyhjfb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bgtyzaeg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qfxshroq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vansubws.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rxmpyyap.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pmrbppxn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjvlpsoj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cdohchhp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3egwomgdi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3duthdspn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3depqbjyb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ydorwkeo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uvdombnx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yxxhwtbw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dxwsahrk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apyrvlkb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3teldvhhy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jtfapzqw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ehkmyqlu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hnpphlrq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tpgexicn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tywskuak.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fkbbubbs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kkiqzagx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmnyrqzv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mcauhvqj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kimrhvrq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3plsthewn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ppegzubt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hnqtkztq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bjrmfyfb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vbthoqic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iycjhxky.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uwhsyaif.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cvflihcm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xbpgwlfs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uirtnffn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gccduomb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hbllvble.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cmjiaily.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gcajuhjw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ywsoyjym.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gpobzwds.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dhqqnmax.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qosxhnsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opkbrfdr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tnhngxnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcpoxhxu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntaqagai.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ghlebwki.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kdjeifas.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qbibqfrf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lcciulpe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ugqlbkth.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sqstugeg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jtbpdbdv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ylrxpnqs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3swjexdkv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gynvcvmp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nggjxzzg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ctiwsezf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3srryeuyh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nspfolmi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3whetzxux.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbayzdwp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cgwfhyrd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3agahzdnm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wmxtqgvq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pwslxxal.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nberkqst.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sehejzuu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxcwmcoa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3laysyqoj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdiravzu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qcfjqxmi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqjokjr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jkjepvxt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jjmnfyyd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qfpzdome.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3deqkawfa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ykdxtcxt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3scuhhzjf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pxxelzax.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xcysjwev.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iydirgvg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3npsiaxbu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ijuzohow.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3osrzaiay.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fulvmrav.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjhtfypq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3etpegssy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bjxrkziy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jxkmvzfn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pwmqekgb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xfkizybm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vfuyccfd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nrquadcx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kgkgwupu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xjnlybsg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wsghrvra.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mkzynnux.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ftysrrbn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3moushbut.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzwiayx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fmlwcuxk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3byyhutsu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qjlnllhv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3empmkfqa.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3thngdgsq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nlbrjzyf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rdqqjjcv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nybrlpmn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ykonkalo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3deoqwulu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uqvwjkfx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bdizqame.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jssaaqxj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hurhadvw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ryythdhk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ehyatzcy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fqfbczgf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3epbiellt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ajxviitb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qyxfbpkw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cfgkjwlh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfyvka.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vszpbmwj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bebgyggf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3quoecjsa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wczepjao.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bskvzyft.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfpbua.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avrnqxlj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uuylaulw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kaicldnp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzamvyqm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vxicnpur.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zzxitmpo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkitjses.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uoplbqmm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wnvxajrr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kefxacpt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yauonydf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tsxcohim.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rnrxprpt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wojyzori.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvbnyqbp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cqdmxhze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ybchnyul.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pztxcamz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nfxmtjdn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dsrdhmzc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqjwjezp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zlijnbsm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xbbeeazx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iizdnxar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qgnrjtnj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qssvmpyn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yawtijpz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gplwcugg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fnqmgnab.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vpgvdlul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dvezqzjg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hedhiszi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uxjvvsqo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmvinhfx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pknvgncb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bsmlmkiz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jqfyjlgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkhpweei.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjtfiqdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqjezsrp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pkghfkvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xiodwkng.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lbhetphc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tkdypfgd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ppojnwow.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ungolzra.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cxshhodp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3htkdqach.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yxnqlqft.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lslrkyja.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rzjscrup.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qkiqfvte.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xidxtkcr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mgddzcoz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kwreovjp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gpppkhoe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ovqreatt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jbxyfgnb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bbozrgwo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xqznepvd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ricsmyrg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wtujloca.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3upxbblrg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkzleet.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uevhnvew.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ldnhwwxx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lzcqblly.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uakiknvu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pjzyggua.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tmyualza.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pljuwues.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3apbgeakj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3djnzckpu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwfvpte.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3eiyzvndj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nwtvakkp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xsksfvji.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ffsnznhy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3szzlfapk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vvokiytm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mexnpbao.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3idcfzfsv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iixrhzsi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ybadqduw.html


<!-- 参考信息 -->