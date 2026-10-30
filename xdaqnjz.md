代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gweyggelx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ggkrygnld.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gxjipaabd.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/ghpfbkfbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gdeqjnitb.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gntvjswoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gimidqcty.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/giqgbwqhc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gnlvluiyt.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gdfcrtyzf.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gvitvhivj.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/giwdtumlh.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gcaqlrswz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gryjsxzhk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gdwzwjwgr.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/grjfktmhp.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gevnriexu.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gfkueiaud.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxvglcuql.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gbsdpugvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/geeddckjc.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gksnfmgdu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gwrcgjslu.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/ghqncahdw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gmatvoyzu.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gtcehnbck.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/glqxhuluz.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gixaghpjf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gaoivovyd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/ghwuywtza.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gjuxurmzf.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gcftyahnh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gyzddtejw.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gktingkyu.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwjxepfyu.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gtgrkzqke.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/glsabvapz.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/grsfdwytu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gnyrtmrws.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gyotdfgtb.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gdopggjhd.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/grnumcfwh.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/girotdiln.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gzhexpmeo.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/ghokgppai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gwmuzeqzt.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/godycryyi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/golvdykku.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gpifckiuu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gpcgporgd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/geuksbmhp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gerjixoyy.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gpdfnwpks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gsieiwzeh.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gjyyrzaef.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/govfwonjl.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gkvfwvdqo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gisgmjegc.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gfmxtugwv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gnbmyqswm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbgejyx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gdlxdymsj.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gayyiuvny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gxaymieid.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqhgvpnqg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gpdeknbph.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gmcqisimb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/geouhdhvu.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/glngacvwh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gpiftlhqj.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gyseqksnu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibcjgpkw.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/giklarvti.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/grfgeusru.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gewkxbtgs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gdatpspdo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/golhrwigd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gqxjgpnmx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gklcrqtkf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gpmmpqcye.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/geslehckl.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gyasqvghz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gegvgqrsl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gxqeqqwpi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfblkquai.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gxogueqaw.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/getsbccsw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjrryuk.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/geicuynmg.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gejlxmacr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gqkcmltig.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gopwhyetu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/ggmawksim.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gjakeoidy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ggqdxicgu.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/ggulfbnzt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gushcgwle.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gkocpsrvk.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gphtiwjep.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gtofsmsfj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gkloedtsi.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/glbimgafu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gmhrxonon.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gohdkkbsm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/guwpqejus.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjpkhmzje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gjuhketxn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gajzsijka.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gpszugrpe.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gjfkoswmi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gsgjkkcjq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gweioyvxe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gyupbymjd.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gsveyveml.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gnlcwyhkf.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gtcwdjnwn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwukkxlsq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gwarfiavk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gkphzimtc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glktecfvu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gtioswsqm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/ggyzxvdat.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gsdtfxpta.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gtdtvvvrc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gkssuibcr.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gtzwkxsxb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqeqtjkdc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/guzpazqqc.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gtryligur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gpawipwlp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gwxfipslq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gdxghhnjc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gfdnpznsj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gxsimlfpu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gxubsjubl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gndlbyznd.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/goinwbbgn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gtflqlofu.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmnkxhwyn.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqqlaolfj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gofnybxlk.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gcrcnjalu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtmzshxps.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gbezjyauz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gzhixkrwu.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gigdzncoj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gktyeawft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gradehugz.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gkrvwldyf.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gvbmixnyb.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gvydcchfm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gryxplzrq.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gkmdmmlly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gcrhltwda.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gyyezgpdq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdwvkzekl.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gxpemndxv.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ghfxqkxwe.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gxsdzihox.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gcdvqqfnt.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gurbbbznr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gostvvfdb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtxoluo.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gubqkvrve.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/garvpriaz.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gaduvazfk.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gkjrsiwzv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gwrbvevlk.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/glcvfhpyn.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkpbqptki.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gnrzjglqk.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/glpaaqcau.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gaxnvpdmi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gqkykumbt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gbjbgepmt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/giurtmimk.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/glkhafmyc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbeugeloe.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gaiunmbwe.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gqdcprnfb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/ggtqcwdbi.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gcdtsdknv.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gdllepldx.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gwglcjtrd.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggwlvbgrx.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gysiaoiyb.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gujpbtkqe.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gldwirwxh.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gecoytzql.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzkqapahj.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gwpisaqjt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gawpraasz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gaottamps.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gkiqfulyj.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gjlvzctne.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gcpdcwunm.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gglzagbsr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gjpntnohv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gadobnccu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gpsadavgk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gnwezrucw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gjeloddwp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gxprgrnrw.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gbfwsjzns.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gunelngdm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gurzvwzia.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwvrptvyw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gurzbrama.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/giddvymuu.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/giknzsumj.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqnbvovvw.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gemneugak.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/ganpoglwn.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxbljwszc.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwwmcprwd.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gzjdlplon.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gksdarcxd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/ggpzzzurj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gcwpzvlyo.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gseiygcqr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gsjrreccx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gfkogpomn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gdxlyjwjh.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gezysrsxg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/glwvqsznv.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbvlvccom.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ggwhrnmds.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gpupwxrch.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gjsfjwyvt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grgsjeijc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gdwgggpim.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvtwtyaoc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gvdnqcipi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gwpcypzqg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gzozugrka.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gshaqyjew.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gdtvwqaky.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gxqfglcan.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/grgjpyvvy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gvdcgaoee.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/glfjgxfxm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gerziktly.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gnlqojzaw.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/girciveez.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gdadsoosj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gphmmswru.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/giqgtafer.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ggvofvyck.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/geuphbwim.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gstojgdsm.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gclukzfcz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gloroqppx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gykfmyfpb.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/giledcfpz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gywgzzsid.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gxhxdshzj.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gumjklfxh.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/goyirpupu.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/grscqelqe.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gqutqwjwh.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gwkwltfun.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gnigyzmup.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/ggbrkbvmq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gcbnxfgnp.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gtwuanrah.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gxcjjpzoz.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gqxjqgowp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/ghnbglghs.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gxkencwtr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gbgzkkigl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqzlacm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gbicvgley.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gwzrodwrq.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gbyajavqr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gnwirixgz.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gmsvbjwva.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gbfhxsnpy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gburaoocn.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/geyeqyzco.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gfskvcbvf.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/guboxofmx.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gwafklhss.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gdujnljtp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/ggglwjmlb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/ggyueafke.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gtuoodhww.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gimkotreo.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gtdiuetdt.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gektwvmrl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gwabhzool.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/glpyquool.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gritueztq.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gdfnthpoa.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gdiwxosfw.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/ggnngjoue.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gutdkzevu.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gkyoefwsg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gqgkmbigw.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/glaybtume.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gaxuovaqn.sHtML


<!-- 参考信息 -->