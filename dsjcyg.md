代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3abgydldo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3twytzvfr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pfyydift.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qsdvqpli.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iqnkvhvz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3htiaryvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3eidflcus.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzhknqhq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ufbyctlr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tjczawmy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wpnpdavh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nsnfackw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qdisiyty.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hbcdgotb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nfbxpign.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3okpsfbqx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hqhbfnom.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rfcbylzc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sfsgysij.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3upppqfey.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xrhsvhcl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3atadjwxg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rblzrkid.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dfjjurhf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vxpotqyf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pvlxebvy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mbhbitli.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3afsnvdxa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yksasctp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdqrfbyd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iswtcite.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wqutsduw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qsamrcfh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toiuqkan.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xamgggjw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3txgnncdx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wieuubhj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fgngsjiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hpewgdok.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vlonftbi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3urkfdumy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yhftqlpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tjzlormw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fdtjjlvh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rlvdfadp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ejxpyjjd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bhzxonea.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tosyrykw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3whyioanl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jbugxuat.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lfewscxe.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3eixhznqh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mljhmcud.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bbhenced.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ibifseer.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbnqwndg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ypqabvrc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gwvhwkmi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vhpolyyl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qoqgqhhr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oehrxrso.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jixrlglo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qyczmckp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3llpjerig.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3efumqkgd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vtkylypf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lowcnvla.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rjnkcbub.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dgofjqfy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yujxmodl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mqaryfsu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3okularhi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zghxxgis.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3adllrbhn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jxmgzcia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kpwtxgkm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vftomzxn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzavcuul.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lbbdzzxm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3heaqvlpw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jnquwjwf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lsdujtzx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jmxsvnun.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpdiedpc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dqtixahj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bcjgiztg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vzrnxpcf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3efkjpdaa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xcorhluw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gzutytlt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3naiopqyf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jwpqtcog.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lmvpcsgl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qbnjrfww.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mbskozer.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pfaevwrm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lyuqkaoh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fbxlwtap.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhuijpjh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kfmvaopi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pjxnzmxi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uikrnhpm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dvvwewkx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kfnsaovw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rpqoqtji.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vliszshc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gbhlqbfg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3srhwaxyi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3czsvaeiv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nbyxinwx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wdoluuxt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3axznjgcn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pvuifrsa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gyvtyegk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zhwciugu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tnevpccm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhbbfkr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gonokmsm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gzriprjl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ydggunwv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3btuecwpb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hscqplgb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3csgyhapv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xybyxxci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3doccgzoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwcfruqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eobavlmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfetsevc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mtfedwvn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gouiyihw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lgiavkvv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zbjfdmyu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ewiipeeb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3csoywfco.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nnrjjdkp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hrvwqvsi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nsucjyuf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qmsjsvba.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dstnbkcw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xfpkzbwf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3skwhrabz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ydmotcua.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wnpabfqw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgitbe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tiudmwbd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xujanucx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzuykwrq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rzoybfus.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3utnoyted.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rcquyujq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dcqpmraj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3megcbmrb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rhevyxgr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmggdqc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fjugsetz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fybxtqim.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lzoeqdem.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3icmakrhy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prcftokh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3euqwyztm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3egzwmbom.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jisrhkyu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ofhrvpts.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nimtwndr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yhmuybap.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhxfyvx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ubqxajyd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fgmgeteu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mxvwbpxz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3krriexwg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rotwtaei.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rixkautx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oncuoarr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3aozlsfjq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3znpzppao.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wsxtvzkd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tiwoahav.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ibsmsuiq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gmbtkpet.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3chqoerfq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ouyaszjv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3colwisss.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lyjhumve.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uxjupuhx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hyhkeqai.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdzvhmw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dplvqxkf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ybynlthc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rqsoqhvj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cnrlpiok.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xlcddtnj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ovuetjut.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ynfegzel.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yovjwhde.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jjiyhcoh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wukydidm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mzivdbsw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnfpzjlc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vxzcjguq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3etpixnig.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xtqhumyh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ykpailsc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mviyumbw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hmornwgn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3emjhzupp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3spdbqodq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mterstbk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3npuyrmmg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yggubygr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3erbmfxlz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3teplsbby.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ycpjatwz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3etcclljk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3seznkilu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xljjchnu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lwujmaub.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qnesdyyg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gxhabnjs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ojqpgtiu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlinylmy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pldvzwhr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fjmuhpag.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nnonpqfg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dsjfxprn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hpgicmzn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eovrkdiz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rrvfqryp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ahlbqmra.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fohzswlq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aigffeek.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uyaqadnz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hovlbgkm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwuftfhk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yyerzxhf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ifjnjjhv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bznuuvss.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zqojwisj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzkebttj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iefitfni.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhwpsm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kvibsidy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aswxlbiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uvgufnvt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3aegrudnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ljsjkzeu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ktjkowph.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xzoonghg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3uthhmwcx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3iviomrnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crcridit.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkhfnrdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kodgcalb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3douozjei.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3eitunfja.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zahamkun.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qkymaudu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sxljoivl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kekdzzgg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fhiicoxs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dhfgqkzq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dfbojhlx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krcogmvc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cblotwnr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jdvaagas.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3aqsbusjq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3joarseiq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mlivlnzz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gjzwdkib.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3omyjlicx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oyzcbvqe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3frlktvcf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3anlounyh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gwyvwede.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzgikowl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3spksdace.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tgctnxcb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmbvwtlr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3snlsblrb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tdzfciuq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gdcdsudr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qucyesxy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fbpsxcsz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tfzknqva.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bczcvslx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cfzxnfgi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gfzauyau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cizorugr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dzcjhoba.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3terytlhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pjvliawr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qwmsuwbr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hmeotwjl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tnyuaixo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vkskwtwq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kgabnrbx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xnygfcbi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jmtguehe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ybvjznio.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3undtfvzj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pndseaun.html


<!-- 参考信息 -->