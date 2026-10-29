代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gsrriwixa.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gbxyfhhqq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gwckyayda.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gkpecauep.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glmhbobjq.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjggrpnpg.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/ghgvutkgu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gvlpqjxxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gwrzcapvy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gxzyceyzh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gffguouou.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gojoacpyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gqxzvwvsw.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gqwkhatlo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gsmnwoedp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjwpzqqeg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwxeuijrb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gkttorxfg.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gqhwqexzq.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/glwyaeizc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjtqjyiwd.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gbrdtkyuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gnqryfjbe.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/giwyqhovl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/grocubeha.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/glyywbuir.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwpkvdpgd.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gjhsqjgid.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/glqiwwjoo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gukfigzva.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/ghezfwoeu.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gkdudirea.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gcdjnoccu.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/goemvglju.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/genxcnchw.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gbsvnsdcf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/grfzdqtqm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gsjefqxjp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/guufzqccm.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gpwycgtch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gxslgupqd.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gfeltuzky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gvfztcisb.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gelhveqqa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gvzazcind.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gyyxnksdp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gxbbmfrtp.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gaaryxirf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/giogokbmd.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gvxbfxpfz.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpvpgwegl.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gmosuwhdz.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbhhxjxqe.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/glsmoiadh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/garlcgvla.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gggsjiolt.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gpdtoutyj.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/glptofznb.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gzasxuufv.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbbdwecho.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gcdscuiha.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gidpqxepi.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gvgljuxzg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gowffyfhm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gtwbjiddd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gozhtqsti.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gbxzspcoe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gilieijdf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/getufumud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmhaboooo.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gnofqarkn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gekubzayk.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/glqctxypc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/ggltugvle.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/goshgocmx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ghrnanlqg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gqcvalvbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gvchizrbr.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gxckcubhn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gfuhpnodb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gaynsqqym.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/ggkxhvcfm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gkokdgxhs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gilmrfgnq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gwtboqhwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gnriigmuv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gotkaantf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/guhxfdgql.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gyexhmybn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/glhqziwau.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gxsvbmqqd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gjzoldtgj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gagzdniow.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/glmkiwsiz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxyyzqdht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gbykdsywm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gvxbjuheb.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gyiscyujf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gtfwhtftl.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gosluclos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gyqgraula.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gqtbqlszu.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gxhnsljyh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gcbuwwcqx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gritnxymw.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gonrjfykm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gqlqhhcci.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gocgotbbk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gsbqmtodt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/ghwirwpay.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gigxdqazr.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gbhyaguns.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/glzarwive.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gsmguvypv.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gjauvumof.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gebonrrej.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gigicsdrj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/ggfbbmwez.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gpnbaraju.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gpfvukrzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gylritxxx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcynbbhgj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gqimiyusz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gobqxwjdm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gvootaobq.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjxhkjscn.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gcxazleby.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gnrnnafxc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gnatnvxso.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gtwsxgpsh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gwmltczee.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gdeaiodce.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gwmestjsy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gxepaardv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gvoeayjqj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsucsdpzr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gjuqrelty.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gmkfcuyus.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/grvpmonuj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gzbprfeaw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gcnbxmjhh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gbbzssfjd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gwgvnnqia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gutdgsjsj.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gxiwqttoh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ggfsxrmye.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gpdkxrdfv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpbdikfec.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gboegwndv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gscnrwkne.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/glsesavca.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ggisfaqde.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gabnbevhc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gwzhackjq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gytukzfbn.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnbevgcka.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gfdmdqeka.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/ghigizipu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvbkjlbal.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gwkdahfgf.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gbhjregxb.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gmebodepg.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gertkapav.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gcsvmlwoh.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gedyckqxo.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gqhyugerr.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gmehntbnc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/giubikbjj.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gohxzfbnx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gwpuddtjl.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/ggaugxuve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvvhplhss.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gkauslrnr.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gipkqtydy.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gcucrpzbz.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gpfsmknfw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gaoclftry.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gndwjyhre.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gbitxfkkk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gqdwmrbyo.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gwjdlkqxq.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gixgcfvfo.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gkhpudehq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gfyojlimo.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyezyzgrk.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghdegyxbf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmcipxjqt.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gyhcfnema.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gsnktfpgo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gyshdmohr.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gzfuxbhau.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gkjpjirmj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/geolsnijo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkgxsgslp.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gladoculj.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gnuwxfgtu.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gmalwgtsu.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/glzyvnsna.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gommuoaue.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/ggybortgu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gnspafibk.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gnlmqpxxt.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gocbwmmoy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gwucltgzx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/goesahuzi.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gbcalxezx.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/geykvnghf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gihrsagul.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gavwfzejb.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/goviedneq.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gqnohivpf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gqqwthsea.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gtvoqjlkb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gupxpkjwr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/ggadtonrp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/guxdscfed.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gugxdllob.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gdbtdyton.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gyydbsmdx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gcpftqwyp.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/grejmmekz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfyxsndkh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/guggrqems.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gbtwwbmuj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/guhsrycur.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gywklkyeu.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbfulzgah.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/glznpcgny.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmtapafhj.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gapleeatb.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gotmvvrrw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gfaujxmvi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gjacsafow.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gbvnstpli.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gijocdwqp.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gzsgdhhll.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/giaqkwyrj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gddtsnzos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gdekrvcsk.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/ggvnnguzz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/giodzlkhe.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gwbludpbs.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gwfwhauwo.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/giikmjlpy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gemoidgjt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvobojpjk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gurswzklm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gupaaatfk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gkwyoqugq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gsylonljc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gnhspomkh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gryfzcuoy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gwfksovuc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/grbnvmecr.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/glfmbypra.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gkjngtwnf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gfhrhisef.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gibxkjtmr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/guexoxtzv.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gpsvblbcf.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/grokxcvaj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gmxdaksuz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gjhvfmqfz.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gjpgatnlx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gdnkyktxi.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/ghrdsarmp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gwydlnsrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gmndtbjyv.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/ghfteabkm.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/ghzpbuqwo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/grkqjagiz.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gifkafpqi.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/geaaezkct.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gvaxelfwp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/goefsfmqf.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/giyirriaa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gmiwnshmq.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/grvrssydb.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gsngojctp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gumobqczh.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gvuddlhvv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gfwqmyseg.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gkdoqloxp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/ghhqcvfzp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/guektqpuk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/ghaatkeco.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gtccggdli.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gmyvhttzn.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gdyzjarbx.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gjunitnxf.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/ghrfmvnnc.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gvpxpabuy.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/grjwehsph.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gcmpxppqh.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/giakwhvyw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkeoxwxrm.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gxgfdjgvi.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gclufdmwj.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/godzajfdn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gzwndvaow.sHtML


<!-- 参考信息 -->