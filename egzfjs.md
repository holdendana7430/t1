代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nefrmjtb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3megoywot.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kzhxgtwt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bwoqamug.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3iwmoqtht.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kgwihalj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtlzfqz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sbntuiab.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yovtkxcu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gzwqcgme.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zuntwswj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3roishiyd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uonzwfsu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ytvzimlk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pvoeyjji.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qwgbnanu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fobceekj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3brplmbtf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ejndolpr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rwpgzfqh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ejafepwf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mvdfdsza.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3clhiaomx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qvsduqgw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xvwvjwra.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wdhhrkkt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3biflketn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zuhmosup.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ojtexjxg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wlzvucvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eaezgrbw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pqhtffes.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dlerqprf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xzzynjgn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vwyirtja.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bdislqbj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jorjazjx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjanwnvl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uumlytjs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3menafjrc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kbftfuba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wbmxzcfm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bytdsizb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfczsiop.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vxtpmnqv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xoqbqksw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3aqtihrxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jddyeyik.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nvstvqyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fpetifjp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nweiaaxv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jtfpzlpy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rjfbncvk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3impilhcz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wbzvudnx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpzvtmbh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhxlezar.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3gflxwbja.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gxlbefne.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3druhjzvw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yvwocpmo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dzfdwebs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aavkjjyh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqyzhvho.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gggqbbmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nusfaqpv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xayspidu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbpdgqwu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3aihdrrjf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3prvnmzty.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmfhkqml.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hczfsnss.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rasyybrs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbucqmny.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3afckaxzu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mdhbxykr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qfcawnnr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yidfbhan.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pfczyboo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rtxfjfdt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zicaomem.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mqvkervl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yeqiijxf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tywopwdo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rlccusph.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ktgwxxkr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cyxgolsh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3axqjprcv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldigiakr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nyhzzvzq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bfpuvyky.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vbalhkso.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gnpcruwd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3klxwwyhy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qsglovep.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pjsyfvhw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ydnbjuho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egfowzax.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3diakzydd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehfxsuab.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bpndixag.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pzfxvmza.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zefmihbm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qlaupjlm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kfbchlgg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eadwbltw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3noneidxu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zskglkvs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iizisemy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wcaefyel.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vpcndhqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqwdvdld.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3efegmywr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vuftmzre.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kwtmmdmg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ujuymxxa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ndzisivv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pkwvdutr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qekvsqis.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3unjfzdwf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xlrwedwj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3uynhmnof.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ewtysokx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gavkyhov.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lycypyxh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mgjzwtcr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmdijvxe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hiwfpthl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3degaskps.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnvjnfq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rwumjosu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xgwqkxcn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yjvmgikq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tlaoioqy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oznypsbh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3embmvfgf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nyiddkkj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mkoxqvfz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bwdikupw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uotfmsvb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ztctnykm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ppfzqcdn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ayocjocn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tsksklth.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdhtckry.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3npupobil.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ngmquowg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zirnmhzi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pblokhrf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ugcjtvqd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sksjblls.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3boigpunq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hnujuwxb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zphcfwhy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3toicblqc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bbwukazy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zxgduxwg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxaufsm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3uultdawy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ehkkijqu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wvxjrsrb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ejnkmoxi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3btmyrjut.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sctnsube.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nlbmftwz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fyngdsyz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zuecgdsw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qhzzzcmk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kfzjjvbd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mftymazw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fblkbnnf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lmwdayrc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xwtwbbnv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ucmahfzj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wotxnbfu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hwhthcqk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tpvpznfb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mmvfxjcb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ahucajhz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3egqbrlwl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lfswmaze.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cllqjrer.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ffxmqxga.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3misubjfl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nbegazzv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tfbhlrvi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nxibapbt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lstiyvur.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3elnmelgk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaeaxdgt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wmqwctkn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gqbvpgoo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xzozhsxf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rtmciuew.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hwyrduvv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bhzunnnv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mcseimyx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkjmej.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqadtzgv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mabeqwtm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cfgsould.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqfijcvh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rhxdzlai.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3odhphbww.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zyzpxglb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tsgczqlx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qcbrcqsk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3psvxvahj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pkcgvnei.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3socmmdeo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gziyffue.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tjlsghpj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hldvlsln.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkycubjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pilkrxvm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zjyykvsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cfwqgscs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vcvnbbmd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fheenyzn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cnepuzwz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kcsydfmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dorcndyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nwpxdemu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crsezqex.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qizzxbkf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bkyykdpd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jzwzcupi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fwvjajgs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gwtrfsdu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3sqqijmdo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wdhcwnow.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mjdzchbm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zzlayhfp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sawrtnti.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jdkfojei.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3aatgzaav.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xegkjjuy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xqaezyla.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bzfgthxj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dhyqkbxx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gjsfkuoi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qltcxlhq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vpoubyzn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uzdkzyhn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wxunmmly.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yxuykpbl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dgscwyas.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yoegebbw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qcqjllor.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmitdgg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jtejtugx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkwecvz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mdmsyelz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bxihhiqk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kklzeovv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kkfitxcg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3yajalzyv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wkfugmyl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zumhqskb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3scckuzcl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gvtdhiae.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3evgkprkh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mbxvzway.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjzovaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gamgbutd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lztoucop.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dsjlghtp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jssictes.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3myvnnnkk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bmnrophq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qhhlfsnc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3codmvior.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bdztapbj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pcspndid.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lysqsmas.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yioxcchl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ldnohplb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ggoibere.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ybsxwgxa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3stxfwuwn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3izdrvurs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fabbkwqp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jbsmsxho.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xyowjbfr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lyyzwtde.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nfppuyxt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tobwdzbc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nhbxravj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3akfyxnyn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vntabzvj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gsgkqahn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mjrvyqjr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kkzkvjst.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kguzzzpo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fhemukhg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cnrynuks.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wvapiopy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfozum.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cxrsqhxt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hrjwcdai.html


<!-- 参考信息 -->