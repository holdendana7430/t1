代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gncfxvzxh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gddscuhwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gbnrqdcxe.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ggwxudktb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gqujuxmtg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gnlogvhqg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gvfseepzu.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grpytlsjn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnnkywk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzliwhics.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gvxtoskan.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gducetxch.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gnowvmxcb.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gpmqzrsls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gpnrptlmi.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/guukexwjo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/ghrbjljyd.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/ghhmhskfw.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/ghrunrtbt.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gvmsvegwg.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gknxselsd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gsqmwjouc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gzjweikvk.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gmjypexje.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/ghhqscsdu.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gthezyfah.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gcsjapqye.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gyqjsafxm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gktlxhitz.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gnxaeqoxv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gkmbrufeg.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gxgxobtih.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gguxouapi.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gibgekcay.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gtnjysamp.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gixvtwifg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gpgmqomzg.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gzxrnobbh.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gqgrumlmz.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/grdhiseke.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gynecgdus.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gmzdeepdt.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gloiujjcs.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gljizuyor.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gijsbnjpz.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/geqticwcl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gjgcrlqyy.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gopbweara.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gjydeftsp.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/ggtksybwz.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gosubexsi.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/grsyhvyqb.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ggeafqxqq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/galigfvkv.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gadzrvzop.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gqdhuxxdy.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gugwjsfwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/grbovjowm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gatsodkww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gcjqttnep.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gyzdqzwhe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggsfnlksn.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gwdbsykrs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gzllqyjeg.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/grvfllpmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvtujpwcg.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gzqpjmxdn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ghalpjjrl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gadvgthhj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gvsbotlbb.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/ggnklytri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/guuholyvs.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gybokmhau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gybagrbok.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gkbnuxsqv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gwqwihqwg.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gcdfhwxim.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/ghtvyrwly.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtsufjwts.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkogktbsf.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/glvnstiqo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gpfpqwovb.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gdjwyiltc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gfkygvqqq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gurzihyne.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gyqctwodh.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gydwywodd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gavtjxpzs.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gfykrhcat.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnyuobywn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gijctnpmm.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/guinyqhrm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gejqlqepi.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gjicmdinj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gwpwlxvjy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gtistoirw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicileoml.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/grcxqlhap.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gdnyescpz.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/glxgztlyc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ghcgavdre.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gkzfmkssx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gvsnrgksf.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gfkdlekfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gacjvgudf.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gtskhhpau.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gxqmlkpgs.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gjfilsfvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gjrmdmfus.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gzlhnfeti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gmtjzpkyp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gjwmmnmnm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/geuexmjsj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxxgaaxda.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gvtvqqbja.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggdcbzuyr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gngqoucwz.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqxeizlkq.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/grijcqpzr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/glksldlvo.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gxbgmvikk.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkvluwvlv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gmagwzoee.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/grjctuyrr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gmpqaxiqq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gdfgobrtw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gqadiufgg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gyzstckql.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gxjnblgdv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gqpgckspa.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gzdfqvpty.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfxsshlnk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gonwdffqa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/glkwqjxwk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gsdndasqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gppqszfbn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gndhgyjkn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gkywyettk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gegcndasb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/giwbczgsg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gplifjhkq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gbdbwjqmd.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gphidnkfs.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gtkqtfwba.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gozxfbicp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gifjmolpg.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/giebiwota.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grkrbetml.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gwmfehwcp.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gmnyicmvw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcemxjefs.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/grqwqjyut.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gglnefohn.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gestqdchk.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gwwynekbn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gajktxfxs.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmhzwlhnb.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/grllmxntn.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gsejlugki.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gcgwrmomp.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/geztibydn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gykzjrxom.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gmgmilkrh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnxfguxua.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gxfmdvlps.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gymngwotg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gskkinejk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gqgqrvxdp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggqldqjml.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gcispiswg.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/giwglvghs.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/grsessfaz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqgnczbff.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gosbcvcbf.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gcdxoupmh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gohghresh.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gtpvmvtxg.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gipnkuzhs.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gjocgakpi.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gflanwwkz.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gryttjlcj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gsvskzdrt.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/glrupvudi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gmbtntmpq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gdjnfpupk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gasvwgnnp.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gohmpmcxl.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gcwfzuiia.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gutzzmdwa.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/ggnlrrjwc.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/guwetcmhn.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gbayivziq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gwelyjuvz.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gexbfrlst.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfjgqdhsa.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/guyfqvoxs.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gkbuamusq.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gsgiqosse.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gftmwhiuz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gcjvbhncp.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gnuijloqh.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/ghvabeuhw.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gukyndkef.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbwcgmnti.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/goyrzzwxy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdzxbirkc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gtffawrxv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gowviizen.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gvbxvwsni.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gzfcdjwkg.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gizdnrlmp.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gnfuscydn.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/ghqycvftw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpafncqff.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjserdoob.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gkkvizswo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gmbnezird.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggvlqpagn.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/grrtbwehb.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gamhxrriz.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gumenccpq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gpvgebmrr.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/giyoahnih.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gzaxeokor.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gqwunbdpq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/geqiecshc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gdbqhdaab.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gsbepzgpf.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gifebjwsw.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gxhfrmujb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gzxijveel.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gkiajygtj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gmnlwgpoy.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gmikzctoc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/giuxnexoh.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gzewunaua.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gfeikneqz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvldcmcgd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gwdiatanj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmotvjxsv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gkzqvotgb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gwpfzwvgp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/grywvdnhw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gdawyupvu.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/guypxbbad.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/goaazthwp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gmcejyinb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gvjgkibee.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/galzvvjnv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/ghnxoranw.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/giphxnlbx.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gchiifrqe.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gojnpedlc.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/giyzarjxo.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gowlbxxgv.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/glfvaidjd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/genzwuleb.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gaqohmeqe.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/guhpakhrj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gtthsxgke.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gxiyqnkgp.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gfgdkhlll.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/ggoozulvn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gnqfyxkxx.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gubygrell.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gaefqdaue.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gxdjzicjh.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gqlwdqqwi.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gpexrqkit.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gqucalapy.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gnajimqyi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gtvksjcgt.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gbehsmsrf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gogmzvmrq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/glhpgqiiq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gcredndlj.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gyzqodxwd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gvwrfewvx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/girldkexb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/geunygqsn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gcdvgpwqc.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gsfeucaik.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/ghagwbkmv.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gtvkgcezn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/grehebket.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/ghfzvtgtv.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gmwjdknym.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvthnbmoj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/ghtretovv.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gsahyhxzx.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gvptnyjyc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gicrwsxka.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gbijqvmnq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gbqwyreyf.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gjmknglln.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gwkcftzpk.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gjhcoirjq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gzljrxjnh.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gayigxqlq.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gnqptpkva.sHtML


<!-- 参考信息 -->