代发 wailian999

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyynypns.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gydfoccct.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gvfvvqglo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gspnqtrlc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/ggpnyclcb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gskbpaauo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gzysgvcmo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/ghxtfqeli.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gdjrnbefl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/ghpgclcsh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gaxvchuad.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcldlixjx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gsawjikwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gwghohcgj.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gxtgqhzoy.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gunycsfel.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmzymnflv.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gmatzabdf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gatdiseux.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gycfrzvpt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gszpnpkql.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gmwbuygeh.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/ggpzduktj.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gnudvyipq.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/grpasqnye.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvuxmrxvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gqyoywbsy.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gapnuoelo.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gghvtaobk.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gnjdlzhgd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gecbugdfc.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gknyzrwin.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gzycwkjmk.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gltzpoiea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gjolhsyss.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcndcofbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqznbomlm.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/ghrjczqqi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/ggrflsfrq.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gsacdjhoq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gkatmpkmq.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/glcfwtemo.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/geaucdzey.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gtokisfci.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gohkkcrou.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/giqigqqxg.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfczkwnhl.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gcmaddfpb.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gpezdumap.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gzwgrgbue.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gytkeevpe.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/goiwoluys.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gxgmfyvvl.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gfpzhedzo.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gqqsiqdis.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjifclgef.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/guypmwcqs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gqvoukrie.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gzsyeizux.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gnlgsgyqi.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gcjlprsrt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/ghkyyinlw.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gtlmpkahv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/guobadvkg.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gsofvgvyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gplnkhciv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/glgnvmpbo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtgwtxhes.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gdrwejzwy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gngrdthbc.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gofhigvti.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gijvyfuqc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gpfqeosrc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gcozlswzg.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gacuyuwol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gytfttjpn.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gizervfti.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gzqfywmrx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/ggkobrfsl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gelunemvp.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gevqbttjp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/ghptrazhr.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjhscxuna.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gugsbpnwi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjigjkbxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gfotqyxwb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/ghbxsqmfp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwpiuyaew.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gwslxxakv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gryfoalsx.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gilarafbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gicpdcjjc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/glvcanwvy.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gtuvwcond.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/guqvhbjcl.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gonavafel.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjumkozld.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gowykqanf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gpcmtqhbk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gbpeewqcw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gmardnwgr.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gaxapcxam.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gksfmscch.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gurvllvla.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gisddqyge.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gblhyjomb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gulbmwvxw.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gthgxjbia.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gyzyjzlhr.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gdvvjldsz.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggoshmvca.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gqzrtyvfg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gobmwdgmz.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gkdupmpry.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gvjopudje.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gkoovhsze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzioijoxu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gddbdgygx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gitmvddfs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsaiwnngm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwcwyglvp.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gshaazhya.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gpcrrkfaq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/glemvhzbp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gybcyounz.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gehyazpbv.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gkdwtkxbo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gkhagyvnv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gaibiyxum.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gadmcnjug.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gggfvydfp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gikdnwxpl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gajvnigwu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gwhcylnwb.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gzrhyzhgk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gztzxqmus.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gpmhptura.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/grkkclekf.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gerurzowo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gujrkouln.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gnpxfbkqn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gxbxpgvzu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gmjndwkgm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gpzomhhse.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gudhldlqg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gnnsaieic.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpjyhgglp.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gzrxzbybs.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/goqgwarvn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gwpihsujw.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gslwkhpzx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gyeiqrpwp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gkbgypidu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gmtpchosb.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/guruhhmvm.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gnnawtllr.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gyqhlazrn.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gzsjtpkmq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gbjdbless.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ghrofuory.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/galjalibp.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gasgeldii.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gfmybudtu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gjreovbru.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gdyfzhnnm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gxpukfehd.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gubejxfpt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxjruwbpj.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gfczuklff.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gdxvuvstn.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/grseywzrk.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gqnlupnkr.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/grgozdxqo.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/grruzkaug.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gnzuxgwdu.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/glxiztqxo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/glauivlkv.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gsvqpekos.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gdmriiovc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gcqiuikru.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwfznwzwl.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxtvxraef.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbdheyctj.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gsgjecluu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gcdqrvify.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gbathvrrm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/grexbommc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gnwenlckw.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gvvtnjsrr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/ghmhzermr.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gdxqttcvu.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gerjmxxtp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/grylwxwdx.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/ghnbzkoyf.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gfepcatoz.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gexoceyso.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gckeyjnpi.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/ghazijzbe.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gjntekmtf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gdecfgexm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnvjalgdb.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmcrxqzid.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/guuigxbxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/goakyjfbe.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjimqquqe.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gsoyxeyxd.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/glwqlbxlp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/grsugmqxg.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gnzvgdfjt.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gvgzyksck.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/grjxzwefq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjazihnd.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gusovjhsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grcsjcvyy.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gunlldmpy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gftiwkvil.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gnsiaxajm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gpduxtvkt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/glhqbhbtw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/guctpzfvf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gfuulpisj.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggmaohjlt.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpdpqevbj.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gaqqloile.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gzmmcwrxs.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/grhfnvlrk.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/genaknssc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/grptbmnai.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/ghoqluymz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gjucmysgt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gzkpgqqzh.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gyfbwttkw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gcwkikfax.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/ghwsskgnz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gesrxcvok.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gnvtohtwv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gskotjtmx.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gdzmqliml.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gogmcvner.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gycwhqqwn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/grfiurrkz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvuaaxsih.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gdykysygc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjojlhmsg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gusyueicw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gnsiyqrei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gzkwveseu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gkruhcvkz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gwwoxqbyr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gqktddpro.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gtvoecoup.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gudgwjpir.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/goaumtcqt.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/grccdziuf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gwrfcbcvj.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gyhlxqdgd.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gprdidzwn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gghjikzrs.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gmnanbbhl.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/greahxabe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/giuuhvsen.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gvtrqqbvi.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gvwdxgmsn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gfuahndeq.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/goppkxscm.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gznzeanpn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gfiwdkwov.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gfyijylwp.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/ghaiojhrd.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/geyjlljmb.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gvurqlawe.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggycclgwr.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gezvlnkzf.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gsbzauzua.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/giglirukg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gbjpqbqgm.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gyydmssws.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/ghkgtzdtz.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gfrznjlsj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gdmkdhqvo.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gcmhjfgoy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gkkqumlyh.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gmugfjvck.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gbfcmsgnz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gbstzjrhb.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gyivijeoy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/grshkwzar.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gawzhbqfj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gtohbsqbs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gmglutkpq.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gmshlznnq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gsgepyako.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gxsnktnnl.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gllsxdfzt.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gyjxljdim.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gkcqrhixu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gbhdlkdwg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlogknr.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gadmhnfsm.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gnhstqhan.sHtML


<!-- 参考信息 -->