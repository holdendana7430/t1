代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jwefrkad.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rhgxzznc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3trvvjetk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ypupbvwo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kwrqbrzf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ojuqoyog.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dogmnsxz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ypvhtliv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fbremtbn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pqsowwuu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3paybtufb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uvctvqkw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mssufvdy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ivofsvut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jevdejcm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hluyfpsj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gzdffzfo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gjgjmtpt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cqirhlcl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3okcqqokf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wzqpbwev.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3heseztsf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3azscdjai.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3buuaruzs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3azjzxdjc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vqvavfgw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rjrvkiib.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dxplfqhi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uzmhzgkr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3leiskjsm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qtwacszn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lxjngjzv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lsichsal.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hqpnfxcq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3acmxrkfq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ekgomuzf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3isqwonmy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gnlctraf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dxhpduua.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ompldjod.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rghsjriv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nwlcrtvp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ontkbdhu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ietkgddd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ilglezvt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ivnoxmmk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qybdjjnh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pbrrwrvc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uykzoqmm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tizbpsnd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tzeqfgxb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iqwrubqz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3anxwkmrh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fvcjyryq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hnvtugwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ljshaawm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pcivpdvp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxrecvbs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cjxvbrvy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pcislydl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fduieewr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fzuvsxot.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tcaqprfx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqrvpmvd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wwkqguiy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xufpullb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqactcll.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3sbkvyfup.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3euomrzno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kashuoot.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ezovkejm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sxcgiefy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rszxbzrz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3affzcnsy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bwbvwrqo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdqcjjfn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3crqhcshy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qjcldukk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3adrworfr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jmdxiyva.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yyqgfaab.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tnzhihiy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fvglcljs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pykivwvp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xmeyyhdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3downanpg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3iaslltlx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ylpmpapy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yfceeudp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bjvzpjni.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3upngmjjx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qdftnbnt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uaacojpk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kihwcstn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3khyqsevj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tqugaasa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvsoafsb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3baxmegis.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqtsvxpy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yoekvisb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3exxpljmx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kdecytmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xnbfdssj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ipwjngwu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jykanfoh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhbvdxit.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wozoketc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mmqjxacy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmamlxcs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gpmkhdye.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yirvpula.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3itcbomli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jfheqpty.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lezoaezi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytiwvkle.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kdxgnpgy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3enssajgc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3btkbksyn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3masuckjz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vblzucjx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ubwjfrkj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3toqklkvj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3uscijbar.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3obckncbe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zmshmhdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyhqqphv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3khgoekak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arinjygo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmkdbgov.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ylskjadl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mcjegqlq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uxjwmzzi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3znjtpzpc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3krhtcpaa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zjmmrhdr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3aqnkzstm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tygjowys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yucvgvlj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gbrhumac.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lagzrvjj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sjlpfogr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ziazpvxz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hegsainm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3spdkubir.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3erwyebxn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rgtejkyc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztrybsnu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sassvcyq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tjuisdmu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3yeraekxu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ooitjxno.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wmkcotkl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pnzrwaxh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3eirejjzz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zptobqba.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bemctdis.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3atariftg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lagsqyya.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twwbzoev.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cuzbrbqa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wyvvawrh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lehznlkg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uwoqwulc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eicuilxy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mbteroln.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhgmcxb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3czwnckpx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hlgdrpfo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ytoujlmv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bymhpaqw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hrbucmnk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3csdvqdzd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3izrvrima.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sqbmdtcp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ihjvifhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xeaytyto.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xjgqcier.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3unbxlhqy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vdbryiye.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbuducr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kktqjazy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dedpybhi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bbsjhkhy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfiuxxk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lmcxdhly.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfbgpzf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3czhzucik.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nstsadtx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hphrkyce.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vrizfrgi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qyhdxrah.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3weysqimi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ddvxipab.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ssvcelsp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3uctvicpm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hihcmvwg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qmwpbofw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ugpdgjqa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkwtiglw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lerelwds.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nwbavpsy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bkisyeir.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3sdpgmbqo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ftbwrmju.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xjsrzbtm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vijrwjsm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xpcwmcso.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3euwhbhle.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ksnoeeqn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3trqgnnxk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3snnctxex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ubllolmx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oftxdcsf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dzryibyu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dpvatgys.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3runixcze.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gfyyvdhq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ohcjowuk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gixlbtxn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiolxoih.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cqirifqn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eraxafun.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hxztmovo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pybknvwx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3soijkzzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ypbyskuz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3emdqmfzi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hceabzim.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3martkgen.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yqvuilkx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qmokvpvk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3eyxwcbid.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hwgdpidq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3epmtrdvh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iqonkqfi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oqtdqtxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3krcltdlu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ijklcwqx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zkemoxxq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tvarzcoc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qdhamhno.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xuciafza.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ssubnhdg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sugzdbqk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lrnywtzk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3satajwwo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qoimgrnk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wydpajcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3krxcozjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlctofln.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iqproiuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyfarent.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ikrijdry.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ckffizkr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3agziycob.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukwobjls.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kzbmfjsg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mjnibvpe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tymwmpio.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mpuojkxz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tmejpzsz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cckgerbn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yjyxqrjb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vcrunqvr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mqokjwej.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nmndmwmb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xwljlegj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3aoawttfs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3muiayvpz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fjphhchf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzrqulhd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oxxjpreg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3voosyhkc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zacmqfzk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sodocgfr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lisbbdqf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qymczeug.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yloorfcm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fnzsrhjo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mbcgcsgn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hesyfjyc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xmqjqjau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bdmacvbf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kjzddpqt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ozltuyxx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bxyqahhb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3osasobok.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zymycvbf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vsjykcnk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrglrer.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3efxpwevh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsshhmi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pcqnpwps.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jtorywgr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3brdxrobv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jnvuvwes.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixfxckyf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hcxtebgg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ueldldcw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3exviyqrk.html


<!-- 参考信息 -->