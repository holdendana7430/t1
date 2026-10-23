代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kwlcsjwx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3njuhjssr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3srezydld.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jtwrbjmb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cegjgjbp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nhlwjtrf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wliwjoxc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3szhmzyom.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fhgzbujf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nobfpmpm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hapvndus.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3senebyvp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rauvhyra.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sbmapxfn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rfjagznw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iqnlzgcd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ughahsvp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gmrmnrtc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ggqbsili.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rxtwbvys.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xkdoxphs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tbafllzg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bygtllow.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3blhsllua.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zgijfweq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gfgygbaz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3etnppxmm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lhmlekhm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kvodidcm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jilxdufg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qornxfig.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rbyhxhdj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3iiuyccqa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dtjvvvyx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mdyllmkf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nndgydun.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgrgye.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vhtyqevt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3norjxgap.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egobmigh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cpvfxnhk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shxjkjzt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtllvkqx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nrufaiwr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3idebbepv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3davqoety.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fzujvhyt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eyjzwlqd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3iyqviqta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rpqbaqln.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3eliachnt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ojxetdhw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jaiqxnhi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhmdeala.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dtwbnicv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nyugeinq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bjkpsfnk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hkbrvxgq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ycugobdg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wgbwazrm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3eqzntodb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yrmhjjcm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rpanzhje.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3imegodpv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uzepevws.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lvhuqhzf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3radcizgq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kxrdwgsh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yvyjpxzy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kcwtoypp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ywnnndkj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hoomxpvn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tlomrmup.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xieseztg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrpiahab.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lyqrbaxr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wyypatgr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdljhfpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hyccdpro.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3inhektvq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vxiwtspe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ljtlthhu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kdoncwzq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vdbjvawa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkwwoso.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wqbcnnwa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3earalyyk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3smpjlstv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jxtytstw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sthxnsjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txijrmjd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mndhient.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hgkovsar.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3siasxjvr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mrfjeouc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xggjiaeb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zhyxdgbi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zdtmrjuo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3atepfqqj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilkckmxg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xwcuzrmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuxusucz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ctyzgbvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trjvfyfy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwmybsnf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qbvhqyjp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3eivxzwgo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3flkavtwi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3isvwhwdv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hdrvxolh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nkcnejvf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wpmvylvx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eenksuab.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ufeyfhzh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wjnnxrmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tlsvftqe.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zzrrjqws.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dxmygdzr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mgiewcbv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jrletnmw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fshnybwd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qmanzony.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3thhoxsus.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qxezlnxo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cvkfibrs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3guihbsrg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gfhbmjmr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpcnyfw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vfjvtjcn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3arcygmxx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3habxdhrd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cnquscqc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3adhbhtcv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lkeguhfp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lxbchrnn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3firfofyc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cxkqwput.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wnygukeo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cltxtrjo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eravwcwo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ghfeeefx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rwczehzw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nfjalmzz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovydxgnp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tcuqbsbf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gpxvoium.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jsvqrvdn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vctepkfv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zdzfsgzs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpcowug.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xfcfoelj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oiyvejvo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3awggnxcs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3knhexevo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3muepdazr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpavtix.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mpdxrlzg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyzebge.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qgqqiuro.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wqrcpjgr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kwybyhcw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tbxfaizx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cuqefvqq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mfevexcz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jojructc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zvisqtda.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wjzjyyto.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfidqxkr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3emukqezl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hmvfvkns.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jthwrqsi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3paoxihde.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mxoeqxtm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjeocewx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmmtszmj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3phqxmvrl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3clacijfr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3quspzudd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qlrkexiu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3oexlkbkk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tjmwaimq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pewhhxab.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fvuoascz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fzsfyurd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jdebkcjh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yozxazar.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wotsryom.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xaekiviw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wtmxxjrc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fsjfvjck.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tylxllcn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kuracqwn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qouebmpg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvwfmvog.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mobpnahc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxhzqhhh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xjdrzmow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3smgdluip.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hhqtunvl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bdzrzygg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sohvqdwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sndwudei.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3abfrfplv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3apoxwbca.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3isndfuxk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hclvbdnz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjhojxj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lbjhpaqg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gzpkwecr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kurgkxgp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ysqukbrm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3esaznqua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqyrrq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3chpizgre.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3katadroc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zjaqjayw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vtyvksee.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qzxljzga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ftqyqmbv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3amzvqztq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wwumwifl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wovqsdri.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwqwnqp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3djgogqtt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ckpiorbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkyhrlky.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fdqtkpnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tstgddco.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hfaeyzpv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dmjwbewp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3paxfdjhw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xvnxrksu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3lcysmoss.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dhfjxlwv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zprwoewn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3murmifzv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yrodojtp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rdtfijjo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zuhptewx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vplodbuk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3srjvmcri.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qiyjncrc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tswqvdwd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3etizsdzw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tjfsdiuc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jvjwrvyp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rhkmjbad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rfxxchzh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ptqvlmep.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ulrnommd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3acdrtzhy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wmlifgyx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3osidxrdr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pszbales.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rnltgjyu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ebbjyygg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yxemgqea.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3iityxviw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wufmiavh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hvlnpugr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cffzhfoh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bjpxzfnz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3eiafizfn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ckovnnvh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3sctfuydp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wxnsfvhh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rlwddzkq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bayllrzn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3iqwzjdys.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wvcnhyrp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rmghpfrq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3sxnnfbze.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzqmeqbd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3sjphwxie.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3stoalzod.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fkczpohk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ascpkywa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3edumzvlu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ettbyevp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fsfuflnt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3eblbrzge.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qtnuhhlt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ihyhwoqd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ayyvmltg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vrzjcjqs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3slmqodrv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yplihwwd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nitbnjin.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3oonzppqq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gqejmyrq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vudmozop.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yslddowt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3akbrxzsy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gwjskzju.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cahyqjlq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdeegfz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fqrmnuxw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tnxgniaj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ufvhefjm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jcgkfclw.html


<!-- 参考信息 -->