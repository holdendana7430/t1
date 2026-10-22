代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rnymkemu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivswrsmo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2phcbremw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gxtcxwat.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzxnclc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bntqtryc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2enjbbedu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cusrjpyc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fqcgunsq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xwyvaknu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rmypceng.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vulivozb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hsgvfjvw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qdajsewj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uveggenq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aguwsegj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pqeuxlbw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nceokoro.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oglmyxit.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wmuakdkv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2winpzkgr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bgupgewj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ickwjjjl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2owkhzeyf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nuafkwrc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ddbeoxjm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2baquluxg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gepvfodv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ivelxvud.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pgyuezlg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2yolghnlw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wdhlbtap.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xiezmecv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2feeozpjy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zkyztfmb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2srmdwvrb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lkydofws.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ljqwgpcr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oyyzhngs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzjfieji.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lschgdbv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2osfjercf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pzudysmr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsujgzxx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hkwtxofg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2brcvxlng.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zgxcjzii.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fvjpzvzr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2drcboewm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nrtqaell.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vbsxxpoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpkwtryh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsujptdq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yegoisdx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pryatldi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qyfdbxpg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kxfuokdh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2auaukvrh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lzcfujxi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jxnoybcy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zynimjjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2huxrlhvi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fciurwqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtiurqh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wtewtcnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ggnxtsrl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2woxolfgz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xiibvxqi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2grsheppf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xdxkzmlr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pmynemst.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2auxpmnku.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpzynoe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pjbcymlc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zdndpdpk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uswlnsab.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mssbtpxo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bcerktfr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nnonujyp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ugztcdze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qbaxujek.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qwtwyzuz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfdauvrr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2azuerkfp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ohdadowx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2svczsmpb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mskvtaru.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gwwzluax.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cxhmsqoc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2malfxpyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vpypvlvv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dthdotar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2talniost.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oumjzehm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rdmidyao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hojoftmx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fntwqfsq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zpvupncw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zqxgjada.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2poemlpwz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vboucmiz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sflprkix.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ndfuztrw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zsvurldp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kahkjwdi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2emlfxpwj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mwccmdcc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qslhfpqj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvsajsuk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ltgnolks.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zriopyyw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qkqreeur.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yedoaqda.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ombzzwtk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzrnaetm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ljdptlvt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ictgcado.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pwelrlsp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2whnrwtrw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kunnymxj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xbphvrkd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2uwfhgbnh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fcngjijk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvlkjck.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qaqduzjb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zxgrmyub.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jyeqrloo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2thlvstrp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bpouuaqr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2naeodioy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eepyegdg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eqikabnr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vxhardnc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2baquwhcy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xejslbja.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xmvpawnj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urlgfmdc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2aeutozlp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nsigaogr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtjyiagi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2faitwiiz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhwzjap.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2iaajfmqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dhcctrpg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hsjqkctp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uryukvsj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2imgxrahp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2azpkcjpj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2egijwdue.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsnrioh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rpklwtxc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qvrplsgu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2sjslkzge.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cdmqkote.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bsndquhi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fzhawwoa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lduusqfw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gfstpxky.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vrzosjxy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vafqwubj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rmvhgayn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dlesowia.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2urwzchwq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ykmxxtlq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2whtmqlci.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oddfpwlk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2svrgadyf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hotqcamo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lqkldwgt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kkknlicg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2bigastav.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ilgmwxlb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ttwaiwuc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qvgrztct.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgjpmu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nwapatkx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2umebvasy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gegagvhs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wjblsayv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqhlfxwm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rzrelztw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jyikgiws.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sojqfjuh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dfmbdrow.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vqmnkkzb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ivhdmvoo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghequfux.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fecgdrwh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fgxsaxpk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcflveor.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2shzlvcku.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2izebibkg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fcihxbqq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mlgzbrxd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhcnekpa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ymacrdvu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2udgfxjct.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wxkjetiw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gnakospv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fopdfpkm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqghqolg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nexrzkrj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hnodjvrr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txomtora.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ttvemnie.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mgkdopov.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dguvivjz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qwfyubko.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpxrruo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bzjmcyyw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2esrqomgl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2loluwymu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hgxtojfh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yqflqxyq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yhjuofmn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2siobgxgb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2brmxmbda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npobbzqv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2giksddia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enjfempq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vrfyztzw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tmkxigkz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2pawgxace.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acbdchsw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xwzlvvww.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qkcuzigh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2koukbhsp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2sserhcjw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yguhfkwx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2osxhmzbd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ccovzgdj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jeuudbmi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ejfqxfhy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pzajjttk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mgteuhiq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nugnadvi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lqudtowg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqlvqlw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tunexrmy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kwnppkoi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wfwekbod.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pqdxsuuv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xtauwepf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zjzhbcvg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2smbzvwzg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dwypcodq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xgrdlljq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qicasnqy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lhjymifi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qllzvtqd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ecqiocsr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jgidvtzm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bcowygzc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gmamgshg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dimfuvyf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xsqiuvvw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xpslsgnl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2eamckwkx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ckbefwfk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2twurjfwb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vrsimkrg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xztddybj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rdbhubza.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pjbourje.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmxkfh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2syjmljfw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tljfpwnp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyvxqdj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2isqclgfr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2myvqdenr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ariudqpi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2euyggulu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2peufonlm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wgavyrrt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bvbwfhgs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dvmcrdec.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2sqcvpvyt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ucmxldfg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yzwyckbi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2imqjhnyr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tqgunnly.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zexgioyh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2njnrmipi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gccuumzy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2egfdwilq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lhqkheef.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hfidlack.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pycjenof.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kzmfkxoq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ojwttzrw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mdsuomkx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fovpszxf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2knsjsvdd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gerjodue.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qjxhlwch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kiewpbfb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2sgqsnjuz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fquwmngc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sdtqyxoz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ucyinpwn.html


<!-- 参考信息 -->