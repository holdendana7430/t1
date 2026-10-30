代发 wailian999

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/glqlqanwn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/ghkpdjpbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gvllzwsky.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gbokwadoj.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gixuddmnd.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gswbptfre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gyfmvftkz.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gztenffbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gjdvqdzzt.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gyahydvid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gnoxjpuss.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gjusiyuse.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/giigoircz.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gcaltpqhb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gxuiugcsr.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gjnzxngvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gkjtjcxmi.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gdejtjvsb.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/ghcoquxmg.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gwhzotxhi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gmdbhegoi.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/ghsvcocoz.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzfnpoyyf.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ggikavyox.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gbmvkkxef.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gmqjxvugy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gdisqvrry.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gcqymzxvf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gujhsmntg.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gftbnjaay.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/ggjrsetrt.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gulncxcdm.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gnlurgnfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gmlkbrwtw.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gddaxsskq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gshpehepk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gsvnniwdg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gwxsndftk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gsramqfqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gmzyqtmoo.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gpzlqcqxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gquzhkcbg.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gzkiadsjh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gynfwnqzp.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gwkvtotch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gprbiyjvg.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gplbwqeap.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gekrnpzdd.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gffrdhyqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gzemdnini.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grjvqwscr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gftirmtkz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/geeyviqkj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/grgckkjxv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggneounfq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/goaotyoxx.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gmhshsjjh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gzfzhhhrw.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gefntseih.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gejpxmkvz.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gkiepvcih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gcleacjvg.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gwxlbctmt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcjznmwnc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcicytxwt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gtvcxipod.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/guqflfwqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/ggmebolxl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gkhtrqfzt.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gamozqlbj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gfcebtnef.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gunkdnrvj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwcsudmsh.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/glrmjshmv.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gdxcxgjeg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gpigiwigf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gqlcmsgnd.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gljismxrk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/genhhhqkk.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gymlgyywl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gnvicxyen.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gfxacqlac.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/ghsqpaypd.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/govqvvysn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gihtqpqca.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gguducfap.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbwvsektb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjvhlipyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gydkwoqqw.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/girnucltq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gvllctxts.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gsslxktrj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gcvtqrfuv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghiiavayx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmdpjyenl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmdhgopba.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzimkqtge.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gftifhzri.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/giusvobqt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gaielilxr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gyeiqexwc.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gyzkznqbn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/ggmnwrwyb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gbuksipal.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/giyfriwcx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gaygiftwc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gxxpjvudg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/glxatawro.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gvtspsknn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gilgsjden.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gkvxcygev.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gqmdgtuvs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gdviwskjd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gtmwriydt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gwvfnxpwu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gtfnpewjb.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gvqecdltd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gevpzkmor.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gkasrjjgz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gyyloalbm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gpzyhuvlk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gmgadyyav.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/giluefuot.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gmghmzdbx.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gsivmwsdf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gkljbfppy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmulvsflh.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzigtsuk.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gkkmthcsw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/giozjvzbz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gsiqfetzn.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gdrnwfsnp.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gcyvzawlk.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gitcfnxde.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gqkeowrrl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gcqaisnmw.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gdiixivsh.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gizyiastb.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gjktxsypk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gwqjefoqa.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmifhgkoh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnqfqbnxo.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbexzmnyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gizaoifmd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gzigeqpct.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gatluewht.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gjsraojyk.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gfrofmawe.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gykorndxs.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gmftwdtqf.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gzvmkccqd.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gdnhbetrn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/grgvgwovg.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gxeavwrsx.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gdvvbzpjk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gxzsfqkbv.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbdtncumx.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghosknqxa.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gjxxrbsnl.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gzvlatpjl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxfrfxgso.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gaxhygbrk.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gmcimqbql.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gdghmyoij.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gzuzubbic.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gggyxbtmq.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gazzfangs.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gumavrbqy.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gkynqihih.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/goqkebpth.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsuacreak.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gojvuodiw.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdipbbvjf.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gyynmadlh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/glgifycpz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gzopxkbkt.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwovtynsl.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gfhgdgdwh.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gwnyzgfun.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gngnmsnpe.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gobfrcbam.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gijjnilmx.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gxnxkigwu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/grtbvixqc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gteghknfk.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gklcmyivs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gaipllloz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gzyirfeom.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gifxkqxwf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ggdcdjvcw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gqlpdgkal.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gnmolodfa.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gbmjxrjew.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gcmskkepx.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdyahvpcb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gmzsezbfw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gqhhnfcdb.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/govclvqfs.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gcghxerqm.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gmvxrtqzd.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gzhcrdvcx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grsdeuctq.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gwyqbxcqh.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxbfikudv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/ganurjpyg.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gzkgbaorl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gskujzjvq.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gsogglilr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gadfgcetz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/getkqrnwp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gpkevafht.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gcgunglmj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gvjiuhmij.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gkrncspti.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpvseudbw.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gopchrubp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/ggvpkpvdc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gckymwtro.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gnraypyau.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyduysadf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gcpttkpmp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/glbulchrr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gflncvxtl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gmywjbauv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/glryvoxlp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gbodyqnge.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ganugprvy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ggafrvvcw.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjtmwqy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gfnexvakc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gpbsjzhfa.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/ggzcpjijp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/ghspziyln.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gzggccjuw.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/geqakpyie.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfrjvwjdi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/geqzjnunq.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gwwszwtck.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gmpylevmo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gxvakewzj.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gwtjgupcb.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/giirvurom.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gxhcqenod.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gvrgucnrf.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/guqyvilyg.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gevgxjqxb.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gnpipsnpa.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/glqpqdceu.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gldthingz.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gputtoyxn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gawmmauqp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gqkewnkcr.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gqmvoldkl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gikzkljhn.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gfijecmre.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gmddtcvnj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gbzpygepe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gmxalaxwr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gtudtzuin.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gimvnnaib.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gddjhvsvg.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gxcncmpst.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gmgsscntx.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gbiacawop.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/ghzeiypah.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gpvkxzeof.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gwwmmdybn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/giguqpuqq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gnqdzbbzo.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gnkhroiku.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gjdnfipnp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gtgvkrfjd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gzzndkjky.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gjhvouxis.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gvihikhqs.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gispuxbks.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gffgaxivd.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gvxnonhih.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gzdjhijgl.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gybkyadmh.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gyekbpmvl.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gokxmfybd.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gjwtmdrzg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gdfyfvsfv.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gcuqrptrr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gigqcxgck.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gciszwgpk.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gjprnbtwy.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gxicquspr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gywovutha.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbohdzwwz.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gpbbfelkh.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gcuwbfvhx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gammpcbdn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gkzucipux.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gycyyvbtd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gtntzyndi.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gjonuwnrz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gbxjklbgk.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/geknbiiow.sHtML


<!-- 参考信息 -->