代发 wailian999

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpfydqqv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozuqsopg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjeqwyf.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoczswqf.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gyblakhyk.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzewpgfm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpbliezkk.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlovjflo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcuaibd.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gckspmqqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdukqocgx.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvrdsmnoj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gvmytqdtj.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/galfzexxj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvknlgqff.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkmllvt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmczeqwz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gaouimegf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvroxmxy.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gehqvitkg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/guunllxdc.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gihhuuchs.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gqwqemzxt.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiibwexr.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gayliivvk.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giblcnpky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzpgnuxt.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gcepnmowg.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gyezclxlg.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gfyizlhvz.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgeaugcs.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohjiwebq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/ggadelmtu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdarmejfx.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgvlfrx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwquxplzx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphyuhyyp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhvqvrd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gbhiiwmje.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gddhwghbv.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grshwsyev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbfyesqfc.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gmzbjksys.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grmzxzztu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/glefqmnbw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiykfgta.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtkifvpkg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwlainoj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gddqzzayq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfqxwbi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkuetzla.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/geijvjlpl.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/geqwtytav.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/goldpnfhc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdxolrz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gtrycpmta.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqwqnizd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gzmfgdtjk.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gyeotamna.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfutwmlz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqaeemw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbxijxtlk.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxppriool.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpbtujqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gifdzjozd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaoijsnw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grpqpinxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbvyrjcd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjxuodlz.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/geojjiuto.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuakxmtd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmuvfqoz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcwarzhv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemlhxydo.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbqpvwv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfhylww.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjrbcdry.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gguupzwyx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gggakgfgu.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbfggfwaq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ggsekuaoc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gghamgugj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmamtxwbz.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuzlqcme.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidobczsm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrbqxkl.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/geyodjjge.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbcjjsqg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhglclaj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijtrlge.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/geykhwmrv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcdwnhnhw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gzaixhjwq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glxaouusr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gbfzysxzx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmjlmioq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbierjtw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghfqaggcn.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goxteufzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ggeykqyve.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggewajpix.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gicrgdgbl.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelateyam.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gfvklfwbn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gastxvlfq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbpsgxku.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhlpvhpf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepmdwjsc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmddujyhp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvarhbkux.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzfqqhh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfnesnqu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudxmnthx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztafjdb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafhjvyx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjollepv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gehfsnqbe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxljurfos.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gmzjrvznk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhanbwzj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/grflvvkzj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmsifimc.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtypvsgy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgsackoo.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gsoxevklb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqxbppmq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gydvuyagh.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoedwoza.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gacdkghku.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grwkonzhh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnwrimjt.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gakinaokb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzypvhko.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gspqxdrqd.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gsdeomnlc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcgrafru.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqfxapdea.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsbywkor.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxtltntb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyttzuxpt.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gktwsxvma.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxgzfwt.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gksqrhsyj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/guwpybbkt.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfycgqkm.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmfwzyna.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gljzljfua.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvethcwt.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/golelzzns.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwggwwnr.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gssyfbvyh.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjjxvvdc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gcwwsccab.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gtingahof.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/guczvalmz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymhqbftc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqmcwxcv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzmmlbuc.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggcosfpfl.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvkshwuk.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gflnfpffd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gcnmxndqh.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gbgexakhj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gjmsvjiye.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrdvhdo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxarqwozy.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxetfdcam.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/giztbnqhy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmrkbjtl.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfasuhrj.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjftdluk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywayxaqb.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfbmithb.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gssfuslba.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrnmcmlm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/grmoyotos.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjkdrkaw.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ghhfzljhj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjshhssb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gsczywmyk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkltixtz.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gvvzecqme.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/glggsismh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqibtydud.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gowbkjask.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsglkubvn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gldywnlta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnauqlzh.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gfnygmyrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvhboqon.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihzoxkn.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynrfgcma.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyhtlknnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogwgydyo.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqmstdh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunplmtce.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gybdymdto.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgcuhnz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyexopto.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyakuljvh.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggkuqjadz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrxoiyl.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzopaosyb.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gfwbctche.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gillkdvgh.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/givyrllrq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgisydql.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gyccwmguo.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjlbzthh.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwskugyfm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdidcuonz.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpzaricg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmmbyhjh.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmroyeg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gpscmwoun.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/grwhoadgw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftnqori.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzptubzh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gswquaepk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdwavyhr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gspnrhfbe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbajizpc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/giqzfcqgu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/govndkjor.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gracrvbcj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmyxkde.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuadgthv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gumfthoio.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkrvbgnq.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzzqfulg.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsynveyv.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvtfddk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbanesqb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gwzlnmxpi.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyzdoxwz.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gomwojpdn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnhwtfz.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfxavrsg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrkowvxk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvbdhlpv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzisecwa.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gllxscjki.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcygxowzb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaijldamw.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmfykjdws.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpolwyujr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxecuvn.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvdvbdao.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjyhbemo.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrxrkvhl.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gpytbxrck.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdxvbep.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahnzwunt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrmbtysy.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzplsrfsn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gwmnlehna.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmffdhqcf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkodzclq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gyatogfko.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvyyygic.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gpewhizqk.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gilgemchv.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gadzymhlx.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/glynytsgq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaqxlpgqe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/golaszfrc.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmjwppgh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujbxwtqe.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gmtqmdequ.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwpowccy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqovnbrlz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gnevxenjx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gotradmvj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/glcyxzvhn.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbqfpihi.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gacmeiskq.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgonuadq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyhfwmku.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/grtvhxiih.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkniswms.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gjwhdqdxx.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqsaevn.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjmopgagj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/grisadtob.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/guyeeehoy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgpuxbnj.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkkembul.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfxfhxzh.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gbghtmhkp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyklelup.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gtgmjndzd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gokwaxdcg.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gjxpzbzbs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gheohbsdm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gtfucocmk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmfmpov.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gglwsxdmb.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gtuinccon.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gchytvktx.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gabodfoqz.sHtML


<!-- 参考信息 -->