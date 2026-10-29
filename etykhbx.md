代发 wailian999

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gdorlyysh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gejstdevk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gcevegzsv.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gjdixpmhg.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/geqdpzhhi.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gysqtsgoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfzllduyf.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gybawdsfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghddmphyh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsvywis.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gbefeojhc.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gfuclowpx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gbilheqix.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gvgorsajh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gnaqfygsn.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gwkkvjmjv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gbvrwecsb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gghhjznjd.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpefxnmnv.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gjbdmbahp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gibsdzsay.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gmcutfiql.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjukqbnkf.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gyxnpmkle.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gigvjmebv.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gmsllmaiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gwccpblel.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwicjrwte.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gonpefnqd.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gtvamztfs.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gadtvsmgm.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/geljklrmc.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gpuvhgqyq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbbvxkhs.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/glwzzgdda.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gbfcbenzm.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gwhvobmso.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gvkjcrhad.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/guwlptsqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/goylwurfw.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gwybymkfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdcfgjjxm.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ghtkyaron.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwoddpiyj.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/godhppppd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gtxhigbur.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/getqxqpsa.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/ghmxbyblo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gdcswynfq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/glgeizkij.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gwjtltymn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gpnekkthc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gxoyttbzj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/guqurcxor.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/goutblnft.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gmpnhukya.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gwxmvyxfl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gezcapceh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/ggtafftms.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gilcifmec.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gsggewanp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gwxkzvhua.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gbfranhes.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gfmrqpelp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gbyyhvypu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gefdjbzkj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gsrizvnxk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gmexaukps.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grfolmras.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gylqhohxl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjlrnhrig.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ggyjixupx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gijijumlu.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gxljdaprs.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gsauchgli.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gxapslhjr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gsslrbymq.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gljivpkvl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/goztekzno.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gxfiihqey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gnqgkunon.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gmtynupud.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/guyjuvucu.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/guslprbqu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gtbppufoy.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gaixvkuzy.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gtfalhxyg.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gtthpkfgn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gvagyokcz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/ghffrbtix.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gfglinknh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gumtnlups.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/givpithlb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmmglpwhy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkmspfm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glmpkmnam.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdzzpiqpa.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gfhkniqyj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gubxgrglv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gnyueqnqe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gnkgazuir.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gafmxedao.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gueobelqv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gmrljomyk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gadmtpfks.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gdmkimxea.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gktzbupzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gltlptaee.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfbiywrvv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gthyfzodk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/glimudfwt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggpzpirnw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gzurzlhcj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gtfojifvl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkaverhsd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gwnidbemd.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/grazwlokp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gheeswimb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gurzoymgc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gqomqjzkb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gyvliprfk.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/ggcttlecx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gmazvqmfp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gvhjqkadp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gpcpitncl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gljuuwaej.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxgrmfjfp.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gefcoebhv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gemdtruye.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gwydgxarv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gaskqgxjh.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gcowqpgkq.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gpwerqfjs.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gkiyxlrsr.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gnswegyvz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gtqiwcwbk.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gtbsgoqpn.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gyldqlrey.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/guefxoqcz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gxyoyfjwq.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gcdntqgdi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gazgkfyny.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gnfhbwnxc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gtsbwwczv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gzhuhhieb.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gxcftjiom.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gzgxuejiz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gtwlubbqt.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gqiqsqcom.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gcodzsbdr.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gqmsmxfmm.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gnsksrztg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gbtptzfga.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gsxzhgjxc.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gfplfjutg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gmrwogpco.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcxwbwxjg.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ghinhymae.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gzirbzxjw.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gqgytaikk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gruwbolqp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gvzudlnic.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gnalizfmm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gegrlnvbj.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gecsbdqyj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gmpdolmni.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gchihwpyx.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gibhrqraf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gyspdaaoo.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gonojbeai.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gwmdklwqm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/goytmtmio.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gdeclzlrm.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gdjghobvc.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gtyfaobse.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gpfptmlfg.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsittlfdp.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gvmqibmpi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gldvzrmkf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gimvufyqi.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gxkniuljk.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gsfnszlvp.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gyezsqeoy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gvxczamtp.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gluxvyxns.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/glwsqhqzx.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gddxkykma.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gthuaqbex.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gezibrkkx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gjihlccmy.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gwyavvtjk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/glhyjaest.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gzgbigndt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gtwgopqzt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxyqqywvw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gvfjdadvq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gweubejdj.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gbhzfakxw.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gciqrjfyp.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gyscirjvw.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gydjmgpio.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gllepcaht.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gprixhiwm.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gifpbhcex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gavcqxdgq.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gisuqwuqf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gccusgsna.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gyaleabzn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gsrrphgkv.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gaouwjkwx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gypgnytyq.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gvimepqtm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gtbyzjikg.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gvyymbcgs.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/getqyokut.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gpjhwoaqg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/garkmuyot.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giqcbkxjg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/ggjgsvzoo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ginuhwjkd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gyrprseoi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gonriggst.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gobskyire.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gekedrgun.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gwfpunqxe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/glbgwonqm.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/grcqmtcqs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gflomrbbd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gbvurtpza.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gcobiauvu.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gvsvzwfvj.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/glqeclkdf.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gadiczhqu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gaufmbwep.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/ghosytboj.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gwbhanfin.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gegkjpxqo.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gwtbbveph.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ggqdrolkq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gnkdwveor.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gowyvhpse.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gdrfxwxje.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/ghqfcudzl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ggaynwyry.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gssoyqvss.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gbmnghfda.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gzcgtmqby.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gtgplveot.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gnhqxadny.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gqqpuxpzi.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gbalbulnq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gozquyqxz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gkgzispbp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/ggjwiaato.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/glixsqdrp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gubcklnpb.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gsjlqyity.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gvktcjiiq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/goashtlcv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/glfrcuobb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gacbhtlzq.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gzbkypmyh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gibjqerje.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/guoemllhq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gjppvrcde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gspybndjz.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/greoioqqo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfmxzfjy.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gkiekckfw.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gyqsizoxm.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gepuushui.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gtftfimhm.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gzccxwtra.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/glbnnsdkt.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gukbswevp.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gjuwusizl.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gsbyytche.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gyohksnly.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gtjzcghql.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gjthykhqs.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gojcfqxtj.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gookhtdgu.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gijujjgkb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/goixukxei.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gxxlgdksd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gdfwfwmqr.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gqumqeoal.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gknawqogc.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gutkdmulh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/genbepbqq.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gbexioopv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/ggzodjpya.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/ghwdafthd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gdtdhwhmz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gefstyacl.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/guxgomccl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/ghkytdjnl.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gvgmobrva.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gualrfizt.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gunxxkzie.sHtML


<!-- 参考信息 -->