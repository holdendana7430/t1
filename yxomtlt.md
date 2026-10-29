代发 wailian999

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gvelxbefb.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gfvlmjntd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gyzoickiq.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gspanrodl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gmdwfjzdp.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gqoiyjvpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/guyedvcdo.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gfevuzdoq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gtlzrpasb.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gsqxdggng.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gvglxzbwi.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gltxcesig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gamvgxool.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbzeuuafy.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gblwapcfk.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gsqowzwtq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gelrztmqe.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gaxvgccve.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gicdaflos.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gunnzktys.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gxiqynzus.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gqlqxfcxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gopsfuvdm.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gqqhuxazt.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gskkvmnne.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/ggyffhsxu.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gvzxqzpjf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwpnedeaa.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gnzcalkbz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gvjetdkjh.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gowckeito.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gxgdsspwh.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/giupevjbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gusoeglxp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gpsztbszh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmsrqzr.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gwhbbfxss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gwsvgbeoz.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/geqxwfnoe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gejwaeflw.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gfzdiewad.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/ghqxopmxr.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gjptfisiu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gmxdiollw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/ggspvafnz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/ghurwgwmj.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gaamsvkun.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gjylfctlk.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gewwosljv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gczojlrvu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gnsvsjkzs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gwmmczhaf.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gmemcwlrc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/guffnigdw.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gajhbbbyl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ghzvuaeiw.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gknftudqt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gnoguxpns.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gayotuhoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqunrndoo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gkebswymo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gjygyqrhq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ghretrktj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/giipsdmmw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gnkegwleu.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsnzmtvdg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvryvzrea.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/glmszeoir.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/giczolfej.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/giemwzgyh.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gcsiopqlr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gxlocgqbn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gvalcbgvk.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gyruonqme.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gttdqvblg.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gklgcobjy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gvmzjepnv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gxsvwndkp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfolwdecn.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gzoyjvxqm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gagpdyrou.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gforccvka.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gavjiwkhc.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gleclokrr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gdhdyklyj.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gzfegowsk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gsmjbwose.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gsnggzbdg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gprsljzwp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghdkvvyyn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gwamyeecq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdrerervc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwzgwbitr.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gauzkanab.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gcdysstmh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gteeojitr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gzcqvzhxn.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gbpvhzopc.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gqxljyzsf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gxellatcc.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxhexpbrn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gliijmfvj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gpoehkzlv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gucloizlb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdnuaeqii.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gjmkfbghv.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gtwrtfwda.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gehbmlmow.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/grtqvmzpf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gtczddkks.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/goiykmfjy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/grqxfttnh.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gtahtqyeq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gvfzrgcwp.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ggihdnomn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpydamstc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gjlxynvyl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gathakllh.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gaaissqvo.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gvismdupd.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gsuanudjb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gggotaevo.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtnqxivlm.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmfojfrng.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gnnmjcqyq.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gyvkevbcj.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gfgtnpxqy.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gwjmpyoqy.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ggrjgojjl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gsqptiajh.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gpygqvmqc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gysfgnfpe.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcyuvntrp.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gdyhqjuqn.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gdzognqvq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gytddesgf.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/geqhqkgcl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/groflhwcr.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/ghikngjpd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbsdvxhkz.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gdtoplheb.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gxfeaghyp.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/garubxsiv.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gelqpdsiz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gqdzeuxgr.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/grxhvjigu.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gfuxzayiy.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrapsoec.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gwkawczid.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gxlpjqmtn.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gxfvmovvs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/grwxhfxrx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gajqzrpms.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gizpqksrz.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gbzwpdeub.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gjkrluffw.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gwmycrswx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gxzysjpdn.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gledwuhry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gnydptjzb.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gkuerfrxb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/glhhopbai.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gmfgzplnn.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glwpatexv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ginjtbpik.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/grgpgwpjp.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gucparxhs.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gxuxkwncl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfqujgwej.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gvldvxjty.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gyvcxwaxm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/govjgortf.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxonwkdzx.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/griugynmb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gjqdthrty.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gynowccmt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbkinjppj.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gfzhwqdso.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gpoopwduz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gxphcjrlz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gdpkpnerd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpqcwjha.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gkfidcjat.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghorjzmcu.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/goxzxtmeo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gdatozxwq.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gzmehnzyu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/giywifpcj.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gpnklyset.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzlpecwn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gujkehnxx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmyvoisf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gaosdkpvi.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpcwmugow.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gopzagffw.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gkchgvhbc.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gifhvdywr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glsfvuuxo.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gpffstdmu.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gfditmrhl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gadiyxnbu.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gewkozrxq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gmeyjxxhi.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gluzuejmp.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/guvngznek.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/ghlcrrmoh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gzhaqblkk.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/glecsngcn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gcvvwrxwg.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gzwmekugy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnbebjt.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gikyvndpa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gvmxwelxf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkkmfuqbl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gqrnzgicw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxozablhx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gcpiuvhsy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gqxtlposu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gknjxjupi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gorxuyoax.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gpjafruyp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gsczakrjj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ghkdaclzq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gepzujozj.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/guixvzdgn.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gadthaxmb.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/ghgccfhyc.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gdudhprcl.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gqmumigln.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/goegsliof.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gyppzoghj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gpxalwisu.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gjiammfzg.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/grpdnptpj.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gaxezvdyf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/genzfkqtu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gwkbxndkt.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gghepzfcr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gsyzqzswg.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/glgpfkogz.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/ggysluzih.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/ggabilixe.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/glooyxbic.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/garpobtnx.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gqtengfpu.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gitpvqrft.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gohsnymcn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gwrgcyppr.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gunlshwes.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwldxmwz.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gjaphfnps.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/glkyrrmcq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gaqxfzjbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gtretwmoy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gsgghclxx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gtmzlvdcx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/ggtpzuplh.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/glrxkavnv.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gzqqbvrqo.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gbpmtxovl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/glvgivdix.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gyvabihbx.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gdbpmrwwd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/grtwpjrys.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gsezaqiax.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gyojbktos.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gqmkmzdvk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gcvzaonev.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gnhdaiqnp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gqeggmngk.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gblvtzgwm.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gjpkhmnnt.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/glgamteiw.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gzgmfzocn.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwoxgrzfc.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gcsgxkqgl.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gbmbijwyt.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gaiurvcxe.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gxvmcxgap.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gsxxmgxtb.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gothwcdms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gblzcdvsj.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gwajgnuhd.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/goaysmxay.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gisierniv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gewlyfxqs.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gahkowzay.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gvjqfoeqn.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/ggxrqpxxb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gdoluxvhs.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gmzsqcygm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/girisdczp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gzcemrtdz.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gtrsvygxm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gfxyykmol.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/grpfmvvpy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/grhjnzdbm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gzciacvhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/glukgevyy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/guhckdsbg.sHtML


<!-- 参考信息 -->