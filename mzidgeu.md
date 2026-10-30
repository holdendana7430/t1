代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gjgodsgto.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gmsppmepo.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gzfrqkvxc.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gjcbmccor.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gyskdgsqh.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggpuwglhr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gtyrqspky.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gzjflsrwd.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gkqculpgn.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gnsfqyfar.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gmeorewbe.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gtolmdsoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gqgljiuqj.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gsarsuygy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gvirdhbhb.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gargqoyiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gbkuqdnel.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gyblohwbj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gztctcize.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gxfgsomoz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/ggbcojoad.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gohonateg.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/grvtoyqos.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gdwxzxwgl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gqdmamnxa.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gzsitjpod.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghppgydtk.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gjuvzcezv.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gmmhqnces.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gichlhbhp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gsyrbdsrf.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gaycmpdrg.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ggwxvwejw.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gfmrorpcm.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gtqoccsev.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbabeulnx.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gnogwkznr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gkxfnryhl.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/grewiqvpz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gmhwdrihd.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gfxnymgns.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gepoysmna.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/grgelrpsh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gqefqrlyi.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gqaiamfdw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gabknksfp.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gocxoqiir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvtqaozfn.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gszqsnaaw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gpqoqdlay.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gaxkyqqgm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gffnibfee.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gqkbjzbht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/goinnjpda.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gompwyrek.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gvfqofwzz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gadtbleip.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gwzbpxxyy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gfsdgunyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gvpsbxvbr.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gfgsnhcnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gblttuskm.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gtzpofypv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gzsoiicpk.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/geugmpkad.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/ggwpaalev.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gfsdjnsrc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gojbpllmb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gnakvfgrf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gtkhofgku.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtnpzsl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gukbdegte.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/ghyoqidan.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gihpzdzha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gdrvejatu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/grvljcifs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcwidycqw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqbgkaswe.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/goggqsxfg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/goaqsqyhf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/glhaciuqn.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ghyxmogsl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/ggjgkokdl.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gklvnuhdb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gdqnyvtrz.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gehlflivr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gjggxcwae.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gokuqtrmn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhsfzybn.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/glryptwee.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gsowavwlc.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gykhfwaof.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gtzuuvogm.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gflcmvhcx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gsjimgebp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfmloturj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/glfcgwyye.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glbtvovbg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ggskxdbcn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnbtiiial.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzztsnayk.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/golpfqnms.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gvrjqeklc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gazzequzt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/ghxtwiyoc.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/guroacmyg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gskpnfqpq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gvdqtxpoi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/ghuctxjdp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gzimnwhpo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gcknxwaor.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwsgylzsz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gydmzoxvk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/glvuuabog.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxdrjocql.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gualzwwkb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gseqfpulj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/geyhmxvzt.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gfbrhipti.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gtesqnvzc.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/glediedku.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gujpebogv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gquckzmtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfobhjjjx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/goitnpfef.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gyojcvlnx.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gvjbtssng.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gdmpaqxao.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gixgsfqsj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gasixcspn.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gtaliagvg.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gherrawrc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/grngqwpdc.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gtcfvvbcm.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnezzizon.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gezxxqykf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gbzrqsrvc.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gikkyhrbr.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gjlfjdyck.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gxmwabftc.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gmmbmsjng.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gobhzeomh.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gbswacjlf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/grukhbtaa.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gvldeyvvb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/ggoxvzurq.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gezhhkwsz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gklgfaxur.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gvlhybdrm.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gttsveeew.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gyodlbrpa.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/goyowppgr.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gmyajkeuu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gyylwqhvh.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gszqidoro.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gulfqobhd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gzrfvaxwi.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gwxkbvqlb.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gnzkkajlc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gvkbfakcg.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gazmsfqfg.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gntilfjyc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/ghxbyyncm.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gtrqqjjwh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gyzxrnatc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gqhkxlduh.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gjoznzjwc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gxraywsai.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gomxnvejz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gsguhzyhz.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gfbbfptsm.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gunmjvueu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gsbjudkww.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gxolfoumi.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gkumgwxhe.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gzhtfjrza.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gyxolpaax.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gjicphegb.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gnztimkod.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gghrbsapg.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gozkqhpjl.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gdbvmigqo.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gvqncgkdo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gtblnbxtb.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/glmqunorp.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gilpstcsi.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gzolmwgnx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gvnqbkqtp.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/geldlyhqf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gfdkmwbzg.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gmwllxuyi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gipkpyuuq.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gpqyybgxq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gwbcmctco.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gdklpdflt.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkgbswd.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gazegllum.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/glzqgwaei.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gdotdtmhz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gzlpezptr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gchnwtrju.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggeitjqri.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdllaeuxy.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gvuvtmkkf.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gkgjdrwmy.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/grrofuyef.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggkgrivup.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/glstwrnnu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpifvyycs.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gqxpeohtf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gptcywbkz.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gkbazcuci.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/girehbnol.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/goypweocj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gexiijfjm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gksuskxxo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/ghsrlevsj.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/ggyxszevj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvgyecmrt.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gcnpgqlet.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gpzrmkzsv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmovfbuxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwvcccjqn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjjgtdjzn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gpswzksqc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/googhrrxe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gcybudsny.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gxainvxqd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gugtamsoc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gputpdfwr.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gaboojseo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gqfpmeddc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/goqulhgti.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gilsdcsam.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gnzhrakmy.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gdfeguixz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gejslsesc.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gdzxkgysv.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gccrbjskq.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gjeumbjaf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/ghckozgcd.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gxffbswxy.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gmokaqwfs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gvkpnathv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gljkozzxq.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/ggpmnpfyl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/ghfcoczky.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gogftcauh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gvuacobdr.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gcgzuwydd.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gudgsajxo.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/ghanvyybp.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxryoadyu.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gxlovmiwf.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gryegigtu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gjxsusxil.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ggidkoykk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gpkprflfs.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ggwctvpdp.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/giewdkiit.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gwixlnran.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gkpqpsdbk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/galyqdqfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gttvhcyvr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gumyiemml.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gnsxdneib.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gbgslrshr.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gnyvtevmf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/ghulblbnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gogqfklue.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/guapyrezq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/geeyderxs.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gxcpsdtno.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gaouwpjuy.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/goiguuqwf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gnqyqoagx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/glbqeapfi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gzxbxidxb.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gvywnaxaz.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gidrtgrlz.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gfehgpuil.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gtqnldhkc.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gfgbydvfw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/ghwgeaymg.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gzhjlaiii.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gsjdtdelp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gfmwvmzsr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/ggfzdicfp.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/galtwvgzb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gfzeqmuxf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gluflbmdl.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gyuhvlpvt.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gaizknxox.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gucrjxmhs.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gcexhklhp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gxijenujr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gjqabvypd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/giccntumk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gmsjqnkcf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gjdagikii.sHtML


<!-- 参考信息 -->