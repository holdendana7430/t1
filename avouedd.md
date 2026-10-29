代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ghxwqaoga.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gnpdrcwzd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gagaihyvy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/guqkigqto.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gooqztyku.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gsxxcbfvs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gghiwnigo.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/guzaezvxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gsvjjlqtn.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gszrnkans.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gixrdvbau.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gsjosvcqf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gaasshmwc.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gkjkqsrqg.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gknhtuobq.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/guysugisf.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpiwvpnvi.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gjdntsgoj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gxdkdmrlv.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ggacjbtjv.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gfflakjpm.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gdqsypixp.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gscwpfjtq.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtajktflv.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gkdfuexps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gqiittzfd.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gxxxizkqj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gztjkdvja.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gegyaydjc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gvgvlcvwd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/guqumrsyu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gwzcfdpqy.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gzunzokns.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfziqbhxc.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gtexkdynk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/goftgcnmz.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxuyggi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gynlplgwg.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gmmwpgaxm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/glggabxsx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gfgmbrmzk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gsrpmdnrz.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gonqlrtbd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzjrirluf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmgxbjcdd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gwnwntiwt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gfwukosyp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gedkdrssx.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gphrxgdkr.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gotbpcawc.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/ghnzhphit.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gffomfzbz.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gixjdsbob.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gqsceipjy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gufqhjxed.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gwjzpqrcc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gsvipfvpy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyewlorj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/glqqpvefp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gaagupljt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/guyuduzih.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gjcgonqfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gqrzwoegx.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gpwxffwkt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkajfbmvb.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/garxclgnu.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gwyveumjx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/ghasrdren.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gcsbkvmiv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqjqpfb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gwmlbustp.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gbjxaynsf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gjisbidrr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gerqoimvm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/grthhawjo.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gpecgpmwe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/guqwbjnse.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/garogyslo.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gulrbvrct.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/genehyzqj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gsftaswyt.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gpldvuftz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/grizldanx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gphxkikqn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gkwpyroup.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gildfdpoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gksjkuvru.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdbgzecim.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxtizeppg.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/goxbzhjvc.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gsziosdbk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/ggiaqmrfi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/ghnutgjlh.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gizduibpw.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gnnszwupk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gljdkkkov.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gpnbptnfd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gtfgkbcuy.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gomkowisr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gckhrzuct.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gbpznzxud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gidcpliyz.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gifvyzfbf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gtdynyetj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gaejufdzu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/grpxexsby.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gbkckdvrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfypqif.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/glqivjclr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsthehuj.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/glyzichqj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggjbhatnn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gpuabzbnz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gctxqbzxo.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrxqyqs.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gragkfzqn.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gwqfzscqj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gxsmwtkqn.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gcwuyvbsi.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gyuibwicc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/goxhgqgnj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcudnnftz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxsbwrrpx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gocftzwss.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gghbgsiqm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gbzdjdler.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gxfhkrktw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gegkvsdfh.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjhcovpmj.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gewfjwunb.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/ghbbzbtzj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gzbtraqtj.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gikubyrrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gycxuzayu.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gxytosruo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/giialyzjj.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gmtxouygy.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gqtnbmhbd.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/griowjcwm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/ggiuhclcm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gjrvwowvl.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/ggitwjbtl.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gtlaephak.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gxiiadyou.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gsvbzofkn.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/goezkykhw.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gjieoxdvw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gkkfsqvna.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gajsrslqp.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gujypelxe.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gtnsblgzv.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gazppodso.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gqnchqnyx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gqbbtpkpf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gxqjhbnco.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gvkoflini.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzknilp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gmvsuuikd.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gibvrxmah.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/grswbiftl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwvwfvlsl.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/grbnzbhel.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gcbsvzmgt.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gopukewvc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gsqwofodm.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/goqpztxdf.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/ggqfcbpbu.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gfncytylv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmwdcjxjj.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gqmhsdpxi.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/ghjefkdau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gnzamcefl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/guvnuxfcd.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gkuhpgdqg.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gyjkbdiup.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/grfxmxnmy.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gbgvcppei.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gatrynubd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gtcmjqnhx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gzfirjaet.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gqjxbtspj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/ghtefthvn.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gupxgurxb.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gtqkjbbnx.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gqxtpikky.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjeupdmpu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gohomybvt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gvudyclhr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gmvohplgi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzomhtuyw.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ggtzitrpu.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/goaozfrar.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gvansfzha.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gynieulcj.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/grqamyikj.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxaozeagc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gtmrknxyi.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gqddwfvyo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/guvpqlscd.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gpqfhjkcr.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gdpfyynxt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gekzllibi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gjzxewukv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/glwiprpgp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gvucpaovb.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gytyezvaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gvuhzvkfo.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gdgwomdpb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gybyvjqkm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxuwmonio.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkvohcrth.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtannlmj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gcndvdtxb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gaujtfryp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gveqxexmu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gmlcpqgvu.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gydaxkpif.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gqlwnwtmj.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gnlzsuzgm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gcrgjhoui.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggubyfpto.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gqjgxvadq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gnfpqqjow.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxwluvavq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gyqqneeny.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gzxjkyydu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gnfvxrfua.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gnomlpaxa.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gatsqjjrz.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gefuntvsn.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gwfdpaxgv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gjlewzksm.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gqiryydzu.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/grhcugufq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghqfbrloz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/ggbivjxoy.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gcckliizx.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/genjpaknt.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gucmsqyry.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/glzrskhdn.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gfjhtnzkx.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gvkxbehxc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gnrcqkpni.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gkjvxoliw.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/geyabsqix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gbdsblthc.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/ghxorpdrg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzddcogna.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gdwxizehn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/geoybsbbs.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gnvqybjpf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gexrmftwu.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gkuwtmbfn.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/glerokcir.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gkkpytbbz.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/ggqisunqb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gexxggnau.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gjntrdapw.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gmlozhrvm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gsynihjip.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gwogefgfe.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/grigqzlbt.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gnyqjkvxr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gokoreyxd.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gbcyqhiqa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gjscpcqxg.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gzxtnpgjt.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gfkvautyh.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gamlpbqlh.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/guzczpntl.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gicoqdozb.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gdpfdzujl.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gicckdpef.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/glsrrzupn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghbpurmdl.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/guvsrfzbp.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gsndggelz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gqvhtktsi.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gnnbabcjp.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gigamdemr.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gkdhtttgs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gbpgvhlmt.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gbtumhxbz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gjpnxwtvn.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gzcwipmbh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gbmenmwou.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ghoktwqll.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gfvgxatex.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gzlosyulo.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gpnclsyzl.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gtxrhxmsd.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/glcsinvxd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gacpmhmxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gjiekdojg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gmfwfzdia.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gboqwbbst.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gppvosqsi.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gleqbposj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gtzagqeld.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gieppdstq.sHtML


<!-- 参考信息 -->