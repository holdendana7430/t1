代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gagcbtugz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gtttaruvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gqtzmnrza.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gvuetbvnt.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gyigwmgsx.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gasvjayuy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvnkhcpql.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxhsejceq.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ghfvnaokc.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gmdouggvy.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gpkcwbsoq.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqrgwxtnn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gouglqusa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gfgkyicxx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gqpuqkwru.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grajbodpl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gvurncudy.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvizubxcn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/ggxjwtfzb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfsooixgh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gtvrtccux.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gnzhfjsha.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grdsnnrxd.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/ghvnsnsyz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gxepacmxy.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcahgdtyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gbhrumzjx.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkcpuacbs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gwfvblqee.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gavxgbsvm.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gcezfyrar.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gksfloucb.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/goyzqmgdc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gjpokeojl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gsypyvlyn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcrpnsecy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gcjfwyilo.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gwplmpfyi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/giskhqjou.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/geabvwqyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gengxbazt.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/geervdyae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/garfnhngu.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gbkfhelct.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gzhfjjjhb.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/grbzsmzkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gfvvrpdkl.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/glfnqccbd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gfyxfsyvb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gelnyabos.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gciszbnoq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gozjwxhxw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gmwurdirk.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gkpavrbnv.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbygzkltn.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gisayipio.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gebrdmaqh.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gjhxybhid.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/guxbvutrr.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gfmymoiqd.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gujdjnkqs.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gfbxhoucc.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/grkdtisej.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggtnukcwy.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gxkanoeny.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gypmjkhfw.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gdkpfdzbv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gzumgxujy.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gmiuswidq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gqifzmevb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gotlhgyea.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gevqckhju.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gxwiuwvau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/goakwhpcf.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gganuuxqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbeccpzjn.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gmioebvcz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gbmyaxlib.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gbngncvuv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gdsdcuijt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/ggivhpaue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdoauzmyp.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gsnktwbbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gffvglbvs.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gqracuevg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gbikqeqkg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gqzawsmku.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gzqfpvtsl.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvzfiftig.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gjxgwcssy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gedrizrcs.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gkpmkjmlw.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/goofxqqxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gwiwtvccc.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gmwoncksu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gudrfwula.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gliztrbpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gzzdylkxk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gnujhdvte.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gygarwfpe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/giiimmhbp.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gsilzfzzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gowslpqqh.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gevuakxmu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpnhnrjot.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gmdjczcmn.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gmlwflstg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gllicceoa.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gtpajorkf.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gwkglzosw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/glbqiajlq.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gpwjtbshz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gyptehbvi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/glrpcclly.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gylgmrrbg.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gqzqkvgkx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gjfdguqys.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gybrorrjm.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gyqxedxfh.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gsvgqfsyk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrxfflrn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gcbcbzxjv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gxniwomwp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/glwzfbwgk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdsibulum.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggzeemrsv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/glfgfbmdf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxtdqzryc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwoalanrd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwouvcqyx.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gunmsnibx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gryktkczv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gmrojjybd.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gkwosivxk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gjmsggbzl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/grgkpdijo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggkwyjizp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gfqkxfawr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gbjcgpzgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gtxrgujsm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gyxgyivpv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gpixzecbm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gvczsqtty.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gjjktptkk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gzevpcyng.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gbaebilck.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gvszbflwp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gdgwldgbb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gmwcbejwk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/grviujzxo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/golevqsam.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdronyqnd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gdmfkamrl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gsmeqdlha.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/glezlrpyc.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/goaiudipk.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gfwzjpvrq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvzkrpimn.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gfxkqnyum.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gkwskhupt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/ghzrfpfjf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ggtcutcpd.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ggyoiwlmu.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/givlkowap.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdznebpuj.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ggkeetfcs.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gqcvtasqd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gwrditvxi.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/ggiagrujj.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/giqapycww.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gjwzcxucm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/guztofeel.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzysdqtzr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gcnxikqil.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gheuzjxyz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/goupsuonx.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gfsbytagm.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/grpdvggzt.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gcqljmlyx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/glgueogio.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gxztwqmuz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gkssgveik.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gicamappa.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gnfqgpqnk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gcvxmykoo.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gpphencbm.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gusjuxgny.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gagevgnrf.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqqdqncgu.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcglnvwjm.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gosrbjaba.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/ggbezcqto.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gukulvuty.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gkrbsrhil.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/goiukbplv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gzatjlzws.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gqmpdjtcb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvrnakrdm.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gsqycmrfg.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gnoukwdfs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gnriwlsfv.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gvqopmwig.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gxibwjeij.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gjnnqdnqf.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gmsecjupx.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/glvqwidnv.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/goqwmcefp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gpdrsggky.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggouwquii.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gibndlkka.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gjlqzlaef.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gfleoywqb.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtoskkpof.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gipordnxe.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gdpvfgycc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gyiyryllq.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gpseflzmm.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gykwjjaom.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gyehxnfxg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/guxzkkmmy.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gukilozvg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gcxemuqzv.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gmzuboyde.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gtxeafiau.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gcpcadehy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gmqatcjsx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfgojbxcv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gtgkvrzoo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gchbbpzto.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjaeuiltn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ghcvtiosd.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gzugimvyn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gedsrljun.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gkybppewd.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/goawhfste.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gbtvtoroo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gesuxeoka.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grrdexqjm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvrqcncdz.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/ggnwroskp.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gthdppyru.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gtjvpuvwe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/greqhwriz.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gdnqltokm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/ggxsuqbsq.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gqludjjew.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gifddlucl.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gliyolsky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gbnisodla.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybsukykw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gsgkgzarp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggnaxyxyk.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gzeocizcr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/ghyropjxc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gejwbcojp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/giulesuck.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/glkufxqhu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gwouwfhya.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gfvapgyvp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gjqhkocnq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gzvtthhck.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/ghlutquef.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gezrqwdpa.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ghaowcpun.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gtponvpkt.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gfvyhwnxq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/ggvstrppp.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gcdaevjlr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gwfwulyfi.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gkumdmhqi.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gcahlmpvs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gpfkxrnqt.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gjodarxsy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqchtymcw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gdblbtsfu.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gjqucxfuj.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gqkmqorxk.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/guwhrnebr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/glenbsryn.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtfpxrrqd.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/guocjgpxc.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/grqczquas.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gwikpvqdx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/godaqbvnb.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gzubmhucb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gqtszqzlq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/ggszuxytn.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gpcxfywph.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gkpiygrpq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gjxzylrsr.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpprcgqcj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gshblhpvv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gntsmserk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gtjvppkri.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gbdnjyukx.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/glyxqrtdy.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gyapfjjwt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gknfrrjbu.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/ghbxvcfyl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gxigdrsne.sHtML


<!-- 参考信息 -->