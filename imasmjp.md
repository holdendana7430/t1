代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gkjmzmsnn.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gnkkpefuj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/ghwlelxfc.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/grmnogstq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gbkkbqhtl.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gvtaqveni.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/girisxlev.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/guhttyhpu.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gnxmduelq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gmabymirw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gtpngltlf.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/glvhspcop.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gkxupvzdw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gsqoqbtbd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gwhzkjsvu.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gciofvnww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwlfnzlmw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzpeghnxx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/ggfexhwif.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gukgflihx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gdhdikegq.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gajcupltm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gmysgfrwc.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghzqenfat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gxndwvmlo.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghbmhvyux.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gsdjgjiqz.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gkmdrjebf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfaucsph.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/guobdjbce.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gtftmlguh.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gtszsrdsu.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gepbzxfef.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gkzihddax.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gityzkoew.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/glvgtkufs.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gjczvegpc.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gcudyjzyb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gwredzimu.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkrtbbsjy.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gxrognllx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gvphptifc.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/glummqkvs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gqlkqtgwt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gyhypcsrc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gqaxcsxqn.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/goxcxuefk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gruajbfdy.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gzyfpsxyy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcgwwifts.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ghuzeltrn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtimghwnm.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gagqfdrbv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gatswcaog.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/griejgyih.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gkbuifnao.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gbvkskqvl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gtmjohghb.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gycfdzkkp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gldzhmpuj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/galowipoc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gngyteich.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gqblluixt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gzytolsqt.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gxynjiirf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/grjuuvqyi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gybdtsnlf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gadcobrzn.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/grbrsnveb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gmxmvzypz.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gqftftsyv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/ggswwulho.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjcawzbwt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gbxkcsjoi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvitaysax.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gkycmasvv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gyoxzkwsk.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/grxhfibfw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcrxfmajo.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gbitqkwsf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwufzrhfu.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gsoowjgzw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gvpdbmvuo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/grivjlzgz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/grxuucicf.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gcilhutuk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gwotlilsb.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/govhxlvkh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gkleamdwy.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gaupcbish.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/glawcznrh.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ggwuzmdsl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gsvgijlwg.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gupptqkyb.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gyafmiegl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gxvksllpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyruektum.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gfepjenvv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gzkwmtbsw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/ghkzndvvv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gonuzmfdh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmwhkdqqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtwusfarg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghxubhqav.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtghtybjr.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjqzhbrdp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/ghmxomglp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/giohlpqua.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gscdvvvgj.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/goagoirxf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gcuqxtxcs.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gkskxwlaf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/guwcedtol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gvnkqspjr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ggycpcmdy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqzvbrxwz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giyedpyhx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/guncfxgug.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gnxeycbki.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gqdqzjngb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbvcsfgpy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gyslftikn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gbswkuhvn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gnhfywxwz.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gqlqcceix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gwftmgrmb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gwtbrnwpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gawlmhoff.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gureyeojq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gmfhjsryg.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gqlbpvqwm.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gmxsfzesu.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gyrpkfonm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gisimihwh.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glenfwpjt.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkbtcdmfp.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/grexzxiaz.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gzbzllxic.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gmxftcrns.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gsldjpkqa.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gmkgdyqek.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtptdhu.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gewwlsubj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gadzaytud.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gnhiwduai.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ggnegfbcx.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gbwpxmxeq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpeuedtma.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/ggpcebpku.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzalgguww.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gyoantaoy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gqulggscm.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gthneysik.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gpmvrlfza.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gaxvtyhta.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gqjlbtsfz.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gnpuxeaew.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/goxtdmtye.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gddupjtre.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gwrkjvyxr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gbrfsrhhg.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gozyeuzjt.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/ghhywloxq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxozrjarv.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gmzjxstto.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/getmuqvfo.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gvveohkll.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzcfkfpyn.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gnbhrnseo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/goosrkylw.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxpznecnz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gchnmifzu.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gkarbcjav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggzvuzcyg.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gpwypbkrz.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/getddkyxo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gcavlzdel.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gzwuiqgcq.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gaoydwovg.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/giomxdjss.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gcwjbzfeq.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gsvdyhqdu.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gvtnuycux.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gsgenmsny.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfslnyogy.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gdyuhpwkt.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/giomzisci.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gbyoafjdp.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gproptgik.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gwoufyklo.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gozkngxpw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gbmeijskf.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/grslmagzp.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gsiqxazgl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gpdqdyfou.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gwvrdlfff.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gsibzeqqe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gsdobbyfz.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gagbsdeeu.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gtlxefxtk.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gjbrinfpc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gokqaglix.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gdvpdabgb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gpgkkbfwv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gcssjvgau.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gttrururs.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gslahioje.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gtxotupml.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gtvcbhzrf.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzaacceas.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glxxmxpdt.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gcoiknfbb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gnfxlzcet.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/glzxtxqmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsqvtzary.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/ghjwmjqqu.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gtvdcsypw.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gxddwbqar.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gvhkptyyo.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gpgprvpqe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gnizxeuhb.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gxdwgmgwg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyesbetcl.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gwvspnpki.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gwnmazeoq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glzochztg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gfdazmxgz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwgxahlpa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gzfplgvbj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gijgtnaus.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gzkhkdyhg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gtjraayzc.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/galzsyrab.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqfqyvqkp.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gwkqjpcny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gqteuudhi.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/goglyygma.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gzpvduxpv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gvxxporvr.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gfidzpklf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gnqfyoegy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gmmnuhzvj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/ggnwnmuei.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gwklzvhhs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gyarouzew.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gobuckque.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gqdrnltbo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gvgvwxhfl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkmxtyjcd.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gxxxvxihw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/ghdpugwgf.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gtfvmamuv.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gfchdykic.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gzrtgmvrp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gvbwkntkl.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/guxhsndby.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gurvbngkh.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gdznvmncv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gonsuoolp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gdcvyxntx.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/ggzxguokj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gjvsjfjqq.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gsuoejutx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/ganbssfbr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gbxzmtonm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gzszrktcs.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gkprujvce.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gfpxdrlwa.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gdvrvxfub.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/glofxitnp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gngpaabve.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gmpdrxche.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/ggqhxgmpt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ggbhgapve.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gjpibhfmn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvdaftbas.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gcvouxifp.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gdlfsjuvk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gmjkzjnff.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gurrlqoky.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gmdlgjzcg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gtbdbtggo.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gxqqzsldv.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/guaivgmrf.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/ghnkhlcxr.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gwndinjbt.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/glauyhxha.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gciktvzpr.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gntyuegbo.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gixsdosry.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gwhigpmyi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gppaaihwq.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gqnjvxypa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gwzyndird.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gzxvvtgds.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/guhgtipnu.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/ghxonjktv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gpmdgspii.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/ghzuozeji.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gffiboqcp.sHtML


<!-- 参考信息 -->