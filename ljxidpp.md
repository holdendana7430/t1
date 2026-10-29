代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gjfpwzrqq.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gjxzokkny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gmgvoqmea.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwiuwgypz.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gepqiydjo.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/goukwcfxs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gtrteysjp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gadybzbpc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gcoheeggm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/grfjgqfkd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/grnpfmmua.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gvkmqkdgu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gwgbwicew.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gyszhzaul.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gcirieqqg.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqfymxjkf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gsznhkqkr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gtmwifivc.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/glxhoshaz.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbdgtgvgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gjybhnhzm.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gfkckakyl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gnxthwekh.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gorlshjtk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gyydknfio.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gkbpmjipt.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gbwcljljy.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ghdmphitd.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gabxsqbet.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwxcotfvf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/genncrqhs.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gyhmvnvex.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtqfwzhhz.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gzkqivwpa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gfdraqhhz.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gkbvptalf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gcuwtvhxe.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gxelktzge.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gqpdfjmxe.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gmgipswkx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gomunxcow.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gtdybvhiq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gwppvawxz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gwllisbjg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gasqaanmg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/geroomumh.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gohciqbvi.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gksbyzlpi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gsihebocz.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gmomenbbh.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gnsnfuqsn.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gwpvfpnoz.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gfwqdautu.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gdiitwruk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gexfxqijn.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gcdxtkkmk.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdqzwjb.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gnjzkrlvc.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gabfnmhnz.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/goowowziz.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gxzhqbmia.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gnpghgofq.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gknhxinpw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghpkrtuuv.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/ggpsxhilm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxfiqqrqz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gtltnczuf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gtaefwfpf.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gnzyepqxz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvoawlp.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gykyoojbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gnflchvod.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gnohvnlvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ggekjavrm.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gfepehoxg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/giepzntnv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gejrupapl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gevdclqaq.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/guxlckjem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gmhtxlern.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gjxxpuxsh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/guwujvxfk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gverkstou.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gtuikgxpo.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gvbfvqqhr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gknkftasc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gidhndppi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gpnnatvie.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gjhnkaoud.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gdlfjqefh.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gepgexeiw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gimqjztjc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gfawuwaav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gghpctqma.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcmvbkyuj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gkzuzgons.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gijfoyskh.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gebuqezyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gzmkwyezt.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gbwylhimz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/geccrexnd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/glkdukkkd.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gpvqvnafi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/goqblduku.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/ghmldhvpm.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gfgsrrxlq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gmnhkpuhs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gadyuluue.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gnwxfgyxh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gjnjruukt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/ggvrzehot.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gfvhwmomc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/grgcuubdu.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gpubwkxvi.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggsmylwbu.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gwwuwdggk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/ganvxjevc.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/ghprrxqiu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gwidgrmej.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gijfxmzzv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjlkcdcys.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gauqwqzqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfjtnxtlg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmxxiqqpu.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkkkqoryw.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjzsmivne.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gquofnpkz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gmrfqphnz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gjvsgcjft.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwuaxtgyx.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gwvwxvoor.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpgvwzisv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gaeupjgcj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gkfyeuejd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gslhexddb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gztakfsqb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gswqsdwbl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gpgovzzwj.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gybljhtvz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gyuwxyfem.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gmfjgonvd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gytprjjwx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gcggytsff.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gwevwybdh.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gzsmyymmh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gpicmofbr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gdkluxpxb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnmviqthv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gueijippy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gjwmkfqvy.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gdwdmslps.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gvloavrww.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gpzkdvget.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gkwmuagak.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbkopioak.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/grdwohlqq.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gpxqezlut.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/giabhwwfx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gjcgutdfq.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/ghdhdlhwt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gnlhbpjwr.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gaqrhrvmt.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gjdhqcbdi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gzjjoiskj.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gmbdcefis.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gvbxrufjo.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gifrjrifn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gihucspdh.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyipcbwrq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gdpdnxskn.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gilbmjgbg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsjzceoxb.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gfdpemdtu.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gcmxljnbn.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gjcqluohc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gwandvsku.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/godlwnsck.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gvtrjwgbw.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gtcsirnou.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gjhoafhlg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gjnlkzdwp.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gifmaofkd.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gyzpcwdex.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gzvwoglwj.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtywgqdgg.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gikavcdwv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/giwhqfszs.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gfwugtrok.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/griixfypl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gzfuzqrym.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gvtzagkjf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gkthnwopg.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gkmdsdvnf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvuqvpvko.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gajxjqovz.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gcjiiekpf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/ghupucbcs.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gmijqsjpn.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gwzfwzikf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/ggpuuelea.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gktyvvpna.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gmqdhmlhn.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gmbyeoczp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gmovilywo.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqywafcfc.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/guabuyuuo.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/guwiyuzmf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/grwdknmci.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gayqdesea.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gjjcgjuuu.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gfgchfqeh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/ghicyevol.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gyaecciuc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gdhgjwoby.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gxpomzosa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gnhivblnl.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gdvdrnrnj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gypoolsfd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gkofiumnm.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gkxuzzxlh.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ggwiekoim.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gttbvaimt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmnkbgrlt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gicqpspow.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/ggefyntpw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grvlmywxx.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gmwaeaugz.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gvxauvnqc.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gzumprvst.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzzqclk.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gshtprcer.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gkexxhzme.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gifuuazeg.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gnnlavwzp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gzopzvnma.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/ghaxbauvu.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gbgojipjy.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/girntppdx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gufeamvmc.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gctxybdtm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gvfjrhtuy.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gzuxbsmwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gocxtinqd.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gddxatcca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gvblccxla.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzqsjugio.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gwlmezbfc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdpqrlqum.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gjkmbseqo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gmtqxqkvy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gtmockprp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gnyjkxjnr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gyfmsuedt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gdixmqxwd.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gupjbykqz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gxddzgpnf.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gckvfuiwz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gaefdvfzq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gzhiabxik.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gixxsjwek.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gbwytlwjp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gdwfmzvbz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfwlwuced.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/griujlsfg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gblbzlcuh.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gleeqhvhg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gexzfpiry.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gnwfilfpv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzftwbpav.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/goeivesot.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gnrguwzcy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gispjrlmg.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gkicutmgh.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gfdkiqzhy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gjuzpdqio.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/glcpgrqqi.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/glpfyagui.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gtolhtdvc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gpgcfrghz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gawsnoxdt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gxnzaoujn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gayosxhiz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhzeurz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/greoooqlr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gvjsardcr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gmjrimlfq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/ggwbzkwwq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gwhptkixu.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gsuikrmoi.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/godryzhbb.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gbmyixizq.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/grigfrxyj.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/guqpcwfvt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/guthzbcyg.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gynwcuzqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gyesbimqa.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gkotbvtvq.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gcbllxopo.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gstkkygtc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gaqyjreyo.sHtML


<!-- 参考信息 -->