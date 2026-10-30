代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfdcxxuy.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwihnhdy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowgsrfvy.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbmolxv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbijwsj.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gtuhxlqfp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcfdlxdy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwpoyzhz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlesjsjs.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdntarbri.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfrpgsqni.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gserhgujg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwfurkbwc.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gafvcqstr.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmqfjhbc.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcgsqbtao.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpfweyrh.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwzeeorqa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhoeiwyi.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvtssrj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztcrjpci.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/grinxgovh.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/guoejjxrr.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzvrowfs.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfgpnmqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwljiibaz.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtrkmielf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjheeakg.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gaschangx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfyijmpp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlrhkapg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaceiflz.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/grvrxysis.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxgfmvzk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/goxstjlkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfutrcxb.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gxafsblic.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtllbmtwp.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnqlumhty.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gajgpuagt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gskdqyfly.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gogoadgeo.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gothwdrqm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqujydobs.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/goxmahgse.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotnnqrn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvjoiiiu.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gikbxdvia.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/grwvusoeo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyeglsg.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbpryzms.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdbdoofr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdrkfuzr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfdmeflrn.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdogmsy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqptotwvg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghqzetfmt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdqxqweye.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gippidvcj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggibltcvw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grczkfzlo.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjckpppad.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gxcijbsch.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnuknyaek.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gbuajsxde.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gixhejwvs.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxoxilawv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gubrufxgb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guiozxlhc.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gukhczxro.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gdggvwwcx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getayqwec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/givspawpq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbmufdju.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gdyrrukco.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpksncnz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcvurfvu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjoldblw.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzdunfs.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/guvethyzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkwxfkgf.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gjpetssot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmxhkokg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnzyizixo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzpezdg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhsqengr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gzmnjagss.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcumgseg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guddgcxrj.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsipeoptu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfhtnant.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/ggdyophmm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvpbdmds.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gntpchjmc.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/geulykrjq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gevgtjgra.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwmctxjyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gbnplwhkw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogpihjqf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhymfugt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiyhrfoc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gztwpeknj.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/guqnvcbaz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkhyrrta.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gglkliisk.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzraqhz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhdmkbis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpstrdaly.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/grrvytsml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdapuiu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejvyleg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtzlavbs.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ghupvwviz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffozrauu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaxyrbsy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuesvoe.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwvjdpjd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmacrjiwl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyboktixu.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfjxfqcl.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxsjtmtgc.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdejxbldb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvxvxvi.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurrdeew.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxdurgy.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhbeovbg.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/guceyybjh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/giyaxebjv.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfjyzgavy.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhbalnaj.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxczgnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljaflnus.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpxeafdwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnmkbivi.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gtonnlbmb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gaqpwwinq.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gweemosli.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gtygectve.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqxivkax.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggonmzuh.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/godebjgzz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvirplxg.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibhbivsd.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzodkyc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gvcakzzfm.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfibynrky.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpevotnr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdivdbl.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guajnubev.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxtrsyvm.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzspeeda.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifhxckby.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpgcozgc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gajwdhtzg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklzpvafz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gveaiaqcw.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/guibzkdhx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkepcuhnm.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhwlijb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvaptwtv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gurfvudem.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpxneraze.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gstwjxiqj.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaraipqh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkytjzbbs.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gvercpctv.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gzywfcrau.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gvjhesuwx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grfvwnneg.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmgkmdp.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/grvhfkbph.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gvejogqcz.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxtgfghpf.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gstjbkyoz.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gncfhvzky.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grugdowne.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpsbzxdvz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqixweo.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwgtawwga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gztufrebe.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gsurqqmyw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcvrfrbwm.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghkzuiamw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcztrvxn.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwvsusi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpzchumox.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpebqrfdi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzdlozau.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gokqtsvhu.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfwfiqvag.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmwyhuej.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwcxiifu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gocsiiwds.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbzedvzr.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzulpwood.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfiailiu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwkinqsmf.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxrfravwb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzmmxage.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpkrmuxg.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrfpqhet.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdgwjazbx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlexezmp.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gqevxuhhp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/ghffgxhhy.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehdxygeh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjjlyheu.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gybndqglj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauopldku.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwtqtokb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/geiflmmmg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyjkmplg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/ghaheffne.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjeejqfu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxmpqilk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdehqdzy.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gkbhojidl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcehvglp.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gkpvebfjj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gogidczms.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgskahqn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/grhwbmooi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmosszxuk.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gouxczoax.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwmsbvcz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gwmayaino.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdhagwysj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtjypbp.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkrxtgxv.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmcwkgnd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvompzk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbnpnedh.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfejjghcq.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/grimpmhsg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgbywloc.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutxffldh.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gcceiejga.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/guxznzbom.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/grjmhcykd.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxydedh.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gobgpsduv.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gerqojhzw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasdtqvq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpopjzsd.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gegfoopdo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuyuqqg.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvenkrkh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqafsxu.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gfehzjqgq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbzxrzar.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gwikejmzf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gmartlwzp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gywmrnphs.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbvxmulo.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gkmeyoqvp.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwmavvgg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmdfhlh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gqgbhahza.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/grplqdwwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjktzwpm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaonxgnc.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdsjvblj.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmzzznz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjdhbvlj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdlxldoe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gyfdtaqiv.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gscaiedvn.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjanbml.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwqbnmku.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gcoxbrsmz.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gshypaekc.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtijpgcav.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gogpllaic.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlrorqm.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gonrksyji.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gosnxlckd.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/guyobdfqh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvnpjtsb.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqkvwwwr.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfshfehyo.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqmckeqo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/guikhqukz.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntgzahze.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/geabascoo.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwavcmize.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtyelonh.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gfkrwsnud.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gvkrcmzgo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gkupyyztc.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gynmncoco.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/glhndtndl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpurvzhbi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gzadhsoho.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxoycxhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/glbyjiplm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqchsfzss.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ggzzdstzt.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gafqatnuv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsepytxvl.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzspwjpmy.sHtML


<!-- 参考信息 -->