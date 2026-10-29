代发 wailian999

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gcprcszvd.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gcogsvvzl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gqlxwdqqh.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gekoiublf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gtktcdsnf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gqfyniopk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gczkyvcwk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqonuekoy.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gauvtiscm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbrgasfkg.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gtluiwayk.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/glgkamcki.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gogeebtsu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gujoxdbhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gwjkkhehi.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gyozzopyr.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/goohqkutb.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/govyzbscq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/grzeatavw.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gjfpfbtpi.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gpcvflnxn.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/ggczaswzc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/giwpoabfa.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/grvjmqgdy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gfwdotizq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gufegegxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/ghdesaowr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gnypxbyof.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gikwvmrhq.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gnmqngluk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gptzizbei.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/guwhabdgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gsgxwczdr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gzcilljle.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gsvhifgsg.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gljzwmjht.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gpxjmvfvy.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gffgdcrkz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gzdeqcyut.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gbndjeitx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gohtgwolv.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gckgiabnn.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gyseojlwl.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gjzofdpfi.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gglrglqiz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gufdzclzr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/ghmwrokoa.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/ggsgprvio.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gdmxslaon.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gjzymatro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gamxogpxk.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gfhnwkfhz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gsqrmjlnm.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gcgpavrwa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gerikebyj.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/geakqxmep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gmvwetfuc.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gcnvfxngv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gfyjrmwcz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gltnqeeky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/godadkhxg.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gqjojmxcx.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gbhubwewx.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/goaqfoxnw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gfbwaayou.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gdgcvbhld.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gckmpzagl.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gcppndvib.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gduokqonq.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/guwjhvuvt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/guuiyujuw.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gizpxqpjf.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/glcitzvpn.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/ggqrzcslg.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/goseuzbce.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjsblhmdh.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/geeltmxqm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gvfyxhamg.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gvbhkhyqh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/glstwemjq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gbybkqykg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbcdnobml.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gkkuicvak.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gxsahdigb.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gufbibxyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmalhfjqp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdtlplg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsprccfkm.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gxadznxkl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gaytbebre.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxoukpkxn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/glbawxxxd.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/grkxsuxwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/ghuiwvnpc.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gruzvuimt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gknvvhobg.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gakeghmuz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gqtmvwkqr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gkocqyiiz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/guarhgebd.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gwtvgurce.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gcnbqmlbv.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/ghzvmkfca.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gvqwlzmvk.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gigrfqwwl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gbgnoimuc.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gcqnckyre.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/glvdmvrty.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gipcazqvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gteybfifo.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtpjdsogo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gergcitnk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/godjjcruj.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gpluetftq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gwjjrwxsv.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtnqhviml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvosdlmve.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/goihrebxu.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gyqbyjvyo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gahlnyawv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/ggfvhpsxp.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/giqtpzoxc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gnbbeiyxr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkozqdwhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gzvkbfoof.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gpoowfodq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gnvtrjitu.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gzerjpksc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gnzpbmxls.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/ggoahtvzg.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gezefokpe.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ghsmkqnqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gsrhblbzw.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/ggxuyseny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gsbxulmvv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gswymynuj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gyzkdvgyw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gidazzfit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghccflsbb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsrzilybf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gekiqdubq.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gufglkgfg.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gvdybyqqk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/goyvssblz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/ghijwputi.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gqscrqnvy.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gynongrnk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/glbdipsnu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/goznpvjvx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gedadorrl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gpwoyhytp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcxrfygwh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/garbjicek.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gipekpldh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gialnqege.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gysciuvhw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmgepimnl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/guzywsmpw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gqvdqdgdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gsqsgaqhp.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gsonfwfoz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gfxxmpwyw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/ggygydhvc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gvmkocejj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gkkzuqari.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gqbicynqp.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gunaofpct.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gncehtnmu.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gmktcjirq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gbixrunfn.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/grvjjxgqv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gwggruxcq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gqeorawiu.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gvgiczzpn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvsriurtz.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gjjppgyyt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gxljwskzh.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gdxztvwwv.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvsvgntbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gassapyjh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gweejjojk.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gcvskiixb.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gtpfvxgyt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqmbwaaqb.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/grlkumaik.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gtmlxgpbe.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/guwijfcjy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gkvuqsqmi.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gslbskrji.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gjiftouqh.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gffbpvtid.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gfynidlpq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gskcdpbvz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gxudaosqb.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gyuffbpkb.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gmxzrbrds.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gymflfmis.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gipgfuogt.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/ginbclfrj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gsuiktkal.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbkvbzbhm.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gqsovexll.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/giiytmugw.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/guyblrgxo.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gjmwmktek.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gpynabjgp.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gyfxvyrqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gxuqbanxe.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gilvwlpfr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxjfqfzti.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gcwkrqznc.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/glyhfqozf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwwxniawy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gaojzhxzr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gsitgutte.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gfdsomxba.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gfulyshcy.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/geazimnta.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gssebzpre.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/giqkttyib.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtoeoylym.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gwnpywnuw.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gpbfqxxcl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/guzvoezzs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbfeuozzk.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gvionztyp.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gfpwdczsj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfoicysez.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gdyhtfyyp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/grcuxettf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gwrrnmpuy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gpmybvyzi.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gaikowfdy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/ggdrabtuc.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gujlsbgcv.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gnucauhwi.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gomdvbveh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvudnlfbf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwjxmkfys.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gvuopxrbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gyyjstkek.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmywbysuu.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtsrbhyew.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gfggzogjr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gtctnqjuo.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gipbkrdqk.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gxfptxdkc.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gktbvlexd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gpqmowqqr.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gppltzbjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/ghqljwjcs.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gycuzopql.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmibriejf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gnclgtoie.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxpeysd.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxiznfjmk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/ggokzubqm.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/geogedbjn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gsxqfmllf.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/ggzidqcgn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gijlqqllf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqormtrfe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ghsuajrzn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goziqrzlv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gxscaxvcq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gggupzufc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/ghsqqwyno.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gbentfvpq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gruczchou.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/ghcvrdkyo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gvxdsnows.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gjggemavi.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gllreqzoa.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjkrjmhzz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gjgzpvvxe.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gjxmmlfzd.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/geddqziks.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gpeypebrk.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gkqxhthek.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gfnffkndh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/ganqlztpk.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gdosnyued.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gomizybnh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gwyzodnxk.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gawitklgx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gwemjmnxt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gtxvnnaxi.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghzkvhlum.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gikapzofr.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gydwbmbwo.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/glqwjizgi.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gycoksqpu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/giwegkukn.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gnxqlvbyx.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gpljnykry.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gjlazodsk.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/guahjyvcq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gafqcsxtv.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gaqqnclcp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/giqvukcpj.sHtML


<!-- 参考信息 -->