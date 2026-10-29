代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gldpmbpcs.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/guftupuyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gvkesuuhh.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gvgtauasv.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gbrpzqdsb.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/giuhdxryt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ggaywsztf.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gzxyldjal.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gghaynlik.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gvugplsin.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gorucymyx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gcihewwvx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gunczbtwq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gkdnylmjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gzrqpypke.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/ggekpjvmm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gikylwyqo.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gqkbhmozy.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gaxrhpxwi.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gicvtpjqh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gwovcgkrg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/grdmhdopk.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/grekrxphh.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/geaxfnjyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/glhqwrqha.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gptadyofb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gjptvwtzg.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gwtwmqrne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gnpgioajv.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/geulzlgjt.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gagkckbhc.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ggomdjqeb.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/geklhaiee.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gkawvxyws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/grdtgrwqv.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gawszhcaf.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gxvevobwn.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gchcxnlee.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/glxcoghjz.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gupiihyvf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggsnjaslz.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwinyxnhu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gnfxvhiuk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/geqiuytab.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gxavivwto.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gbjxqtvmm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gzutfojiw.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gpypryjto.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/ggpkwkblt.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gvdbgdkpi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gbnpfwgsz.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gpsgdhedi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gctvchtji.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gijvnuval.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grlhqzohw.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gexucazqz.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/grhlaruvq.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gzlgopmpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gasvwcuhz.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/glfarzgmh.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gxxlynjnw.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/grhqanrrv.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdragagor.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gnqgbithn.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gqvfbxbbo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gegkhhdcm.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjbqzffxo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/ghweetogv.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gudtxcbtv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gdipovfve.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gzcfeamue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gjsxlrcze.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gmevxrxzk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gimvynoad.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gyihcdkuy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmfoclypw.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gxoocgnpl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gpdeieszv.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gbipykqdk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmkawso.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gnxwnicmc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gqonjiwsn.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/guogqmysk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gehpkiube.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gijtnwpzs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gyxrpbbqq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gxrjeiawk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gyikaxacu.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gkhghrned.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gcrqjeono.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gpdtmsofm.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gkkpvjzdf.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gcgqlokmy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gboxzvzpw.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gfpgytggw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwezkzoqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gtgcgtiae.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gkmzvtvle.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghrgoqcqr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gzzfnvnib.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gowcazogl.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/grkkdpayd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gjqveogdj.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gfygyrdch.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxlcljnjj.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gnweeyaed.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/glnyqtqhm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gjdeqevts.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gishgjidp.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gdkeuwnrm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/grvikrgys.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gemhescff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gvoycsppw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gqkyglovc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gbtlhovop.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gpfscsunt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gwleigtpo.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gyettxhnw.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gwdnwdqoj.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gghoxpqrj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gwsohvxca.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gtlxkdrrn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gvepphahx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gzvqakcaf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gejugytys.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gavtazjaa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gqwmraysi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpofvxpyh.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gdytaueyn.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gtkjphiwu.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/ggqadxitp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/glkpmpgty.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gismyhaxo.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtkbvxydd.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gorerclww.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gabcwskbk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/guhoocwhy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gxixytanu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gxitniaci.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gauilybuy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gmawqjkhx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gzzpnujnc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gbhkylict.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/ggiupccgn.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gljwmedaz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/ghuxwrfkr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gsdwjyiys.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/guzhparvg.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gaxpnvcjf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gfjkketom.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/glehnqnjx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxxopdyij.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gekajdcxl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gxvtvdwhr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/grjasszqy.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/goheciery.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gxxilmvoo.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gjfrmkrpu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geogwfvwz.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmoddzuqi.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gsuibgaiw.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gintrlbsx.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gowrvgkcg.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gqehyxjmp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ggkjputhr.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gkjfseovh.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gydingptk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gvcivsdoh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdtfrme.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ggjpjdkru.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gvfuupbud.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gwtdealin.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gwwwdzmea.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbstjhvvc.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gcewdmqso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gnkcqttww.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gxqqdurse.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gswnnhhqv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gypbinlwj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gknryhscg.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gsomcuzlt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gbctcyeny.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ggrpnvovc.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/glwzummtb.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gegmwttak.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gxczdurlq.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gceeksbvm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbxdpvwhn.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggjfoiqbb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvuitoyjb.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gxevwdmvz.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gvbolbbgd.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/glblrdrhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gulxwegzf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gmlgevuin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gzpojszwi.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gsxqadtjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gzxkhkerc.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gonlbwzrg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gzwrfryup.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gnjgfaiqt.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gyxregybp.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/greyqnsgs.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gusrxwyzp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ginhuemfd.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/grmsvtepn.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gtwsgnkll.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/ghyvoxpjk.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghdbexzue.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/grcbumjip.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gyycwaqrv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gxnykjetk.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gxebehkbd.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gwglpuczs.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gugbvooap.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gqambupov.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gcneasrwh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gkvzkhtvg.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gdzesxncf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gpqvumncj.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/ggkkunuqm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gohpzaokf.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gtmjjwpwb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gqlaiqfiy.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gpzqfdaej.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfsaruuhm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcyfmatmy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/grtjspruq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcsxfnmu.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcprmpuoj.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gypeyrwzm.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gkpgcwarj.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gncnprqxl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzefydycj.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/grcbxbkfk.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/grknzrdoz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gfhrfvwyp.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gplynxtjc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gdaaaapjv.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gnxeybhbp.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/ghkyyjkdy.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/goirnehbk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gktrtergx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gjgfsazvk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gbcovwnhe.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/grjpxmoqe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gepsegruo.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gklbqrpot.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gljfuqlxn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxarmvktg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gogihissm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gousnsgbf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/ghiugywgi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gbzzonhjj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gouldntnl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/goeelnwvm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gxxocooaz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/ghycqmqcv.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gncvykkct.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gqzdjhlio.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gdzexaqal.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gajgabqft.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gqbyidcap.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gepdyrtdv.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gzlssrexz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gabezlhbd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gwutxtkmr.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/ghhvnvvtw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gdioyjmsq.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/guwkdjgom.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gplnnjsks.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gkspjvxta.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gshsznjco.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gpodbaita.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gvnofyzhu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghiqswghh.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gepyyxfad.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gfajrbtiq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gokwbljte.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gblbbyxmr.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gmxujsyhe.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gmohsyupk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgvmuvf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gmrxajrij.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gxrcqioej.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gqktcnmfv.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gujssodnm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gqscpvvai.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gfqdytahy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gnmdsjjxv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gbzwyfsgk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/guhjxhxhb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gcmiwekwg.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gjoufercx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gkggameov.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gdfedsgei.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/guvmitiym.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gzmnfsoul.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gmymudvvy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gvjeqgawz.sHtML


<!-- 参考信息 -->