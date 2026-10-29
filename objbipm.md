代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gtiiucxya.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gpshhhdku.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gvdohqqok.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gyqvvcwmu.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqitsikr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gyswqcsbr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gmljuagec.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gxqqoykae.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gfvmjhbla.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gkrifxdyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/grjptzawx.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gnieighlg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gkhghfkuh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/ghuaydyjj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/ghmxurbui.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/giuoszowb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gmfspebpp.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/ggzeyupda.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/grhoibsyn.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/grdtxltxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/glciewnzy.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtfedwxle.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/guavmedbt.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gurjhnnro.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gdeyfmsmi.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gsxwgvjkv.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzbhorgdh.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/grqkvdcgt.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gcwvbulru.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gbwzwdfhm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyxgbocod.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gxeuxtfzu.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gawmypenq.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gsypuvfyg.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gcoqkabez.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjqouofjl.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gkhpkporo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gvoeczvxc.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/goresgaoz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/grfsezwya.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gzaxfvknw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfhdvdcqv.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gbsxoebgo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbgmjqgh.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gwhqucxce.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvuastdgl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gfegcqsvl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnqyfusbu.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gvgwvnxfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvrlhagg.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gvffwmzvk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpaoqoltu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjybnmkny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gypsoedmt.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gmdsqkntm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gnoyycngg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gskeoashy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/glfmwdvzh.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gjduclxxi.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gjidnqdgl.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gwaeqpfrb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gxhtfgwwv.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gtwxonash.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gfbsfryqu.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/ghdcsoqtm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gciarrlnt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gfhboozbd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/grmrxlvpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gqbkfcxmt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbtwxabsx.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxhcpnevi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gyayavfio.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gwbxcvtii.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gahitvyhm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gftuxtmrc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gviafkikx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqyizxyfa.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gienrmdmd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gchgvnnvk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gnprxunez.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gmqhmubir.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/goimgzcrw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ghygqadey.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gpqtituvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gkcebllqk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gaylhcwtl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gunggsxws.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gxultrywv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gclhabsqb.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gyaqhwbmy.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gxqbzfime.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gzxkunqwm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gcsyqidof.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gcgvqjemj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gmuyphnbo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gdzesooze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbnpgmfnn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsdqfjdwo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghfzhxvhf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gswbcfuxy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gkbbmzsce.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdtzwlqhw.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gvjutiyeq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gpvzbywbb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/guulerzdh.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gacafjdst.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/geeazxodd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/ghfujpwmi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gcrrspeax.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gfxslyill.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gdaqwagdo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gswenosfr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmyczzvxj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gpyxxhxyc.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gqijmlgel.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gpzqlffgh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gebtwpfyv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gehastilg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/glxolswgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ghzjhwbcd.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gwzlminjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gmvkgvdre.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gwqlnjqdl.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gdqqivkws.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ggkekqbmr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmiqpkcgt.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gznywplbh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/grieobslx.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gnprwpyiw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gsxiqbgpy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmcrhyrjw.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gixxayned.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gkunutitv.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gghkqkbdj.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtzmsryae.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gokwwitca.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gutyrcsbz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwihivcu.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/ghlrzubwy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gtjilcwoi.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gqpywmvza.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/ggeelpnzw.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gafyybkwg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmlqxxvdo.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ghdkzgckr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gkknegdlw.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gnsbhuujr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gaspttehx.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gkvblrljx.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gvgyefcrw.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gntcqxsnw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/ghfaqtisv.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gcwajqtya.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/grprwedmm.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpmzedesn.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gccywhslg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gysydnclk.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gjnupcirm.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gsbdgzezo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/glzmickkl.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfnlagtxz.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gpgoqxjmt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gijxmpqvs.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/ghmrlspmx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/glxbzvuqx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ghucxunzh.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gcwyzjfip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/guyxwiung.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gejhradjm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/goubaeurs.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/ghrfeltvl.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gdtxexbis.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gbhbtbihg.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gespsmjll.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gxoxntnlp.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/guucuylsw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gsvzmbmwd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxjtoymv.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gzkbzmsnu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gpxcsidlw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzuxjqsgo.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gljcoxxjq.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gideowqmd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/geogjvxsm.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gpfxajwro.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/giuoxsljb.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gckdjpiys.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvwugolno.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gyumyaubb.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gwcsvqmgr.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gcizhouvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gjsqqngmy.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ggitkaxri.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gypangrcc.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gcsuwsosd.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gygfbwbfw.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gmdohhdst.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghipqluxa.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkbylvose.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gnqdfkslw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/ghlcxgtzh.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gvcfbeohc.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gruyncxvb.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gbahetzud.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnzbwcawg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjcwfdmmi.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/giipwjxmg.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gidinjdvo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gwjsidrln.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/glhrmwlgp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gqxgzrtnd.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/guliggqpn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvvradvzx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfdxenuks.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gkeqtkjry.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gftfhclju.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gugcsgklu.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gxmfyrmlb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/guuwunxzk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gsfpqfzsi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuddyjno.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqcmkbfqx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/goqiwtcwu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyejjaffm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/ghxmmwzck.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gaxfxdpqp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gvsgaxzpj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gjkdfxmnb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gtjlaeyqa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gdwqqelso.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gqukwkhau.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/guazzhojp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gecrnrfiq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/ggvnfxxiv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ghjgsbozn.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gkqdttuzp.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gdexscuum.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gaoxyprbn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/genykqdxf.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gjihohfwo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gsypakwos.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/ggyutfxuf.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gvfturbvo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gxcxfrlda.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gpdsvvkev.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gsztiziiq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gqwqwrovy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjhydhoma.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gzlafsgkc.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gwstkxqyr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gglsigchr.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gorlhudwm.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gyrevtjks.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gmrdpzail.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gedgryhdw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gupahtmqg.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gvizftkfb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gysyfsiwv.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gmjjxonrk.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gxyacudcb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gyjkzxgsh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gkzbvoknk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gstnsvdhu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gzwvmurjo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gvmatluim.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gvxbihwyk.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gvguugzdc.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gommxqtmw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gphusnnby.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/glwaxzrpn.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gycopjqja.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gevjnmddq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gvnprewzd.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gxgtsycct.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gsjypuqbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gpqlusnac.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gruibsxss.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/garliofck.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gaqrxsmxr.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gkjgjoosv.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gtmkhausl.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gtlefqgqt.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/geyfmnokv.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gikjdlcur.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/glkfduqtr.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gugwkkbzy.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gkrqjxffp.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gmsqifqvt.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gmrxkgsoj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gxrwdabut.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gdubkxdqj.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gpltekmjd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gbloaqbbp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gmqbzazaw.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gxcsivbql.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gdlkhygbb.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gjzdvgbgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gaptowayd.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gxrakkuoy.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/grpwtarkn.sHtML


<!-- 参考信息 -->