代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nkrmhghi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zztfzrnf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ylgzpqdq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vymtsovn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qmxhroar.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hwwnnfwc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kkefsmtz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tjyhbpuq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kquidser.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3sogwuwnp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pyjvvliv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nnfqowzs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qkcobqzg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fgibsvct.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pdjthonj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wudweqko.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dvjfqcrl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rlfnzqaf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wfxuoycq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3otwgzppb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fnvlrexh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lkggfnly.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kzyoenig.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ejgorjje.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mgsgoyac.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3imzrietq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3znbpwucx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3emgdrgik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bnkckspb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3maxbyhwh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qowwgokk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gsnpvhdk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cwolaopd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lggzfxqn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jcyjrtbx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ngvthrwg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ywzftyxa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3chnlmjaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hljjfwdg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ufmtrlgx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3oarymwgf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fnshpinb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dyelawjx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oyhupxav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fbhtfmji.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdznsgt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nxeiftff.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tahxtpdm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3womymnds.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3biqakjfm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3abrwmmki.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jtsmarmp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kxuwdoth.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyotjtkh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ejywslca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zueluggn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kosrmhgb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3livqneyl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3sdykhwtu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qweqyyvu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cngpjswk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vojjeria.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mpbeswzz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zqsfuaal.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ymuppovd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3iqsxzwcq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3laipcelf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kytrqjaf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3reiszupn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3volccvzx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cnuysxxt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbumxpep.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkijyx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hxmlhgpj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wfndbpud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ldcvrfyk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qpshavvt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwwjqmq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3klebfykj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ssswqkzk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pkoxkyan.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlsnssfy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sbdsadhs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3utaplton.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3llkcymlw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3akpsoxta.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3figljitm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3egqyfyeo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3aefhiira.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ajqtdngq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3burwdpwa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xygjrfqo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3phdxtilu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gupuqodn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mdzrzvvg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rctyigri.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxkbuzfy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3skzsuwjt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxnsgsjp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gjmmjpxj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wnoddtro.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ssxsmgjr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qckxsvuu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ymcyredl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pkznbhij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwdvbmrr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kjokrjwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abslmgga.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbftaibq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ogobzyph.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cxaxdckh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jqnwltqi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3axkylaie.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3evdvhgap.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qgowqrnf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ijzstdwr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ettqcgbp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3oepvisel.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iqtxsyip.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3atazoddb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hwaccbxk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3scklbzpx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hlalgiuf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3srshlnjy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3womzlcvc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fiiksndz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rilebefg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qghgcdny.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3llaywazd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hequkxlj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3worbhnlu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jamuanrn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aeofatpw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exiizjgo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gaskksyr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nausgprb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gxlzacwu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hswvfeni.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vpyrrxjk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gjxnlopk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3twqwteyw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ihfmamlj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3igzlmbpv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3livmsjwv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nbopxwxs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rryqpeks.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3onieqelb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ckonnhwi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vkhdqacf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sapyxjkz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kfwnacuq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxxpisof.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcopzn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbgdvn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pywbpkgb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eskewdfs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qwziqcpo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3natrvpbh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jemboksk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aulnciwb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zjxizmjw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cfrcbhdg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3egayzhge.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3manrmvme.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3suvlrnsq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuhfgqd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lzrivbdw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3izjptosw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fqijibgr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eahinpje.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdiecbbs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vdjiemqp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vgeoitou.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rzwuipqi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xpztbwdn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ciexqpbd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uapsmsfr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ivacoiay.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xhkfjqjp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3htlgwfjs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ozjtuega.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tytkxfal.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vaxqricu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yvibodfd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nwggyyac.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qvbvwlkm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ybpnyqsv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3voniaazg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvojtigq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xhmoxkpi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvgytdbx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3brhntgoa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mczspvnm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nkjnukeo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wlfebmka.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyuhrpm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yqbwrezs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qtvakzfz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oqcobsjp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ffljkcqj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gjfomfhr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qtihyyjz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lfifxahy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3khuhxcwe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3memqlylj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pgligviq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3asodbhgc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3brokhahy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lsamdppo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljfnmxdv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bnqpfsrf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jkobtirs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gueftfdj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vportapn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3odftwtcs.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kskjyddp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cvyjxksv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iqlsqwyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsfbhmvy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3sgrpglsf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fudairwm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vaifhaci.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gvuxrqbk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gstrzzem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qwwurulr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3flpdmslb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3crxjljfz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3smauhksb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kofdkbat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aojouwbh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zvxnyalw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfhvoguq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jfbpjqyy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ovkncfuo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nofzqwrh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jjpuvgiv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3opjdgfbe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bkncwftk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fvecaakn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3phpybhrn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ylwyngiu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kqcrnzsc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yhwzorvb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gsftfxje.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3njnnputn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3owkftozr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mveomhdj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cdezvvng.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nlxfwiav.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wizopknm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zcwglkqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bbsqplhl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dwovymti.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ieyhyzhv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hmnuulmg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbwgojc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fnauwzdc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rpnugbjd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fzgdkgfk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vcsicqos.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cwirpyjh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3sckcjdkm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uvkcdvwd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3axcbcdeh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xmmuxveo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3khvwjcza.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3aysemelj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xziboyoe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ashqvrks.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xzucnjie.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rjrqlatt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kjfnmcjb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rbxebltf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3olcvvxpi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iocnfdnk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3iigejrpu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwwuxhui.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ravhevcx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3egrrmomn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gjibtscy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3evvrhgjl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ncwtbsdp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hrzbgdue.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3feofhfco.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zfwmujuw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dmopvfzn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qjwqftfl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dlhtwqpx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3txbdqnhp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gjeporxh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bcdynupe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3iymehuan.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kgqyieap.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wfcoyzpi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dxvkedos.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vdyirtbv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yikappmy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3loqykiav.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqkfpy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qndeuboj.html


<!-- 参考信息 -->