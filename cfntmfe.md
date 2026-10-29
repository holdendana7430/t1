代发 wailian999

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gwsoqcoya.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gaerniqdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gmhaeacvw.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxkufbvyq.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/glcwxsoky.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gvwdrtqoe.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gignudnjx.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gygszwosl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gpnxumddg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gymojmzjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gtqdiwpvz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gcgbiryjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gtxbfkmzx.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gzqrmqtsg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gcmsfrygq.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghfwkeiuf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/geziimvkq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbstffgg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gkdujsauk.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/getbxuijm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gtbalrchp.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gnbmqtkmm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gjtkwjkmi.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/grirfsqph.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/ghborhgov.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gxjobsgbd.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gpyyrwmay.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gysksxyar.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/grpsbfdos.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxxctwtry.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gkoujdwdj.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/guzllforg.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gczbseegl.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/georkddlb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gvjhtdzpx.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gxvdomzio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtcstlapf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gkdmgsoej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gbcwsbapf.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gxcsmwkhm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gedpowrkr.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/giswbembf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/goonbsmsm.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gdublqwqp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gqsfyxqnz.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gzwurexhw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gengsqtgc.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/guknneezx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/ghjdgzywu.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gmrlhrdil.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpbzzremn.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gtlvqlifr.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsnmiqbmh.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/geoppckis.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxdptfdjd.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gafbmgyhf.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gtunngaur.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gqdkthetj.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gqtmwggvm.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gncbhpqak.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gokfmchqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gmovajtjd.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gdlruinrp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ggapzanct.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gmyeyvxnr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gwjjthwxl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gqnrzrpnr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gsjpydywl.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gnjmtxexh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnemchlim.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gzsnsreyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzqlvwuxw.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ggkjnhsvf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ghdneizpw.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/ghziqmsnj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gwnpqcpqc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/ggjopcgca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gtehuxowk.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gpazgnxfj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbshrayyf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gmqzjpyxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/grfnvpjgd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/grywlwixm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gmocyomcz.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gcfvmrmht.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gutjcpjsu.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/ghnhblkrz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gjgrgtdqg.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/ggfkmlycu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gcvzckkog.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gxohwqxmr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gldllbnod.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gghkvxhmz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ggzkqgoyf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkaebtilj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gfghtkgrm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gffavocnv.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ghmkrrcvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gtwnidcuu.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gkzmjtxoj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvbugdmub.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/ggwsgyipg.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/giahoklhd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gpypggkfk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gbcpccdqy.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gkdhwrdfz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gazeyvfjk.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gqrpcucwx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gedhbqfue.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gfsppgvpq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gebtpzrto.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gxppqmxkp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gygajzbix.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gkjdjsjce.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxhuhaggn.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/genglafqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbuldif.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gwphnbjzb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gjgovxdej.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/ghpbhstpj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gccepjmea.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glgkjqefe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gdtcshggh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkhcimknd.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdnsnfmye.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gobuucber.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gooapkjol.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gnsmcnuqn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gvahhhqdp.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gpqzgpgty.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gokygxaln.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gpgwdnlhy.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gtfnwhvjk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gdffmzdlc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gjjodtxvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/ggrkcjfya.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gdrjeopnn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gyaxallnd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gkebbvtov.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvatbeo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/genxorwfz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gpczjmbes.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gotshmldx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/giulyxced.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gtgcbhuej.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/grhwqkkcm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gyaobdgzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghtxutqpw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gpovcpvjb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gvzkwylmr.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gkjleqwhg.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gsobtozta.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gleagvoxi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtqselyhz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdtmatzzh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ghkuuogpc.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gxynlimkq.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gjpugipwv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxoexmomz.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gchzpglcc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gojymnaax.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gvtpnfznf.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gkthqdidu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gyxancsxr.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gbcxsztoz.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/golzwzoyr.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gywcvbcfa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/grcmfwfqo.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gabjtqktc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gxvstrvgr.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gcyzeejfu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glgapnfcv.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gmtshbpud.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/grpasbvgp.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gmifsuuog.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxupkrzqk.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gpdkgctgj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gpqwrgujv.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gyakmhqre.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gjlxtkiou.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gptloswcl.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/giisdlqgc.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gqcelsljf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gofvlbutf.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqeoltwlo.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggaippvbf.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gqpjckeon.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gzujbgjib.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gjuqnlifd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gmmvuzlpz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/golkbvpio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/goshkwtsf.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gqxwiwpnw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gfgofwvji.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/grrmgrsif.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gupoxxguz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gclztyvdx.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gncmkjrab.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gvunmcsiy.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gewqyhweo.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gaeznhtnj.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gflscbmzf.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gntpskhjc.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpvmjwe.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/ggygwmowh.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gyjevxpvv.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gxwmtbrqu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gfgqewgrk.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gawhjlloi.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gbavwmbtx.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gxxtznhhq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gehamvdfk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/geejbvewr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gwdeecvlx.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gxpyprgpl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gfvgeckpl.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gfqnefvsq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gmrnymfyc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gqgzxrqnh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gypzdtyny.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/grzszudqq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gstpyzceo.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gmsbjyfcc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gemiuvrsd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gttwrdpdi.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfkvdqflo.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gijmmehvm.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gcesaksjy.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gwufogwok.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gnwhvfsfx.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gdpjgccoj.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gooshgkzu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjggogzql.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfotjlmni.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gmjdsgaju.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gqvdernbg.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjiotkjrf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gmsfgjfvm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/ggafyqotc.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/grbrytjzx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gohrqsqxg.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gmhgpnybx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/glnhhdsir.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gxairwoud.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gnsanytoq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghsqtmkkd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/ghpsodaol.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghvqymqlo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gqmbagkeq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gagxihisf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gcgiwbyde.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gbhjyklpc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gfpgusymj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/ggjmofxlg.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gcmghndog.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/ghhinlcub.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gppqtkdge.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gobecnfui.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gegyugctn.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gpocoqyaw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gajycmnep.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gijjxcfdx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gsytjqjna.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gqzfmhklp.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gyukffzke.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gauopucsv.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/ghebyacxr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gmpadlyyh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggzhelnfe.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gszjkuolr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ggxufcrve.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwlepsjys.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gloczwxiq.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gafexfwor.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gqyosduvi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gaweurwrs.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gmmoqjkpd.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gpeioefha.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gqvnpawcq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gwbbclptw.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/giisdzoiu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqakyjc.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/guujsdwex.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghduxszxd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/guimabjpy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gosjhuxif.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gpoiabsmf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gwqtsonxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gtaxijcfh.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gixhzuftw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gmowxvuho.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gvzouhlkz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gubrjtrxd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gtgoeaxfo.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gkzrryodf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/ghkxllplf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gjfofyouh.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjaeayvw.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gsmljywqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gvjrdlxeq.sHtML


<!-- 参考信息 -->