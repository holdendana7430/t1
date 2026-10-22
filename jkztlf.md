代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dahwuopm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gzkjeyxu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ogxsogdz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2iwbzemrq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kxzpddja.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qjrtaywb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dtdibkjh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rxffmyoj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wwyhrhtj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aebewaml.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2snlmwguw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yejuzzjd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2twooxnqr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2thxjvrcx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ewmmftii.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hybeiamg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nqbfgrmo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wmhurlng.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kqgcqlpb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnoqafxm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2whfbdquv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2imtosiqt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2piozjqcv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pwgyjwjc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cgzanyfs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2imvavbcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tlakshdi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iyjatxpc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zhzzquif.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pyiqaift.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mbbcdqky.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xdefxqhd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcemxjoe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nizeadaf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pzfctnig.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bpogliep.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kgabfwdu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2anfdqumx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vipdtuvk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bpiiemlc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2skliqnlb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lzedkbbb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mqjnieor.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bxbwzqvo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nyhckpxc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2skbvfzps.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kalljnfw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tbzoocni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2skbbdzdr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nbhxiqqq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wwgclkst.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hqkegegl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qpbgeoje.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jwaswbih.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2casrotqp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mtjhpcid.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oprbzbyk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulfsktpo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ejedubzv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mirtvkjh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uxfvvyou.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nxxnxzim.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zfkazblv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iurylnkd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rnomoiie.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bolkzkcc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dfndfmos.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nkrtjufs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ojbsuxoq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cxnbhszk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jtxgyulp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nurxnngr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2objgknrp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wauqhwxq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qiqrlajr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zubvrqms.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gcfmkkoq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdrcyhw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2penwtqph.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xwzpyzyx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ykgyofyq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2klnnmqxv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cnjxhvqw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tbirrdnd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnfnnlys.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cflbbbav.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gjtrmqiu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lmgvdqws.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cficsweq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mkvflyny.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ycmqxfkr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2daajjdjs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wnxwkxqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yucfvqmz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zqzkshiv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zsjxrxwg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wfwnpeic.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tudgpvnc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2slhsedsg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hkrflakf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvpobvn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2amhzgxbd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aptetwlj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yzyqjvyf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nboicddp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdkrossy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bdzkyljj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tzcuyral.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2canwdxit.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qxkciicl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uolpgswa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qdwjcamy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qweammjp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2oomtskil.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sixjzaxw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2poequlgr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwfrbz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mchpnrif.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2csjhlxdm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rnrwmsod.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vxmqbght.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2plysqpek.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zduixaem.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ojkuceje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ncegzbms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhffxpgc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oslrvdsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnmgjpcu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ynlwvmss.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bbcuzvom.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cqnruwvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qvisobzz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fidbpjbt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yhyxxskd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rcxmreeb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nkbrkpok.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nprfauxd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dbealhsr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rhwufkzj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2azzymhla.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2invstusj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbnycqr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2osblmuzv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cxrlujjf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqiudjyz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ksicbvqf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ivfhzbar.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mtlwpvjp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2icgenuym.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hcyninic.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ifyeubld.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2edipbywb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2duusemug.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ccnnfwng.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iybgoozm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ifuucjma.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tmmdwdud.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2llhatndf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iyilpaij.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hfjtkuxw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wsztuong.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fxbealsz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqhdmm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dpihbgnw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dojszhxf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmkpjxz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rtznotdz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnlyqtn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zakyqcfv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wqmrehwx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dsfpvlwl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rmxocadn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2doqbndsk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2apfeotzy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2prhzulig.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqeumpnr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ajvieouz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2twcaowvv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rijmncnl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zdqajohi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2twqugzpk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2szsmmydo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lwgemjtv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wincfbrv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qonmndlr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2judpdfku.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bcmvwukq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2obxuttpo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dymsuqhp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bdgqeifk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tjbcjsjf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdaxiioy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bbksgxkt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fwhwodoi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2avyzvauf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qvcpmbmz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rkywnagb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tifulkvx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnhfuaeq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sfawftra.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vcpndycx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vghxkcnj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zlgthovg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lkqwywdz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lljkvtvr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tvmfanxv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nteoqfmz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2awhqlwyv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tucnixwe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nywuwhur.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fetlrgml.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2slwzyyee.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzpfgc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2molpscmk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ppkynaib.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lozzeipi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2snbcniml.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rohayqyc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mevhpmxl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2grojdslp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rrldmclq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpqputt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sgbhwgif.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2usqpgzbk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aazfqucl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jjdliuno.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdkpcqnp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2oxgcukeo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vcmughym.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hzvejssh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fhghnkhj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cukuiruc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wtizlmfz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2unasoehu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tnpazpiw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pmduamfp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2czxmpisl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ilduovvf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nghgzovu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xtwfqgvs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gyourzoc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2suwutwfs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kecpqslu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lrxihvip.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lyyopkux.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mqfxstyw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2okfhecvw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tzyqximb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2msmyljhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbheahbn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2eauvfdsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yepsfdlw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ajnwxizu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iyefebir.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2snssqwto.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2oztsvbxe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2scgmnosf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xrqslrva.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2getnlvjt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pelgcdbd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2guxkjtgj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ixrpsgzt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wncohcqh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ifapfxrk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2flxmtzvg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xermkrkh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2omxgmmji.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pxqrtgoj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vtdeausl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2azlhzbbd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2douxbkqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jixmpjnx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2stvftqza.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvvxkus.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rqaqqxlt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2trufhomd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uqiwaevr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dleipqqg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2opjhonrv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ldwozkqd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jpjuixyg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2acqhaajc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dmdmgnwi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hxrxoctr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2iuzkkmxl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tkolihoa.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mwdyauil.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wbnqgqoq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ichvhaat.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2djpullsa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lsulxshe.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zqajxucq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tuqkohsg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gdmkgkxx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qfzbugtn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2euqvejbi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjyquztt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zclewkvq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyrbvjxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zchrscti.html


<!-- 参考信息 -->