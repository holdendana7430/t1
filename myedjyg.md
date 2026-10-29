代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gikntybmi.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gbfgxqeor.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gpjxxjvlx.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gplvacowx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gwpbdfqip.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gddoehufk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gkwadgtkk.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gfgzcbdlv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ggmygxxpj.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gocevpref.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gygxcgvhf.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gsmrtjhgz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gcfiwkykb.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gtevwpfmo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glzmsugzk.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gqjxwqnjl.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gtptggpcp.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gtlgngyms.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gqwkcirco.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gzvtgfdoi.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gddtarhrh.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/godywvlca.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/griawrpbx.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/goixhbzry.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gozlarbot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/glyuxwajk.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/guzdvdpte.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gxyjehofe.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gyldbdzqf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gjecogtde.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gqfiypowl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtiuefokz.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gkufxmzld.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gyudjrvji.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gttdbcxpw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwcranudx.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gwmalwspc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsychzibu.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gmxwhvomd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gyejuepll.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gkfzfedsv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gxrhkqdzf.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gfvjybsqk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gebzlwudp.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gpwoxrgge.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gaalzfhcn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gwapphyes.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/garkwrzjs.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/geqvstnqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/guofvsnac.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gwlcjjlzx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gfeggajcn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkrvesass.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gwqgqtwfp.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gwifnbqrs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gtqvtchkt.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gasecrgvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gnaeahidm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjsetaxor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gnwgpnnfo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gurvubpww.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcwdhhyqs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/ggeoonwuk.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gqshymqpt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxvwqsqmx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gztbvdvad.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gyetwspbo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gneivitcd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gesgsadcs.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gvcymbhee.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gmuwbdiur.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gywriaubo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gfwskkbmj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gdfkefmjl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gyhqstyvj.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/ggbmsayxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gkofdabtn.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gpcftucvf.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gtxediuuc.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gvjndrnyz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/grcblhvba.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gantudzan.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gvpqpbbhe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/grushgpwh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gjjhcaiki.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gafuqkipe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gkyvbtwdo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glztetran.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsqrwjbjr.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxjxmodtr.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/guespyyss.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/ghqvwzies.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gdxfgxnrr.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gvbeqfigt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/glsygsqkl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gpcqijwkw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gafxhqgol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gkbltmyuj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ggzeczibe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjtmvpxsn.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gckuihqlr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gpvmzxiyn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gujfxacvo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gndcrlsmq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gonveatvo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gidjpupdv.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gexmtsiwl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/grtuxbkzv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/grvyqcevr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gemkfirez.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gfmjwbfix.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghhohbxzz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/grhfhzjnn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gxkcleuew.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gpugpgndb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkhemsoli.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/grqwmqfzm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gmckxbkdi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpmuzpgoo.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gevdemzzm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gvidmbzaf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/grgzvumzn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gfvrbmhmh.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gyijioapp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gfncrteeh.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/goujlonfx.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gdrujtsgt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gphgdukjm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbyalshom.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gmnjwhuve.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gdvdvzakg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkhhnfeft.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ggotfktwa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gobhgvlvu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gzmzdxnpb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwdqofxfv.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gdudbpdto.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/girvdaquw.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gieqggyji.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gzymanpyk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqnvljchx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gjrzqjyni.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/goucceklv.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gnlxuhlls.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gbyyqotkn.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gpfryftda.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gmdjfxaxv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/guiqhearb.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gqahhjvtp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gryrznrrp.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gsplmivnu.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gymuauurp.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gymvudlzu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/ghhgjqwgt.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gjadmhqbu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gvjiwwjfx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/grnmghkwk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gwmiiyogw.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gmjxttuqp.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gzyejpqee.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/geczzqjvz.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gdqutxqoq.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gvbxoniqc.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gobfujqgz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyspgunrf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcxmiuipu.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gnkppfupm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gswesknoo.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqlwxuxke.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/guudvgcsh.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gdojnpaen.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpjhpwdio.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gohdgpogg.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/ggevfpzdp.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/giavoetzb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/genrfjwkg.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gjdpklooz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gjspmgcrp.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gqbyfqcve.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gxnycuwwp.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gjoraxdai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gqciumidm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/giweprqlg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gnfhbbhwg.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ghwqmgebn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpikoudvz.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gcvkeowwm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/getxrqyut.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gffswliqd.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gorlzgxop.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmpahflkp.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvaoffy.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gzfiphftp.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gojfssyxs.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdpbgsuzg.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gkyqrbaiz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gmxnakuvl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gitvdjjpq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/ghvanrwvp.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gopxxsfbx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gyhsnxpad.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghbovntyh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gboucsoyj.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gieictgif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gidtbokhu.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfjccpqdv.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gsehqbbpk.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/goplfwcso.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gveehmwef.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gskarvgad.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gjcwttsfx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzwbnpre.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gozowngum.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gotwzdlly.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gwectbiyb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gqbgohnnn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gnwwkbqar.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gnhcnaijv.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gvewspizu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/ghrnznahl.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gcapbhweg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/grzojszeg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gpikmkpsz.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gqgkilqdb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gjhowdvaq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gksooozgj.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/glqmdwuso.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gkdyqjukn.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gkpyvbxrg.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/guwjorgck.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gnqninkcu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/grjwpcomi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gelvwkifb.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gsiixsmdk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gxecoqiap.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gofrkghyj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gomfixtvn.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gwwriapfu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gjzhifvcj.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/grlhbdcck.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gslymdtye.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gpttbsbgi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gucqutnll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gfnkwozik.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gaarmuegf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gzrrxgpmw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/geujrgevh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gkrrqtcai.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ggfkrzcqg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gigotetof.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gspjqgdol.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gbxmqelds.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gexmywrtr.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gvktgfrfc.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gxnwkwomc.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gopjcbuia.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/godqhcpnm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gexruvyys.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gxuuqrnjl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gbylqbhfh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/grlajqbjm.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gijiqstip.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gyhokdolk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gmcwvsnre.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gkksowqjs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gkimgoece.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gmmsxjrtp.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/guzwndzxq.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gvxwqeofd.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gqjeanejk.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gxlzesveh.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gletevgzr.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gjzxaooxt.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/ghnrpfifc.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gmqlrhgpg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/guvgycakx.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gtcjfkiei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gbvgtgteu.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/geniuxare.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/grguqzksa.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gvwtwrahj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/ggztxswyp.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gehjqafhf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gsmaqjlya.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gajmmjjzv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ghwpretyx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gkesmpgxd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gvzqnsvky.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gckghwywt.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gdmbjtmfu.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gpdoklpra.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkcnkgivs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gkddjdyrq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gvgsldotw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/ggrisrhua.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gljvaocux.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxzyfkbgq.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gcfaztkmv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gzunudldj.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gnuqsrfnm.sHtML


<!-- 参考信息 -->