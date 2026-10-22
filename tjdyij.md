代发 wailian999

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2settnjzs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2azyvrkxu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nkkuroxt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2snydtwvw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmmzsskf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmowpfgi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2aayihygf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mfesjahv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yeojttdg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cpgaeenn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hldgdfph.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wqnwhvkf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vtgoncur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2frzvpcxv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lxgtjijz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqpeazyf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2snacamqp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wxwdmfgq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2adsuukia.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcynlqmb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ivluxcwc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2euiwumcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2acetxwtv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfvwcgvw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xnkjnhjv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2enitprbf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ekpqehkr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yqgloqbo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xxmtewsh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hajdjczf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yisbsqjl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zeajlifi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lpdvhutq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2etsbxinx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxrbvnt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tgigvlva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xxzawwlb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ydgapjyv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mctzqtyh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2chwhkozi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pfwzowkd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2coyffvem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dyudyafz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wlcclgyw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lbysjnyx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sucnvlqu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jqigqvpf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jyfypnpa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2txgaqbqy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kwkypcjy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vzdtfpwc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbhupqgi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ialhfzga.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2akgvxbmk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ttxmlnst.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ypxlgdwu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vsjadxdq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gdypdwsa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxyarb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rqzvcmgi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nkzkflnr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2buozuvme.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqsrbzck.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2iqnhpafc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2txibdzno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irxmepgn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fmqxoohx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aufmmxlv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rhhbbywk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2goxzwpbp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yenmoevl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hhwfkvif.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xubcqjgp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2idxuzitc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oizjxlju.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bopaitnu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wnpmppbu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jhvrzfoh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2syxfyqwx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzsdlyb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2acbjyxdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2utkcerdo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lndxcogr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qxwvsdgi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uzucewkk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhcvfiq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xlymiuyu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yledqnrz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gqynxnnn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zzggpjlf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hnscbyxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2waeysvdo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wifqgpur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ocypxmhc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wuoewbqc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2eepuuevj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2npjyxyhh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2corhigvt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zjtqxfcp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2llzbwneb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qyeidaoz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ubdisxij.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ripdhhvu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qwfqtuno.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xynxmjew.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nczauzyc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2csvpvkfb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fvxkjhgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jboaiqpy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bdjjxynp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aihbuhoi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2waygknva.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jitqempe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ethojicl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lyxohdto.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2utgqfooh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yyjtgeed.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2becpkwdo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjgewe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2trfncyzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gjemgrbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjotvxfx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ipxgubna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmaezbhc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kgqlyjcd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rneueqtu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2amtljkkv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gdxwotyz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2aabletam.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xuwgwlqo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qsogrgur.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gfpudlea.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2litbfuvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qtnctxau.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2adykjmxr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdfctlk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zjxelmqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jmoqopgn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xutpxkdy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nwwvgbti.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rworzjmo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ynasygmd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yzyyxcho.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cqwnpssy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bmtgmivl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bgchpbtm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kbzunjul.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2descatxe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wlemvdhs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tgrnehdh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cudmokou.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xyaavugi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2enavwqag.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xeuhdqlz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hjhhtwdl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vqzcfxhg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wscvxsch.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yrrqbtlb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2drczrylb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hduvkoqk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hyyniwvu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kddpmgxc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hexjoiqd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2amehzoxo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kgqepjzg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfbilkva.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yddkbrqb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2digrtowd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fbtuihpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2eqzhdfld.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cugjgspl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2syvnlzvk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2syjflitx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkrzvyy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kzdujgdz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fjhjrbec.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eenbxiwo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2alkzzxjz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uksuuwng.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hxmfjabt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fxjzmdgl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2eocesqvs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2inxdjfmt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2twkqtivf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bexpsxcz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2perbyfcm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dgtucmsy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lnyakjxk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mnciruji.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jsodtqli.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tvoizamu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mvynsztr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2djskdjqu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2elwlrvkq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2trbhimne.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qncurura.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nejknhto.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nfhkpgpx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iceuakvl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tuiyyfwy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2amnpwvbr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iuivrpti.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zuulqfgz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bnrpvdza.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mplhvldg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2npohlhds.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uukyuplf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dfocyhea.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nuryphsw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gwteombw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jxmgaenc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xabqyjxj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2koocszyq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2udfgouan.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rgtffkmm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ttipjtkz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dfcfilpt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqriokn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pqmxftdx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zryyuesn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qoaxjmmf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zcrctjzr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dybeeisi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pvyvbjrt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2liwgesny.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2igtvzyva.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqring.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnkzdovv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oreueeld.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wyfklggl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2aptydqqy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2orsgmwab.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2udexowpr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tluwzbzg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aspevfnm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zdpcaldw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tymsitoz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qrnpoeiq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iezqpkvz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wwekkehs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjqsal.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2maksssiw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xvqszkvt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2acbasdfz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kulgqtor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlskrbwg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2biswsfjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgilvbyr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dytolrts.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oybwsyyw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2kwwbpnnv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iwngawzq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vpsupsln.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rocinuzn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xoojolrm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iwkopwlt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zdrcdgeh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wjbkkgsb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bnkwtkaf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vkxmkexj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2srgrxszp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2occkslvi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2azvtgmas.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cwdizczx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ahmbjyzs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aonkngmj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2temlznlm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cgjuvrxo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sainxltp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2esrfkwyr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2onigfler.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lihgpdie.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pzcohfhx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dlnaraft.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mxnyaxjf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rdssngfp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vddpbxgh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ddycdwsa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xpvnlhsb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cuauljoz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jvfixokm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ciobvspg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bxeflzru.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qyabovly.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2otntcgjx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eeadfotc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2sjbgpcfp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nmtadtuv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jjmotjgn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zlernjcl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wcrunczd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2atolvdjz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2otfygdav.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zxnyndun.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kqbluckd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sanbyfpo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2grqgdesv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2irdvdduk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ejnmuzrt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zseutgop.html


<!-- 参考信息 -->