代发 wailian999

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gysnsycvs.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gyyzautwu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ginvruyfn.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gvkdhoefi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghdmyyfwo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gyhzvoqmq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gidvtbqfd.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gnbiiupbf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gspukuocz.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/golpqgtds.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gucpcvarg.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/glwbslhwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ghgmdoteb.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gpbyouiig.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/ghqnwnlmu.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gtyhilsfh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gvymotxrc.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gwidylvsx.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grscwxbcx.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gehuuflmw.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/giejlncbf.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/girltvkle.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/glchjfgkg.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gznjlqitx.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbjfjhbca.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gpjhukowb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gvosnejki.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnsqwepun.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gtxyulzhm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/glwmcjpkk.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gmycmqurj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gndwmraym.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gkywsrqnk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gnopdbvdd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ghdkgjaek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/giugfnrwa.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/guwoepwmp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjcjibbry.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gzdlvznug.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghmtxyjut.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gvaaiysul.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gerxeiqki.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ggkmyzpaz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gkqdjbyfr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gjckppzpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gplnkpjag.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gzxrhbohr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gymjkbjvr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gwjzwutiy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/grflsnqmz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gpyiteici.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gpiijyqpb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ggwnoream.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gxkuabdit.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/ghjopqmpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjjjxjlai.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gmkvucxpa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gssokmutl.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gfwndcoyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gnytmsdbs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gmrbbxbdv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gqpusmqkf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqywcqmuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gmafsutek.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gwxyctotf.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gxeuwhvmv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gzreygtnh.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gmzuxwfku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqawflvpa.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gchmribnu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gvkvfpbko.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gvsbeutkz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gqkxppxxu.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gahyqkzxl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gqmhhwxtc.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gyppijkek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gpmwrvmwp.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gobjjvrew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gmtokeuhn.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gbiomybby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gvvzmvkin.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/ghuevzwyh.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyuvptun.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/ghwdsuukk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gdfqmbqbv.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gfzvsfayy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gwydfbmcm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ghkfqjong.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbgkofohe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gitphmxsg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gffrawdle.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gntexxvat.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gxhguxblz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gopubhpif.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gcsycdnhw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gvanicpuw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/galaeuqew.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ghtjpbyty.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gfpxdzszw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/girjozzhn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gqluailqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gsfugjcpw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gceceuxcc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/givpvurzh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gclvdxvzw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gomvygpce.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/glnrliuqt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gesclgngh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gqpaeirvs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gdyxluyis.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gbjrogfso.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gqyidriax.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gafagnqrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gkiaznnys.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gemqowdrq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcbzeytuq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gczqeakhm.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gbsmojltr.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gbamkphya.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gddujqzgp.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gldrcpnic.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/ghxusznzo.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjpjyrlni.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gbgyxombf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gehenworx.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gfyjkliqb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gvyrjpeph.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gwjvwsuae.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/ghrzdpbaf.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gmqbkbfvr.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gjvlwhpvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gvdwgdejr.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/guwensrqy.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gaiiiycbg.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gsicirnol.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gorteazds.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gzgcupkrz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gncchutku.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/grnsiqorb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/geuankmcr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gzstepmnq.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gncufbdxu.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gkivlmrea.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/glcfnaron.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/girwqlnlx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gvauxibvw.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gytjcmcmn.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gjvtbrcah.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ggnshmltk.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gthmngfyd.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gtzzafvsz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gztixqmns.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gapzzvcle.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpxoktluv.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gjqcjnnzf.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gsbkfqnpj.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/ghjpfstjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gzyvbjadq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gtakxbkdp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gffskgjmc.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/ghiwzutvh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/giwpdqxod.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gzhrfarxu.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gojqhtblt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gobfvyoyw.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gsekmoziy.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gxefikxmc.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gpdspexqy.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gybqcfirp.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gqkttpcyx.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gjxhfzgab.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gerytsrhy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqfgvtdtk.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gcjbivpqu.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gknftyvih.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gvjqqrwok.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gjezxhpgt.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/giowvaeic.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gftklgywb.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gliozjxoa.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gmodbmtfk.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gwmsgerei.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gyudfmaob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gemwqfexk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gyzqehxwq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gwfzdyaov.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gitpqgtty.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/ggkvofgtv.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gxmfhemgn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gidgeplbc.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ggpaacmbc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gopxlkhtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/golpxnlro.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gqkujlkkz.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ggvajudrg.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gwrynzuxc.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gesbogstp.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gfxgdyhyq.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/guryuuyqq.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/guvgruyqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gbwruosfs.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/guwybeazb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gajgetrrq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrqweii.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gpqydrtub.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/glpslddny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gfidxyydt.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gmefxnpmw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/grrzrikua.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gwwnirlzt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/ghvemqhkj.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gjailoxls.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gssjovmgq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfeekdytm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gpwphqnqd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grfxqjqlj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/geomlygub.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gsmlnudcg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/ggiarwbgk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmydcghno.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gfztvmpyt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gpjiuznmy.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gzlkffeba.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gcktmkgbr.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gweroqrpp.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gpoxdrthc.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gdvwinlbe.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gwhkfjqnn.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gnjntdhvl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/goerkoabt.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gdtygmnjh.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gjkmvweph.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ghnunjmly.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gilwrjccd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gyrgiitnq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gprhlhcns.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gappouhfo.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/ggsflvgku.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/ghranuktm.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gofmedwlo.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gqqwfcdkd.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gprmkqmnz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gdfoohqea.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gvzqxdzwz.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/glwdeojaw.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gifnvdlwn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gvkufgjab.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gfjkdexyt.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/ggkbhjivb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gtxyadrmy.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gewzkziml.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gnndqxydl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/geslymabc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gzyzovfhw.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gltblyven.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gdrqcabya.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gtierqmre.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gtugbtiwr.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/ggzmiykjo.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/goyyltfgy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gqehuykts.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gkrerlbcx.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/ghmiqzfvc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gvuwlaeva.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gpnmzcgkd.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/glifgikxt.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gkrcfwsvm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gdrcutbmd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gfjelfzqx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gapinzpwc.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gszksnjkl.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gojvbraeu.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gjkzwxjpn.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gdgwfsyda.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gbrnspflw.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gurhekhpf.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gtsmjyyga.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gyftfzaim.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gpnszxujo.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gpcxaject.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/giplzhmyb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gxkyrvdwa.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gzfildjru.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gfojatjaf.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gdijwesqi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gvaqrovqc.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gogfkzbda.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/ghseeabgg.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gkkwdjuxm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gyojoaafy.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/geukueslk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gkxpnyvzn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gbggewjje.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gghutvfni.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/ggakherjh.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gdckauquz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gbsiyuuzf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gqyssbakx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gyimblssf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gapzicjmg.sHtML


<!-- 参考信息 -->