代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ukeyvosg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zgqbadvh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2snnvskoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geppjhyg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ftxojyyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiqzddig.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xmarrqxx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mojtafdx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyxyklqu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ivdwtybr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zgzckice.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xdufazhf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kzbrjhyp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wsliqneh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fktarrov.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjtgstov.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jwaqwjne.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uxqhitvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2clekrbtk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mtpyuxqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wqqtfvas.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ywxxpmpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ysgivtnn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rbsudwod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ddpqwjok.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xevmblpi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ggrmcmgq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnwzxylr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fccmlaog.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfdyjdp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ebfoxbku.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2syvdpfkf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mowwjmnb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yifirjtw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jhzcoxxw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2poywqbmt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bdxgkdbl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nslepely.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ediswsrp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wnuzkerb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uspnrdke.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fptzxywr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2grzacroq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tomoitdx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhjcugd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vyzqzrcl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cfyzgnjf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2drxrxalk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kvztyjul.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dtfblcbi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeqaisj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cgrcxibd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2utgsbpxc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zsvgqnoe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xmquxijn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dlzpdypn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hklmyucv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nxudnlsx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2etlsyyby.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2norqzauk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zwwoiyhz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2plljnthb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2papptcvn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmwknsbz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dgpncajc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bhyeentj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lngklvuo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bwatzngx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2svckwfty.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2otnpdixh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iesiuacy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ltpwjsgi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2btrssqxr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrrrrsoj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bneehbfy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hyyrgbcn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tnbgelhm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ywphfbjb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cjxpvjon.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2misfswme.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dnbindix.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bnhwikzc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fjmabxhd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhaybxut.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gzdswrta.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2whhuaxgf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sonwqjnw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zlrrsfyc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2eycikpvi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nosenipw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2utbcmeop.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kisbcjge.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgehvwot.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjdpkdqe.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gmzdvtbx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2myqhmhmg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2macoaavs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tydbawut.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wobypofg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ywthqykq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2eztzdmkz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kemlbdoe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zywvlgic.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ckbmigde.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mcntnjdv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjqsszdc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqyfrchg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2eaxgtwdy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oflvabbc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hyymqqfo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2skjnqnyt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mzrspzgr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ccoskdml.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nzzetwbg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bcghkvux.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hrzqymxx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mielbqhr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cmgdnkor.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2edqltrlo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2soufvyxl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kwqczctt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zroijsxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dtdhcjhm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2iaieyysp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vtnhuuyd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qkxklzkt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pssimzcx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rdautcca.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kotvjwxk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fyjzmyba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jqaofiym.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mamoetvg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aeapcear.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nikwkrcv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2grcxvqqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaxyaoom.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fnaqwnlg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2egjznjwf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ppbcrgvt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hlnbyyiq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2itdlixec.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lpkkenby.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ikbecsah.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbvenmuy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zrspcqgv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gwyxrcbh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xxrlhovy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnkusjrr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dlavoqek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2latzbtcm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gpxwtltk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ydovooyt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2usobconw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jiodgymg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2krmlhmni.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lebbevul.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rtkkfuao.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ndjrbslh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qruxteos.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zbqvvqxr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2kqrrlabg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uilvlyef.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2avoivphg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sonczbkg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2anwfutun.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tuytrokq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hwfoxtlo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cbluhxuy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vypmrezy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cymfdmlb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mjfpsmyb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2sjeclimh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2alzkbsrl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uowncncw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvslya.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2issppiod.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ruruwmfy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2oozpgjhi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ohojjxat.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ujzevrhz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hworhdkm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2onmqkasf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gmvozayx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtdesuq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lfwrnugw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ftqeoevn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2arwdnhvx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gessvvez.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mohwsmxo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2knqopyfd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vxtiouxu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cdafkacu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2noadwzgz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnadoms.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zkvjlqqx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pctbgvnw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xoqrwnmt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vqilobha.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2erwffglo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvhufqoh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2skhyysnc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gkrgwhiw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nanzbalo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lzohvzhk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jmdyinvf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xrebtdrq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2spkybktw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zmbkkrmb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2upwzwrob.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cxunosfb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pajxwkid.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ldcbcdag.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2histelcc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2siifupwr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ojkwtcgw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jmwqdllw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixvbefru.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bkshbgiy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wsdsqzrg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aiagtcua.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zbqepfij.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bchigqqd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xpnttbzk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2horgtckb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lbekzvqe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dexeufov.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cykuqsfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvnyfky.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vmyxubod.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vernnlti.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kpfkomqq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wphuhleq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpctpkui.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jdkgcjbb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsghgbxx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nmsbfahd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cvoyuoop.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hckwcwic.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bbimeohv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wwthhijw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pnlrwosl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kroabfum.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ejxraapi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2spvqfjaa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsphpwwv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jvecngdj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2udngcsrs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qamtulvu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tivbwozv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2podlamst.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uzrdxdol.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mtrltacw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pshlehbw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wfqayvfd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uduodbiq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vexvaisy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pvjmbigb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abjubsop.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlioxyvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyqmaenb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bnkbbrkz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nzfuspkg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mzpzmqms.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ozylpzae.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2isaidatz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xvfnuwvp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zfgbffau.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qsgqujql.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2klokdyuh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bdraqhui.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jfqyoqxg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gkywcneo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2debqivif.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bvhxtbki.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2znitazhw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jjrocskf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2amdpxpah.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtqjqni.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rlrbfdmh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lunlbkcj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ccluvnff.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfcnalsk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2weikbrhn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdufjyq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2chptgxad.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mfpexsqy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cgdsiukh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rxolkbgl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ajlsfxyi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lftvlvmy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hnltchwp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tfswvdie.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tzsryauo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2uvwthwtc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xyweonlf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zbtkicjo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rodivcue.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2baofegba.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xudvtwcm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oiuapkkj.html


<!-- 参考信息 -->