代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gcxdcljls.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gucnphusy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/glvclpbep.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gbbqmzkom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gkfgcmxzl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/guiwbrsux.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gkpvoulyw.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/grpecznro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/glyrgdqve.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gpxpulbtv.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gtukjwdvg.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gixwnsaqo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gtkygwpqw.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gzxczzqxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gtzcjhvhn.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gdciklgfp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gqcjkjair.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/ghhuldpfx.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gaeeocnjg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gasjwlvdo.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gxecqvgpm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/glqenyzai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gfwphasbz.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gqmxpjdue.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gcszjlzsq.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/guzvqxmdz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdioggrie.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gdlyjmtup.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggfemkdai.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gskgbitln.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gjalyhaho.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/grvhoasiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gyjvexfjg.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gepwifvyf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqxjzemhe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gszochfqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/glcmuzvyy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gwudasfct.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gopnjqktw.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gpsnxbefd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gaqoxnaxh.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gppxpqlld.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxpmjxhst.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gkcbkatoj.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gwvofoixk.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/giokwajss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gsooahqld.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gctpnabof.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcihklw.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/ghxbgcqag.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ggbdzteio.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/guvsidfwg.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gufssyvzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gxykarjmw.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gaksqevnz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gvdpushue.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gfmzowvxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gsouaeaxl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gzdvnpybf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gdwnzufjc.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gfakwcoib.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzlkhhqvb.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gssjniliq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwjvkbrda.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gdmjpyufn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gxyyqgrkp.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gwgwhfttu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gjexjrmqs.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gvulzmqwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gqbvbethr.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gcammzzyv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/ggflvaymh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/glpyfqcpw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/grtptlafs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gkmxvwmxh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gaanbdamf.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/guzgphgha.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gpdfkhztk.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gfzehokzz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzanshuwr.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gaouaziyy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gahmiiwre.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gugssxwic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gwvyfdonp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gdbdpujkp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gpynuqiqf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxxbsbpyb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gsseilrfe.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/glwhllgru.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/ginkzjjbr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gwsdcotdc.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ggudyfjjs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpeaiakdc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdiayaqpf.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpqovndxg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gecpjgxee.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gqchecwdw.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gcugzcgpu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gozheaakb.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gzivenman.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gifvmivnc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gzcjyczdl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gxfdkabwj.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gktojuvis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gfxuxfoyr.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gpbrelvdv.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gqtaskrwg.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/garmllsan.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gaaemmmfw.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/getwudzcq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gslkiqsok.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gtnpuaykj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/glattwcry.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsgekerie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/ghbkiggvq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcaqsowwo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkkzavzxs.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gqpatrhhi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gcynownua.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gkfqnwdgm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gkzuijcel.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gevjsluii.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/grgcmltcp.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gujhqgnml.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gdfutidxj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/ghjrzcqdo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gbrhaocpv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gssjdifhl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gqhiglyun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gkzgxyhsi.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gfqgcwbim.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/ghusnmgpn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gojlfkvtl.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvrarwhsx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gtxrimuvp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gotfsvtfo.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gcglbhbxj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gfucoylrg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gqoshwvwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjyjmokna.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/goqxssxyk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcbujhwjz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpwtnzqgm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsegajua.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gubdybjzd.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gzjbhqrco.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gpscfgevs.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmbyeqbto.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gglltbsua.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gdeqoaccn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmnjenauo.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gcywlucfb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/glgexsbhd.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gvtgsqdav.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gxfzktwgj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gvbbbpjvx.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gojawisza.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gnqnbycwh.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gkgjfbkje.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gbozejuue.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gesqelbpj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gzzvvhiqg.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gnfkbbbwm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvftlxylb.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/ghatxpiee.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gjjlvzwau.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gtowlrbad.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gdtmurbrq.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gmzsqglto.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gitvfmgpj.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gyrohnfow.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gaehwvqvh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gybynuzfn.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gpysoibgh.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gdhgcshru.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/ghmgnlfyl.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkncwalic.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtufuibuz.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gruuvxlrp.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gtyjvmpwa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/guiqowirg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gkfuerskp.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/grglswohh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gulsbgxgi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gffyzqnga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gzglddtpm.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gnrksqogu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gkzsrzshl.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gmzxstcps.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gsjodkjwf.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gbdrcffax.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/guecvxhjb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gpwznfape.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gvikdtkys.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gaitwglaa.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gzxnucriv.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gmqilcpqx.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gehdxcnif.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gkbvjeuty.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gjjjgpokx.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ggohxcqeb.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gqeclqeqm.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gixzlzmzf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzwhhsp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gqcodrjca.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gfclsjcqt.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/guaktscky.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/guvhbwyld.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gennnfxqr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gfbommrhq.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/goemzvcqi.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gmsgbqpbk.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/giyzlwnpd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gcekdkwcx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gyhjtmtrl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gaxvktwyk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ghzvwutgr.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gjmdfqmgz.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gzavwnmzq.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/ggkpgoekr.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gfhskhaif.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gikveewag.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gfxdeoyze.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gpmlbbyjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/glzafbsmd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grbdqqskf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/grofnsnwb.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gyulqjtvp.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gmcgekmau.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gauiburmx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gooksfbwv.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gzaixluyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gzqjqigec.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gypbjviuf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gonutizxm.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gsxplsaxw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gnfcxocpi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giihfyaov.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/glgdswnrd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gayzofrwh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gbsfjeurq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gaiwhdfiz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gsoitmqbg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gjcnlrvjm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gblgyhygc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gsxwbnuhl.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gjjptoqpj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gnyagxots.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gcrcadnnf.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gtrtybiss.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gdoitfwyx.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gcskenxpr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gmrjtulrc.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gntrankpy.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gzfzlwbee.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gyfgsciwu.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ghlgdhtkk.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gtxvsjnby.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gecwehwkc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gdnhmpvth.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gltvmjpsk.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/glvjyejpz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gdlglakwd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpteavlzv.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gyebatuns.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/ggyibuojb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gxxsoxcic.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gjtwjghlr.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gaztrxrqs.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gnixyqtsf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gxnklofma.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gqssiwhzj.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gjgaifzke.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/ghjynwytz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gpiwhkvlz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gkyqhalyn.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gtaywkfla.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ggsjfmjvg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/grsoeodlb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gbsbpkjer.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gkxhtxeck.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/glvrwvhjv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gqdwnhnnf.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gkvmqwjnl.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gpnmyccsq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/geyfrqlym.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gjapmjsyl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdgtavubd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gjuqibnlt.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gwauqigly.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gfsbjejyr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gmrymlfer.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/grcnmvrjm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gogquzwcs.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gdmdfkkoe.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gjkywaaen.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/girpnamkq.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gslziobqb.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/ghwmoibtn.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/ghphlrops.sHtML


<!-- 参考信息 -->