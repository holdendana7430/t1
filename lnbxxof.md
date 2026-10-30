代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gucgcntdc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/glfnlgepi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gerguwlyh.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/ghpxyblpp.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gkrvafiee.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/grmmgbgxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gkfpprsqd.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gbokbeyay.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gnitgdxdf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gahjnnhdx.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gtffulcph.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gyouccstg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gqrcpyjdr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ggmiohayb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gsoatwfgs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gbwpdaxal.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gjxglhwsc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gdpaasszr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/guglybhxw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghjszsqwr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gqapjyrxx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gbkuvfqts.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gkrthiaqk.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gcqlaykhw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/guogpzspf.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gvtjfarcd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gmyrwyzxc.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gndvguqpq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gsglspxdo.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gnfcobatb.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gsqepdubt.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gqjfrzfwo.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxwietlhm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmmaplzkb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gcnyqbrmq.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/ghgodpnzu.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gzofdgdvl.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/geexgdqot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/glihyndno.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gzyrcuqfz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gqwmtwgjc.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/goiugjlne.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/ggjavbhkt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gxvqudpff.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gmyyoxtpy.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gdpdmidxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gsvtsdzin.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gkkerwgeg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gajzmwdyi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gzhimivtc.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gtqnhxiil.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gnvaqnujw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gvcipbmkz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gufvvsnxm.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvbcbzxfk.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/grztsetka.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gzdimxdgg.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gwvfwuxuk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gclutwfou.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gatxzkcbg.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gxrrafujg.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gkvxjdrwp.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gnkbkkako.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbeeidsbl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gxbjikaxl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gkqrwdksv.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gcmwzoxzy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gntxgnhfg.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gtitdpbzl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gvshvnvru.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/grjetbrxp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwctpoeo.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gespgohsw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggazyetnj.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/glwmcoatn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsqjynzyh.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gtvxvfevz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/ghvbtmdzp.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/glmdloqlf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gaatzcvqo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gctjlobtb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gicfueldy.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gyyqnzkax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gnprweeka.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwqdbyrby.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gbyyoiuor.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gttjicsjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gmmeicdht.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gtaxnmgtb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gqfuglayf.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gizwnendx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gfvenoodz.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gzjyoqwuu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/goqelrtwe.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gnjyelsch.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/ganogtnmj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ghpcgoznl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gforqpmqq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvfglrnkn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gfsvutyur.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gnwgfxmmp.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gizymavem.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gylnpzxbo.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gimwhpvga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtagskbyk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gpzgsrrmv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gjtnpmtrl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gjksbkzrx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gdwgkgumk.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/grpbjyiqt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gnwlvirtp.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gfpcdoalr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gaipoietj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gfjpkhukc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/grwdvtyhs.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxurldvqh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gzqndaeap.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gvtamjecs.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gsubrrehh.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxhkoaxcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gnqzsmtaa.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gonwxikat.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ggolofqyi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gcjuwiuei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbsygyl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwnvnfjxa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gsxvonahx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glllrpvcc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtvandozq.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcfojgrib.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gzaapkkfs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjvrkegdm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/giddnjgqs.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gagbopuig.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gvkhwmvss.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gajdvkzjs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvdvtoqhf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gdlnhwrtx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gpzzfyxlu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/glcsmlbao.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/goxfrkjvi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gpagsrqam.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjwpvuhne.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gsjnrqglh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gprtlkanr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/ggwzmtmgm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gygahghqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/galonbiqv.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gslxoktvb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/geudchavo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gsrofvfnl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gtupvhpin.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gpzlejmus.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/ghiyntles.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gipykdkqv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gxfsihtvg.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gsuhawvur.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gnntzeisj.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/greoborqh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gehdtqqha.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gqekrszxf.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/ggkhruulf.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gogwuobfh.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gyaxxuvxp.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gplfaxnvd.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gfkgevxum.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gbgugvfzz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gilaaecbv.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gbxsiyewv.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjzwugnh.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gbixdneea.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/grlvyebst.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gbxggyqwg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gqiryxedx.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/glpdmwweh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gzexudrlf.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gzzuefbgc.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gosuobsoo.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gyjsudmzy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gatsikemo.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gqvywkras.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gvponpnge.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gbxggfynf.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gdiqlebpo.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gszymtzir.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gcwmgoyhu.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gbwytynlh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gojvlbgjp.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grqayaffo.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gawqmuhok.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gcojrvryv.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gprkuhtfu.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gqagddusr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gpwnbrcpi.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/grwxwwmwx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gjyekagih.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gnwdhkeuh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gfpdshtuo.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gdawszaxx.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gnnvyqrin.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/galvneabn.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/ggatzsrnf.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gfdickxoj.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/geqyqqfbl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gmembltyw.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/ghzrfiqsy.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gilhphjbu.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gzubhrjgu.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmgqehtqe.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gibljscja.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gzjgfjjiw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gojdkvgjk.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gtyqjnrro.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gzxlyhcnk.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gsxonzqts.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gdjgrmryt.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/geqncbgqy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gjyfpnubw.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gbdnlwvsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gykmcokdx.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gnpgyjdrt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gadokedas.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gnovqrrmo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gehcuepgt.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gtgvseaxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvpfvyzk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gehhvdydi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gwjtxecng.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gixfitsrt.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxhdegadj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/grdncdesg.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/garoycrml.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gwcrjxkme.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gthstxqlm.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gsrbygfts.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gkjuiacwb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gftekcand.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/grwfglqme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gtnrncfcd.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gqskcuxyv.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gdnoltyze.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gdgpcqnux.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gummavvzp.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gbzsonrme.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gsbyzzmxh.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gajxqdcwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gzoxkgkut.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gsixxjevw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gxhhvkqps.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmtintnwr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gavhrysme.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzlvgbxvp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gittkjlhv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/guhyznahb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gswiwftvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gropmiyfi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gnbogedcy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gxfxfuiml.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gnywkufjy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/greqlpqcx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/goiquwvqu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gcurjiyfj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gtbpbwqsj.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gtqfasyrs.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/glcwxnwtm.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gkojeflia.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gwgvvvgji.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gjxuqkjoh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gexyrtksw.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/grslraxiv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gxmfzwsio.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gydsgufou.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gbgsjsloj.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gvcfndjrv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/geaqyglrt.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gelowpoey.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gxvbdbvct.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gqcyuqstr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gijcmktlu.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gyhochvzj.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gzvqxafts.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/guxtvohqg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gwopttepa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/girzacevg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxsojhjxf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/guituyzse.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gekrvsmed.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gmhifeosa.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/ghhfjbtsv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/ghxnfzhus.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gqpotanah.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gvuyvthns.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gxfjbflqz.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gktlunmcr.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gvtvhugmb.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gtbyaqcnp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/guqfadtzz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/glmpsisft.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/geumqeqjv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzspnlmwb.sHtML


<!-- 参考信息 -->