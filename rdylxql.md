代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihwvpdt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrzasnud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gozwqbjmk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnoguojm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvrfftosp.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhlsted.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfhezzix.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasndgseu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcagexbu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuusplrw.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gofotzkyc.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghupbxddt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gemfsnjwf.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdcnkqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuxnoui.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glypmuwji.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuqkitan.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtzmfnaa.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/giignzqzf.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/goluavzpd.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpulxha.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gferimawt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkcnkyus.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjuayty.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaactzhlb.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gldhbasnf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/geyotflkk.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxuanywdd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gztrptpcm.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ggziicrqu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqgdstrn.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gvevvnsaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/goyyoeguc.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/giklsisqu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuxjgmab.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzwjakrb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmzopvl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepznout.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmjtndim.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gqjljnhnm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkqaldcx.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvwppzpcz.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtwcptdc.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoqtyrfw.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehfhzba.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/grinuwioz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdwcdrxq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxekfjby.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/girqndeqy.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbstrju.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyceznot.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnhfbypa.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/givdwxreo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gazavhcal.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzrvcltx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/guxxbtgur.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcrojmrv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gobwgujho.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gbdlfgcso.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfamqdzpg.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiqwtszs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvtabkfi.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gjtocbwth.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gokbyrfzw.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdijupqff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gufcndhca.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqruukkr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggalcisbb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrdlvxpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gfghvudrw.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlunzlrj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknrwygl.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghcauemug.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gzwbenoug.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gulqbsktb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbozazn.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gaotxgdqx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gtgkbpwqe.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjqkxko.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvoxkrmjz.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gneikylcz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzvdizpbc.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gnvigwdia.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggjapcynl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvrksjvuo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbdaizci.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gktmvbpvl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvtqmvva.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtftiigsc.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghazqzozh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfvdoewiu.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrancmh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwfxjxep.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwzamejhu.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvnosfsai.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqebuho.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcdeopbc.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gepjdcvqo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gktckapgy.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmsvhiu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvkkxwav.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtrabrdu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnwgoclm.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gpflthxxt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhfbecs.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwehlfvtb.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghozvgnjp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplacoqgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/ggnkbsmbk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhebgeqb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmgdlat.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgqdvqv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvierdy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaxzgohx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwpbnxz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gruvdoxjr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmxrhfmo.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gifaskyoq.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gciyacrlo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gkrtepchx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/geqghvkfo.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gsmcecwhz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gyczehihq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqajipe.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhgfdog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcjjbaoe.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/grbjrmkbx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwhrgfjb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gztwvdryv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwwdvvjy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrbcebab.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcldlkcia.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzizjubv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gjlpskghv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjjvppqjc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gocdkwvbz.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gcgixhkiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdssavfrm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gqicddjsx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizydbqbi.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/glboxiajs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoefagsy.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxzeawttc.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gomikzqbm.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gxynfkdpm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/glzivflrh.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtrutvlv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghnxlbpzg.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gsgnlamsr.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzgdbdrkr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxendxzhd.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gsngbqekm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnliwdrju.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzoooniu.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/giwvptkkx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfzyyehh.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/goswnzona.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gffzzzbkm.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgfuuwvf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhjkpikj.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiextzgy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/grdzymzdr.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqhztuml.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzotxpvue.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gymtfwfae.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtctpmxwd.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gnawppfna.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gvohvcrdf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjiooowqf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnojqyxel.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfhxwgdg.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnzkwxov.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gbftkxhmx.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialoalar.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcabwqti.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfphqyydd.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmxdibjx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdgrjorr.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcjfgaqzt.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnrqoggzo.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmmtwin.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gumocldlj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkehpkelq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccyhtty.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gctbqfcor.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gidadshac.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gunocxhjn.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gzwwbjomm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gknzfexyj.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gethrovmp.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvofrbhe.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gmlgpsius.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gebeqigov.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyykqqeog.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfygtpofx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gahvgzuam.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjehehvwg.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gttkedzdu.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbvcsrlq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzssebfdy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gybuthfpq.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gkvgxsyxv.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gromucvvj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhevzdco.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gesdyzkqr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gperjhzix.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlfdlvhs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxkvqbel.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gqffpendq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqhktwiqx.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqieqhzpw.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwnpocaf.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhhrvrh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhntwasg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtnefdq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhqkxchx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnqdetvwh.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvdufjd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzwchnpk.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfjenegi.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbubtiefg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/grhrplgqj.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gyihgsbuz.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gbooleaqg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfxkdriy.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxssjnvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgbqsaz.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gjkeemdse.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxuucuaq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghczvniwe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gshzyisjf.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikilvyx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdqnzwon.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwonrenj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gwefmupsy.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsemeyrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geujnsuir.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkqvgafr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gsipzdzxq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqeykpij.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/guyhraaoc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/glrwboivr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gwlelqnxi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gathxjljy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhoipioc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqnvwfvh.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gagonlntt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gbpwwvnao.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwftfdald.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/geqzmysgs.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyegilxaa.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gckvedccu.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaakebgoa.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gigeodusa.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbqhawq.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsmwggmk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhhvxlz.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmindzufq.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/guxvqtekg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gftpoqpsj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheprchvp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecochrcr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqfqrymr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxswfjikb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gutiywlyd.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/glrggzsqh.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzodtfei.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgcusax.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gftuwuxia.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/grxblvxso.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjbovcte.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnadogcr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduznvcmz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdbbtpel.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gemoojmjd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtatynwsf.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpgnycmr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpncurvhz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjrylfbw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvlutqmr.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhggrtqy.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlfspkzc.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/goudwwcaz.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gdteacbvs.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquetrgin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/grfmvdhmx.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/guhhefrep.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmjtwer.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfwfrrgr.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gvzxlofzr.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gcgqhywsr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgukquyg.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxnjfzlu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gbobdpcpc.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gheuugvej.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gpzsodmfx.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gkewaxrlu.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiowthxc.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghywoadwb.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqkbegwq.sHtML


<!-- 参考信息 -->