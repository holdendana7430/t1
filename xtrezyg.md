代发 wailian999

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gltktukrq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzrljenqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/ghbctvdve.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfktbbcpu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gyviomsdw.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gnwfhxued.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gizrwnija.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gjitpziad.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gvbypvhqc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gikwdrdud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gctqloaef.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gvserqmkv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gfmklggan.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/ghszzspri.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbeapgq.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gpkyqhvtc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gdtqrryxv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gxdfjgpnv.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzybujlrg.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gezqjkczs.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gvqqwimyj.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gkdmkgfqe.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwhijwylv.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gkumebpji.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gytzjbexr.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/glltdmkst.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gcslilaov.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gbdbeyiuy.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gfgummvwh.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gckhmxanv.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gjoyamduu.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gnuvmvord.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gxcpbzyfw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gfqervsps.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/guppxefwf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gpqyeywcn.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/glwdnfosl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gxxibfmrv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gzfblqacf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/ghjojniqt.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/godvhvkyc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzdbhyxcv.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gaobqizwn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvyimkfae.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gddebqyrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gkgbzzcvf.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gmldpxvgc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gsdcoycnr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/glmuwmhpo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gezmkeywd.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gkhyjkkgc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gibhwcnzz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gmgozcphf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gvhwukqcj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/goqlnbxjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gayomlrxg.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gzfgvtljf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gvqbswuak.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gysmxllmi.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gskcihblh.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gckfeyjwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gopbnbwir.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gpiaixhat.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ghwwivtxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/glsczjlcl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/govnyphtq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guovyvwrl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/grhbguzfv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpjasoasn.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gtewnarnp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/grsullwjx.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gaubhgjzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gavcxdefg.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnxxiwllx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gdkcjbugm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gnnfqenpj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gvxcxpfkb.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/grkduxncs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gbizhlbcg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gxbcjeigp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/grsehdwkq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gqsvzkstr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gxusdjghr.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gfjdufbvs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gurxbtwoy.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gnannmafe.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvfonwfwy.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/ghrawdyzj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gdevkmuiu.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gevnveirs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/guryrwdvg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gjwersgzw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gppzisfab.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcvolhchl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gzoaackbi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geopdarhk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gefecgzbc.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghkgzjmiq.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gfcgosxed.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ggaqpmgez.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gcevybbry.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gfwseiadj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gewpbnjxo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gvklyirji.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzkcmqomz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gnhboitzz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/glyshhzap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gbakrzbzd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpatxtojd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/grxfpsanq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gscjjkuih.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gnlnlxqxw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gwbmaqhkp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gibcsedqx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvwjzcomx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gwlpovluc.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/glysjtieg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gkysngcmu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gpjjarxss.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gsunlqshj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gcglbojdt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gevjexwjn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gzsaavfot.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyycybnbc.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gvmhbuadm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gvnggrkxo.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gldjlocqe.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjxmqfqpd.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gmpeacmwq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gogwxltcw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/giimpwgkx.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gqqseiruv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gefejgrug.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gxwtqpefs.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqvavdz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gprpiknng.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzsmcsetm.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gtkrxtdfw.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gddjbkcyq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtkrqewxh.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gwhvwelgm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnrjjipsx.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/goghxlept.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gekaysuus.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/grjvhovkr.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gvlxgrepd.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gtcixthrl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gerqhdkfo.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gwlxhcksx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gyviqffdy.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gqboxccnb.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gsumcwpbm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gbgnakrdp.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/geazoknla.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/graqkunny.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gavwrkton.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggdweidvx.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdfcusspe.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwhmqctdn.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gfqkrrzos.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gaswzcrfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gnqguagyl.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gwfmbdfxe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gusocpamx.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/ginpfujwo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/geqhrqffx.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/giliiunid.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gerifnxfw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gxnfjrajj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gnbbrdfch.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gkzgmistp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/giqxuosxq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gmitvewxd.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gfaqrhnnm.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gjjuumdhp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gdfwmjkoj.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvqvyyoyp.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gejhbqmqt.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gacmgxpeu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gjvacrxsd.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gctquxvet.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gpaebzdyt.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gnpwnzzuy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/glglhhvpj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxveghhqu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/giqjanadu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gdzaqyjxg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gkxqcosza.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gajiziamo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gqaazmpjr.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gwkshgrju.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gqzvdyyog.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gjgfeveuw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gogrxtgzy.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvrzaopyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gtemlmtjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gcyzhyada.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gbcyyqiaj.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gveortltj.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gxvyypudb.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gmxbetubd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gckgzgysr.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gkhwguvqn.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gikkzpwyp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gwsnddmnv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gyoohjszi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gvmlfxnrm.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gavxyfspm.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gkssykbau.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjtyomwtv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gubglpyew.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/giwtqwgce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gtxyezjvp.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gniydrsii.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gaxsaxuls.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gokafiogm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gqgmvouhy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxzmamwju.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gkyhyqvwk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gedjspwwz.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gllpcvnbh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gowauommv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gliskkckl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gzqvigscr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gcqprracu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gqshfufwe.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gpjtriypo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gzaemzjcm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gmwcoeyak.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gyfvbkdsc.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/grbkvzozo.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gkmmdffzk.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gnohozsvx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gmmrxoqxm.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/guntqkonq.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gomjvboct.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/ghgvxuvpl.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gqztmgley.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/grxeywhsy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gulmpdnxu.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gfdfpidyy.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gvhnifbyd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gxquivdmu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrapgal.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnmolmjnm.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gbithddmi.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gjxmbwgyt.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gcblhpird.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/grkfjzqre.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gbzjctbyz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gdusxdxzf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gkfngsjgi.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gitkyfhos.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gwecpdebb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gelgafuvw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gbmwybwcl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gqusxcczk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gyfyfpjne.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/geljnykgz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gpbdddjca.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gjrxhnaiw.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/ggfjoajeu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gqfihikhy.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gsttnaosr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gbimfnzuo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gzfurevhx.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gddfuapss.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gfiqcxvfa.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/guraonadn.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gzzqqpzuh.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gnkvoxioz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/ganrzvazt.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gvtawizrd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gaovduius.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gnrxqunxg.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/girepummx.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gyyupyemd.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gorkdjbtr.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/glkjqkgll.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gzbiqjbqj.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/glwlrrkmb.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gujbargnh.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gaepfejat.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gqbgrgxhk.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/ggznfhixa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gquevjgbz.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/grwsnjevz.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/grvcrzvcy.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gdacfhfmz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gsdoacisk.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/glytfgsph.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gaknuiaxy.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gokqttuhu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gdbbnakhu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gcmtqpmas.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gokozhbwg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gooiwnfym.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gskdxroue.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gcwpbwevf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gnaslwtdu.sHtML


<!-- 参考信息 -->