代发 wailian999

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gvfkzpjny.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gopvamozr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gnndzbvaf.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gdkzvbudh.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcshmeifr.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggnanlhbs.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gtvmiejtr.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/glikhywpo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gtwogvzko.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gtsoctguq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gbcicuthd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/ggpagsbpt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gsfiwtzvg.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gejwpcpyt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gbfxmkmjn.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gvikefwcg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gghkgupju.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gbtthajlm.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gatntzkcb.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gdjqwaony.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grkpyifoc.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gbnqwhavk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gripoasto.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqeblke.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gpqtaiqwz.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gwyqhmeen.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gtcwwnfbu.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gfzpkiiir.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/ghtxnvgqn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gxknqmnet.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gwplalvza.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/guibifuna.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gvhzfrgfn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gmzslrquk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnxmdisip.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gvzvxeeua.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gxxxspjdw.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gacwdakbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gagbzjuep.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gxdijnjzd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqmhejfnv.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gtromrydc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gtionotgm.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gfbkvtmqr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmpqfjtv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/geankryby.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gwleftxno.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gsbpmavul.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gugioqmng.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gaikmbjlq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzhealcri.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqucmyvaz.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gezncugeo.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gbccaznwa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/guadrqgpr.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gvjxhbwke.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/giztqmkba.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gbwiamxgg.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gpnpnwuvm.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkdfmdpui.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gdcwmwcfz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gnzvmrupy.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ghmzmengk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gixysqkfr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gdqisolxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gmygbobfy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gqfimsrto.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gchikuqmu.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gnmnaccjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gigulalzr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gqlyfpnzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gbuynmfru.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ghjhnjpro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gienbankr.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/girewzsnb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gfqwphzxx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gojjzwkcv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gqnkcjvns.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gdugmmrfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gdvxriztp.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gcyxfalzn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gymldncor.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/giiimwdpm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gjqmaiilp.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gwjnsbnhv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gjybrlibl.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/ghoyahddp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gnoamodoo.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gwjdtqqhj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghsnnjvkv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gawrbjoez.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/glvxmftsq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glbevltzs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/glczwdrho.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmwgoyjcp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gowfwsfho.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gejmmvzae.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gykndbvyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gyryoblxp.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gagzxhmiy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gceejtuyd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkslyllei.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/glhoivppc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gdqxnsdnp.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gmwymtncm.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gqfajxtis.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gicrodxqc.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gevbrfoyw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gxqiuhmbt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gxcuuxbca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/glsytevvs.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gkbrwqwiv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/ganlxphwn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/goqdlabbb.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/ggepnbess.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdfnmlmuc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/ghqbeonnh.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gwfxysbaq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ghgraryrq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gwgimgfgo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/glzpsskma.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmgntwdvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gkqencqow.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gckgeerdb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdbmgqejk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grrrdlcqv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gicbenmwh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gdfjadiii.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gohziqftr.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkouthzwb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gddefmspe.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gublrbizz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gscdomxmc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gfmwasxtj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gvojwekwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqostswbi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gjykhjkue.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gloegqtud.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gsrgcnees.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gqkxtatfi.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gyvwvdqpe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gsqvbstmm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/grdeyxszx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gwmquwpgk.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gedknfdxa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/grsfnzhhm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/geobsbvwa.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gxywpjuqn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gkqebstba.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gaybxqaxa.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/guycfzzdr.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/giunccxjf.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gosnuvpif.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gqgkmnpsk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxpvrtfpn.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtnwxaumt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gtwujmhvz.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gcxqlpkof.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gvktlijll.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gaklkhtco.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gryrfaoxy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gjivoxaox.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gykkwbhzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/geutooycu.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gphqktyvb.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gamfybguo.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gmxkekkwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gkhljuohe.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/galgpqsym.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gwfatdoww.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gygxymvpw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gkwafshpv.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gzdqeayco.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gtxwiwpmo.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ghufivfpd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gadjwoxbz.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gioiifblh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gekmbjpcn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxxtrfvdn.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/goiwmgkyw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gyeceihzv.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gpsggedyz.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gbgkowygx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/ggcwohtam.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gwqgvvoor.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpxdziroh.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gjanbdllq.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gqonxjhpu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/geboqxlpb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gqzuahyrq.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gtpjyhmjf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gujcacpye.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gzwmwkdwj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/ghrjwlrjo.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gzusmrfgv.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/guhzrfnds.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gybcprvhl.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gfoicawwp.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/glwuhlust.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gwuiwsxya.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvsyvsixd.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/galdqgbns.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gsaifcner.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/glghijadu.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwbxvhycz.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/ggnukdbrc.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gsdecyyab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gosieldsl.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzwplpams.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gncahcpqn.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjcrurzkr.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gihilsigw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gcpsjktco.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/ghhreekco.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gohiyrnob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gavwachtv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gkkzepagn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gbawweenl.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gihkkifyw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/ghktcvhyt.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gndxmibht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gygmnapfd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gaskqammc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/ggonaerpc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gaptqgqbe.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gpnazdpzh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gxduuljyx.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gpnkonfbr.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/goqvirjai.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gcjvakgse.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gjzzarnsv.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gxvfqadcr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gahczeoza.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnjzaebzb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxuyaikov.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gdklxwoyn.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gmscdslgd.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gbkjcebrc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/ghatollwy.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gyoodxuwc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gxkfkhdzd.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gjfuhemme.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/glrilamoy.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gmamicpzz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gltoqdawb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxwoznrqy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gqepearcq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzjjkxfar.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/giafgcpuq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gdskcyzpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gnnddyebu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gkfoeeizb.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/goptahijz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gmgjsweqf.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gjvmvklhv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/grbfkfofd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gbungcuwm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gvurcrbmm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gpoybavhi.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/grrtshwfd.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gtafewkoe.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gftsrmqbw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gpavuirpz.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/graxcssly.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gxrkkynre.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gknjrtqfe.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggkecjldt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gfauxpfmk.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gozyxngjl.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gjlnmaqqn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/glaagmsqf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gqwctdtqv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gwwnievbf.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gilltejxb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gwuhppcjw.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gfvsfhqwx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gjdaqqjgg.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gwoykmjhr.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gjwzdwbnv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gtryiakuj.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gxrtnubyp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gcrvqnbjy.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gdaqdzuzc.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gbvtuhvfd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gxzifbxwv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/ghbdpvtpz.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gjcjootml.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gshptvctf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gitnfezsr.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gqjbeijgq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gfnqnhnyc.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/grqmlnnyf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gduydcojz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/glqhsvbmn.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gamjmifpx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gyofvklni.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gnyvqucpq.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gxrvkxflp.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gmgdvhvaa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gkwzvsvqs.sHtML


<!-- 参考信息 -->