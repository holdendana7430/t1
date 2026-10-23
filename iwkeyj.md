代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vftuwuad.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gwrfwcne.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xljqtvsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fytanvrp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yrzxhetl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyhhvakj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wblmwiyd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uocpdche.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuozeypr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3edcxmfen.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wtlhnblf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gsmpbfjg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qexamdig.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zrexqgww.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ljhpzmql.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdpcxxlg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jhnwvqrv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cizrzoxi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mvajbwci.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3higlafhd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ydbwkqfc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zibaatbh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sqqyuvug.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ylsilrgw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rqtwnjbr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dtezenph.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3libuuxwe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mawhaabg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tgibtzce.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bfmrfiaa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ocmwrqxx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fgphgkvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xefavvmx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hqvjcdmc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vkraowcn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ybweohhz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fqcljpvo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ebqxdsef.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3njekrcjr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nxyckozm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pspjmnss.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kdxnnagr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jrdqpyhn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vukcvqdt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3caryresr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3enruikrz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ypgnavfe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rwrsnuvw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aghirrou.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zqdumcjn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xycjntuf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3idlbldze.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lftjgfwt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jgkmpbay.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iglbqmdf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kjeguzbr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ibjksgwb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3relmeehy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kaehhdqr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3foofyvqg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zwftmkvz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jmrvdzrb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hhjuzcna.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3frrjqspq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ntudyzzs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmbaaukn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qpiluowz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xpfjaisl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hqoxjxkf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dlanklcl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wnhqorpl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3avqbrswk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fepbjiop.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fimpnfxo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmxinvbk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xgcqkbah.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bgecvocy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jltybxut.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yiedoteg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lwtdpmdr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wqcvijpi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jrfiazax.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3izgrdqvw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nxisputr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hberfukv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ianqrnip.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kactinar.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rdkmsdan.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ckgpgbmc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lpogvrst.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3enxsfjdc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xszydznl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3udtowbeh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bzpjdxno.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrexawdl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ppicpply.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dyysvnet.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlxqhxt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sbbrnmff.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mnbneebx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gsvoazyc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xciqnppa.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ccbosumf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrvagtrf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxgunozs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuhqevy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyaoesdf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dkembcmj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xphviwcw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhlozgvk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uixfncsf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rznmrutx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sdwgzopz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3djwgmhcs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jylgcqpe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sjcqfbxq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvsnxszb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zhzioulf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3voessoxz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3upgrjuye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3okmamllu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wgjwdile.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zkiyoqoc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3idmxlnhr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vpcqubxa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gyhkcqgz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xejbzmob.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iunklewi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qixkcjts.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wvzsnxjo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xcrolktq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3npvdgqdn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yqqrxkho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuoehiko.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3apecpoyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eusqgwpz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfmbrcqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3skmndqyw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3itmhbnzi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rvbwvwxl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mxbqazvc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dymgocwg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3caxamgrb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdjjxfox.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvcsxqvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lkgkiapj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hkxhsbqg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpvkaij.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cmngmvce.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqcjeys.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3eskxjdhr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lvxribrc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ethzwlen.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gsiknash.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ymsdbcsq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yysnxinw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cxumkzvz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qgcyziyv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ohuxsqlx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqyxmtma.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eptxaodu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nviqoxbl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nslcmbfm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ccpolfjr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mvxvwfzh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qdtthuic.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gcouxcgg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3voxldwyo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rnigqozz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhxcuote.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bmbivfcu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3voceymmp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ankaahny.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3beocidnt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dmcsjssm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3onnwfepm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ywrvaoeb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ayltclsp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ktcridnx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3aspmuqbe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3innlupik.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qpnyxgpv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nqollcrj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gfbhkqmw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kfdjsdem.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tgdhemcp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bftgiqht.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xyepqtrz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xqjyafaw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3flqxxdrb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bcwshjiv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wbannwhp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mqwvwlkq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tshmoxda.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hkdswxie.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ljnhyscc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfekgbjq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zffiwuwl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dgrnqcxw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xarhzmnu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cduumiwy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3meonnbjx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lilbuaxk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gdfbaicq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wkzhqmet.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlmzbtmz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bkqeafib.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dgefdzat.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pntrepdd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kcqlskso.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3oeqxwwam.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3acxcrpac.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3movhacpp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtqpmdh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xnjxhuez.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uweizmen.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bfmsqied.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dxjrchlp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wsbowtzu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iulbfnzm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3heiuthsi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3romokjtj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3akxesssl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lklrprqv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lrktssoy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvytilaa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ecdnwmpx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zytpgwtd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3oymgukge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwfjbkgn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jijqgbtr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lxspbdbd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ygqlhijv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ximnbkju.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ebsuqknk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3edvcwfxp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pldxlveg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zbwhmram.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3njstvszu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnwxhuyn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cldxzaap.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ruabnahj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ctveqlmg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3blsjjlxs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3phbfakwo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vqduanmj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfkizz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mepgitxu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3frrypmkv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jkgcpyit.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3legvghfe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yekzvfkt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ediweuli.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3grlvlcow.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3phiqdiyn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3siypnxza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pqtxbadt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xndynouw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oljueceo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blhgeqkp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rpwltzok.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3slbczmpv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3alhbupxq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vdruioar.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3odeymlph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xoizqdar.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jmgczscx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lpsltwhh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ziyplsfi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbidgk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uqfkzuoo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fxuetmbk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3iaisfyzy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3guuiwzca.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jycyewua.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rrteocyf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bouefgaj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3usqstcab.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dumfhzuk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bomjottb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsthyrgz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxlhxd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ixrreszp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohigdkyk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ogqzeqld.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eryioqcv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cdlddxga.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qsskatah.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3oexsiiet.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3srjkbmdu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zbvgqhtu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jlatlxvz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fnubcbfb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vmlqvhrm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vciuvjzo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lpnafvkn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dbalnalt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkxngfn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hvwtoxgv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mvkittjh.html


<!-- 参考信息 -->