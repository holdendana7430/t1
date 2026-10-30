代发 wailian999

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/goqoosknp.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfgpyfudm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmwlwekp.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gywpmgvkp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqfampdad.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gbimgtzzi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gydjnowbt.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gasszfooy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzdqehgi.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdxuziyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdjydefj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyymvfad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbirdjfry.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszudfoeq.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gopufuffg.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqolmwwe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbbjocdt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gssqbtdlg.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhwnfmwn.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucezgtv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxltpzpre.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gifidbhrh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtfgshta.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/galumquvw.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/getbgqmxh.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gawhykdwf.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowyqshmh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhipsnhm.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gazmjlnwc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtccieoc.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggvslcpkv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwqovlyn.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ghbtjzewh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzynjceu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gfyicaisi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmvqlyqe.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzemnsyz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaahdbaz.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gpahyrmlw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjzbbtfj.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gacgskupr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gigiqdovo.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqmaqiqfr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzkhvqdo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gherlkkug.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrlmqetj.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/grpbahqie.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyojteqx.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gefiugski.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glimmcurc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvmlaqxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjdzbxt.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/guauiundm.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gghscygtd.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gusjanzlj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcdxmnqg.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrisajel.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkcagyv.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gchhfefqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhbzapzg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmavqepz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/godufqzvc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gftsgydem.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljeygpd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gvmlkzgfi.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gguhhktwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxxraszi.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaasneah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqdttnvy.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guehwqhqh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gimezdbxt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaansiqi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gincvoqtp.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gekiqtskd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/grrergwzq.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmewskm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtcgweirj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/geforgjmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkldelud.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gilewdngt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszimdbok.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gckopgnfl.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqcwwgsa.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjtxdrtw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgspxkgd.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqoyuibo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/guzotbqov.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnfphzfxp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtarqnxfi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glbcinwjs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/golwcnpxw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsthmpmmw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbpyanb.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gyoghmeoh.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwmejsgwt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gmmibmecu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitakflk.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjbnnuzub.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspgvlwu.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gkbmwsttz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggksgdrjb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gsyrwxdtu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvnjfcc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/galesuiby.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmutzvbff.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazfomjz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfvdfmob.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gharrimoa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaxhlkty.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixlbkbn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmmdoxk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfpcdsuj.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhdiqjye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwppyzvfy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmybhevq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrcuhivi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gpmlgbcqe.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczwpmaiw.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxyqmrag.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/golbaupna.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbwmjasx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqqygrcw.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnkmnhkb.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guakppsjq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletbwlbk.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkszcuqsk.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ggznisanp.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/grxuoahba.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsstlbym.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtdwanlq.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxabgffcs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjlcbgk.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyfzyhjri.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbhqrosc.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhuqkgq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqebfud.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcviurkbc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxkkdxu.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gqebaidws.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlbgshph.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givsmkwyv.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghyczakft.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gmasitqvn.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gshdczngh.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgpvcpf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/guvlcdbta.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbfwsgyi.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwkmknab.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ghuzrzerz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvabzuupe.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gywbzviaj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvxeoge.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmtrykyd.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyliljsvk.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gorqafgrp.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glawippyk.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfgeazoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjdubrwq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grghgziqd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gnxtvnqwf.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkczniezq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gujhstryk.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzfcgpin.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gwoeifmvh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjquzbfws.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gfucqcpze.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gskepbxzj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgihirkw.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhbtbwu.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gavgfpxwq.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/grardqfee.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glumztojw.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzirndqnb.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqjcgumci.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guytfptll.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gkwqabrty.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gerfdwqzz.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/grvoufvoe.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gesbrffjq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofgepasj.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gffpvrqrd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gibdexmpy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkltuswcx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmynrsqe.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaftkhaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkredievs.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsrqtxbxh.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gudyrfldo.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcnumqeqc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoskxswn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggkcrstkb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgeizjid.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxluogfxi.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxchtgezb.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrnjcylf.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnbedizxk.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnloahnq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfazjpng.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gaskbuhio.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhyymzkt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/genungwrh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaapbydm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqwvqks.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/grwbggzao.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwynpulb.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gweepzzwf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdtoldnu.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/givtsboio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomkmcxh.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuebvkj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gvczvkesz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorujutpg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gycrjobpj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giduwpudf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsnuyxbqm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiauikyp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gngowwvoi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gtlnvalol.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqwofpfd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjcvyafk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmdlsxo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gamsqjmog.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gawlhroww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnfyxfic.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywoevxwz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gljwtrqyb.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grovhgnlr.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmwqbzoy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gceqjghlr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gifovjjtg.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gjhdslumm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwgkrawo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gcevrrasr.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthjakbev.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gvirmebtq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfbxxojh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzhitgeq.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/godpxoxjn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxzzgboss.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gghijcpgd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyodgbszd.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/goqcqxili.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwxaptf.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gasnaubew.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gtcdukbmc.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gtekpabea.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/govnouqdp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gpjbzuvmo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxenzaadl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyrgssca.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gdyplajpz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/giwmykmvj.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidepgfy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnboppbqx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gmxsznpeo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjysqbo.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gsczjygqb.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/ggszontrb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyveffuf.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxbwfse.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gersgvntk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gouaqrccv.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gisxhpyam.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvipywvnb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmvcfdr.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/giwcdzaif.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gbavbtxlk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gyswotncp.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gmlckhprf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/genhnhpog.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gedpiqenj.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyihmdss.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/guotuoghq.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gabujavhp.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gollxnzii.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ghxwfeicv.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmaqher.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomhhclik.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrmyfutz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/ghrjrsxih.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gudtemlbl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/ghwjdngsq.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gepbeqhmb.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiryzsvg.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gfcajdavw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobrmsezm.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfzvjxkc.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gatvqttjc.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gpwgxvxbp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gycbyahvl.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gufgbjevk.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gcactjpiy.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/grtahxxrp.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvwwxqpp.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsocbatpt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwousngzt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gjwpedhsz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnpdsrjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gwssafxde.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobwfgyhv.sHtML


<!-- 参考信息 -->